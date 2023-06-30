# Comparing `tmp/openqaoa-0.1.3.tar.gz` & `tmp/openqaoa-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-0.1.3.tar", last modified: Fri Apr 21 10:55:20 2023, max compression
+gzip compressed data, was "openqaoa-0.1.3rc1.tar", last modified: Fri Jun 30 09:19:25 2023, max compression
```

## Comparing `openqaoa-0.1.3.tar` & `openqaoa-0.1.3rc1.tar`

### file list

```diff
@@ -1,203 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.937017 openqaoa-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-21 10:53:10.000000 openqaoa-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-21 10:55:20.937017 openqaoa-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-04-21 10:53:10.000000 openqaoa-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 10:53:10.000000 openqaoa-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:55:20.941017 openqaoa-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-21 10:53:10.000000 openqaoa-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-azure/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backends/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-braket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-braket/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/gates_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/qaoa_braket_qpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28209 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/baseworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/managed_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28190 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/workflow_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/basebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/cost_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/devices_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/gates_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/plugin_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_analytical_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    29828 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33489 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/derivative_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/qfim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/logger_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/CANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/SPSA.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/iCANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/is_independent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/quantum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/qaoa_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/training_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/binpacking.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/maximalindependentset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/maximumcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/minimumvertexcover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/numberpartition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/portfoliooptimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/vehiclerouting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21328 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    57894 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-pyquil/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/gates_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-qiskit/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/gates_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.933016 openqaoa-0.1.3/src/openqaoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.937017 openqaoa-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_analytical_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_aws_managed_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    36050 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_circuit_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_custom_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    47713 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_optimizers_pennylane.py
--rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_parameters_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    66604 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_pyquil_qvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_rqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_sample_from_wavefunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_sim_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    43760 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)    95997 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-azure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-azure/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/tests/test_devices_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-azure/tests/test_qpu_qiskit_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.919151 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/jobs/managed_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/gates_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/qaoa_braket_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.915151 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/jobs_test_input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/jobs_test_input/aws_braket_source_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/jobs_test_input/aws_braket_source_module/openqaoa_qaoa_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/jobs_test_input/aws_braket_source_module/openqaoa_rqaoa_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_aws_managed_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_devices_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_gate_applicators_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_gates_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_qpu_braket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/baseworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28187 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.923151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/workflow_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/basebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/cost_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/devices_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/gates_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/plugin_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_analytical_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30340 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33483 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/derivative_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/qfim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/logger_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/CANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/SPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/iCANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/natural_grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/newton_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/fourier/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.927151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/is_independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/matrix_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/multi_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/quantum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/single_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.931151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.931151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32442 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/qaoa_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/training_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.931151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/binpacking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/maximalindependentset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/maximumcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/minimumvertexcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/numberpartition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/portfoliooptimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/vehiclerouting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.931151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.935151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gatemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.935151 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/annealingparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/extendedparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/fourierparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/standardparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63680 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_analytical_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_bin_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10833 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_custom_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_gate_applicators_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_maximum_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_minimum_vertex_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_mis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_number_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47708 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19308 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_optimizers_pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_parameters_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_portfolio_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_rqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_sample_from_wavefunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_shortest_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50252 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_vrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63781 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-pyquil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/gates_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/qaoa_pyquil_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_circuit_routing_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_gate_applicators_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_gates_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_pyquil_backend_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_pyquil_qvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_workflows_pyquil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.939151 openqaoa-0.1.3rc1/src/openqaoa-qiskit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/gates_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/qaoa_qiskit_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_backends_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_circuit_routing_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_devices_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_gate_applicators_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_gates_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_qiskit_backend_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_qpu_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_result_object_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_sample_from_wavefunction_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_sim_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_workflows_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/src/openqaoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 09:19:25.000000 openqaoa-0.1.3rc1/src/openqaoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-06-30 09:19:25.000000 openqaoa-0.1.3rc1/src/openqaoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:19:25.000000 openqaoa-0.1.3rc1/src/openqaoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 09:19:25.000000 openqaoa-0.1.3rc1/src/openqaoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 09:19:25.000000 openqaoa-0.1.3rc1/src/openqaoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:19:25.943152 openqaoa-0.1.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-30 09:15:43.000000 openqaoa-0.1.3rc1/tests/test_notebooks.py
```

### Comparing `openqaoa-0.1.3/LICENSE` & `openqaoa-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/PKG-INFO` & `openqaoa-0.1.3rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: openqaoa
-Version: 0.1.3
-Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
-Home-page: https://github.com/entropicalabs/openqaoa
-Author: Entropica Labs
-License: MIT
-Keywords: quantum optimisation SDK
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: all
-License-File: LICENSE
-
 <div align="center">
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo_offW.png" width="650">
   <img alt="OpenQAOA" src="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo.png" width="650">
 </picture>
 
@@ -34,92 +15,97 @@
   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/entropicalabs/openqaoa.git/main?labpath=%2Fexamples)
   [![Discord](https://img.shields.io/discord/991258119525122058)](https://discord.gg/ana76wkKBd)
   [![Website](https://img.shields.io/badge/OpenQAOA-Website-blueviolet)](https://openqaoa.entropicalabs.com/) 
 </div>
 
 # OpenQAOA
 
-A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators.
-
+A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators. Check out the OpenQAOA website at [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
+ 
 **OpenQAOA is currently in OpenBeta.**
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
-Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
-
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
+OpenQAOA is divided into separately installable plugins based on the requirements of the user. The core elements of the package are placed in `openqaoa-core` which comes pre-installed with each flavour of OpenQAOA. 
 
+Currently, OpenQAOA supports the following backends and each can be installed exclusively with the exception of `openqaoa-azure` which installs `openqaoa-qiskit` as an additional requirement because Azure backends support circuit submissions via `qiskit`.
+- `openqaoa-braket` for AWS Braket
+- `openqaoa-azure` for Microsoft Azure Quantum
+- `openqaoa-pyquil` for Rigetti Pyquil
+- `openqaoa-qiskit` for IBM Qiskit
+
+The OpenQAOA metapackage, `openqaoa` allows you to install all OpenQAOA plug-ins together.
+### Install via PyPI
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 ```
 pip install openqaoa
 ```
+### Install via git clone
+Alternatively, you can install OpenQAOA manually from the GitHub repository by following the instructions below. 
 
-Alternatively, you can install manually directly from the GitHub repository by
-
+**NOTE:** We recommend creating a python virtual environment for this project using a python environment manager, for instance Anaconda. Instructions can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 1. Clone the git repository:
-
 ```
 git clone https://github.com/entropicalabs/openqaoa.git
 ```
-
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
-
-3. After cloning the repository `cd openqaoa` and pip install the package. 
-
+2. After cloning the repository `cd openqaoa` and pip install the package with instructions from the Makefile as follows
 ```
-pip install .
+make local-install
 ```
-If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
 
+### Installation instructions for Developers
+Users can install OpenQAOA in the developer mode via the Makefile. For a clean editable install of the package run the following command from the `openqaoa` folder.
 ```
-pip install .[tests]
+make dev-install
 ```
+The package can be installed as an editable with extra requirements defined in the `setup.py`. If you would like to install the extra requirements to be able run the tests module or generate the docs, you can run the following
 
+```
+make dev-install-x,   with x = {tests, docs, all}
+```
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
-The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
-
-We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
+The API documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/). We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
 
 - [Run your first OpenQAOA workflow](https://el-openqaoa.readthedocs.io/en/latest/notebooks/01_workflows_example.html)
 - [How about trying some RQAOA for a change?](https://el-openqaoa.readthedocs.io/en/latest/notebooks/09_RQAOA_example.html)
 - [Introducing EL's fast QAOA simulator](https://el-openqaoa.readthedocs.io/en/latest/notebooks/06_fast_qaoa_simulator.html)
 - [Discover OpenQAOA's custom parametrizations](https://el-openqaoa.readthedocs.io/en/latest/notebooks/05_advanced_parameterization.html)
 
 ### Key Features
 
 - **Build advanced QAOAs**. Create complex QAOAs by specifying custom _parametrisation_, _mixer hamiltonians_, _classical optimisers_ and execute the algorithm on either simulators or QPUs.
 
 - **Recursive QAOA**. Run RQAOA with fully customisable schedules on simulators and QPUs alike. 
 
-- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, and `Amazon Braket`.
+- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, `Amazon Braket` and `Azure Quantum`.
 
 
 ### Available devives 
 
 Devices are serviced both locally and on the cloud. For the IBM Quantum experience, the available devices depend on the specified credentials. For QCS and Amazon Braket, the available devices are listed in the table below:
 
-| Device location  | Device Name |
-| ------------- | ------------- |
-| `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
+| Device location | Device Name |
+| --------------- | ----------- |
+| local | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
 | [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
-
 ## Running the tests
 
-To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
-
-> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
+To run the unit-tests, first, make sure to have installed all the optional testing dependencies by running `make dev-install-tests`. Next type `pytest tests/ /src/*/tests/` from the project's root folder. This runs the common metapackage unit-tests and the unit-tests for each OpenQAOA plugin.
 
-> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
+:warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
+:warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+     
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
+We are always interested to hear about projects built with OpenQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.3/README.md` & `openqaoa-0.1.3rc1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: openqaoa
+Version: 0.1.3rc1
+Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
+Home-page: https://github.com/entropicalabs/openqaoa
+Author: Entropica Labs
+License: MIT
+Keywords: quantum optimisation SDK
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo_offW.png" width="650">
   <img alt="OpenQAOA" src="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo.png" width="650">
 </picture>
 
@@ -15,92 +31,97 @@
   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/entropicalabs/openqaoa.git/main?labpath=%2Fexamples)
   [![Discord](https://img.shields.io/discord/991258119525122058)](https://discord.gg/ana76wkKBd)
   [![Website](https://img.shields.io/badge/OpenQAOA-Website-blueviolet)](https://openqaoa.entropicalabs.com/) 
 </div>
 
 # OpenQAOA
 
-A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators.
-
+A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators. Check out the OpenQAOA website at [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
+ 
 **OpenQAOA is currently in OpenBeta.**
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
-Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
-
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
+OpenQAOA is divided into separately installable plugins based on the requirements of the user. The core elements of the package are placed in `openqaoa-core` which comes pre-installed with each flavour of OpenQAOA. 
 
+Currently, OpenQAOA supports the following backends and each can be installed exclusively with the exception of `openqaoa-azure` which installs `openqaoa-qiskit` as an additional requirement because Azure backends support circuit submissions via `qiskit`.
+- `openqaoa-braket` for AWS Braket
+- `openqaoa-azure` for Microsoft Azure Quantum
+- `openqaoa-pyquil` for Rigetti Pyquil
+- `openqaoa-qiskit` for IBM Qiskit
+
+The OpenQAOA metapackage, `openqaoa` allows you to install all OpenQAOA plug-ins together.
+### Install via PyPI
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 ```
 pip install openqaoa
 ```
+### Install via git clone
+Alternatively, you can install OpenQAOA manually from the GitHub repository by following the instructions below. 
 
-Alternatively, you can install manually directly from the GitHub repository by
-
+**NOTE:** We recommend creating a python virtual environment for this project using a python environment manager, for instance Anaconda. Instructions can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 1. Clone the git repository:
-
 ```
 git clone https://github.com/entropicalabs/openqaoa.git
 ```
-
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
-
-3. After cloning the repository `cd openqaoa` and pip install the package. 
-
+2. After cloning the repository `cd openqaoa` and pip install the package with instructions from the Makefile as follows
 ```
-pip install .
+make local-install
 ```
-If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
 
+### Installation instructions for Developers
+Users can install OpenQAOA in the developer mode via the Makefile. For a clean editable install of the package run the following command from the `openqaoa` folder.
 ```
-pip install .[tests]
+make dev-install
 ```
+The package can be installed as an editable with extra requirements defined in the `setup.py`. If you would like to install the extra requirements to be able run the tests module or generate the docs, you can run the following
 
+```
+make dev-install-x,   with x = {tests, docs, all}
+```
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
-The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
-
-We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
+The API documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/). We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
 
 - [Run your first OpenQAOA workflow](https://el-openqaoa.readthedocs.io/en/latest/notebooks/01_workflows_example.html)
 - [How about trying some RQAOA for a change?](https://el-openqaoa.readthedocs.io/en/latest/notebooks/09_RQAOA_example.html)
 - [Introducing EL's fast QAOA simulator](https://el-openqaoa.readthedocs.io/en/latest/notebooks/06_fast_qaoa_simulator.html)
 - [Discover OpenQAOA's custom parametrizations](https://el-openqaoa.readthedocs.io/en/latest/notebooks/05_advanced_parameterization.html)
 
 ### Key Features
 
 - **Build advanced QAOAs**. Create complex QAOAs by specifying custom _parametrisation_, _mixer hamiltonians_, _classical optimisers_ and execute the algorithm on either simulators or QPUs.
 
 - **Recursive QAOA**. Run RQAOA with fully customisable schedules on simulators and QPUs alike. 
 
-- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, and `Amazon Braket`.
+- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, `Amazon Braket` and `Azure Quantum`.
 
 
 ### Available devives 
 
 Devices are serviced both locally and on the cloud. For the IBM Quantum experience, the available devices depend on the specified credentials. For QCS and Amazon Braket, the available devices are listed in the table below:
 
-| Device location  | Device Name |
-| ------------- | ------------- |
-| `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
+| Device location | Device Name |
+| --------------- | ----------- |
+| local | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
 | [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
-
 ## Running the tests
 
-To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
-
-> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
+To run the unit-tests, first, make sure to have installed all the optional testing dependencies by running `make dev-install-tests`. Next type `pytest tests/ /src/*/tests/` from the project's root folder. This runs the common metapackage unit-tests and the unit-tests for each OpenQAOA plugin.
 
-> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
+:warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
+:warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+     
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
+We are always interested to hear about projects built with OpenQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-azure/backends/devices.py` & `openqaoa-0.1.3rc1/src/openqaoa-azure/openqaoa_azure/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-braket/backends/devices.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     def __init__(
         self,
         device_name: str,
         s3_bucket_name: str = None,
         aws_region: str = None,
         folder_name: str = "openqaoa",
     ):
-
         """Input the device arn and the name of the folder in which all the
         results for the QPU runs would be saved on the pre-defined s3 bucket.
         Note that the user is required to authenticate through the AWS CLI
         before being able to use this Device object.
 
         See: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html for further details.
 
@@ -62,15 +61,14 @@
         self.aws_region = aws_region
         self.folder_name = folder_name
 
         self.provider_connected = None
         self.qpu_connected = None
 
     def check_connection(self) -> bool:
-
         self.provider_connected = self._check_provider_connection()
 
         if self.provider_connected == False:
             return self.provider_connected
 
         # Only QPUs that are available for the specified aws region on Braket
         # will be shown. We filter out QPUs that do not work with the circuit model
@@ -96,15 +94,14 @@
 
         if self.provider_connected and self.qpu_connected:
             return True
         else:
             return False
 
     def _check_backend_connection(self) -> bool:
-
         if self.device_name in self.available_qpus:
             self.backend_device = AwsDevice(self.device_name, self.aws_session)
         else:
             print(
                 """
                 These are the only available devices for this aws region: 
                 {}. Try a different aws region if the device you are looking 
@@ -123,15 +120,14 @@
                 "OpenQAOA is unable to retrieve the number of qubits available in the selected QPU."
             )
             return False
         else:
             return True
 
     def _check_provider_connection(self) -> bool:
-
         try:
             sess = Session(region_name=self.aws_region)
             self.aws_session = AwsSession(sess, default_bucket=self.s3_bucket_name)
             self.aws_region = self.aws_session.region
             self.s3_bucket_name = self.aws_session.default_bucket()
             return True
         except NoRegionError:
```

### Comparing `openqaoa-0.1.3/src/openqaoa-braket/backends/gates_braket.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/gates_braket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,84 @@
 from typing import Callable
 
 from braket.circuits import gates, Circuit
 
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 import openqaoa.qaoa_components.ansatz_constructor.gates as gates_core
 
-class BraketGateApplicator(gates_core.GateApplicator):
 
+class BraketGateApplicator(gates_core.GateApplicator):
     BRAKET_OQ_GATE_MAPPER = {
+        gates_core.X.__name__: gates.X.x,
         gates_core.RZ.__name__: gates.Rz.rz,
         gates_core.RX.__name__: gates.Rx.rx,
         gates_core.RY.__name__: gates.Ry.ry,
         gates_core.CX.__name__: gates.CNot.cnot,
         gates_core.CZ.__name__: gates.CZ.cz,
         gates_core.RXX.__name__: gates.XX.xx,
         gates_core.RZZ.__name__: gates.ZZ.zz,
         gates_core.RYY.__name__: gates.YY.yy,
         gates_core.CPHASE.__name__: gates.CPhaseShift.cphaseshift,
-        gates_core.RiSWAP.__name__: gates.XY.xy
+        gates_core.RiSWAP.__name__: gates.XY.xy,
     }
 
-    library = 'braket'
+    library = "braket"
+
+    def create_quantum_circuit(self, n_qubits) -> Circuit:
+        """
+        Function which creates and empty circuit for the braket backend.
+        Needed for SPAM twirling but more general than that.
+        """
+        return Circuit()
 
     def gate_selector(self, gate: gates_core.Gate) -> Callable:
         selected_braket_gate = BraketGateApplicator.BRAKET_OQ_GATE_MAPPER[gate.__name__]
         return selected_braket_gate
 
     @staticmethod
     def apply_1q_rotation_gate(
-        braket_gate,
-        qubit_1: int,
-        rotation_object: RotationAngle,
-        circuit: Circuit
+        braket_gate, qubit_1: int, rotation_object: RotationAngle, circuit: Circuit
     ) -> Circuit:
-        circuit += braket_gate(
-            qubit_1, 
-            rotation_object.rotation_angle
-        )
+        circuit += braket_gate(qubit_1, rotation_object.rotation_angle)
         return circuit
 
     @staticmethod
     def apply_2q_rotation_gate(
         braket_gate,
         qubit_1: int,
         qubit_2: int,
         rotation_object: RotationAngle,
-        circuit: Circuit
+        circuit: Circuit,
     ) -> Circuit:
-        circuit += braket_gate(
-            qubit_1, 
-            qubit_2, 
-            rotation_object.rotation_angle
-        )
+        circuit += braket_gate(qubit_1, qubit_2, rotation_object.rotation_angle)
         return circuit
 
     @staticmethod
-    def apply_1q_fixed_gate(
-        braket_gate,
-        qubit_1: int,
-        circuit: Circuit
-    ) -> Circuit:
+    def apply_1q_fixed_gate(braket_gate, qubit_1: int, circuit: Circuit) -> Circuit:
         circuit += braket_gate(qubit_1)
         return circuit
 
     @staticmethod
     def apply_2q_fixed_gate(
-        braket_gate,
-        qubit_1: int,
-        qubit_2: int,
-        circuit: Circuit
+        braket_gate, qubit_1: int, qubit_2: int, circuit: Circuit
     ) -> Circuit:
         circuit += braket_gate(qubit_1, qubit_2)
         return circuit
 
     def apply_gate(self, gate: gates_core.Gate, *args) -> Circuit:
         selected_braket_gate = self.gate_selector(gate)
         if gate.n_qubits == 1:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,rotation_object,circuit)
                 return self.apply_1q_rotation_gate(selected_braket_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1,circuit)
                 return self.apply_1q_fixed_gate(selected_braket_gate, *args)
         elif gate.n_qubits == 2:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,qubit_2,rotation_object,circuit)
                 return self.apply_2q_rotation_gate(selected_braket_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1,qubit_2,circuit)
                 return self.apply_2q_fixed_gate(selected_braket_gate, *args)
         else:
-            raise ValueError("Only 1 and 2-qubit gates are supported.")
+            raise ValueError("Only 1 and 2-qubit gates are supported.")
```

### Comparing `openqaoa-0.1.3/src/openqaoa-braket/backends/qaoa_braket_qpu.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/backends/qaoa_braket_qpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from copy import deepcopy
 from typing import Optional, List
 import warnings
 
 from braket.circuits import Circuit
 from braket.circuits.gates import H
 from braket.circuits.result_types import Probability
 from braket.circuits.free_parameter import FreeParameter
@@ -59,25 +60,25 @@
         prepend_state: Optional[Circuit],
         append_state: Optional[Circuit],
         init_hadamard: bool,
         cvar_alpha: float,
         disable_qubit_rewiring: bool = False,
         initial_qubit_mapping: Optional[List[int]] = None,
     ):
-
         QAOABaseBackendShotBased.__init__(
             self,
             qaoa_descriptor,
             n_shots,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
         )
         QAOABaseBackendCloud.__init__(self, device)
+        self.gate_applicator = BraketGateApplicator()
 
         self.qureg = list(range(self.n_qubits))
         self.problem_reg = self.qureg[0 : self.problem_qubits]
         if self.initial_qubit_mapping is None:
             self.initial_qubit_mapping = (
                 initial_qubit_mapping
                 if initial_qubit_mapping is not None
@@ -128,37 +129,44 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         qaoa_circuit: `Circuit`
             The final QAOA circuit constructed using the angles from variational params.
         """
+        parametric_circuit = deepcopy(self.parametric_circuit)
+
+        if self.append_state:
+            parametric_circuit += self.append_state
+
+        # TODO: needs to be fixed --> measurement operations on problem qubits
+        parametric_circuit += Probability.probability()
 
         angles_list = self.obtain_angles_for_pauli_list(self.abstract_circuit, params)
         memory_map = dict(
             zip(
                 [
                     each_free_param_obj.name
                     for each_free_param_obj in self.braket_parameter_list
                 ],
                 angles_list,
             )
         )
-        new_parametric_circuit = self.parametric_circuit.make_bound_circuit(memory_map)
-        return new_parametric_circuit
+        circuit_with_angles = parametric_circuit.make_bound_circuit(memory_map)
+
+        return circuit_with_angles
 
     @property
     def parametric_qaoa_circuit(self) -> Circuit:
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
         the circuit.
         """
         parametric_circuit = Circuit()
-        gate_applicator = BraketGateApplicator()
 
         if self.prepend_state:
             parametric_circuit += self.prepend_state
 
         # Initial state is all |+>
         if self.init_hadamard:
             for each_qubit in self.problem_reg:
@@ -170,23 +178,17 @@
             if each_gate.gate_label.type.value in ["MIXER", "COST"]:
                 angle_param = FreeParameter(each_gate.gate_label.__repr__())
                 self.braket_parameter_list.append(angle_param)
                 each_gate.angle_value = angle_param
             decomposition = each_gate.decomposition("standard")
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0](gate_applicator, *each_tuple[1])
+                gate = each_tuple[0](self.gate_applicator, *each_tuple[1])
                 gate.apply_gate(parametric_circuit)
 
-        if self.append_state:
-            parametric_circuit += self.append_state
-
-        # TODO: needs to be fixed --> measurement operations on problem qubits
-        parametric_circuit += Probability.probability()
-
         return parametric_circuit
 
     def get_counts(self, params: QAOAVariationalBaseParams, n_shots=None) -> dict:
         """
         Execute the circuit and obtain the counts
 
         Parameters
@@ -255,15 +257,14 @@
         #     final_counts = permute_counts_dictionary(final_counts,
         #                                             self.final_mapping)
         # # Expose counts
         self.measurement_outcomes = final_counts
         return final_counts
 
     def log_with_backend(self, metric_name: str, value, iteration_number) -> None:
-
         """
         If using AWS Jobs, these values will be logged.
         """
 
         try:
             if os.environ["AMZN_BRAKET_JOB_NAME"] is not None:
                 in_jobs = True
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/baseworkflow.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/baseworkflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 
 from abc import ABC
 from typing import List
 import json
 import gzip
 from os.path import exists
 
-from .workflow_properties import BackendProperties, ClassicalOptimizer
+from .workflow_properties import (
+    BackendProperties,
+    ErrorMitigationProperties,
+    ClassicalOptimizer,
+)
 from ..backends.devices_core import DeviceBase, DeviceLocal
 from ..problems import QUBO
 from ..utilities import delete_keys_from_dict, is_valid_uuid, generate_uuid
 from ..backends.qaoa_backend import (
     DEVICE_NAME_TO_OBJECT_MAPPER,
     DEVICE_ACCESS_OBJECT_MAPPER,
 )
@@ -86,17 +90,19 @@
         ----------
         device: `DeviceBase`
             Device to be used by the optimizer. Default is using the local 'vectorized' simulator.
         """
 
         self.device = device
         self.backend_properties = BackendProperties()
+        self.error_mitigation_properties = ErrorMitigationProperties()
         self.classical_optimizer = ClassicalOptimizer()
         self.local_simulators = list(DEVICE_NAME_TO_OBJECT_MAPPER.keys())
         self.cloud_provider = list(DEVICE_ACCESS_OBJECT_MAPPER.keys())
+        self.available_error_mitigation_techniques = ["spam_twirling"]
         self.compiled = False
 
         # Initialize the identifier stamps, we initialize all the stamps needed to None
         self.header = {
             "atomic_id": None,  # the id of the run it is generated automatically in the compilation
             "experiment_id": generate_uuid(),  # the id of the experiment it is generated automatically here
             "project_id": None,
@@ -148,14 +154,19 @@
         """
         if project_id is not None:
             if not is_valid_uuid(project_id):
                 raise ValueError(
                     "The project_id is not a valid uuid, example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
                 )
 
+        if not is_valid_uuid(project_id):
+            raise ValueError(
+                "The project_id is not a valid uuid, example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
+            )
+
         if experiment_id is not None:
             if not is_valid_uuid(experiment_id):
                 raise ValueError(
                     "The experiment_id is not a valid uuid, \
                         example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
                 )
             else:
@@ -223,14 +234,16 @@
                 on shot-based simulators and QPUs. Defaults to 100.
             cvar_alpha: float
                 The value of alpha for the CVaR cost function
             noise_model: `qiskit.providers.aer.noise.NoiseModel`
                     The Qiskit noise model to be used for the simulation.
             qiskit_simulation_method: str, optional
                 The method to be used for the simulation.
+            qiskit_optimization_level: int, optional
+                The qiskit.transpile optimization level to use. Choose from 0,1,2,3
             seed_simulator: int
                 Optional argument to initialize a pseudorandom solution. Default None
             active_reset:
                 #TODO
             rewiring:
                 Rewiring scheme to be used for Pyquil.
                 Either 'PRAGMA INITIAL_REWIRING "NAIVE"' or
@@ -247,14 +260,43 @@
                     f"Specified argument `{value}` for `{key}` in set_backend_properties is not supported"
                 )
 
         self.backend_properties = BackendProperties(**kwargs)
         return None
 
     @check_compiled
+    def set_error_mitigation_properties(self, **kwargs):
+        """
+        Set the error mitigation properties, if any.
+
+        Parameters
+        ----------
+            error_mitigation_technique: str
+                The specific technique used to mitigate the errors. Only a simple state preparation and measurement twirling with bitflip averages, under the name "spam_twirling" is currently supported.
+            n_batches: int
+                The number of batches specifies the different negating schedules at random. Total number of shots is distributed accordingly.
+            calibration_data_location: str
+                The location of the json file containing calibration data. For spam twirling this is the measurement outcomes of an empty circuit under the bit-flip averaging.
+
+        """
+        for key, value in kwargs.items():
+            if hasattr(self.error_mitigation_properties, key) and (
+                kwargs["error_mitigation_technique"].lower()
+                in self.available_error_mitigation_techniques
+            ):
+                pass  # setattr(self.error_mitigation, key, value)
+            else:
+                raise ValueError(
+                    f"Specified argument `{value}` for `{key}` in set_error_mitigation_properties is not supported"
+                )
+
+        self.error_mitigation_properties = ErrorMitigationProperties(**kwargs)
+        return None
+
+    @check_compiled
     def set_classical_optimizer(self, **kwargs):
         """
         Set the parameters for the classical optimizer to be used in the optimizers workflow
 
         Parameters
         ----------
             method: str
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/managed_job.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/openqaoa_braket/algorithms/jobs/managed_job.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_benchmark.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,21 +280,19 @@
                 ["benchmark", "reference"], [run_main, run_reference]
             )
             if boolean
         ]
 
         # loop over the benchmarked QAOA object and the reference QAOA object (if requested)
         for qaoa, values, string in zip(both_qaoa, both_values, both_strings):
-
             if verbose:
                 print(f"Running {string}.")
 
             # evaluate all the points in the grid, in the order provided by the function __ordered_points. We loop over the indices of the grid.
             for k, i_point in enumerate(self.__ordered_points(n_params, n_points_axis)):
-
                 if verbose:
                     self.__print_expected_time(
                         k, n_points_axis**n_params
                     )  # print the expected remaining time, info for the user
 
                 new_params = [
                     axis[i] for axis, i in zip(axes, i_point)
@@ -435,15 +433,14 @@
             )
             fig, ax = plt.subplots(nrows=nrows, ncols=1, figsize=(6.5, 5 * nrows))
 
         # plot the requested plots
         count_sp = 0  # counter of subplots
         for key in values:
             if values[key][0]:  # skip the plot if it is not requested
-
                 # raise an exception if the values for a plo requested are not available
                 if values[key][1] is None:
                     raise Exception(
                         "You must run the benchmark before plotting the results, there are no values for the "
                         + key
                         + " plot"
                     )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_result.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
-from typing import Type, List, Union
+from typing import Type, List, Union, TYPE_CHECKING
 
 import copy
 import numpy as np
 import matplotlib.pyplot as plt
 
 from ...qaoa_components import Hamiltonian
+if TYPE_CHECKING:
+    from ...optimizers.logger_vqa import Logger
 from ...utilities import (
     qaoa_probabilities,
     bitstring_energy,
     convert2serialize,
     delete_keys_from_dict,
 )
 from ...backends.basebackend import QAOABaseBackend, QAOABaseBackendStatevector
@@ -47,15 +49,15 @@
         The cost Hamiltonian for the problem statement
     type_backend: `QAOABaseBackend`
         The type of backend used for the experiment
     """
 
     def __init__(
         self,
-        log: "Logger",
+        log: Logger,
         method: Type[str],
         cost_hamiltonian: Type[Hamiltonian],
         type_backend: Type[QAOABaseBackend],
     ):
         """
         init method
         """
@@ -625,7 +627,61 @@
             ],
             "probabilities": [
                 measurement_outcomes[solution_bitstring[args_sorted[ii]]] / total_shots
                 for ii in range(n_bitstrings)
             ],
         }
         return best_results
+    
+    def calculate_statistics(self, include_intermediate=False) -> dict:
+        """
+        A function to calculate statistics of measurement outcomes associated with a QAOA workflow
+
+        Parameters
+        ----------
+        include_intermediate: `bool`
+            Whether it is necessary to calculate statistics for intermediate results. Defaults to False.
+        """
+        if len(self.intermediate["measurement_outcomes"]) == 0 and include_intermediate == True:
+            raise ValueError(
+                "The underlying QAOA object does not seem to have any intermediate measurement result. Please, consider saving "
+                "intermediate measurements during optimization by setting `optimization_progress=True` in your workflow."
+            )
+
+        if isinstance(self.optimized["measurement_outcomes"], dict):
+            optimized_measurement_outcomes = self.optimized["measurement_outcomes"]
+        elif isinstance(self.optimized["measurement_outcomes"], np.ndarray):
+            optimized_measurement_outcomes = self.get_counts(
+                self.optimized["measurement_outcomes"]
+            )
+        else:
+            raise TypeError(
+                f"The measurement outcome {type(self.optimized['measurement_outcomes'])} is not valid."
+            )
+
+        if isinstance(self.intermediate["measurement_outcomes"], list):
+            if len(self.intermediate["measurement_outcomes"]) > 0:
+                if isinstance(self.intermediate["measurement_outcomes"][0], dict):
+                    intermediate_measurement_outcomes = self.intermediate["measurement_outcomes"]
+                elif isinstance(self.intermediate["measurement_outcomes"][0], np.ndarray):
+                    intermediate_measurement_outcomes = [self.get_counts(i) for i in self.intermediate["measurement_outcomes"]]
+                else:
+                    raise TypeError(
+                        f"The measurement outcome {type(self.intermediate['measurement_outcomes'][0])} is not valid."
+                    )
+        else:
+            raise TypeError(
+                f"The measurement outcome {type(self.intermediate['measurement_outcomes'])} is not valid."
+            )
+
+        def sorted_mean_std_deviation(counts: dict):
+            values = list(counts.values())
+            return {
+                'sorted': dict(sorted(counts.items(), key=lambda x: x[1], reverse=True)),
+                'mean': np.mean(values),
+                'std_deviation': np.std(values)
+            }
+
+        return {
+            'intermediate': [sorted_mean_std_deviation(i) for i in intermediate_measurement_outcomes] if include_intermediate else [],
+            'optimized': sorted_mean_std_deviation(optimized_measurement_outcomes)
+        }
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/qaoa/qaoa_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     create_qaoa_variational_params,
 )
 from ...qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
 from ...utilities import get_mixer_hamiltonian, generate_timestamp
 from ...optimizers.qaoa_optimizer import get_optimizer
+from ...backends.wrapper import SPAMTwirlingWrapper
 
 
 class QAOA(Workflow):
     """
     A class implementing a QAOA workflow end to end.
 
     It's basic usage consists of
@@ -74,15 +75,15 @@
     Examples
     --------
     Examples should be written in doctest format, and should illustrate how
     to use the function.
 
     >>> q = QAOA()
     >>> q.compile(QUBO)
-    >>> q.optimise()
+    >>> q.optimize()
 
     Where `QUBO` is a an instance of `openqaoa.problems.problem.QUBO`
 
     If you want to use non-default parameters:
 
     >>> q_custom = QAOA()
     >>> q_custom.set_circuit_properties(
@@ -244,20 +245,34 @@
             variational_params_dict=self.circuit_properties.variational_params_dict,
             linear_ramp_time=self.circuit_properties.linear_ramp_time,
             q=self.circuit_properties.q,
             seed=self.circuit_properties.seed,
             total_annealing_time=self.circuit_properties.annealing_time,
         )
 
+        backend_dict = self.backend_properties.__dict__.copy()
+
         self.backend = get_qaoa_backend(
             qaoa_descriptor=self.qaoa_descriptor,
             device=self.device,
-            **self.backend_properties.__dict__,
+            **backend_dict,
         )
 
+        # Implementing SPAM Twirling error mitigation requires wrapping the backend.
+        # However, the BaseWrapper can have many more use cases.
+        if (
+            self.error_mitigation_properties.error_mitigation_technique
+            == "spam_twirling"
+        ):
+            self.backend = SPAMTwirlingWrapper(
+                backend=self.backend,
+                n_batches=self.error_mitigation_properties.n_batches,
+                calibration_data_location=self.error_mitigation_properties.calibration_data_location,
+            )
+
         self.optimizer = get_optimizer(
             vqa_object=self.backend,
             variational_params=self.variate_params,
             optimizer_dict=self.classical_optimizer.asdict(),
         )
 
         # Set the header properties
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_result.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_utils.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     Examples
     --------
     Examples should be written in doctest format, and should illustrate how
     to use the function.
 
     >>> r = RQAOA()
     >>> r.compile(QUBO)
-    >>> r.optimise()
+    >>> r.optimize()
 
     Where `QUBO` is a an instance of `openqaoa.problems.problem.QUBO`
 
     If you want to use non-default parameters:
 
     Standard/custom (default) type:
 
@@ -274,15 +274,14 @@
         super().compile(problem=problem)
 
         # if type is custom and steps is an int, set steps correctly
         if (
             self.rqaoa_parameters.rqaoa_type == "custom"
             and self.rqaoa_parameters.n_cutoff <= problem.n
         ):
-
             n_cutoff = self.rqaoa_parameters.n_cutoff
             n_qubits = problem.n
             counter = self.rqaoa_parameters.counter
 
             # If schedule for custom RQAOA is not given, we create a schedule such that
             # n = self.rqaoa_parameters.steps spins is eliminated at a time
             if type(self.rqaoa_parameters.steps) is int:
@@ -375,15 +374,14 @@
         self.header["execution_time_start"] = generate_timestamp()
 
         # flag, set to true if the problem vanishes due to elimination before reaching cutoff
         total_elimination = False
 
         # If above cutoff, loop quantumly, else classically
         while n_qubits > n_cutoff:
-
             # put a tag to the qaoa object to know which step it is
             q.set_exp_tags({"rqaoa_counter": counter})
 
             # Run QAOA
             q.optimize()
 
             # save the results if dump is true
@@ -517,16 +515,14 @@
         qaoa_optimized_angles = q.result.optimized["angles"]
         qaoa_optimized_counts = q.result.get_counts(
             q.result.optimized["measurement_outcomes"]
         )
         analytical = isinstance(qaoa_backend, QAOABackendAnalyticalSimulator)
 
         return exp_val_hamiltonian_termwise(
-            variational_params,
-            qaoa_backend,
             cost_hamiltonian,
             mixer_type,
             p,
             qaoa_optimized_angles,
             qaoa_optimized_counts,
             analytical=analytical,
         )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/rqaoa/rqaoa_workflow_properties.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/algorithms/workflow_properties.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/algorithms/workflow_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Optional, Union
 import numpy as np
+import json
 from scipy.optimize._minimize import MINIMIZE_METHODS
 
 from ..optimizers.training_vqa import CustomScipyGradientOptimizer, PennyLaneOptimizer
 from ..backends.devices_core import SUPPORTED_LOCAL_SIMULATORS
 from ..backends.basebackend import QuantumCircuitBase
 from ..utilities import convert2serialize
 
@@ -73,15 +74,14 @@
         linear_ramp_time: Optional[float] = None,
         variational_params_dict: Optional[dict] = {},
         mixer_hamiltonian: Optional[str] = "x",
         mixer_qubit_connectivity: Optional[Union[List[list], List[tuple], str]] = None,
         mixer_coeffs: Optional[float] = None,
         seed: Optional[int] = None,
     ):
-
         self.param_type = param_type
         self.init_type = init_type
         self.qubit_register = qubit_register
         self.p = p
         self.q = (
             q
             if param_type.lower() in ["fourier", "fourier_extended", "fourier_w_bias"]
@@ -205,14 +205,16 @@
     initial_qubit_mapping: Union[List[int], numpy.ndarray]
         Mapping from physical to logical qubit indices, used to eventually
         construct the quantum circuit.  For example, for a system composed by 3 qubits
        `qubit_layout=[1,3,2]`, maps `1<->0`, `3<->1`, `2<->2`, where the left hand side is the physical qubit
         and the right hand side is the logical qubits
     qiskit_simulation_method: str
         Specify the simulation method to use with the `qiskit.AerSimulator`
+    qiskit_optimization_level: int, optional
+        Specify the qiskit.transpile optimization level. Choose from 0,1,2,3
     seed_simulator: int
         Specify a seed for `qiskit` simulators
     active_reset: bool
         To use the active_reset functionality on Rigetti backends through QCS
     rewiring: str
         Specify the rewiring strategy for compilation for Rigetti QPUs through QCS
     disable_qubit_rewiring: bool
@@ -227,29 +229,30 @@
         append_state: Optional[Union[QuantumCircuitBase, np.ndarray]] = None,
         init_hadamard: bool = True,
         n_shots: int = 100,
         cvar_alpha: float = 1,
         noise_model=None,
         initial_qubit_mapping: Optional[Union[List[int], np.ndarray]] = None,
         qiskit_simulation_method: Optional[str] = None,
+        qiskit_optimization_level: Optional[int] = None,
         seed_simulator: Optional[int] = None,
         active_reset: Optional[bool] = None,
         rewiring: Optional[str] = None,
         disable_qubit_rewiring: Optional[bool] = None,
     ):
-
         self.init_hadamard = init_hadamard
         self.n_shots = n_shots
         self.prepend_state = prepend_state
         self.append_state = append_state
         self.cvar_alpha = cvar_alpha
         self.noise_model = noise_model
         self.initial_qubit_mapping = initial_qubit_mapping
         self.seed_simulator = seed_simulator
         self.qiskit_simulation_method = qiskit_simulation_method
+        self.qiskit_optimization_level = qiskit_optimization_level
         self.active_reset = active_reset
         self.rewiring = rewiring
         self.disable_qubit_rewiring = disable_qubit_rewiring
 
     # @property
     # def cvar_alpha(self):
     #     return self._cvar_alpha
@@ -258,14 +261,79 @@
     # def cvar_alpha(self, value):
     #     if (value <0) or (value>1) :
     #         raise ValueError(
     #             f"cvar_alpha must be between 0 and 1. Received {value}.")
     #     self._cvar_alpha = value
 
 
+class ErrorMitigationProperties(WorkflowProperties):
+    """
+    Optional, choose an error mitigation technique for the QAOA circuit. Currently supports only SPAM Twirling.
+
+    Parameters
+    ----------
+    error_mitigation_technique: str
+        The name of the error mitigation technique. Only 'spam_twirling' supported for now.
+    n_batches: Optional[int] = int
+        Number of batches in which the total number of shots is divided to. For every batch, we choose a set of qubits at random to which we apply X gates and classical negating. The dafault value is set to 10 to be comparable with most problem sizes in NISQ without creating too much of an overhead.
+    calibration_data_location: str
+        The path to the file containing calibration data for the specific device.
+    """
+
+    def __init__(
+        self,
+        error_mitigation_technique: Optional[str] = None,
+        n_batches: Optional[int] = 10,
+        calibration_data_location: Optional[str] = None,
+    ):
+        self.error_mitigation_technique = (
+            error_mitigation_technique.lower()
+            if type(error_mitigation_technique) == str
+            else error_mitigation_technique
+        )
+
+        if isinstance(n_batches, int) and n_batches > 0:
+            self.n_batches = n_batches
+        else:
+            raise ValueError("n_batches must be a positive integer.")
+
+        if calibration_data_location != None:
+            try:
+                with open(calibration_data_location, "r") as file:
+                    # Parse the JSON file
+                    calibration_data = json.load(file)
+
+                    # Check if the file has the expected structure
+                    calibration_measurements = calibration_data["results"][
+                        "measurement_outcomes"
+                    ]
+                    calibration_registers = calibration_data["register"]
+
+            except FileNotFoundError:
+                raise FileNotFoundError(
+                    "Calibration data file not found at specified location: {}".format(
+                        calibration_data_location
+                    )
+                )
+            except ValueError:
+                raise ValueError(
+                    "Calibration data file {} is not a valid JSON file".format(
+                        calibration_data_location
+                    )
+                )
+            except KeyError:
+                raise KeyError(
+                    "Calibration data file {} structure not as expected".format(
+                        calibration_data_location
+                    )
+                )
+
+        self.calibration_data_location = calibration_data_location
+
+
 class ClassicalOptimizer(WorkflowProperties):
     """
     The classical optimizer for the QAOA optimization routine
     of the QAOA circuit parameters.
 
     Parameters
     ----------
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/basebackend.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/basebackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #                                            wavefunction_expectation)
 """
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union, List, Dict, Optional, Any, Tuple
 from copy import deepcopy
 import numpy as np
 
-from .devices_core import DeviceBase
+from .basedevice import DeviceBase
 from ..qaoa_components import (
     GateMap,
     QAOADescriptor,
 )
 from ..qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
@@ -118,15 +118,14 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         prepend_state: Optional[Union[QuantumCircuitBase, List[complex], np.ndarray]],
         append_state: Optional[Union[QuantumCircuitBase, np.ndarray]],
         init_hadamard: bool,
         cvar_alpha: float,
     ):
-
         super().__init__(prepend_state, append_state)
 
         self.qaoa_descriptor = qaoa_descriptor
         self.cost_hamiltonian = qaoa_descriptor.cost_hamiltonian
         self.n_qubits = self.qaoa_descriptor.n_qubits
         self.init_hadamard = init_hadamard
         self.cvar_alpha = cvar_alpha
@@ -146,15 +145,14 @@
                     range(len(self.qaoa_descriptor.final_mapping))
                 )
         else:
             self.initial_qubit_mapping = None
             self.final_mapping = None
 
     def assign_angles(self, params: QAOAVariationalBaseParams) -> None:
-
         """
         Assigns the angle values of the variational parameters to the circuit gates
         specified as a list of gates in the ``abstract_circuit``.
 
         Parameters
         ----------
         params: `QAOAVariationalBaseParams`
@@ -519,15 +517,14 @@
         qaoa_descriptor: QAOADescriptor,
         n_shots: int,
         prepend_state: Optional[QuantumCircuitBase],
         append_state: Optional[QuantumCircuitBase],
         init_hadamard: bool,
         cvar_alpha: float,
     ):
-
         super().__init__(
             qaoa_descriptor, prepend_state, append_state, init_hadamard, cvar_alpha
         )
         # assert self.n_qubits >= len(prepend_state.qubits), \
         # "Cannot attach a bigger circuit to the QAOA routine"
         # assert self.n_qubits >= len(append_state.qubits), \
         # "Cannot attach a bigger circuit to the QAOA routine"
@@ -559,15 +556,16 @@
     """
     QAOA backend that can be accessed over the cloud offered by the
     respective provider through an API based access
     """
 
     def __init__(self, device: DeviceBase):
         self.device = device
-        self.device.check_connection()
+        if getattr(self.device, "provider_connected", None) is None and getattr(self.device, "qpu_connected", None) is None:
+            self.device.check_connection()
 
 
 class QAOABaseBackendParametric:
     """
     Base class to indicate Parametric Circuit Backend
     """
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/cost_function.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/cost_function.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/gates_vectorized.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/gates_vectorized.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,76 @@
 from typing import Callable
 from ..qaoa_components.ansatz_constructor import gates as gates_core
 from ..qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 
-class VectorizedGateApplicator(gates_core.GateApplicator):
 
+class VectorizedGateApplicator(gates_core.GateApplicator):
     VECTORIZED_OQ_GATE_MAPPER = lambda x: {
+        gates_core.X.__name__: x.apply_x,
         gates_core.RZ.__name__: x.apply_rz,
         gates_core.RX.__name__: x.apply_rx,
         gates_core.RY.__name__: x.apply_ry,
         gates_core.RXX.__name__: x.apply_rxx,
         gates_core.RZX.__name__: x.apply_rzx,
         gates_core.RZZ.__name__: x.apply_rzz,
         gates_core.RYY.__name__: x.apply_ryy,
         gates_core.RYZ.__name__: x.apply_ryz,
-        gates_core.RiSWAP.__name__: x.apply_rxy
+        gates_core.RiSWAP.__name__: x.apply_rxy,
     }
 
-    library = 'vectorized'
+    library = "vectorized"
 
-    def gate_selector(self, gate:gates_core.Gate, vectorized_backend: 'QAOAvectorizedBackendSimulator'):
-        selected_gate = VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(vectorized_backend)[gate.__name__]
+    def gate_selector(
+        self,
+        gate: gates_core.Gate,
+        vectorized_backend: "QAOAvectorizedBackendSimulator",
+    ):
+        selected_gate = VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(
+            vectorized_backend
+        )[gate.__name__]
         return selected_gate
 
     @staticmethod
     def apply_1q_rotation_gate(
-        vectorized_gate: Callable,
-        qubit_1: int,
-        rotation_object: RotationAngle
+        vectorized_gate: Callable, qubit_1: int, rotation_object: RotationAngle
     ):
-        vectorized_gate(
-            qubit_1,
-            rotation_object.rotation_angle
-        )
+        vectorized_gate(qubit_1, rotation_object.rotation_angle)
 
     @staticmethod
     def apply_2q_rotation_gate(
         vectorized_gate: Callable,
         qubit_1: int,
         qubit_2: int,
-        rotation_object: RotationAngle
+        rotation_object: RotationAngle,
     ):
-        vectorized_gate(
-            qubit_1,
-            qubit_2,
-            rotation_object.rotation_angle
-        )
+        vectorized_gate(qubit_1, qubit_2, rotation_object.rotation_angle)
 
     @staticmethod
-    def apply_1q_fixed_gate(
-        vectorized_gate: Callable,
-        qubit_1: int
-    ):
-        vectorized_gate(
-            qubit_1
-        )
+    def apply_1q_fixed_gate(vectorized_gate: Callable, qubit_1: int):
+        vectorized_gate(qubit_1)
 
     @staticmethod
-    def apply_2q_fixed_gate(
-        vectorized_gate: Callable,
-        qubit_1: int,
-        qubit_2: int
-    ):
-        vectorized_gate(
-            qubit_1,
-            qubit_2
-        )
+    def apply_2q_fixed_gate(vectorized_gate: Callable, qubit_1: int, qubit_2: int):
+        vectorized_gate(qubit_1, qubit_2)
 
     def apply_gate(self, gate: gates_core.Gate, *args):
         selected_vector_gate = self.gate_selector(gate, args[-1])
         # Remove argument from tuple
-        args=args[:-1]
+        args = args[:-1]
         if gate.n_qubits == 1:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,rotation_object)
                 self.apply_1q_rotation_gate(selected_vector_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1)
                 self.apply_1q_fixed_gate(selected_vector_gate, *args)
         elif gate.n_qubits == 2:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,qubit_2,rotation_object)
                 self.apply_2q_rotation_gate(selected_vector_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1,qubit_2)
                 self.apply_2q_fixed_gate(selected_vector_gate, *args)
         else:
-            raise ValueError("Error applying the requested gate. Please check in the input")
+            raise ValueError(
+                "Error applying the requested gate. Please check in the input"
+            )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/plugin_finder.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/plugin_finder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 import sys
 from importlib.metadata import entry_points
 
-
-def plugin_finder_dict() -> dict:
+def plugin_finder_dict() -> list:
+    
     """
-    Returns a dictionary whose key:value pairs are the names of the plugin and
-    the backend_config module of the respective plugin.
+    This function searches the openqaoa.plugins entry point group to see if
+    any of the openqaoa plugins have been installed. If they are, this function
+    returns a dictionary whose keys are the names of the plugin libraries and
+    whose values are the plugin's utilities module. 
     """
-
+    
     if sys.version_info >= (3, 10):
-        available_plugins = entry_points().select(group="openqaoa.plugins")
+        available_plugins = entry_points().select(group='openqaoa.plugins')
     else:
-        available_plugins = entry_points()["openqaoa.plugins"]
-
+        available_plugins = entry_points()['openqaoa.plugins']
+    
     output_dict = dict()
     for each_plugin_entry_point in available_plugins:
         try:
             output_dict[each_plugin_entry_point.name] = each_plugin_entry_point.load()
         except ModuleNotFoundError:
-            print(
-                "The {} module has not been installed.".format(
-                    each_plugin_entry_point.name
-                )
-            )
+            print("The {} module has not been installed.".format(each_plugin_entry_point.name))
         except AttributeError:
-            print(
-                "An error has occured when trying to attach the {} plugin.".format(
-                    each_plugin_entry_point.name
-                )
-            )
-
+            print("An error has occured when trying to attach the {} plugin.".format(each_plugin_entry_point.name))
+    
     return output_dict
+    
+#     output_dict = dict()
+    
+#     try:
+#         available_plugins = entry_points()['openqaoa.plugins']
+    
+#         for each_plugin_entry_point in available_plugins:
+#             try:
+#                 output_dict[each_plugin_entry_point.name] = each_plugin_entry_point.load()
+#                 print(output_dict)
+#             except ModuleNotFoundError:
+#                 print("The {} module has not been installed.".format(each_plugin_entry_point.name))
+#             except AttributeError:
+#                 print("An error has occured when trying to attach the {} plugin.".format(each_plugin_entry_point.name))
+            
+#     except KeyError:
+#         print("No plugins were found.")
+    
+#     return output_dict
+
+PLUGIN_DICT = plugin_finder_dict()
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_analytical_sim.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_analytical_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         prepend_state=None,
         append_state=None,
         init_hadamard=True,
         cvar_alpha=1,
     ):
-
         # checking if not supported parameters are passed
         for k, val in {
             "Prepend_state": (prepend_state, None),
             "append_state": (append_state, None),
             "init_hadamard": (init_hadamard, True),
             "cvar_alpha": (cvar_alpha, 1),
         }.items():
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_backend.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,64 @@
+from __future__ import annotations
 from typing import Union, Optional, List
 import numpy as np
 
-from .plugin_finder import plugin_finder_dict
+from .plugin_finder import PLUGIN_DICT
 from .qaoa_vectorized import QAOAvectorizedBackendSimulator
 from .qaoa_analytical_sim import QAOABackendAnalyticalSimulator
 from .devices_core import DeviceBase, DeviceLocal
 from .basebackend import QuantumCircuitBase, QAOABaseBackend
 from ..qaoa_components import QAOADescriptor
 
-PLUGIN_DICT = plugin_finder_dict()
 
 def _create_mappers(input_plugin_dict: dict) -> dict:
-    
     DEVICE_NAME_TO_OBJECT_MAPPER = dict()
     DEVICE_ACCESS_OBJECT_MAPPER = dict()
-    
+
     DEVICE_NAME_TO_OBJECT_MAPPER["vectorized"] = QAOAvectorizedBackendSimulator
-    DEVICE_NAME_TO_OBJECT_MAPPER["analytical_simulator"] = QAOABackendAnalyticalSimulator
-    
+    DEVICE_NAME_TO_OBJECT_MAPPER[
+        "analytical_simulator"
+    ] = QAOABackendAnalyticalSimulator
+
     for each_entry_key, each_entry_value in input_plugin_dict.items():
-        if hasattr(each_entry_value, 'device_access'):
+        if hasattr(each_entry_value, "device_access"):
             DEVICE_ACCESS_OBJECT_MAPPER.update(each_entry_value.device_access)
-        if hasattr(each_entry_value, 'device_name_to_obj'):
+        if hasattr(each_entry_value, "device_name_to_obj"):
             DEVICE_NAME_TO_OBJECT_MAPPER.update(each_entry_value.device_name_to_obj)
-        
+
     return DEVICE_NAME_TO_OBJECT_MAPPER, DEVICE_ACCESS_OBJECT_MAPPER
 
+
 DEVICE_NAME_TO_OBJECT_MAPPER, DEVICE_ACCESS_OBJECT_MAPPER = _create_mappers(PLUGIN_DICT)
 
+
 def _backend_arg_mapper(
     backend_obj: QAOABaseBackend,
     n_shots: Optional[int] = None,
     seed_simulator: Optional[int] = None,
     qiskit_simulation_method: Optional[str] = None,
+    qiskit_optimization_level: Optional[int] = None,
     noise_model=None,
     active_reset: Optional[bool] = None,
     rewiring=None,
     disable_qubit_rewiring: Optional[bool] = None,
     initial_qubit_mapping=None,
 ):
-    
     BACKEND_ARGS_MAPPER = {
         QAOABackendAnalyticalSimulator: {},
         QAOAvectorizedBackendSimulator: {},
     }
-    
+
     local_vars = locals()
-    
+
     for each_plugin_entrypoint in PLUGIN_DICT.values():
-        if hasattr(each_plugin_entrypoint, 'backend_args'):
+        if hasattr(each_plugin_entrypoint, "backend_args"):
             for each_key, each_value in each_plugin_entrypoint.backend_args.items():
                 # Convert list of accepted parameters into a dictionary with
-                # the name of the variable as a key and the local value of the 
+                # the name of the variable as a key and the local value of the
                 # variable
                 var_values = [local_vars[each_name] for each_name in each_value]
                 input_dict = {each_key: dict(zip(each_value, var_values))}
                 BACKEND_ARGS_MAPPER.update(input_dict)
 
     final_backend_kwargs = {
         key: value
@@ -158,11 +161,11 @@
                 device=device,
                 prepend_state=prepend_state,
                 append_state=append_state,
                 init_hadamard=init_hadamard,
                 cvar_alpha=cvar_alpha,
                 **backend_kwargs,
             )
+
     except Exception as e:
         raise ValueError(f"The backend returned an error: {e}")
-
     return backend_obj
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_device.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import annotations
 
-from .plugin_finder import plugin_finder_dict
+from .plugin_finder import PLUGIN_DICT
 from .devices_core import DeviceBase, DeviceLocal
 
 
-PLUGIN_DICT = plugin_finder_dict()
-
-
-
 def device_class_arg_mapper(
     device_class: DeviceBase,
     hub: str = None,
     group: str = None,
     project: str = None,
     as_emulator: bool = None,
     as_qvm: bool = None,
@@ -23,15 +19,14 @@
     engagement_manager: EngagementManager = None,
     folder_name: str = None,
     s3_bucket_name: str = None,
     aws_region: str = None,
     resource_id: str = None,
     az_location: str = None,
 ) -> dict:
-
     DEVICE_ARGS_MAPPER = dict()
 
     local_vars = locals()
 
     for each_plugin_entrypoint in PLUGIN_DICT.values():
         if hasattr(each_plugin_entrypoint, "device_args"):
             for each_key, each_value in each_plugin_entrypoint.device_args.items():
@@ -44,15 +39,15 @@
 
     final_device_kwargs = {
         key: value
         for key, value in DEVICE_ARGS_MAPPER[device_class].items()
         if value is not None
     }
     return final_device_kwargs
-    
+
 
 def create_device(location: str, name: str, **kwargs):
     """
     This function returns an instance of the appropriate device class.
 
     Parameters
     ----------
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_vectorized.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/backends/qaoa_vectorized.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])
 )
 
 # Projection (measurement) operators
 P0 = csc_matrix(np.array([[1, 0], [0, 0]]))
 P1 = csc_matrix(np.array([[0, 0], [0, 1]]))
 
+
 # Parametrised rotations
 def RX(theta: float) -> csc_matrix:
     return csc_matrix(expm(-1j * theta * constX / 2))
 
 
 def RY(theta: float) -> csc_matrix:
     return csc_matrix(expm(-1j * theta * constY / 2))
@@ -256,15 +257,14 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         prepend_state: Optional[Union[np.ndarray, List[complex]]],
         append_state: Optional[Union[np.ndarray, List[complex]]],
         init_hadamard: bool,
         cvar_alpha: float = 1,
     ):
-
         assert (
             cvar_alpha == 1
         ), "Please use the shot-based simulator for simulations with cvar_alpha < 1"
 
         QAOABaseBackendStatevector.__init__(
             self,
             qaoa_descriptor,
@@ -282,17 +282,15 @@
             self.wavefn[0] = 1
             self.wavefn = self.wavefn.reshape([2] * self.n_qubits)
         else:
             self.wavefn = []
 
         # Handle prepend state
         if self.prepend_state is not None:
-
             if isinstance(self.prepend_state, np.ndarray):
-
                 if np.shape(self.prepend_state) == np.shape(self.wavefn):
                     self.wavefn = self.prepend_state
                 elif np.shape(self.prepend_state) == (2**self.n_qubits,):
                     self.wavefn = self.prepend_state.reshape([2] * self.n_qubits)
                 else:
                     raise ValueError(
                         "Error : Unsupported prepend_state specified."
@@ -302,19 +300,17 @@
             else:
                 raise ValueError(
                     "Error : Unsupported prepend_state specified. Not an ndarray."
                 )
 
         # Handle append state
         if self.append_state is not None:
-
             if isinstance(self.append_state, np.ndarray) and np.shape(
                 self.append_state
             ) == (2**self.n_qubits, 2**self.n_qubits):
-
                 # check unitarity of append_state matrix
                 if not np.allclose(
                     np.eye(2**self.n_qubits),
                     self.append_state.dot(self.append_state.conj().T),
                 ):
                     raise ValueError("append_state is not a unitary matrix")
 
@@ -329,14 +325,37 @@
             for i in range(self.n_qubits):
                 self.apply_hadamard(i)
 
         # store the initialisation part of wavefunction
         self.wavefn_init = copy(self.wavefn)
 
     # Apply gate methods
+    def apply_x(self, qubit_1: int):
+        r"""
+        Applies the X gate on ``qubit_1`` in a vectorized way.
+
+        Parameters
+        ----------
+        qubit_1:
+            Qubit index to apply gate.
+
+        Returns
+        -------
+            None
+        """
+
+        rotation_angle = np.pi
+        C = np.cos(rotation_angle / 2)
+        S = -1j * np.sin(rotation_angle / 2)
+        wfn = (C * self.wavefn) + (
+            S * np.flip(self.wavefn, self.n_qubits - qubit_1 - 1)
+        )
+
+        self.wavefn = wfn
+
     def apply_rx(self, qubit_1: int, rotation_angle: float):
         r"""
         Applies the RX($\theta$ = ``rotation_angle``) gate on ``qubit_1`` in a vectorized way.
         
         **Definition of RX($\theta$):**
 
         .. math::
@@ -818,15 +837,15 @@
             ``QAOAVariationalBaseParams`` object that contains rotation angles and gates to be applied.
 
         Returns
         -------
             None
         """
         gates_applicator = VectorizedGateApplicator()
-        
+
         # generate a job id for the wavefunction evaluation
         self.job_id = generate_uuid()
 
         # reset the wavefunction back to its initialisation state
         self.reset_circuit()
 
         # Assign angles and apply gates
@@ -838,22 +857,20 @@
 
         for each_tuple in low_level_gate_list:
             gate = each_tuple[0](gates_applicator, *each_tuple[1])
             gate.apply_gate(self)
 
         # Handle append state
         if self.append_state is not None:
-
             # Flatten (2,...,2) shaped wfn into a 2**n-dim column vector before multiplying with unitary matrix, ...
             self.wavefn = np.matmul(self.append_state, self.wavefn.flatten())
             # then re-shape it back to (2,...,2)
             self.wavefn = self.wavefn.reshape([2] * self.n_qubits)
 
     def wavefunction(self, params: Type[QAOAVariationalBaseParams] = None) -> list:
-
         """
         Get the wavefunction of the state produced by the parametric circuit.
 
         Parameters
         ----------
         params:
             The QAOA parameters - an object of one of the parameter classes, containing
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/derivatives/derivative_functions.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/derivative_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
         "Unknown derivative computation method specified - please choose between "
         + str(derivative_methods)
     )
 
     params = deepcopy(params)
 
     if derivative_type == "gradient":
-
         if derivative_method == "finite_difference":
             out = grad_fd(backend_obj, params, derivative_options, logger)
         elif derivative_method == "param_shift":
             assert (
                 params.__class__.__name__ == "QAOAVariationalStandardParams"
             ), f"{params.__class__.__name__} not supported - only Standard Parametrisation is supported for parameter shift/stochastic parameter shift for now."
             out = grad_ps(backend_obj, params, params_ext, derivative_options, logger)
@@ -203,15 +202,14 @@
                 logger,
                 stochastic=True,
             )
         elif derivative_method == "grad_spsa":
             out = grad_spsa(backend_obj, params, derivative_options, logger)
 
     elif derivative_type == "gradient_w_variance":
-
         if derivative_method == "finite_difference":
             out = grad_fd(
                 backend_obj, params, derivative_options, logger, variance=True
             )
         elif derivative_method == "param_shift":
             assert (
                 params.__class__.__name__ == "QAOAVariationalStandardParams"
@@ -239,15 +237,14 @@
             )
         elif derivative_method == "grad_spsa":
             out = grad_spsa(
                 backend_obj, params, derivative_options, logger, variance=True
             )
 
     elif derivative_type == "hessian":
-
         if derivative_method == "finite_difference":
             out = hessian_fd(backend_obj, params, derivative_options, logger)
         else:
             raise ValueError(
                 "Only support hessian derivative method is finite_difference. Your choice: {}".format(
                     derivative_method
                 )
@@ -494,15 +491,14 @@
         Callable derivative function.
     """
 
     # Set default value of eta
     eta = gradient_options["stepsize"]
 
     def grad_fd_func(args, n_shots=None):
-
         # get the function to compute the gradient and its variance
         __gradient_function = __gradient(args, backend_obj, params, logger, variance)
 
         # if n_shots is int or None create a list with len of args
         # (if it is none, it will use the default n_shots)
         n_shots_list = __create_n_shots_list(len(args), n_shots)
 
@@ -598,15 +594,14 @@
     # with the `n_associated_params` list, add a 0 in the first position and
     # sum the list cumulatively (so that this list indicate which gate is associated with which coefficient)
     l = np.insert(
         np.cumsum(n_associated_params), 0, 0
     )  # the i-th coefficient is associated with extended parameters with indices in range [l[i], l[i+1]]
 
     def grad_ps_func(args, n_shots=None):
-
         # Convert standard to extended parameters before applying parameter shift
         args_ext = params.convert_to_ext(args)
 
         # get the function to compute the gradient and its variance
         __gradient_function = __gradient(
             args_ext, backend_obj, params_ext, logger, variance
         )
@@ -749,15 +744,14 @@
     grad_spsa_func: `Callable`
         Callable derivative function.
 
     """
     eta = gradient_options["stepsize"]
 
     def grad_spsa_func(args, n_shots=None):
-
         # if variance is True, add the number of shots per argument to the logger
         if variance:
             logger.log_variables({"n_shots": [n_shots]})
 
         # get the function to compute the gradient and its variance
         __gradient_function = __gradient(args, backend_obj, params, logger, variance)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/derivatives/qfim.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/derivatives/qfim.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from ..optimizers.logger_vqa import Logger
 from ..qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
 
 
 def log_qfim_evals(logger: Logger) -> Logger:
-
     current_total_eval = logger.func_evals.best[0]
     current_total_eval += 1
     current_qfim_eval = logger.qfim_func_evals.best[0]
     current_qfim_eval += 1
     logger.log_variables(
         {"func_evals": current_total_eval, "qfim_func_evals": current_qfim_eval}
     )
@@ -24,15 +23,14 @@
 
 def qfim(
     backend_obj: QAOABaseBackend,
     params: QAOAVariationalBaseParams,
     logger: Logger,
     eta: float = 0.00000001,
 ):
-
     """
     Returns a callable qfim_fun(args) that computes the
     Quantum Fisher Information Matrix at `args` according to :
     $$[QFI]_{ij} = Re(<∂iφ|∂jφ>) − <∂iφ|φ><φ|∂jφ>$$.
 
     Parameters
     ----------
@@ -60,15 +58,14 @@
     log_qfim_evals(logger)
 
     qfim_array = np.zeros((len(params), len(params)))
 
     copied_params = deepcopy(params)
 
     def qfim_fun(args):
-
         for i in range(len(args)):
             for j in range(i + 1):
                 vi, vj = np.zeros(len(args)), np.zeros(len(args))
                 vi[i] = eta
                 vj[j] = eta
 
                 copied_params.update_from_raw(args + vi)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/logger_vqa.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/logger_vqa.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,105 +6,93 @@
 import networkx as nx
 
 
 class UpdateMethod(ABC):
     @classmethod
     @abstractmethod
     def update(self):
-
         pass
 
 
 class LoggerVariable(object):
     def __init__(
         self,
         attribute_name: str,
         history_update_method: UpdateMethod,
         best_update_method: UpdateMethod,
     ):
-
         self.name = attribute_name
         self.best = []
         self.history = []
 
         self.history_update_method = history_update_method
         self.best_update_method = best_update_method
 
     def update(self, new_value):
-
         self.update_history(new_value)
         self.update_best(new_value)
 
     def update_history(self, new_value):
-
         return self.history_update_method.update(self, "history", new_value)
 
     def update_best(self, new_value):
-
         return self.best_update_method.update(self, "best", new_value)
 
 
 class AppendValue(UpdateMethod):
     def update(
         self, attribute_name: str, new_value: Union[list, int, float, str]
     ) -> None:
-
         get_var = getattr(self, attribute_name)
         get_var.append(new_value)
         setattr(self, attribute_name, get_var)
 
 
 class ReplaceValue(UpdateMethod):
     def update(
         self, attribute_name: str, new_value: Union[list, int, float, str]
     ) -> None:
-
         setattr(self, attribute_name, [new_value])
 
 
 class EmptyValue(UpdateMethod):
     def update(
         self, attribute_name: str, new_value: Union[list, int, float, str]
     ) -> None:
-
         setattr(self, attribute_name, [])
 
 
 class IfLowerDo(UpdateMethod):
     def __init__(self, update_method: UpdateMethod):
-
         self._update_method = update_method
 
     def update(
         self,
         logger_variable: LoggerVariable,
         attribute_name: str,
         new_value: Union[int, float],
     ) -> None:
-
         try:
             old_value = getattr(logger_variable, attribute_name)[-1]
             if new_value < old_value:
                 self._update_method.update(logger_variable, attribute_name, new_value)
         except IndexError:
             AppendValue.update(logger_variable, attribute_name, new_value)
 
 
 class IfHigherDo(UpdateMethod):
     def __init__(self, update_method: UpdateMethod):
-
         self._update_method = update_method
 
     def update(
         self,
         logger_variable: LoggerVariable,
         attribute_name: str,
         new_value: Union[int, float],
     ) -> None:
-
         try:
             old_value = getattr(logger_variable, attribute_name)[-1]
             if new_value > old_value:
                 self._update_method.update(logger_variable, attribute_name, new_value)
         except IndexError:
             AppendValue.update(logger_variable, attribute_name, new_value)
 
@@ -125,39 +113,36 @@
         "Append": AppendValue,
     }
 
     @classmethod
     def create_logger_variable(
         self, attribute_name: str, history_update_bool: bool, best_update_string: str
     ) -> LoggerVariable:
-
         history_update_method = self.history_bool_mapping[str(history_update_bool)]
         best_update_method = self.best_string_mapping[best_update_string]
 
         return LoggerVariable(attribute_name, history_update_method, best_update_method)
 
 
 class Logger(object):
     def __init__(self, initialisation_variables: dict, logger_update_structure: dict):
-
         for attribute_name, attribute_properties in initialisation_variables.items():
             self._create_variable(
                 attribute_name=attribute_name,
                 history_update_bool=attribute_properties["history_update_bool"],
                 best_update_string=attribute_properties["best_update_string"],
             )
         self._create_logger_update_structure(
             logger_update_structure["root_nodes"],
             logger_update_structure["best_update_structure"],
         )
 
     def _create_variable(
         self, attribute_name: str, history_update_bool: bool, best_update_string: str
     ):
-
         """
         If a variable was created was this method, ensure that the logger update
         strucuture is updated to include the new variable. Else the best value
         of the new variable will not be updated.
         """
 
         setattr(
@@ -167,15 +152,14 @@
                 attribute_name, history_update_bool, best_update_string
             ),
         )
 
     def _create_logger_update_structure(
         self, root_nodes: List[str], best_update_relations: Tuple[List[str]]
     ):
-
         """
         This method creates an internal representation based on the way in which
         the Logger Variables should be updated using a NetworkX Directed Graph.
 
         Parameter
         ---------
         root_nodes: `list`
@@ -190,40 +174,35 @@
         self.best_update_structure = nx.DiGraph()
 
         self.root_nodes = root_nodes
         self.update_edges = best_update_relations
 
     @property
     def update_edges(self):
-
         return self._update_edges
 
     @update_edges.setter
     def update_edges(self, update_edges: Tuple[List[str]]):
-
         self.best_update_structure.add_edges_from(update_edges)
         self._update_edges = update_edges
 
         return self._update_edges
 
     @property
     def root_nodes(self):
-
         return self._root_nodes
 
     @root_nodes.setter
     def root_nodes(self, root_nodes: List[str]):
-
         self.best_update_structure.add_nodes_from(root_nodes)
         self._root_nodes = root_nodes
 
         return self._root_nodes
 
     def log_variables(self, input_dict: dict):
-
         """
         Updates all the histories of the logger variables.
         Best values of the logger variables are only updated according to the rules
         specified by its update structure. If the attribute is not in the update
         structure it isnt updated.
 
         input_dict:
@@ -237,18 +216,16 @@
 
         # Updates based on best_update_structure, the networkx graph.
         change_dict = dict()
 
         node_list = deepcopy(self.root_nodes)
 
         while len(node_list) != 0:
-
             mid_list = []
             for each_node in node_list:
-
                 change_bool = False
 
                 # Checks if a nodes predecessor has been updated. If not all
                 # of them were updated, the node is skipped.
                 node_predecessor = self.best_update_structure.pred[each_node]
                 updated_pred_count = np.sum(
                     [
@@ -279,15 +256,13 @@
                 # was changed.
                 if change_bool == True:
                     mid_list.extend(self.best_update_structure.adj[each_node].keys())
 
             node_list = list(set(mid_list))
 
     def _log_history(self, attribute_name: str, attribute_value):
-
         attr_to_update = getattr(self, attribute_name)
         attr_to_update.update_history(attribute_value)
 
     def _log_best(self, attribute_name: str, attribute_value):
-
         attr_to_update = getattr(self, attribute_name)
         attr_to_update.update_best(attribute_value)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/CANS.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/CANS.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     coeffs=None,
     maxiter=100,
     tol=10 ** (-6),
     jac_w_variance=None,
     callback=None,
     **options
 ):
-
     # check that the stepsize is small enough
     lipschitz = np.sum(np.abs(coeffs))
     if not stepsize < 2 / lipschitz:
         raise ValueError(
             "Stepsizec is bigger than 2/Lipschitz: it should be smaller than {0:.3g}".format(
                 2 / lipschitz
             )
@@ -45,15 +44,14 @@
     improved = True
     stop = False
 
     testx = np.copy(bestx)
     testy = besty
 
     while improved and not stop and niter < maxiter:
-
         # compute gradient and variance
         gradient, variance, n_shots_used = jac_w_variance(testx, n_shots=n_shots)
 
         # compute gradient descent step
         testx = testx - stepsize * gradient
         testy = np.real(fun(testx, *args))
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/SPSA.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/SPSA.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/iCANS.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/iCANS.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     coeffs=None,
     maxiter=100,
     tol=10 ** (-6),
     jac_w_variance=None,
     callback=None,
     **options
 ):
-
     # check that the stepsize is small enough
     lipschitz = np.sum(np.abs(coeffs))
     if not stepsize < 2 / lipschitz:
         raise ValueError(
             "Stepsizec is bigger than 2/Lipschitz: it should be smaller than {0:.3g}".format(
                 2 / lipschitz
             )
@@ -45,15 +44,14 @@
     improved = True
     stop = False
 
     testx = np.copy(bestx)
     testy = besty
 
     while improved and not stop and niter < maxiter:
-
         # compute gradient and variance
         gradient, variance, n_shots_used = jac_w_variance(testx, n_shots=list(n_shots))
 
         # compute gradient descent step
         testx = testx - stepsize * gradient
         testy = np.real(fun(testx, *args))
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/natural_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/newton_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/rmsprop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/optimization_methods/stochastic_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 """
 
 from .pennylane_optimizers import *
 from . import numpy
 from . import math
 from . import fourier
 
+
 # empty class to be used as a placeholder for the QNode class from PennyLane
 class QNode:
     def __init__(self):
         pass
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/fourier/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/fourier/reconstruct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
     # Extract the Fourier coefficients
     R = (L - 1) // 2
     a0 = W[0]
     a = anp.asarray(W[1 : R + 1], like=interface)
     b = anp.asarray(W[R + 1 :], like=interface)
 
     x0 = anp.asarray(np.float64(0.0), like=interface) if x0 is None else x0
+
     # Construct the Fourier series
     def _reconstruction(x):
         """Univariate reconstruction based on arbitrary shifts."""
         x = x - x0
         return (
             a0
             + qml.math.tensordot(qml.math.cos(spectrum * x), a, axes=[[0], [0]])
@@ -312,15 +313,14 @@
         jobs = {}
 
         # If no shifts are provided, compute them
         for arg_name, inner_dict in ids.items():
             _jobs = {}
 
             for par_idx in inner_dict:
-
                 # Determine spectrum and number of frequencies, discounting for 0
                 _spectrum = spectra[arg_name][par_idx]
                 R = len(_spectrum) - 1
                 _shifts, need_f0 = _parse_shifts(
                     shifts, R, arg_name, par_idx, atol, need_f0
                 )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/is_independent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/is_independent.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     else:
         np.random.seed(seed)
         rnd_args = [
             tuple(np.random.random(np.shape(arg)) * width + bounds[0] for arg in args)
             for _ in range(num)
         ]
         if interface == "autograd":
-
             # Mark the arguments as trainable with Autograd
             rnd_args = [
                 tuple(pnp.array(a, requires_grad=True) for a in arg) for arg in rnd_args
             ]
 
     return rnd_args
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/matrix_manipulation.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/multi_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/quantum.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/quantum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/single_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/utils.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/math/utils.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/fft.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/random.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/random.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from autograd.core import VSpace
 
 
 __doc__ = (
     "NumPy with automatic differentiation support, provided by Autograd and PennyLane."
 )
 
+
 # Hotfix since _np.asarray doesn't have a gradient rule defined.
 @primitive
 def asarray(vals, *args, **kwargs):
     """Gradient supporting autograd asarray"""
     if isinstance(vals, (onp.ndarray, _np.ndarray)):
         return _np.asarray(vals, *args, **kwargs)
     return _np.array(vals, *args, **kwargs)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/numpy/wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/optimization_methods_pennylane.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     jac=None,
     callback=None,
     nums_frequency=None,
     spectra=None,
     shifts=None,
     **options
 ):
-
     """
     Minimize a function `fun` using some pennylane method.
     To check available methods look at the available_methods_dict variable.
     Read https://docs.pennylane.ai/en/stable/introduction/interfaces.html#optimizers
 
     PARAMETERS
     ----------
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/adagrad.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
         if self.accumulation is None:
             self.accumulation = [0.0] * len(args)
 
         trained_index = 0
         for index, arg in enumerate(args):
             if getattr(arg, "requires_grad", False):
-
                 self._update_accumulation(index, grad[trained_index])
 
                 coeff = self.stepsize / sqrt(self.accumulation[index] + self.eps)
                 args_new[index] = arg - coeff * grad[trained_index]
 
                 trained_index += 1
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             * sqrt(1 - self.beta2 ** self.accumulation["t"])
             / (1 - self.beta1 ** self.accumulation["t"])
         )
 
         trained_index = 0
         for index, arg in enumerate(args):
             if getattr(arg, "requires_grad", False):
-
                 self._update_accumulation(index, grad[trained_index])
                 args_new[index] = arg - new_stepsize * self.accumulation["fm"][
                     index
                 ] / (sqrt(self.accumulation["sm"][index]) + self.eps)
 
                 trained_index += 1
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/momentum.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
         if self.accumulation is None:
             self.accumulation = [0.0] * len(args)
 
         trained_index = 0
         for index, arg in enumerate(args):
             if getattr(arg, "requires_grad", False):
-
                 self._update_accumulation(index, grad[trained_index])
                 args_new[index] = arg - self.accumulation[index]
 
                 trained_index += 1
 
         return args_new
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/rms_prop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/rotosolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     pennylane as qml,
 )  # changed from the original PennyLane code
 
 
 def _brute_optimizer(fun, num_steps, bounds=None, **kwargs):
     r"""Brute force optimizer, wrapper of scipy.optimize.brute that repeats it
     ``num_steps`` times. Signature is as expected by ``RotosolveOptimizer._min_numeric``
-    below, returning a scalar minimal position and the function value at that position."""
+    below, returning a scalar minimal position and the function value at that position.
+    """
     Ns = kwargs.pop("Ns")
     width = bounds[0][1] - bounds[0][0]
     center = (bounds[0][1] + bounds[0][0]) / 2
     for _ in range(num_steps):
         range_ = (center - width / 2, center + width / 2)
         center, y_min, *_ = brute(
             fun, ranges=(range_,), full_output=True, Ns=Ns, **kwargs
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/pennylane/pennylane_optimizers/spsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         A (float): The stability constant; if not provided, set to be 10% of the maximum number
             of expected iterations.
         a (float): A hyperparameter expected to be small in noisy situations,
             its value could be picked using `A`, :math:`\alpha` and :math:`\hat{g_0} (\hat{\theta_0})`.
             For more details, see `Spall (1998b)
             <https://www.jhuapl.edu/spsa/PDF-SPSA/Spall_Implementation_of_the_Simultaneous.PDF>`_.
     """
+
     # pylint: disable-msg=too-many-arguments
     def __init__(self, maxiter=None, alpha=0.602, gamma=0.101, c=0.2, A=None, a=None):
         self.a = a
         self.A = A
         if not maxiter and not A:
             raise TypeError("One of the parameters maxiter or A must be provided.")
         if not A:
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/qaoa_optimizer.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/qaoa_optimizer.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/optimizers/training_vqa.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/optimizers/training_vqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # TODO: Find better place for this
 
 import pandas as pd
 from typing import Any
 
 
 def save_parameter(parameter_name: str, parameter_value: Any):
-
     filename = "oq_saved_info_" + parameter_name
 
     try:
         opened_csv = pd.read_csv(filename + ".csv")
     except Exception:
         opened_csv = pd.DataFrame(columns=[parameter_name])
 
@@ -92,15 +91,14 @@
 
     def __init__(
         self,
         vqa_object: Type[VQABaseBackend],
         variational_params: Type[QAOAVariationalBaseParams],
         optimizer_dict: dict,
     ):
-
         if not isinstance(vqa_object, VQABaseBackend):
             raise TypeError(f"The specified cost object must be of type VQABaseBackend")
 
         self.vqa = vqa_object
         # extract initial parameters from the params of vqa_object
         self.variational_params = variational_params
         self.initial_params = variational_params.raw()
@@ -358,15 +356,14 @@
 
     def __init__(
         self,
         vqa_object: Type[VQABaseBackend],
         variational_params: Type[QAOAVariationalBaseParams],
         optimizer_dict: dict,
     ):
-
         super().__init__(vqa_object, variational_params, optimizer_dict)
 
         self.vqa_object = vqa_object
         self._validate_and_set_params(optimizer_dict)
 
     def _validate_and_set_params(self, optimizer_dict):
         """
@@ -509,15 +506,15 @@
                     bounds=self.bounds,
                 )
         except ConnectionError as e:
             print(e, "\n")
             print(
                 "The optimization has been terminated early. Most likely due to a connection error."
                 "You can retrieve results from the optimization runs that were completed"
-                "through the .results_information method."
+                "through the .result method."
             )
         except Exception as e:
             raise e
         finally:
             self.results_dictionary()
 
         return self
@@ -566,15 +563,14 @@
 
     def __init__(
         self,
         vqa_object: Type[VQABaseBackend],
         variational_params: Type[QAOAVariationalBaseParams],
         optimizer_dict: dict,
     ):
-
         super().__init__(vqa_object, variational_params, optimizer_dict)
 
         self.vqa_object = vqa_object
         self._validate_and_set_params(optimizer_dict)
 
     def _validate_and_set_params(self, optimizer_dict):
         """
@@ -732,15 +728,15 @@
                     bounds=self.bounds,
                 )
         except ConnectionError as e:
             print(e, "\n")
             print(
                 "The optimization has been terminated early. Most likely due to a connection error."
                 "You can retrieve results from the optimization runs that were completed"
-                "through the .results_information method."
+                "through the .result method."
             )
         except Exception as e:
             raise e
         finally:
             self.results_dictionary()
 
         return self
@@ -780,15 +776,14 @@
 
     def __init__(
         self,
         vqa_object: Type[VQABaseBackend],
         variational_params: Type[QAOAVariationalBaseParams],
         optimizer_dict: dict,
     ):
-
         super().__init__(vqa_object, variational_params, optimizer_dict)
 
         self.vqa_object = vqa_object
         self._validate_and_set_params(optimizer_dict)
 
     def _validate_and_set_params(self, optimizer_dict):
         """
@@ -894,15 +889,15 @@
                 bounds=self.bounds,
             )
         except ConnectionError as e:
             print(e, "\n")
             print(
                 "The optimization has been terminated early. Most likely due to a connection error."
                 "You can retrieve results from the optimization runs that were completed"
-                "through the .results_information method."
+                "through the .result method."
             )
         except Exception as e:
             raise e
         finally:
             self.results_dictionary()
 
         return self
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/binpacking.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/binpacking.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union
 from docplex.mp.model import Model
 
 from .problem import Problem
 from .converters import FromDocplex2IsingModel
 from .qubo import QUBO
 
+
 class BinPacking(Problem):
     """
     Creates an instance of the bin packing problem.
     https://en.wikipedia.org/wiki/Bin_packing_problem
 
     Parameters
     ----------
@@ -40,18 +41,22 @@
         # include_ineqs: True if including the inequalities
         if method not in ["slack", "unbalanced"]:
             raise ValueError(
                 f"The method '{method}' is not a valid method. Choose between 'slack' and 'unbalanced'"
             )
         for weight in weights:
             if int(weight) != weight:
-                raise TypeError(f"The weights must be integer numbers. Format {type(weight)} found.")
-        
+                raise TypeError(
+                    f"The weights must be integer numbers. Format {type(weight)} found."
+                )
+
         if int(weight_capacity) != weight_capacity:
-            raise TypeError(f"The weight_capacity must be integer. Format {type(weight_capacity)} found.")
+            raise TypeError(
+                f"The weight_capacity must be integer. Format {type(weight_capacity)} found."
+            )
         self.weights = [int(weight) for weight in weights]
         self.weight_capacity = weight_capacity
         self.penalty = penalty
         self.n_items = len(weights)
         self.method = method
         self.simplifications = simplifications
         if n_bins is None:
@@ -67,15 +72,15 @@
         y_{j} -> represents if bin j is used
         x_{i}_{j} -> represent if item i is in bin j
 
         Returns
         -------
         solution : dict
         Dictionary with keys equal to the variables of the problem and values 0, 1, or None
-        None for those values to be optimized otherwise the simplifications that can be 
+        None for those values to be optimized otherwise the simplifications that can be
         used in this problem.
 
         """
         solution = {f"y_{j}": -1 for j in range(self.n_bins)}
         for i in range(self.n_items):
             for j in range(self.n_bins):
                 solution[f"x_{i}_{j}"] = -1
@@ -147,15 +152,15 @@
         vars_pos = {var.name: n for n, var in enumerate(mdl.iter_binary_vars())}
 
         mdl.minimize(objective)
         if self.simplifications:
             list_items = range(1, self.n_items)
         else:
             list_items = range(self.n_items)
-            
+
         eq_constraints = {}
         ineq_constraints = {}
         for i in list_items:
             # First set of constraints: the items must be in any bin
             eq_constraints[f"eq_{i}"] = [
                 [vars_pos[f"x_{i}_{j}"] for j in range(self.n_bins)],
                 [1],
@@ -221,17 +226,20 @@
                 qubo_docplex = FromDocplex2IsingModel(cplex_model)
             elif self.method == "unbalanced":
                 qubo_docplex = FromDocplex2IsingModel(
                     cplex_model, unbalanced_const=True
                 )
 
         ising_model = qubo_docplex.ising_model
-        return QUBO(n_vars, ising_model.terms+[[]],
-                    ising_model.weights + [ising_model.constant],
-                    self.problem_instance)
+        return QUBO(
+            n_vars,
+            ising_model.terms + [[]],
+            ising_model.weights + [ising_model.constant],
+            self.problem_instance,
+        )
 
     def classical_solution(self, string: bool = False):
         """
         Return the classical solution of the bin packing problem
 
         Parameters
         ----------
@@ -249,17 +257,15 @@
             The classical solution of the specific problem as a string or a dict.
 
         """
         cplex_model = self.docplex_model
         docplex_sol = cplex_model.solve()
 
         if docplex_sol is None:
-            raise ValueError(
-                f"solution not found: {cplex_model.solve_details.status}"
-            )
+            raise ValueError(f"solution not found: {cplex_model.solve_details.status}")
 
         if string:
             solution = ""
         else:
             solution = self.solution.copy()
         for var in cplex_model.iter_binary_vars():
             if string:
@@ -283,14 +289,15 @@
         -------
         fig : matplotlib.pyplot.Figure()
             The plot visualization of the solution.
 
         """
         import matplotlib.pyplot as plt
         from matplotlib import colormaps
+
         cplex_model = self.docplex_model
         if isinstance(solution, str):
             sol = self.solution.copy()
             for n, var in enumerate(cplex_model.iter_binary_vars()):
                 sol[var.name] = int(solution[n])
             solution = sol
         colors = colormaps["jet"]
@@ -304,15 +311,15 @@
                 for i in range(self.n_items):
                     if solution[f"x_{i}_{j}"]:
                         ax.bar(
                             j,
                             self.weights[i],
                             bottom=sum_items,
                             label=f"item {i}",
-                            color=colors(i/self.n_items),
+                            color=colors(i / self.n_items),
                             alpha=0.7,
                             edgecolor="black",
                         )
                         sum_items += self.weights[i]
         ax.hlines(
             self.weight_capacity,
             -0.5,
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/converters.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/helper_functions.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/helper_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .minimumvertexcover import MinimumVertexCover
 from .numberpartition import NumberPartition
 from .shortestpath import ShortestPath
 from .tsp import TSP
 from .vehiclerouting import VRP
 from .maximalindependentset import MIS
 from .binpacking import BinPacking
+from .portfoliooptimization import PortfolioOptimization
 from .qubo import QUBO
 
 
 def create_problem_from_dict(problem_instance: dict) -> Problem:
     """
     Creates an object of the class corresponding to the problem type
     in the input instance, with the same attributes as the input instance.
@@ -41,14 +42,15 @@
         "knapsack": Knapsack,
         "slack_free_knapsack": SlackFreeKnapsack,
         "minimum_vertex_cover": MinimumVertexCover,
         "shortest_path": ShortestPath,
         "vehicle_routing": VRP,
         "maximal_independent_set": MIS,
         "bin_packing": BinPacking,
+        "portfolio_optimization": PortfolioOptimization,
     }
 
     # check if the problem type is in the mapper
     assert (
         problem_instance["problem_type"] in problem_mapper
     ), f"Problem type {problem_instance['problem_type']} not supported."
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/knapsack.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/knapsack.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
     @property
     def values(self):
         return self._values
 
     @values.setter
     def values(self, input_values):
-
         if not isinstance(input_values, list):
             raise TypeError("The input parameter, values, has to be a list")
 
         for each_entry in input_values:
             if not isinstance(each_entry, int):
                 raise TypeError("The elements in values list must be of type int.")
 
@@ -57,15 +56,14 @@
 
     @property
     def weights(self):
         return self._weights
 
     @weights.setter
     def weights(self, input_weights):
-
         if not isinstance(input_weights, list):
             raise TypeError("The input parameter, weights, has to be a list")
 
         for each_entry in input_weights:
             if not isinstance(each_entry, int):
                 raise TypeError("The elements in weights list must be of type int.")
 
@@ -73,15 +71,14 @@
 
     @property
     def weight_capacity(self):
         return self._weight_capacity
 
     @weight_capacity.setter
     def weight_capacity(self, input_weight_capacity):
-
         if not isinstance(input_weight_capacity, int):
             raise TypeError(
                 "The input parameter, weight_capacity, has to be of type int"
             )
 
         if input_weight_capacity <= 0:
             raise TypeError(
@@ -92,15 +89,14 @@
 
     @property
     def penalty(self):
         return self._penalty
 
     @penalty.setter
     def penalty(self, input_penalty):
-
         if not isinstance(input_penalty, int) and not isinstance(input_penalty, float):
             raise TypeError(
                 "The input parameter, penalty, has to be of type float or int"
             )
 
         self._penalty = input_penalty
 
@@ -256,15 +252,14 @@
     -------
         An instance of the SlackFreeKnapsack problem.
     """
 
     __name__ = "slack_free_knapsack"
 
     def __init__(self, values, weights, weight_capacity, penalty):
-
         super().__init__(values, weights, weight_capacity, penalty)
 
     @staticmethod
     def random_instance(**kwargs):
         """
         Creates a random instance of the Knapsack problem.
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/maximalindependentset.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/maximalindependentset.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,37 +14,36 @@
     """
     Creates an instance of the maximal independent set (MIS) problem.
     https://en.wikipedia.org/wiki/Maximal_independent_set
 
     Parameters
     ----------
     G: networkx.Graph
-        Networkx graph of the problem 
+        Networkx graph of the problem
     penalty: float
         Penalty for the edge constraints.
 
     Returns
     -------
         An instance of the MIS problem.
     """
 
     __name__ = "maximal_independent_set"
 
-    def __init__(self, G, penalty:Union[int, float]=2):
+    def __init__(self, G, penalty: Union[int, float] = 2):
         self.G = G
         self.penalty = penalty
         # self.cplex_model = self.docplex_model()
 
     @property
     def G(self):
         return self._G
 
     @G.setter
     def G(self, input_networkx_graph):
-
         if not isinstance(input_networkx_graph, nx.Graph):
             raise TypeError("Input problem graph must be a networkx Graph.")
 
         # Relabel nodes to integers starting from 0
         mapping = dict(
             zip(input_networkx_graph, range(input_networkx_graph.number_of_nodes()))
         )
@@ -78,37 +77,42 @@
         G = nx.generators.random_graphs.fast_gnp_random_graph(
             n=n_nodes, p=edge_probability, seed=seed
         )
         return MIS(G)
 
     @property
     def docplex_model(self):
-        mdl = Model('MIS')
+        mdl = Model("MIS")
         num_vertices = self.G.number_of_nodes()
 
         x = {i: mdl.binary_var(name=f"x_{i}") for i in range(num_vertices)}
 
-        mdl.minimize(-mdl.sum(x) + self.penalty * mdl.sum(
-            x[i] * x[j] for (i, j) in self.G.edges
-        ))
+        mdl.minimize(
+            -mdl.sum(x) + self.penalty * mdl.sum(x[i] * x[j] for (i, j) in self.G.edges)
+        )
         return mdl
 
     @property
     def qubo(self):
         """
         Returns the QUBO encoding of this problem.
 
         Returns
         -------
             The QUBO encoding of this problem.
         """
         cplex_model = self.docplex_model
         qubo_docplex = FromDocplex2IsingModel(cplex_model).ising_model
-        
-        return QUBO(self.G.number_of_nodes(), qubo_docplex.terms + [[]], qubo_docplex.weights + [qubo_docplex.constant], self.problem_instance)
+
+        return QUBO(
+            self.G.number_of_nodes(),
+            qubo_docplex.terms + [[]],
+            qubo_docplex.weights + [qubo_docplex.constant],
+            self.problem_instance,
+        )
 
     def classical_solution(self, string: bool = False):
         """
         Return the classical solution of the maximal independent set problem
         Parameters
         ----------
         string : bool, optional
@@ -163,11 +167,28 @@
         colors = ["#5EB1EB", "#F29D55"]
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
         pos = nx.circular_layout(self.G)
         num_vertices = self.G.number_of_nodes()
-        nx.draw(self.G, pos=pos, edgecolors="black", labels={i:str(i) for i in range(num_vertices)}, node_color=[colors[solution[f"x_{i}"]] for i in range(num_vertices)], ax=ax, edge_color="#0B2340")
-        ax.plot([],[], marker="o", markersize=10, label="MIS", linewidth=0,color=colors[1], markeredgecolor="black")
+        nx.draw(
+            self.G,
+            pos=pos,
+            edgecolors="black",
+            labels={i: str(i) for i in range(num_vertices)},
+            node_color=[colors[solution[f"x_{i}"]] for i in range(num_vertices)],
+            ax=ax,
+            edge_color="#0B2340",
+        )
+        ax.plot(
+            [],
+            [],
+            marker="o",
+            markersize=10,
+            label="MIS",
+            linewidth=0,
+            color=colors[1],
+            markeredgecolor="black",
+        )
         ax.legend(loc="upper center", bbox_to_anchor=[0.5, 1.1])
         return fig
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/maximumcut.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/maximumcut.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,24 +20,22 @@
     """
 
     __name__ = "maximum_cut"
 
     DEFAULT_EDGE_WEIGHT = 1.0
 
     def __init__(self, G):
-
         self.G = G
 
     @property
     def G(self):
         return self._G
 
     @G.setter
     def G(self, input_networkx_graph):
-
         if not isinstance(input_networkx_graph, nx.Graph):
             raise TypeError("Input problem graph must be a networkx Graph.")
 
         # Relabel nodes to integers starting from 0
         mapping = dict(
             zip(input_networkx_graph, range(input_networkx_graph.number_of_nodes()))
         )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/minimumvertexcover.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/minimumvertexcover.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,24 @@
     -------
     An instance of the Minimum Vertex Cover problem.
     """
 
     __name__ = "minimum_vertex_cover"
 
     def __init__(self, G, field, penalty):
-
         self.G = G
         self.field = field
         self.penalty = penalty
 
     @property
     def G(self):
         return self._G
 
     @G.setter
     def G(self, input_networkx_graph):
-
         if not isinstance(input_networkx_graph, nx.Graph):
             raise TypeError("Input problem graph must be a networkx Graph.")
 
         # Relabel nodes to integers starting from 0
         mapping = dict(
             zip(input_networkx_graph, range(input_networkx_graph.number_of_nodes()))
         )
@@ -50,29 +48,27 @@
 
     @property
     def field(self):
         return self._field
 
     @field.setter
     def field(self, input_field):
-
         if not isinstance(input_field, int) and not isinstance(input_field, float):
             raise TypeError(
                 "The input parameter, field, has to be of type float or int"
             )
 
         self._field = input_field
 
     @property
     def penalty(self):
         return self._penalty
 
     @penalty.setter
     def penalty(self, input_penalty):
-
         if not isinstance(input_penalty, int) and not isinstance(input_penalty, float):
             raise TypeError(
                 "The input parameter, penalty, has to be of type float or int"
             )
 
         self._penalty = input_penalty
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/numberpartition.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/numberpartition.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
     @property
     def numbers(self):
         return self._numbers
 
     @numbers.setter
     def numbers(self, input_numbers):
-
         if not isinstance(input_numbers, list):
             raise TypeError("The input parameter, numbers, has to be a list")
 
         for each_entry in input_numbers:
             if not isinstance(each_entry, int):
                 raise TypeError("The elements in numbers list must be of type int.")
 
@@ -78,15 +77,14 @@
         terms = []
         weights = []
         constant_term = 0
 
         # Consider every pair of numbers (ordered)
         for i in range(self.n_numbers):
             for j in range(i, self.n_numbers):
-
                 # If i equals j, then whatever random sign we choose, if we square
                 # it we can back 1. So we have a constant term.
                 if i == j:
                     constant_term += self.numbers[i] * self.numbers[j]
 
                 # Otherwise the weight is computed as being the product of the
                 # numbers in the pair, multiplied by 2 (since we account for
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/portfoliooptimization.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/portfoliooptimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,16 +159,16 @@
         if string:
             solution = ""
         else:
             solution = {}
         for var in cplex_model.iter_binary_vars():
             if string:
                 # round is used because sometimes docplex gives the solution close to 1 but not 1,
-                #if we want to store this as an integer and use int(value) and the value is 0.999999
-                #it will store a zero.
+                # if we want to store this as an integer and use int(value) and the value is 0.999999
+                # it will store a zero.
                 solution += str(round(docplex_sol.get_value(var), 1))
             else:
                 solution[var.name] = round(docplex_sol.get_value(var), 1)
         return solution
 
     def plot_solution(self, solution, ax=None):
         G = nx.Graph()
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/problem.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/problem.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/qubo.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/qubo.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self,
         n,
         terms,
         weights,
         problem_instance: dict = {"problem_type": "generic_qubo"},
         clean_terms_and_weights=False,
     ):
-
         # check-type for terms and weights
         if not isinstance(terms, list) and not isinstance(terms, tuple):
             raise TypeError(
                 "The input parameter terms must be of type of list or tuple"
             )
 
         if not isinstance(weights, list) and not isinstance(weights, tuple):
@@ -111,15 +110,14 @@
 
     @property
     def n(self):
         return self._n
 
     @n.setter
     def n(self, input_n):
-
         if not isinstance(input_n, int):
             raise TypeError("The input parameter, n, has to be of type int")
 
         if input_n <= 0:
             raise TypeError(
                 "The input parameter, n, must be a positive integer greater than 0"
             )
@@ -211,15 +209,14 @@
         # Will record the weight for the unique terms (note that since Sets are
         # unhashable in Python, we use a dict with integers for the keys, that
         # are mapped with the corresponding indices of terms from unique_terms)
         new_weights_for_terms = defaultdict(float)
 
         # We do one pass over terms and weights
         for term, weight in zip(terms, weights):
-
             # Convert the term to a set
             term_set = set(term)
 
             # If this term is not yet recorded, we add it to the list of unique
             # terms and we use that it is the last element to find its index
             if term_set not in unique_terms:
                 unique_terms.append(term_set)
@@ -259,15 +256,14 @@
         """Convert QUBO terms and weights to their Ising equivalent"""
         ising_terms, ising_weights = [], []
         constant_term = 0
         linear_terms = np.zeros(n)
 
         # Process the given terms and weights
         for term, weight in zip(qubo_terms, qubo_weights):
-
             if len(term) == 2:
                 u, v = term
 
                 if u != v:
                     ising_terms.append([u, v])
                     ising_weights.append(weight / 4)
                 else:
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/shortestpath.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/shortestpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     -------
         An instance of the Shortest Path problem.
     """
 
     __name__ = "shortest_path"
 
     def __init__(self, G, source, dest):
-
         # Relabel nodes to integers starting from 0
         mapping = dict(zip(G, range(G.number_of_nodes())))
         self.G = nx.relabel_nodes(G, mapping)
 
         self.source = source
         self.dest = dest
 
@@ -69,15 +68,15 @@
         )
         G = nx.generators.random_graphs.fast_gnp_random_graph(
             n=n_nodes, p=edge_probability, seed=seed
         )
 
         DEFAULT_WEIGHTS = 1.0
 
-        for (u, v) in G.edges():
+        for u, v in G.edges():
             G.edges[u, v]["weight"] = DEFAULT_WEIGHTS
         for w in G.nodes():
             G.nodes[w]["weight"] = DEFAULT_WEIGHTS
 
         return ShortestPath(G, source, dest)
 
     def terms_and_weights(self):
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/tsp.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/tsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             G = G if G else nx.complete_graph(n_cities)
             if n_cities != len(G):
                 raise ValueError(
                     "Number of cities does not match the number of nodes in graph"
                 )
 
             # Set edge weights to be the distances between corresponding cities
-            for (u, v) in G.edges():
+            for u, v in G.edges():
                 G[u][v]["weight"] = distance_matrix[u, v]
 
         # Set number of cities
         self.n_cities = n_cities
 
         # Set the graph, making sure it is directed (useful when looping over edges during QUBO creation)
         self._G = nx.DiGraph(G)
@@ -173,15 +173,15 @@
             Graph encoding the connectivity between cities (can be directed)
 
         Returns
         -------
             None
         """
         # Set edge weights to be the distances between corresponding cities
-        for (u, v, weight) in G.edges(data="weight"):
+        for u, v, weight in G.edges(data="weight"):
             print(weight)
             if not isinstance(weight, float) and not isinstance(weight, int):
                 raise TypeError("The edge weights must be of type float or int")
 
             if weight < 0:
                 raise ValueError("Edge weights should be positive")
 
@@ -284,28 +284,28 @@
             for u in range(2, self.n_cities + 1):
                 for v in range(2, self.n_cities + 1):
                     interaction_terms.append(
                         ([get_variable_index(u, j), get_variable_index(v, j)], self.A)
                     )
 
         # Constraint which penalizes going through edges which are not part of the graph
-        for (u, v) in nx.complement(self.graph).edges():
+        for u, v in nx.complement(self.graph).edges():
             for j in range(1, self.n_cities + 1):
                 interaction_terms.append(
                     (
                         [
                             get_variable_index(u + 1, j),
                             get_variable_index(v + 1, j + 1),
                         ],
                         self.A,
                     )
                 )
 
         # Terms to account for the path cost
-        for (u, v) in self.graph.edges():
+        for u, v in self.graph.edges():
             for j in range(1, self.n_cities + 1):
                 interaction_terms.append(
                     (
                         [
                             get_variable_index(u + 1, j),
                             get_variable_index(v + 1, j + 1),
                         ],
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/problems/vehiclerouting.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/problems/vehiclerouting.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,22 +139,22 @@
         return VRP(
             G, pos, n_vehicles, subtours=subtours, method=method, penalty=penalty
         )
 
     @property
     def docplex_model(self):
         """
-        Return a docplex model of the vehicle routing problem using the linear 
-        programming approach. In this approach, the edges between different nodes 
-        of the graph are the variables of the problem. Therefore, x_i_j will represent 
+        Return a docplex model of the vehicle routing problem using the linear
+        programming approach. In this approach, the edges between different nodes
+        of the graph are the variables of the problem. Therefore, x_i_j will represent
         if the path between nodes i and j is selected. The idea is to minimize the distance
         traveled
-        
+
         sum_{i, j > i} r_{ij} x_{ij}.
-        
+
         where r_{ij} is the distance between nodes i and j (self.G.edges[i, j]["weight"]).
 
         Returns
         -------
         mdl : Model
             Docplex model of the Vehicle routing problem.
 
@@ -192,15 +192,15 @@
                     == 2 * self.n_vehicles
                 )
 
         if self.subtours == -1:
             # When subtours are not added, by default all the possible subtours are added.
             # However, it is really costly for large instances (above 10 nodes)
             list_subtours = [[i for i in range(num_nodes) if i != self.depot]]
-            for nodes in list_subtours: # costly for large instances
+            for nodes in list_subtours:  # costly for large instances
                 for i in range(3, num_nodes - 2 * self.n_vehicles):
                     for subtour in itertools.combinations(nodes, i):
                         tour = sorted(subtour)
                         n_subtour = len(subtour)
                         mdl.add_constraint(
                             mdl.sum(
                                 [
@@ -225,15 +225,17 @@
                                 for i in range(n_subtour)
                                 for j in range(i + 1, n_subtour)
                             ]
                         )
                         <= n_subtour - 1
                     )
         else:
-            raise ValueError(f"{type(self.subtour)} is not a valid format for the subtours.")
+            raise ValueError(
+                f"{type(self.subtour)} is not a valid format for the subtours."
+            )
         return mdl
 
     @property
     def qubo(self):
         """
         Returns the QUBO encoding of this problem.
 
@@ -355,15 +357,17 @@
                         break
                 max_edges -= 1
                 if max_edges < 0:
                     raise ValueError("The subtours in the solution are broken.")
             i += 1
         return {"paths": paths, "subtours": subtours}
 
-    def plot_solution(self, solution: Union[dict, str], ax=None, edge_width=4, colors=None):
+    def plot_solution(
+        self, solution: Union[dict, str], ax=None, edge_width=4, colors=None
+    ):
         """
         A visualization method for the vehicle routing problem solution.
         Parameters
         ----------
         solution : Union[dict, str]
             The solution of the specific vehicle routing problem as a string or dictionary.
         ax : matplotlib axes, optional
@@ -372,16 +376,18 @@
         -------
         fig : matplotlib.pyplot.Figure()
             The graph visualization of the solution.
         """
 
         colors = colormaps["jet"] if colors is None else colors
         if type(colors) is list and len(colors) != self.n_vehicles:
-            raise ValueError(f"The length of colors {len(colors)} and the number of vehicles {self.n_vehicles} do not match")
-            
+            raise ValueError(
+                f"The length of colors {len(colors)} and the number of vehicles {self.n_vehicles} do not match"
+            )
+
         if isinstance(solution, str):
             sol = {}
             for n, var in enumerate(self.docplex_model.iter_binary_vars()):
                 sol[var.name] = int(solution[n])
             solution = sol
         paths_and_subtours = self.paths_subtours(solution)
         paths = paths_and_subtours["paths"]
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/baseparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 from abc import ABC, abstractproperty
-from typing import List, Union, Tuple, Any, Callable, Iterable, Optional
+from typing import List, Union, Tuple, Any, Callable, Iterable, Optional, TYPE_CHECKING
+if TYPE_CHECKING:
+    from ...backends.basedevice import DeviceBase
 import numpy as np
 from enum import Enum
 import copy
 
 from .operators import Hamiltonian
 from .hamiltonianmapper import HamiltonianMapper
-from .gatemap import RotationGateMap, SWAPGateMap
+from .gatemap import RotationGateMap, SWAPGateMap, GateMap
 from .gatemaplabel import GateMapType
 
 
+
+
 def _is_iterable_empty(in_iterable):
     if isinstance(in_iterable, Iterable):  # Is Iterable
         return all(map(_is_iterable_empty, in_iterable))
     return False  # Not an Iterable
 
 
 class shapedArray:
@@ -233,15 +237,14 @@
     def n_qubits(self) -> int:
         if self.routed == True:
             return len(self.final_mapping)
         else:
             return self.cost_hamiltonian.n_qubits
 
     def __repr__(self):
-
         """Return an overview over the parameters and hyperparameters
 
         Todo
         ----
         Split this into ``__repr__`` and ``__str__`` with a more verbose
         output in ``__repr__``.
         """
@@ -274,45 +277,42 @@
         )
 
         return string
 
     def _assign_coefficients(
         self, input_block: List[RotationGateMap], input_coeffs: List[float]
     ) -> None:
-
         """
         Splits the coefficients and gatemaps into qubit singles and qubit pairs.
         """
 
         single_qubit_coeffs = []
         pair_qubit_coeffs = []
         qubit_singles = []
         qubit_pairs = []
 
         if len(input_block) != len(input_coeffs):
             raise ValueError(
                 "The number of terms/gatemaps must match the number of coefficients provided."
             )
         for each_gatemap, each_coeff in zip(input_block, input_coeffs):
-
             if each_gatemap.gate_label.n_qubits == 1:
                 single_qubit_coeffs.append(each_coeff)
                 # Giving a string name to each gatemap (?)
                 qubit_singles.append(type(each_gatemap).__name__)
             elif each_gatemap.gate_label.n_qubits == 2:
                 pair_qubit_coeffs.append(each_coeff)
                 qubit_pairs.append(type(each_gatemap).__name__)
 
         return (single_qubit_coeffs, pair_qubit_coeffs, qubit_singles, qubit_pairs)
 
     @staticmethod
     def block_setter(
-        input_object: Union[List["RotationGateMap"], Hamiltonian], block_type: Enum
-    ) -> List["RotationGateMap"]:
-
+        input_object: Union[List[RotationGateMap], Hamiltonian], block_type: Enum
+    ) -> List[RotationGateMap]:
         """
         Converts a Hamiltonian Object into a List of RotationGateMap Objects with
         the appropriate block_type and sequence assigned to the GateLabel
 
         OR
 
         Remaps a list of RotationGateMap Objects with a block_type and sequence
@@ -349,17 +349,16 @@
             raise ValueError(
                 "The input object defining mixer should be a List of RotationGateMaps or type Hamiltonian"
             )
         return block
 
     @staticmethod
     def set_block_sequence(
-        input_gatemap_list: List["RotationGateMap"],
-    ) -> List["RotationGateMap"]:
-
+        input_gatemap_list: List[RotationGateMap],
+    ) -> List[RotationGateMap]:
         """
         This method assigns the sequence attribute to all RotationGateMap objects in the list.
         The sequence of the GateMaps are implied based on their positions in the list.
 
         Parameters
         ----------
         input_gatemap_list: `List[RotationGateMap]`
@@ -393,31 +392,30 @@
         return input_gatemap_list
 
     def reorder_gates_block(self, gates_block, layer_number):
         """Update the qubits that the gates are acting on after application
         of SWAPs in the cost layer
         """
         for gate in gates_block:
-
             if layer_number % 2 == 0:
                 mapping = self.final_mapping
                 gate.qubit_1 = mapping[gate.qubit_1]
                 if gate.gate_label.n_qubits == 2:
                     gate.qubit_2 = mapping[gate.qubit_2]
             else:
                 pass
 
         return gates_block
 
     @staticmethod
     def route_gates_list(
-        gates_to_route: List["GateMap"],
+        gates_to_route: List[GateMap],
         device: "DeviceBase",
         routing_function: Callable,
-    ) -> List["GateMap"]:
+    ) -> List[GateMap]:
         """
         Apply qubit routing to the abstract circuit gate list
         based on device information
 
         Parameters
         ----------
         gates_to_route: `List[GateMap]`
@@ -479,15 +477,14 @@
             gates_list,
             list(initial_physical_to_logical_mapping.keys()),
             final_mapping,
         )
 
     @property
     def abstract_circuit(self):
-
         # even layer inversion if the circuit contains SWAP gates
         even_layer_inversion = -1 if self.routed == True else 1
         _abstract_circuit = []
         for each_p in range(self.p):
             # apply each cost_block with reversed order to maintain the SWAP sequence
             _abstract_circuit.extend(
                 self.cost_blocks[each_p][:: (even_layer_inversion) ** each_p]
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gatemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,28 @@
     @abstractmethod
     def _decomposition_standard(self) -> List[Tuple]:
         pass
 
 
 class SWAPGateMap(GateMap):
     def __init__(self, qubit_1: int, qubit_2: int):
-
         super().__init__(qubit_1)
         self.qubit_2 = qubit_2
         self.gate_label = GateMapLabel(n_qubits=2, gatemap_type=GateMapType.FIXED)
 
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (CX, [self.qubit_1, self.qubit_2]),
             (CX, [self.qubit_2, self.qubit_1]),
             (CX, [self.qubit_1, self.qubit_2]),
         ]
 
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
-
         return [
             (
                 RZ,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (
                 RZ,
@@ -109,79 +106,73 @@
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, -np.pi / 2)],
             ),
         ]
 
 
 class RotationGateMap(GateMap):
     def __init__(self, qubit_1: int):
-
         super().__init__(qubit_1)
         self.angle_value = None
         self.gate_label = GateMapLabel(n_qubits=1)
 
     @property
     def _decomposition_trivial(self) -> List[Tuple]:
         return self._decomposition_standard
 
 
 class RYGateMap(RotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RY,
                 [
                     self.qubit_1,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class RXGateMap(RotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RX,
                 [
                     self.qubit_1,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class RZGateMap(RotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RZ,
                 [
                     self.qubit_1,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class TwoQubitRotationGateMap(RotationGateMap):
     def __init__(self, qubit_1: int, qubit_2: int):
-
         super().__init__(qubit_1)
         self.qubit_2 = qubit_2
         self.gate_label = GateMapLabel(n_qubits=2)
 
     @property
     def _decomposition_trivial(self) -> List[Tuple]:
-
         low_level_gate = eval(type(self).__name__.strip("GateMap"))
         return [
             (
                 low_level_gate,
                 [
                     self.qubit_1,
                     self.qubit_2,
@@ -190,15 +181,14 @@
             )
         ]
 
 
 class RXXGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RY,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
             (
@@ -227,22 +217,20 @@
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
         ]
 
 
 class RXYGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         raise NotImplementedError()
 
 
 class RYYGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RX,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (
                 RX,
@@ -267,15 +255,14 @@
             ),
         ]
 
 
 class RZXGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (
                 RY,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
             (CX, [self.qubit_1, self.qubit_2]),
@@ -294,30 +281,28 @@
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
         ]
 
 
 class RZZGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         return [
             (CX, [self.qubit_1, self.qubit_2]),
             (
                 RZ,
                 [
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
             (CX, [self.qubit_1, self.qubit_2]),
         ]
 
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
-
         return [
             (
                 RZ,
                 [
                     self.qubit_1,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
@@ -339,47 +324,43 @@
             ),
         ]
 
 
 class RYZGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         raise NotImplementedError()
 
 
 class RiSWAPGateMap(TwoQubitRotationGateMap):
     """
     Parameterised-iSWAP gate
     """
 
     @property
     def _decomposition_standard(self) -> List[Tuple]:
-
         total_decomp = RXXGateMap.decomposition
         total_decomp.extend(RYYGateMap.decomposition)
         return total_decomp
 
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
-
         return [
             (
                 RiSWAP,
                 [
                     self.qubit_1,
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class RotationGateMapFactory(object):
-
     PAULI_OPERATORS = ["X", "Y", "Z", "XX", "ZX", "ZZ", "XY", "YY", "YZ"]
     GATE_GENERATOR_GATEMAP_MAPPER = {
         term: eval(f"R{term}GateMap") for term in PAULI_OPERATORS
     }
 
     def rotationgatemap_list_from_hamiltonian(
         hamil_obj: Hamiltonian, gatemap_type: GateMapType = None
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gatemaplabel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from enum import Enum
 from typing import Union
 
 
 class GateMapType(Enum):
-
     MIXER = "MIXER"
     COST = "COST"
     FIXED = "FIXED"
 
     @classmethod
     def supported_types(cls):
         return list(map(lambda c: c.name, cls))
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gates.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 
     def apply_vector_gate(self, input_obj):
         input_obj.apply_rzz(
             self.qubit_1, self.qubit_2, self.rotation_object.rotation_angle
         )
 
 
+class X(OneQubitGate):
+    __name__ = "X"
+
+
 class RZ(OneQubitRotationGate):
     __name__ = "RZ"
 
 
 class RY(OneQubitRotationGate):
     __name__ = "RY"
 
@@ -121,8 +125,8 @@
 
 
 class CPHASE(TwoQubitRotationGate):
     __name__ = "CPHASE"
 
 
 class RiSWAP(TwoQubitRotationGate):
-    __name__ = "RiSWAP"
+    __name__ = "RiSWAP"
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/hamiltonianmapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         """
         # Initialize sorted pauli string and indices
         sorted_pauli_str = ""
         sorted_qubit_indices = []
 
         # Sorting
         for index, string in sorted(zip(qubit_indices, pauli_str)):
-
             # Ensure string is a valid Pauli operator
             if string not in PAULIS_SET:
                 raise ValueError(
                     f"{string} is not a valid Pauli. Please choose from the set {PAULIS_SET}"
                 )
 
             # Store sorted indices and strings
@@ -463,15 +462,14 @@
             qubit_mapper = dict(zip(physical_qureg, self.qureg))
 
         self.terms = []
         self.coeffs = []
         self.constant = constant
 
         for term, coeff in zip(pauli_terms, coeffs):
-
             # Identity terms are added to the constant
             if term._is_trivial:
                 self.constant += coeff
 
             # Remap terms if required
             else:
                 if need_remapping:
@@ -662,15 +660,14 @@
         Hamiltonian:
             Classical Hamiltonian.
         """
         pauli_ops = []
         pauli_coeffs = []
 
         for term, coeff in zip(terms, coeffs):
-
             # Check coeffcient type
             if not isinstance(coeff, int) and not isinstance(coeff, float):
                 raise ValueError(
                     "Classical Hamiltonians only support Integer or Float coefficients"
                 )
 
             # Construct Hamiltonian terms from Pauli operators
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/ansatz_constructor/rotationangle.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/annealingparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/extendedparams.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         return 2 * (self.cost_1q_coeffs * self.gammas_singles)
 
     @property
     def cost_2q_angles(self):
         return 2 * (self.cost_2q_coeffs * self.gammas_pairs)
 
     def update_from_raw(self, new_values):
-
         self.betas_singles = np.array(new_values[: len(self.mixer_1q_coeffs) * self.p])
         self.betas_singles = self.betas_singles.reshape(
             (self.p, len(self.mixer_1q_coeffs))
         )
 
         new_values = new_values[len(self.betas_singles.flatten()) :]
 
@@ -281,15 +280,14 @@
             + gamma_single_constraints
             + gamma_pair_constraints
         )
 
         return all_constraints
 
     def plot(self, ax=None, **kwargs):
-
         list_names_ = ["betas singles", "betas pairs", "gammas singles", "gammas pairs"]
         list_values_ = [
             self.betas_singles % (2 * (np.pi)),
             self.betas_pairs % (2 * (np.pi)),
             self.gammas_singles % (2 * (np.pi)),
             self.gammas_pairs % (2 * (np.pi)),
         ]
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/fourierparams.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,14 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         q: int,
         v: List[Union[float, int]],
         u_singles: List[Union[float, int]],
         u_pairs: List[Union[float, int]],
     ):
-
         # setup reg, qubits_singles and qubits_pairs
         super().__init__(qaoa_descriptor)
         if not self.cost_1q_coeffs or not self.cost_2q_coeffs:
             raise RuntimeError(
                 f"Please choose {type(self).__name__} parameterisation for problems "
                 "containing both Cost One-Qubit and Two-Qubit terms"
             )
@@ -322,15 +321,14 @@
         return 2 * np.outer(self.gammas_singles, self.cost_1q_coeffs)
 
     @property
     def cost_2q_angles(self):
         return 2 * np.outer(self.gammas_pairs, self.cost_2q_coeffs)
 
     def update_from_raw(self, new_values):
-
         # overwrite x_rotation_angles with new ones
         self.v = np.array(new_values[0 : self.q])
         # cut x_rotation_angles from new_values
         new_values = new_values[self.q :]
 
         self.u_singles = np.array(new_values[0 : self.q])
         new_values = new_values[self.q :]
@@ -502,15 +500,14 @@
         qaoa_descriptor: QAOADescriptor,
         q: int,
         v_singles: List[Union[float, int]],
         v_pairs: List[Union[float, int]],
         u_singles: List[Union[float, int]],
         u_pairs: List[Union[float, int]],
     ):
-
         # setup reg, qubits_singles and qubits_pairs
         super().__init__(qaoa_descriptor)
         assert q is not None, f"Depth q for {type(self).__name__} must be specified"
         self.q = q
         self.v_singles = v_singles
         self.v_pairs = v_pairs
         self.u_singles = u_singles
@@ -575,15 +572,14 @@
     def cost_2q_angles(self):
         if self.u_pairs.size > 0:
             return 2 * (self.cost_2q_coeffs * self.gammas_pairs)
         else:
             return 2 * (self.cost_2q_coeffs * np.empty(shape=(self.p, 0)))
 
     def update_from_raw(self, new_values):
-
         self.v_singles = np.array(new_values[: len(self.mixer_1q_coeffs) * self.q])
         self.v_singles = self.v_singles.reshape((self.q, len(self.mixer_1q_coeffs)))
         new_values = new_values[self.q * len(self.mixer_1q_coeffs) :]
 
         self.v_pairs = np.array(new_values[: len(self.mixer_2q_coeffs) * self.q])
         self.v_pairs = self.v_pairs.reshape((self.q, len(self.mixer_2q_coeffs)))
         new_values = new_values[self.q * len(self.mixer_2q_coeffs) :]
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/standardparams.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,14 @@
     def __init__(
         self,
         qaoa_descriptor: QAOADescriptor,
         betas: List[Union[float, int]],
         gammas_singles: List[Union[float, int]],
         gammas_pairs: List[Union[float, int]],
     ):
-
         super().__init__(qaoa_descriptor)
         if not self.cost_1q_coeffs or not self.cost_2q_coeffs:
             raise RuntimeError(
                 f"Please choose {type(self).__name__} parameterisation for "
                 "problems containing both Cost One-Qubit and Two-Qubit terms"
             )
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_baseparams.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     cost_1q_coeffs
     cost_2q_coeffs
     mixer_1q_coeffs
     mixer_2q_coeffs
     """
 
     def __init__(self, qaoa_descriptor: QAOADescriptor):
-
         self.qaoa_descriptor = qaoa_descriptor
         self.p = self.qaoa_descriptor.p
 
         try:
             self.cost_1q_coeffs = qaoa_descriptor.cost_single_qubit_coeffs
             self.cost_2q_coeffs = qaoa_descriptor.cost_pair_qubit_coeffs
             self.mixer_1q_coeffs = qaoa_descriptor.mixer_single_qubit_coeffs
@@ -50,19 +49,17 @@
         int:
             the length of the data produced by self.raw() and accepted by
             self.update_from_raw()
         """
         raise NotImplementedError()
 
     def __repr__(self):
-
         raise NotImplementedError()
 
     def __str__(self):
-
         return self.__repr__()
 
     @property
     def mixer_1q_angles(self) -> np.ndarray:
         """2D array with the X-rotation angles.
 
         1st index goes over p and the 2nd index over the qubits to
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_params_converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/qaoa_components/variational_parameters/variational_params_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,14 @@
             )
         except:
             raise ValueError(
                 f"For the selected {params_type} parameterisation, please specify a"
                 f" dictionary with correct {VARIATIONAL_PARAMS_DICT_KEYS[params_type]} keys"
             )
     elif init_type == "ramp":
-
         if isinstance(linear_ramp_time, float) or isinstance(linear_ramp_time, int):
             assert (
                 linear_ramp_time > 0
             ), "Please specify the linear ramp time. Only positive values are allowed."
         elif linear_ramp_time is None:
             pass
         else:
```

### Comparing `openqaoa-0.1.3/src/openqaoa-core/utilities.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/openqaoa/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 
 def quick_create_mixer_for_topology(
     input_gatemap: TwoQubitRotationGateMap,
     n_qubits: int,
     qubit_connectivity: Union[List[list], List[tuple], str] = "full",
     coeffs: List[float] = None,
 ) -> Tuple[List[TwoQubitRotationGateMap], List[float]]:
-
     """
     Quickly generates a gatemap list and coeffs for a specific topology.
     Can only be used with 2-Qubit Gates.
 
     Parameters
     ----------
     input_gatemap: `TwoQubitRotationGateMap`
@@ -291,15 +290,14 @@
 
     # Add nodes for each qubit in the register
     for qubit in hamiltonian.qureg:
         G.add_node(qubit, weight=0)
 
     # Add each term to the graph as an attribute
     for term, weight in zip(hamiltonian.terms, hamiltonian.coeffs):
-
         # Extract indices from Pauli term
         term_tuple = term.qubit_indices
 
         # If term is linear add as a node with a weight attribute
         if len(term) == 1:
             G.add_node(term_tuple[0], weight=weight)
 
@@ -391,15 +389,14 @@
     G = nx.random_regular_graph(degree, len(nodes), seed)
 
     # Relabel nodes
     nx.relabel_nodes(G, {i: n for i, n in enumerate(nodes)})
 
     # Add edges between nodes
     for edge in G.edges():
-
         # If weighted attribute is False, all weights are set to 1
         if not weighted:
             G[edge[0]][edge[1]]["weight"] = 1
 
         # If weighted attribute is True, weights are assigned as random integers
         else:
             G[edge[0]][edge[1]]["weight"] = np.random.rand()
@@ -561,15 +558,14 @@
         # Store linear terms and coefficients
         for qubit, coeff in zip(bias_qubits, bias_coeffs):
             terms.append([qubit])
             weights.append(coeff)
 
     # Generate quiadratic terms, scanning all possible combinations
     for q1, q2 in itertools.combinations(reg, 2):
-
         # Choose at random to couple terms
         are_coupled = np.random.randint(2)
 
         # If coupled, generate coefficients and store along with term
         if are_coupled:
             couple_coeff = np.random.rand() if weighted else 1
             terms.append([q1, q2])
@@ -627,15 +623,14 @@
     register = range(n_qubits)
 
     # Intialize energies
     energies = np.zeros(2 ** len(register))
 
     # Obtain spectrum, scanning term by term
     for i, term in enumerate(hamiltonian.terms):
-
         # Extract coefficient
         out = np.real(hamiltonian.coeffs[i])
 
         # Compute tensor product
         for qubit in register:
             if qubit in term.qubit_indices:
                 out = np.kron([1, -1], out)
@@ -679,15 +674,14 @@
         The energy of the given bitstring with respect to the cost Hamiltonian.
     """
     # Initialize energy value
     energy = 0
 
     # Compute energy contribution term by term
     for i, term in enumerate(hamiltonian.terms):
-
         # Compute sign of spin interaction term
         variables_product = np.prod(
             [(-1) ** int(bitstring[k]) for k in term.qubit_indices]
         )
 
         # Add energy contribution
         energy += hamiltonian.coeffs[i] * variables_product
@@ -720,15 +714,14 @@
     energy = 0
 
     # Number of measurement shots
     shots = sum(measurement_counts.values())
 
     # Compute average energy adding one by one the contribution from each state
     for state, prob in measurement_counts.items():
-
         # Number of ones (spins pointing down) from the specific
         # configuration for each Hamiltonian term
         num_ones_list = [
             sum([int(state[i]) for i in term.qubit_indices])
             for term in hamiltonian.terms
         ]
 
@@ -777,15 +770,14 @@
     register = range(n_qubits)
 
     # Intialize energies
     energies = np.zeros((2 ** len(register)))
 
     # Obtain spectrum, scanning term by term
     for i, term in enumerate(hamiltonian.terms):
-
         # Extract coefficients
         out = np.real(hamiltonian.coeffs[i])
 
         # Compute tensor product
         for qubit in register:
             if qubit in term.qubit_indices:
                 out = np.kron([1, -1], out)
@@ -993,15 +985,14 @@
 
     # Initialize expectation value
     exp_val = 0
     norm = sum(prob_dict.values())
 
     # Compute correlation
     for bitstring, prob in prob_dict.items():
-
         # If 0, spin is pointing up, else it is pointing down
         Z = int(bitstring[spin])
 
         # Add contribution if spin points up or subtract if points down
         exp_val += -prob / norm if Z > 0 else prob / norm
 
     return exp_val
@@ -1033,44 +1024,37 @@
 
     # Initialize correlation
     corr = 0
 
     norm = sum(prob_dict.values())
     # Compute correlation
     for bitstring, prob in prob_dict.items():
-
         # If 0 or 2, spins are aligned, else they are anti-aligned
         num_ones = sum([int(bitstring[i]) for i in spins])
 
         # Add contribution if spins aligned or subtract if anti-aligned
         corr += prob / norm if num_ones % 2 == 0 else -prob / norm
 
     return corr
 
 
 def exp_val_hamiltonian_termwise(
-    variational_params: QAOAVariationalBaseParams,
-    qaoa_backend,
     hamiltonian: Hamiltonian,
     mixer_type: str,
     p: int,
     qaoa_optimized_angles: Optional[list] = None,
     qaoa_optimized_counts: Optional[dict] = None,
     analytical: bool = True,
 ):
     """
     Computes the single spin expectation values <Z_{i}> and the correlation matrix Mij = <Z_{i}Z_{j}>,
     using the optimization results obtained from QAOA tranining the specified QAOA cost backend.
 
     Parameters
     ----------
-    variational_params: `QAOAVariationalBaseParams`
-        Set of variational parameters in the QAOA ansatz.
-    qaoa_backend: `QAOABaseBackend`
-        Chosen backend on which QAOA is performed.
     hamiltonian: `Hamiltonian`
         Hamiltonian object containing the problem statement.
     p: `int`
         Number of layers in QAOA ansatz.
     qaoa_optimized_angles: `list`
         Optimized angles of the underlying QAOA.
     qaoa_optimized_counts: `dict`
@@ -1100,69 +1084,146 @@
     # If single layer ansatz use analytical results
     if (
         analytical == True
         and p == 1
         and mixer_type == "x"
         and isinstance(qaoa_optimized_angles, list)
     ):
-
         # Compute expectation values and correlations of terms present in the Hamiltonian
         for term in terms:
-
             # If bias term compute expectation value
             if len(term) == 1:
                 i = term.qubit_indices[0]
                 exp_vals_z[i] = exp_val_single_analytical(
                     i, hamiltonian, qaoa_optimized_angles
                 )
 
             # If two-body term compute correlation
             elif len(term) == 2:
                 i, j = term.qubit_indices
                 corr_matrix[i][j] = exp_val_pair_analytical(
                     (i, j), hamiltonian, qaoa_optimized_angles
                 )
-
-            # If constant term, ignore
             else:
                 continue
 
     # If multilayer ansatz, perform numerical computation
     else:
-
         if isinstance(qaoa_optimized_counts, dict):
             counts_dict = qaoa_optimized_counts
         else:
             raise ValueError(
                 "Please specify optimized counts to compute expectation values."
             )
 
         # Compute expectation values and correlations of terms present in the Hamiltonian
         for term in terms:
-
             # If bias term compute expectation value
             if len(term) == 1:
                 i = term.qubit_indices[0]
                 exp_vals_z[i] = exp_val_single(i, counts_dict)
 
             # If two-body term compute correlation
             elif len(term) == 2:
                 i, j = term.qubit_indices
                 corr_matrix[i][j] = exp_val_pair((i, j), counts_dict)
 
-            # If constant term, ignore
-            if len(term) == 0:
+            else:
                 continue
 
     # Remove expectation value contribution from the correlations
     corr_matrix -= np.outer(exp_vals_z, exp_vals_z)
 
     return exp_vals_z, corr_matrix
 
 
+@round_value
+def calculate_calibration_factors(
+    hamiltonian: Hamiltonian,
+    calibration_measurements: dict,
+    calibration_registers: list,
+    qubit_mapping: list,
+) -> Dict:
+    """
+    Computes the single spin and pairs of spins calibration factors, which are the expectation value of the observables found in the particular Hamiltonian, <Z_{i}> and <Z_{i}Z_{j}>, from the calibration data provided. The calibration data is obtained under BFA on an empty (initial state = |000..0>) QAOA circuit.
+    See arXiv:2012.09738 and arXiv:2106.05800.
+
+    Parameters
+    ----------
+    hamiltonian: `Hamiltonian`
+        Hamiltonian object containing the problem statement.
+    calibration_measurements: `dict`
+        Dictionary containing the measurement counts of an empty QAOA circuit.
+    calibration_registers: `list`
+        List specifying the physical (device) qubits on which the calibration data has been obtained.
+        This is required because the calibration is usually performed over the whole device and hence the measurement outcomes (the calibration data) are strings with the size of the whole device while usually only a particular section is used.
+    qubit_mapping: `list`
+        List specifying the physical (device) qubits on which the QAOA circuit is executed. Related to qubit selection and qubit routing.
+
+    Returns
+    -------
+    calibration_factors: `dict`
+        Calibration factors as a dict.
+    """
+    calibration_registers_dict = {v: k for k, v in enumerate(calibration_registers)}
+
+    # Define number of qubits, problem hamiltonian and QAOA parameters
+    n_qubits = hamiltonian.n_qubits
+
+    # Extract Hamiltonian terms
+    terms = list(hamiltonian.terms)
+
+    if qubit_mapping == None:
+        qubit_mapping = np.arange(0, n_qubits)
+
+    # Initialize an empty dict
+    calibration_factors = {}
+
+    # Compute single spin and pairs of spins expectation values of terms present in the Hamiltonian
+    for term in terms:
+        # If bias term compute single spins expectation value
+        if len(term) == 1:
+            i = term.qubit_indices[0]
+            i_phys = qubit_mapping[i]
+            i_cal = calibration_registers_dict[i_phys]
+            exp_val_z = exp_val_single(i_cal, calibration_measurements)
+            calibration_factors.update({(i,): exp_val_z})
+
+        # If two-body term compute pairs of spins expectation values
+        elif len(term) == 2:
+            i, j = term.qubit_indices  # problem indices, ex: (0,1)
+            i_phys, j_phys = (
+                qubit_mapping[i],
+                qubit_mapping[j],
+            )  # physical indices, ex: (133, 131) after routing
+            i_cal, j_cal = (
+                calibration_registers_dict[i_phys],
+                calibration_registers_dict[j_phys],
+            )  # calibration indices, i.e. to which location on the measurement string each physical qubit corresponds to, ex: (63, 61)
+            exp_val_zz = exp_val_pair((i_cal, j_cal), calibration_measurements)
+
+            calibration_factors.update(
+                {(i, j): exp_val_zz}
+            )  # calibration factors are calculated for the terms in the hamiltonian/problem
+
+        # If constant term, ignore
+        if len(term) == 0:
+            continue
+
+    assert all(
+        value != 0 for value in calibration_factors.values()
+    ), "One (or more) of the calibration factors is 0 which means that the measurement is faulty. Please check the data."
+
+    assert all(
+        value <= 1 for value in calibration_factors.values()
+    ), "One (or more) of the calibration factors is larger than 1 which is not physical. Please check the data."
+
+    return calibration_factors
+
+
 ################################################################################
 # ANALYTIC & KNOWN FORMULAE
 ################################################################################
 
 
 def exp_val_single_analytical(spin: int, hamiltonian: Hamiltonian, qaoa_angles: tuple):
     """
@@ -1211,15 +1272,14 @@
     iter_qubits = [j for j in range(0, spin)] + [j for j in range(spin + 1, n_qubits)]
 
     # Initialize products
     exp_val = -np.sin(2 * beta) * np.sin(2 * gamma * h_u)
 
     # Loop over edges connecting u and v to other spins
     for n in iter_qubits:
-
         # Edges between the spin and others in the register
         edge = tuple([min(spin, n), max(spin, n)])
 
         # If edge not present in the graph the associated weight is set to 0
         J_un = 0 if hamil_graph.get(edge) is None else hamil_graph[edge]
 
         # Add factor to the products
@@ -1296,15 +1356,14 @@
     prod1 = s**2 / 2 * np.cos(2 * gamma * (h_u - h_v))
     prod2 = -(s**2) / 2 * np.cos(2 * gamma * (h_u + h_v))
     prod3 = -c * s * np.sin(2 * gamma * J_uv) * np.cos(2 * gamma * h_u)
     prod4 = -c * s * np.sin(2 * gamma * J_uv) * np.cos(2 * gamma * h_v)
 
     # Loop over edges connecting u and v to other spins
     for n in iter_qubits:
-
         # Edges between u,v and another spin in the register
         edge1 = tuple([min(u, n), max(u, n)])
         edge2 = tuple([min(v, n), max(v, n)])
 
         # If edge not present in the graph the associated weight is set to 0
         J_un = 0 if hamil_graph.get(edge1) is None else hamil_graph[edge1]
         J_vn = 0 if hamil_graph.get(edge2) is None else hamil_graph[edge2]
@@ -1341,21 +1400,18 @@
     terms = [pauli_term.qubit_indices for pauli_term in hamiltonian.terms]
     coeffs = hamiltonian.coeffs
 
     energy = 0
 
     # Compute the expectation value of each term and add its local energy contribution
     for coeff, term in zip(coeffs, terms):
-
         if len(term) == 2:
-
             local_energy = exp_val_pair_analytical(term, hamiltonian, angles)
 
         else:
-
             local_energy = exp_val_single_analytical(term[0], hamiltonian, angles)
 
         energy += coeff * local_energy
 
     # Add constant shift contribution
     energy += hamiltonian.constant
 
@@ -1423,14 +1479,84 @@
 
     for key, value in counts_dictionary.items():
         output_counts_dictionary[key[::-1]] = value
 
     return output_counts_dictionary
 
 
+def permute_counts_dictionary(
+    counts_dictionary: dict, final_qubit_layout: List[int]
+) -> dict:
+    """Permutes the order of the qubits in the counts dictionary to the
+    original order if SWAP gates were used leading to modified qubit layout.
+    Parameters
+    ----------
+    counts_dictionary : `dict`
+        The measurement outcomes obtained from the Simulator/QPU
+    original_qubit_layout: List[int]
+        The qubit layout in which the qubits were initially
+    final_qubit_layout: List[int]
+        The final qubit layout after application of SWAPs
+
+    Returns
+    -------
+    `dict`
+        The permuted counts dictionary with qubits in the original place
+    """
+
+    # Create a mapping of original positions to final positions
+    original_qubit_layout = list(range(len(final_qubit_layout)))
+    mapping = {
+        original_qubit_layout[i]: final_qubit_layout[i]
+        for i in range(len(original_qubit_layout))
+    }
+    permuted_counts = {}
+
+    for basis, counts in counts_dictionary.items():
+
+        def permute_string(basis_state: str = basis, mapping: dict = mapping):
+            # Use the mapping to permute the string
+            permuted_string = "".join(
+                [basis_state[mapping[i]] for i in range(len(basis_state))]
+            )
+            return permuted_string
+
+        permuted_counts.update({permuted_string: counts})
+
+    return permuted_counts
+
+
+def negate_counts_dictionary(counts_dictionary: dict, s: int) -> dict:
+    """Negates every bitstring of the counts dictionary according to
+    the position of the X gates before the measurement.
+    Used in SPAM Twirling.
+    Parameters
+    ----------
+    counts_dictionary : `dict`
+        The measurement outcomes obtained from the Simulator/QPU
+    s: int
+        Syndrome whose binary representation denotes the negated qubits. For example, 4 = 100, signifies that the first qubit had an X gate just before the measurement, which requires the first digit of the every key to be classically negated inside this function.
+
+    Returns
+    -------
+    `dict`
+        The negated counts dictionary
+    """
+    negated_counts = {}
+    for key in counts_dictionary.keys():
+        n_qubits = len(key)
+        negated_key = s ^ int(
+            key, 2
+        )  # bitwise XOR to classically negate randomly chosen qubits, specified by s
+        negated_counts.update(
+            [(format(negated_key, "b").zfill(n_qubits), counts_dictionary[key])]
+        )
+    return negated_counts
+
+
 @round_value
 def qaoa_probabilities(statevector) -> dict:
     """
     Return a qiskit-style probability dictionary from a statevector.
 
     Parameters
     ----------
@@ -1449,15 +1575,14 @@
     # Extract number of qubits from size of probability
     n_qubits = int(np.log2(len(prob_vec)))
 
     # Initialize probability dictionary
     prob_dict = {}
 
     for x in range(len(prob_vec)):
-
         # Define binary representation of each state, with qubit-0 most significant bit
         key = np.binary_repr(x, n_qubits)[::-1]
 
         # Update probability dictionary
         prob_dict.update({key: prob_vec[x]})
 
     return prob_dict
```

### Comparing `openqaoa-0.1.3/src/openqaoa-pyquil/backends/devices.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/src/openqaoa-pyquil/backends/gates_pyquil.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/gates_pyquil.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,90 +2,81 @@
 
 from pyquil import Program, gates
 from pyquil.quilatom import QubitPlaceholder
 
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 import openqaoa.qaoa_components.ansatz_constructor.gates as gates_core
 
-class PyquilGateApplicator(gates_core.GateApplicator):
 
+class PyquilGateApplicator(gates_core.GateApplicator):
     PYQUIL_OQ_GATE_MAPPER = {
+        gates_core.X.__name__: gates.X,
         gates_core.RZ.__name__: gates.RZ,
         gates_core.RX.__name__: gates.RX,
         gates_core.RY.__name__: gates.RY,
         gates_core.CX.__name__: gates.CNOT,
         gates_core.CZ.__name__: gates.CZ,
         gates_core.CPHASE.__name__: gates.CPHASE,
-        gates_core.RiSWAP.__name__: gates.XY
+        gates_core.RiSWAP.__name__: gates.XY,
     }
 
-    library = 'pyquil'
+    library = "pyquil"
+
+    def create_quantum_circuit(self, n_qubits) -> Program:
+        """
+        Function which creates and empty circuit specific to the pyquil backend.
+        Needed for SPAM twirling but can be used more generally.
+        """
+        return Program()
 
     def gate_selector(self, gate: gates_core.Gate) -> Callable:
         selected_pyquil_gate = PyquilGateApplicator.PYQUIL_OQ_GATE_MAPPER[gate.__name__]
         return selected_pyquil_gate
 
     @staticmethod
     def apply_1q_rotation_gate(
-        pyquil_gate,
-        qubit_1: int,
-        rotation_object: RotationAngle,
-        circuit: Program
+        pyquil_gate, qubit_1: int, rotation_object: RotationAngle, circuit: Program
     ) -> Program:
-        circuit += pyquil_gate(
-            rotation_object.rotation_angle,
-            qubit_1
-        )
+        circuit += pyquil_gate(rotation_object.rotation_angle, qubit_1)
         return circuit
 
     @staticmethod
     def apply_2q_rotation_gate(
         pyquil_gate,
         qubit_1: int,
         qubit_2: int,
         rotation_object: RotationAngle,
-        circuit: Program
+        circuit: Program,
     ) -> Program:
-        circuit += pyquil_gate(
-            rotation_object.rotation_angle,
-            qubit_1, 
-            qubit_2
-        )
+        circuit += pyquil_gate(rotation_object.rotation_angle, qubit_1, qubit_2)
         return circuit
 
     @staticmethod
-    def apply_1q_fixed_gate(
-        pyquil_gate,
-        qubit_1: int,
-        circuit: Program
-    ) -> Program:
+    def apply_1q_fixed_gate(pyquil_gate, qubit_1: int, circuit: Program) -> Program:
         circuit += pyquil_gate(qubit_1)
         return circuit
 
     @staticmethod
     def apply_2q_fixed_gate(
-        pyquil_gate,
-        qubit_1: int,
-        qubit_2: int,
-        circuit: Program
+        pyquil_gate, qubit_1: int, qubit_2: int, circuit: Program
     ) -> Program:
         circuit += pyquil_gate(qubit_1, qubit_2)
         return circuit
 
     def apply_gate(self, gate: gates_core.Gate, *args):
         selected_pyquil_gate = self.gate_selector(gate)
         if gate.n_qubits == 1:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,rotation_object,circuit)
                 return self.apply_1q_rotation_gate(selected_pyquil_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1,circuit)
                 return self.apply_1q_fixed_gate(selected_pyquil_gate, *args)
         elif gate.n_qubits == 2:
-            if hasattr(gate, 'rotation_object'):
+            if hasattr(gate, "rotation_object"):
                 # *args must be of the following format -- (qubit_1,qubit_2,rotation_object,circuit)
                 return self.apply_2q_rotation_gate(selected_pyquil_gate, *args)
             else:
                 # *args must be of the following format -- (qubit_1,qubit_2,circuit)
                 return self.apply_2q_fixed_gate(selected_pyquil_gate, *args)
         else:
-            raise ValueError("Only 1 and 2-qubit gates are supported.")
+            raise ValueError("Only 1 and 2-qubit gates are supported.")
```

### Comparing `openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/qaoa_pyquil_qpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import Counter
 import numpy as np
+from copy import deepcopy
 from pyquil import Program, gates, quilbase
 from typing import List, Optional
 import warnings
 
 from .devices import DevicePyquil
 from .gates_pyquil import PyquilGateApplicator
 from openqaoa.backends.basebackend import (
@@ -17,15 +18,14 @@
 )
 from openqaoa.qaoa_components.ansatz_constructor.gatemap import RZZGateMap, SWAPGateMap
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 from openqaoa.utilities import generate_uuid
 
 
 def check_edge_connectivity(executable: Program, device: DevicePyquil):
-
     '''
     Check that the program does not contain 2-qubit terms that is not present
     in the QPU's topology (to prevent quilc from crashing).
 
     Parameters
     ----------
     executable: `Program`
@@ -45,15 +45,14 @@
     instrs = [instr for instr in executable if type(instr) == quilbase.Gate]
     pair_instrs = [
         list(instr.get_qubits()) for instr in instrs if len(instr.get_qubits()) == 2
     ]
 
     for term in pair_instrs:
         if len(term) == 2:
-
             assert (
                 term in qpu_graph.edges()
             ), f"Term {term} is not an edge on the QPU graph of {device.device_name}."
 
 
 class QAOAPyQuilQPUBackend(
     QAOABaseBackendParametric, QAOABaseBackendCloud, QAOABaseBackendShotBased
@@ -100,26 +99,27 @@
         append_state: Program,
         init_hadamard: bool,
         cvar_alpha: float,
         active_reset: bool = False,
         rewiring: str = "",
         initial_qubit_mapping: Optional[List[int]] = None,
     ):
-
         QAOABaseBackendShotBased.__init__(
             self,
             qaoa_descriptor,
             n_shots,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
         )
         QAOABaseBackendCloud.__init__(self, device)
 
+        self.gate_applicator = PyquilGateApplicator()
+
         self.active_reset = active_reset
         self.rewiring = rewiring
         self.qureg = list(range(self.n_qubits))
         self.problem_reg = self.qureg[0 : self.problem_qubits]
 
         if self.initial_qubit_mapping is None:
             self.initial_qubit_mapping = (
@@ -138,20 +138,14 @@
 
         if self.device.n_qubits < self.n_qubits:
             raise Exception(
                 "There are lesser qubits on the device than the number of qubits required for the circuit."
             )
 
         self.parametric_circuit = self.parametric_qaoa_circuit
-        native_prog = self.device.quantum_computer.compiler.quil_to_native_quil(
-            self.parametric_circuit
-        )
-        self.prog_exe = self.device.quantum_computer.compiler.native_quil_to_executable(
-            native_prog
-        )
 
         # Check program connectivity against QPU connectivity
         # TODO: reconcile with PRAGMA PRESERVE
 
         # check_edge_connectivity(self.prog_exe, device)
 
     def qaoa_circuit(self, params: QAOAVariationalBaseParams) -> Program:
@@ -163,24 +157,51 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         `pyquil.Program`
             A pyquil.Program (executable) object.
         """
+        parametric_circuit = deepcopy(self.parametric_circuit)
+        # declare the read-out register
+        ro = parametric_circuit.declare("ro", "BIT", self.problem_qubits)
+
+        if self.append_state:
+            parametric_circuit += self.append_state
+
+        if self.final_mapping is None:
+            for i, qbit in enumerate(self.problem_reg):
+                parametric_circuit += gates.MEASURE(self.qubit_mapping[qbit], ro[i])
+        else:
+            # Measurement instructions
+            for i, qubit in enumerate(self.final_mapping[0 : len(self.problem_reg)]):
+                cbit = ro[i]
+                parametric_circuit += gates.MEASURE(self.qubit_mapping[qubit], cbit)
+        parametric_circuit.wrap_in_numshots_loop(self.n_shots)
+
+        native = self.device.quantum_computer.compiler.quil_to_native_quil(
+            parametric_circuit
+        )
+
+        prog_exe = self.device.quantum_computer.compiler.native_quil_to_executable(
+            native
+        )
+
         angles_list = np.array(
             self.obtain_angles_for_pauli_list(self.abstract_circuit, params),
             dtype=float,
         )
-        angle_declarations = list(self.parametric_circuit.declarations.keys())
+        angle_declarations = list(parametric_circuit.declarations.keys())
+
         angle_declarations.remove("ro")
+
         for i, param_name in enumerate(angle_declarations):
-            self.prog_exe.write_memory(region_name=param_name, value=angles_list[i])
+            prog_exe.write_memory(region_name=param_name, value=angles_list[i])
 
-        return self.prog_exe
+        return prog_exe
 
     @property
     def parametric_qaoa_circuit(self) -> Program:
         """
         Creates a parametric QAOA circuit (pyquil.Program object),
         given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
@@ -191,16 +212,15 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         `pyquil.Program`
             A pyquil.Program object.
         """
-        gates_applicator = PyquilGateApplicator()
-        
+
         if self.active_reset:
             parametric_circuit = Program(gates.RESET())
         else:
             parametric_circuit = Program()
 
         if self.rewiring != None:
             if self.rewiring in [
@@ -214,17 +234,14 @@
                     "Rewiring command not recognized. Please use "
                     'PRAGMA INITIAL_REWIRING "NAIVE"'
                     " or "
                     'PRAGMA INITIAL_REWIRING "PARTIAL"'
                     ""
                 )
 
-        # declare the read-out register
-        ro = parametric_circuit.declare("ro", "BIT", self.problem_qubits)
-
         if self.prepend_state:
             parametric_circuit += self.prepend_state
 
         # Initial state is all |+>
         if self.init_hadamard:
             for i in self.problem_reg:
                 parametric_circuit += gates.RZ(np.pi, self.qubit_mapping[i])
@@ -256,35 +273,23 @@
                     qubits = each_tuple[1][:-1]
                 else:
                     rotation_angle = None
                     qubits = each_tuple[1]
                 if not isinstance(qubits, list):
                     qubits = [qubits]
                 new_qubits = [self.qubit_mapping[qubit] for qubit in qubits]
-                    
+
                 if rotation_angle is None:
-                    gate = each_tuple[0](gates_applicator, *new_qubits)
+                    gate = each_tuple[0](self.gate_applicator, *new_qubits)
                 else:
-                    gate = each_tuple[0](gates_applicator, *new_qubits, rotation_angle)
+                    gate = each_tuple[0](
+                        self.gate_applicator, *new_qubits, rotation_angle
+                    )
                 gate.apply_gate(parametric_circuit)
 
-        if self.append_state:
-            parametric_circuit += self.append_state
-
-        if self.final_mapping is None:
-            for i, qbit in enumerate(self.problem_reg):
-                parametric_circuit += gates.MEASURE(self.qubit_mapping[qbit], ro[i])
-        else:
-            # Measurement instructions
-            for i, qubit in enumerate(self.final_mapping[0 : len(self.problem_reg)]):
-                cbit = ro[i]
-                parametric_circuit += gates.MEASURE(self.qubit_mapping[qubit], cbit)
-
-        parametric_circuit.wrap_in_numshots_loop(self.n_shots)
-
         return parametric_circuit
 
     def get_counts(self, params: QAOAVariationalBaseParams, n_shots=None) -> dict:
         """
         Execute the circuit and obtain the counts.
 
         Parameters
```

### Comparing `openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/openqaoa_pyquil/backends/qaoa_pyquil_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         prepend_state: Program = None,
         append_state: Program = None,
         init_hadamard: bool = True,
         cvar_alpha: float = 1,
     ):
-
         QAOABaseBackendStatevector.__init__(
             self,
             qaoa_descriptor,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
@@ -56,15 +55,15 @@
 
         Returns
         -------
         `pyquil.Program`
                 A pyquil.Program object.
         """
         gates_applicator = PyquilGateApplicator()
-        
+
         self.assign_angles(params)
 
         circuit = Program()
         if self.prepend_state:
             circuit += self.prepend_state
 
         # Initial state is all |+>
```

### Comparing `openqaoa-0.1.3/src/openqaoa-qiskit/backend_config.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backend_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,31 @@
-from .backends import (DeviceQiskit, QAOAQiskitQPUBackend, 
-                       QAOAQiskitBackendShotBasedSimulator,
-                       QAOAQiskitBackendStatevecSimulator)
+from .backends import (
+    DeviceQiskit,
+    QAOAQiskitQPUBackend,
+    QAOAQiskitBackendShotBasedSimulator,
+    QAOAQiskitBackendStatevecSimulator,
+)
 
 device_access = {DeviceQiskit: QAOAQiskitQPUBackend}
-device_name_to_obj = {"qiskit.qasm_simulator" : QAOAQiskitBackendShotBasedSimulator, 
-                      "qiskit.shot_simulator" : QAOAQiskitBackendShotBasedSimulator, 
-                      "qiskit.statevector_simulator" : QAOAQiskitBackendStatevecSimulator}
-device_location = 'ibmq'
+device_name_to_obj = {
+    "qiskit.qasm_simulator": QAOAQiskitBackendShotBasedSimulator,
+    "qiskit.shot_simulator": QAOAQiskitBackendShotBasedSimulator,
+    "qiskit.statevector_simulator": QAOAQiskitBackendStatevecSimulator,
+}
+device_location = "ibmq"
 device_plugin = DeviceQiskit
-device_args = {DeviceQiskit: ['hub', 'group', 'project', 'as_emulator']}
-backend_args = {QAOAQiskitBackendStatevecSimulator: [], 
-                QAOAQiskitBackendShotBasedSimulator: ['n_shots', 'seed_simulator', 
-                                                      'qiskit_simulation_method', 
-                                                      'noise_model', 
-                                                      'initial_qubit_mapping'], 
-                QAOAQiskitQPUBackend: ['n_shots', 'initial_qubit_mapping']}
+device_args = {DeviceQiskit: ["hub", "group", "project", "as_emulator"]}
+backend_args = {
+    QAOAQiskitBackendStatevecSimulator: [],
+    QAOAQiskitBackendShotBasedSimulator: [
+        "n_shots",
+        "seed_simulator",
+        "qiskit_simulation_method",
+        "noise_model",
+        "initial_qubit_mapping",
+    ],
+    QAOAQiskitQPUBackend: [
+        "n_shots",
+        "initial_qubit_mapping",
+        "qiskit_optimization_level",
+    ],
+}
```

### Comparing `openqaoa-0.1.3/src/openqaoa-qiskit/backends/devices.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from qiskit_ibm_provider import IBMProvider
 from qiskit_aer import AerSimulator
 from typing import List
-from openqaoa.backends.devices_core import DeviceBase
+from openqaoa.backends.basedevice import DeviceBase
 
 
 class DeviceQiskit(DeviceBase):
     """
     Contains the required information and methods needed to access remote
     qiskit QPUs.
 
@@ -108,27 +108,29 @@
 
     def _check_provider_connection(self) -> bool:
         """
         Private method for checking connection with provider.
         """
 
         try:
-            #Use default
+            # Use default
             self.provider = IBMProvider()
-            #Unless exact instance is specified
+            # Unless exact instance is specified
             if all([self.hub, self.group, self.project]):
-                instance_name = self.hub + '/' + self.group + '/' + self.project
+                instance_name = self.hub + "/" + self.group + "/" + self.project
                 assert instance_name in self.provider.instances()
                 self.provider = IBMProvider(instance=instance_name)
             elif any([self.hub, self.group, self.project]):
-                #if only partially specified, print warning.
-                raise Exception("You've only partially specified the instance name. Either"
-                                "the hub, group or project is missing. hub: {}, group: {}, project: {}.\n"
-                                "The default instance will be used instead. (This default can "
-                                "be specified when doing `IBMProvider.save_account`)")
+                # if only partially specified, print warning.
+                raise Exception(
+                    "You've only partially specified the instance name. Either"
+                    "the hub, group or project is missing. hub: {}, group: {}, project: {}.\n"
+                    "The default instance will be used instead. (This default can "
+                    "be specified when doing `IBMProvider.save_account`)"
+                )
             return True
         except Exception as e:
             print(
                 "An Exception has occured when trying to connect with the provider."
                 "Please note that you are required to set up your IBMQ account locally first."
                 "See: https://quantum-computing.ibm.com/lab/docs/iql/manage/account/ibmq"
                 "for how to save your IBMQ account locally. \n {}".format(e)
```

### Comparing `openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/qaoa_qiskit_qpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,30 +58,40 @@
         qaoa_descriptor: QAOADescriptor,
         device: DeviceQiskit,
         n_shots: int,
         prepend_state: Optional[QuantumCircuit],
         append_state: Optional[QuantumCircuit],
         init_hadamard: bool,
         initial_qubit_mapping: Optional[List[int]] = None,
+        qiskit_optimization_level: int = 1,
         cvar_alpha: float = 1,
     ):
-
         QAOABaseBackendShotBased.__init__(
             self,
             qaoa_descriptor,
             n_shots,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
         )
         QAOABaseBackendCloud.__init__(self, device)
 
         self.qureg = QuantumRegister(self.n_qubits)
         self.problem_reg = self.qureg[0 : self.problem_qubits]
+        self.creg = ClassicalRegister(len(self.problem_reg))
+
+        if qiskit_optimization_level in [0, 1, 2, 3]:
+            self.qiskit_optimziation_level = qiskit_optimization_level
+        else:
+            raise ValueError(
+                f"qiskit_optimization_level cannot be {qiskit_optimization_level}. Choose between 0 to 3"
+            )
+        self.gate_applicator = QiskitGateApplicator()
+
         if self.initial_qubit_mapping is None:
             self.initial_qubit_mapping = (
                 initial_qubit_mapping
                 if initial_qubit_mapping is not None
                 else list(range(self.n_qubits))
             )
 
@@ -99,15 +109,14 @@
             raise Exception(
                 "Connection to {} was made. Error connecting to the specified backend.".format(
                     self.device.device_location.upper()
                 )
             )
 
         else:
-
             raise Exception(
                 "Error connecting to {}.".format(self.device.device_location.upper())
             )
 
         if self.device.n_qubits < self.n_qubits:
             raise Exception(
                 "There are lesser qubits on the device than the number of qubits required for the circuit."
@@ -124,32 +133,45 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         qaoa_circuit: `QuantumCircuit`
             The final QAOA circuit after binding angles from variational parameters.
         """
-
         angles_list = self.obtain_angles_for_pauli_list(self.abstract_circuit, params)
         memory_map = dict(zip(self.qiskit_parameter_list, angles_list))
         circuit_with_angles = self.parametric_circuit.bind_parameters(memory_map)
-        if self.qaoa_descriptor.routed == True:
+
+        if self.append_state:
+            circuit_with_angles = circuit_with_angles.compose(self.append_state)
+
+        # only measure the problem qubits
+        if self.final_mapping is None:
+            circuit_with_angles.measure(self.problem_reg, self.creg)
+        else:
+            for idx, qubit in enumerate(self.final_mapping[0 : len(self.problem_reg)]):
+                cbit = self.creg[idx]
+                circuit_with_angles.measure(qubit, cbit)
+
+        if self.qaoa_descriptor.routed is True:
             transpiled_circuit = transpile(
                 circuit_with_angles,
                 self.backend_qpu,
                 initial_layout=self.initial_qubit_mapping,
-                optimization_level=0,
+                optimization_level=self.qiskit_optimziation_level,
                 routing_method="none",
             )
         else:
             transpiled_circuit = transpile(
                 circuit_with_angles,
                 self.backend_qpu,
                 initial_layout=self.initial_qubit_mapping,
+                optimization_level=self.qiskit_optimziation_level,
             )
+
         return transpiled_circuit
 
     @property
     def parametric_qaoa_circuit(self) -> QuantumCircuit:
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
@@ -157,17 +179,15 @@
 
         Parameters
         ----------
             params:
                 Object of type QAOAVariationalBaseParams
         """
         # self.reset_circuit()
-        creg = ClassicalRegister(len(self.problem_reg))
-        parametric_circuit = QuantumCircuit(self.qureg, creg)
-        gate_applicator = QiskitGateApplicator()
+        parametric_circuit = QuantumCircuit(self.qureg, self.creg)
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.problem_reg)
 
@@ -177,28 +197,17 @@
             if each_gate.gate_label.type.value in ["MIXER", "COST"]:
                 angle_param = Parameter(each_gate.gate_label.__repr__())
                 self.qiskit_parameter_list.append(angle_param)
                 each_gate.angle_value = angle_param
             decomposition = each_gate.decomposition("standard")
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0](gate_applicator, *each_tuple[1])
+                gate = each_tuple[0](self.gate_applicator, *each_tuple[1])
                 gate.apply_gate(parametric_circuit)
 
-        if self.append_state:
-            parametric_circuit = parametric_circuit.compose(self.append_state)
-
-        # only measure the problem qubits
-        if self.final_mapping is None:
-            parametric_circuit.measure(self.problem_reg, creg)
-        else:
-            for idx, qubit in enumerate(self.final_mapping[0 : len(self.problem_reg)]):
-                cbit = creg[idx]
-                parametric_circuit.measure(qubit, cbit)
-
         return parametric_circuit
 
     def get_counts(self, params: QAOAVariationalBaseParams, n_shots=None) -> dict:
         """
         Execute the circuit and obtain the counts
 
         Parameters
@@ -211,33 +220,33 @@
 
         Returns
         -------
             A dictionary with the bitstring as the key and the number of counts
             as its value.
         """
 
-        n_shots = self.n_shots if n_shots == None else n_shots
+        n_shots = self.n_shots if n_shots is None else n_shots
 
         circuit = self.qaoa_circuit(params)
 
         job_state = False
         no_of_job_retries = 0
         max_job_retries = 5
 
-        while job_state == False:
+        while job_state is False:
             # initial_layout only passed if not azure device
             # if type(self.device).__name__ == "DeviceAzure":
             # job = self.backend_qpu.run(circuit, **input_items)
             job = self.backend_qpu.run(circuit, shots=n_shots)
 
             api_contact = False
             no_of_api_retries = 0
             max_api_retries = 5
 
-            while api_contact == False:
+            while api_contact is False:
                 try:
                     self.job_id = job.job_id()
                     counts = job.result().get_counts()
                     api_contact = True
                     job_state = True
                 except (IBMJobApiError, IBMJobTimeoutError):
                     print("There was an error when trying to contact the IBMQ API.")
```

### Comparing `openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/openqaoa_qiskit/backends/qaoa_qiskit_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,24 @@
         append_state: Optional[QuantumCircuit],
         init_hadamard: bool,
         cvar_alpha: float,
         qiskit_simulation_method: str = "automatic",
         seed_simulator: Optional[int] = None,
         noise_model: Optional[NoiseModel] = None,
     ):
-
         QAOABaseBackendShotBased.__init__(
             self,
             qaoa_descriptor,
             n_shots,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
         )
-
+        self.gate_applicator = QiskitGateApplicator()
         self.qureg = QuantumRegister(self.n_qubits)
 
         if self.prepend_state:
             assert self.n_qubits >= len(prepend_state.qubits), (
                 "Cannot attach a bigger circuit " "to the QAOA routine"
             )
         # options = {"seed_simulator":1}
@@ -131,30 +130,35 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         qaoa_circuit: `QuantumCircuit`
             The final QAOA circuit after binding angles from variational parameters.
         """
-
         angles_list = self.obtain_angles_for_pauli_list(self.abstract_circuit, params)
         memory_map = dict(zip(self.qiskit_parameter_list, angles_list))
-        new_parametric_circuit = self.parametric_circuit.bind_parameters(memory_map)
-        return new_parametric_circuit
+        circuit_with_angles = self.parametric_circuit.bind_parameters(memory_map)
+
+        if self.append_state:
+            circuit_with_angles = circuit_with_angles.compose(self.append_state)
+        circuit_with_angles.measure_all()
+
+        return circuit_with_angles
 
     @property
     def parametric_qaoa_circuit(self) -> QuantumCircuit:
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
         the circuit.
         """
         # self.reset_circuit()
-        parametric_circuit = QuantumCircuit(self.qureg)
-        gate_applicator = QiskitGateApplicator()
+        parametric_circuit = QuantumCircuit(
+            self.qureg
+        )  # consider changing this too with my new function
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.qureg)
 
@@ -170,21 +174,17 @@
                 in QAOAQiskitBackendShotBasedSimulator.QISKIT_GATEMAP_LIBRARY
             ):
                 decomposition = each_gate.decomposition("trivial")
             else:
                 decomposition = each_gate.decomposition("standard")
             # Create Circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0](gate_applicator,*each_tuple[1])
+                gate = each_tuple[0](self.gate_applicator, *each_tuple[1])
                 gate.apply_gate(parametric_circuit)
 
-        if self.append_state:
-            parametric_circuit = parametric_circuit.compose(self.append_state)
-        parametric_circuit.measure_all()
-
         return parametric_circuit
 
     def get_counts(self, params: QAOAVariationalBaseParams, n_shots=None) -> dict:
         """
         Returns the counts of the final QAOA circuit after binding angles from variational parameters.
 
         Parameters
@@ -272,29 +272,29 @@
         self,
         qaoa_descriptor: QAOADescriptor,
         prepend_state: Optional[Union[np.ndarray, QuantumCircuit]],
         append_state: Optional[Union[np.ndarray, QuantumCircuit]],
         init_hadamard: bool,
         cvar_alpha: float = 1,
     ):
-
         QAOABaseBackendStatevector.__init__(
             self,
             qaoa_descriptor,
             prepend_state,
             append_state,
             init_hadamard,
             cvar_alpha,
         )
 
         assert (
             cvar_alpha == 1
         ), "Please use the shot-based simulator for simulations with cvar_alpha < 1"
 
         self.qureg = QuantumRegister(self.n_qubits)
+        self.gate_applicator = QiskitGateApplicator()
 
         if self.prepend_state:
             assert self.n_qubits >= len(prepend_state.qubits), (
                 "Cannot attach a bigger circuit " "to the QAOA routine"
             )
 
         # For parametric circuits
@@ -343,16 +343,16 @@
             The final QAOA circuit after binding angles from variational parameters.
         """
         # generate a job id for the wavefunction evaluation
         self.job_id = generate_uuid()
 
         angles_list = self.obtain_angles_for_pauli_list(self.abstract_circuit, params)
         memory_map = dict(zip(self.qiskit_parameter_list, angles_list))
-        new_parametric_circuit = self.parametric_circuit.bind_parameters(memory_map)
-        return new_parametric_circuit
+        circuit_with_angles = self.parametric_circuit.bind_parameters(memory_map)
+        return circuit_with_angles
 
     @property
     def parametric_qaoa_circuit(self) -> QuantumCircuit:
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
         the circuit. To do this, you will need to subsequently execute the command self.eng.flush().
@@ -360,15 +360,14 @@
         Parameters
         ----------
             params:
                 Object of type QAOAVariationalBaseParams
         """
         # self.reset_circuit()
         parametric_circuit = QuantumCircuit(self.qureg)
-        gate_applicator = QiskitGateApplicator()
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.qureg)
 
@@ -384,15 +383,15 @@
                 in QAOAQiskitBackendStatevecSimulator.QISKIT_GATEMAP_LIBRARY
             ):
                 decomposition = each_gate.decomposition("trivial")
             else:
                 decomposition = each_gate.decomposition("standard")
             # Create Circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0](gate_applicator,*each_tuple[1])
+                gate = each_tuple[0](self.gate_applicator, *each_tuple[1])
                 gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit = parametric_circuit.compose(self.append_state)
 
         return parametric_circuit
```

### Comparing `openqaoa-0.1.3/src/openqaoa.egg-info/PKG-INFO` & `openqaoa-0.1.3rc1/src/openqaoa.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: openqaoa
-Version: 0.1.3
+Version: 0.1.3rc1
 Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo_offW.png" width="650">
   <img alt="OpenQAOA" src="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo.png" width="650">
@@ -34,92 +31,97 @@
   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/entropicalabs/openqaoa.git/main?labpath=%2Fexamples)
   [![Discord](https://img.shields.io/discord/991258119525122058)](https://discord.gg/ana76wkKBd)
   [![Website](https://img.shields.io/badge/OpenQAOA-Website-blueviolet)](https://openqaoa.entropicalabs.com/) 
 </div>
 
 # OpenQAOA
 
-A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators.
-
+A multi-backend python library for quantum optimization using QAOA on Quantum computers and Quantum computer simulators. Check out the OpenQAOA website at [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
+ 
 **OpenQAOA is currently in OpenBeta.**
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
-Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
-
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
+OpenQAOA is divided into separately installable plugins based on the requirements of the user. The core elements of the package are placed in `openqaoa-core` which comes pre-installed with each flavour of OpenQAOA. 
+
+Currently, OpenQAOA supports the following backends and each can be installed exclusively with the exception of `openqaoa-azure` which installs `openqaoa-qiskit` as an additional requirement because Azure backends support circuit submissions via `qiskit`.
+- `openqaoa-braket` for AWS Braket
+- `openqaoa-azure` for Microsoft Azure Quantum
+- `openqaoa-pyquil` for Rigetti Pyquil
+- `openqaoa-qiskit` for IBM Qiskit
 
+The OpenQAOA metapackage, `openqaoa` allows you to install all OpenQAOA plug-ins together.
+### Install via PyPI
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 ```
 pip install openqaoa
 ```
+### Install via git clone
+Alternatively, you can install OpenQAOA manually from the GitHub repository by following the instructions below. 
 
-Alternatively, you can install manually directly from the GitHub repository by
-
+**NOTE:** We recommend creating a python virtual environment for this project using a python environment manager, for instance Anaconda. Instructions can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 1. Clone the git repository:
-
 ```
 git clone https://github.com/entropicalabs/openqaoa.git
 ```
-
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
-
-3. After cloning the repository `cd openqaoa` and pip install the package. 
-
+2. After cloning the repository `cd openqaoa` and pip install the package with instructions from the Makefile as follows
 ```
-pip install .
+make local-install
 ```
-If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
 
+### Installation instructions for Developers
+Users can install OpenQAOA in the developer mode via the Makefile. For a clean editable install of the package run the following command from the `openqaoa` folder.
 ```
-pip install .[tests]
+make dev-install
 ```
+The package can be installed as an editable with extra requirements defined in the `setup.py`. If you would like to install the extra requirements to be able run the tests module or generate the docs, you can run the following
 
+```
+make dev-install-x,   with x = {tests, docs, all}
+```
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
-The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
-
-We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
+The API documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/). We also provide a set of tutorials to get you started. Among the many, perhaps you can get started with the following ones:
 
 - [Run your first OpenQAOA workflow](https://el-openqaoa.readthedocs.io/en/latest/notebooks/01_workflows_example.html)
 - [How about trying some RQAOA for a change?](https://el-openqaoa.readthedocs.io/en/latest/notebooks/09_RQAOA_example.html)
 - [Introducing EL's fast QAOA simulator](https://el-openqaoa.readthedocs.io/en/latest/notebooks/06_fast_qaoa_simulator.html)
 - [Discover OpenQAOA's custom parametrizations](https://el-openqaoa.readthedocs.io/en/latest/notebooks/05_advanced_parameterization.html)
 
 ### Key Features
 
 - **Build advanced QAOAs**. Create complex QAOAs by specifying custom _parametrisation_, _mixer hamiltonians_, _classical optimisers_ and execute the algorithm on either simulators or QPUs.
 
 - **Recursive QAOA**. Run RQAOA with fully customisable schedules on simulators and QPUs alike. 
 
-- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, and `Amazon Braket`.
+- **QPU access**. Built in access for `IBM Quantum`, `Rigetti QCS`, `Amazon Braket` and `Azure Quantum`.
 
 
 ### Available devives 
 
 Devices are serviced both locally and on the cloud. For the IBM Quantum experience, the available devices depend on the specified credentials. For QCS and Amazon Braket, the available devices are listed in the table below:
 
-| Device location  | Device Name |
-| ------------- | ------------- |
-| `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
+| Device location | Device Name |
+| --------------- | ----------- |
+| local | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
 | [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
-
 ## Running the tests
 
-To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
-
-> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
+To run the unit-tests, first, make sure to have installed all the optional testing dependencies by running `make dev-install-tests`. Next type `pytest tests/ /src/*/tests/` from the project's root folder. This runs the common metapackage unit-tests and the unit-tests for each OpenQAOA plugin.
 
-> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
+:warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
+:warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+     
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
+We are always interested to hear about projects built with OpenQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.3/tests/test_analytical_simulator.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_analytical_simulator.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_aws_managed_jobs.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_aws_managed_jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import pytest
 import unittest
 import networkx as nw
 from braket.jobs.local import LocalQuantumJob
 from unittest.mock import MagicMock
 
 from openqaoa.problems import MinimumVertexCover
-from openqaoa.algorithms import AWSJobs
+from openqaoa_braket.algorithms import AWSJobs
 from openqaoa.algorithms import QAOA, RQAOA
 from openqaoa.backends import create_device
 
 
 class TestingAwsJobs(unittest.TestCase):
     def setUp(self):
         # the input data directory opt/braket/input/data
-        os.environ["AMZN_BRAKET_INPUT_DIR"] = "./tests/jobs_test_input/"
+        os.environ["AMZN_BRAKET_INPUT_DIR"] = "./src/openqaoa-braket/tests/jobs_test_input/"
         # the output directory opt/braket/model to write ob results to
         os.environ["AMZN_BRAKET_JOB_RESULTS_DIR"] = "/oq_release_tests/testing_jobs/"
         # the name of the job
         os.environ["AMZN_BRAKET_JOB_NAME"] = "oq_release_test"
         # the checkpoint directory
         os.environ["AMZN_BRAKET_CHECKPOINT_DIR"] = "oq_test_suite_checkpoint"
         # the hyperparameter
@@ -59,18 +59,17 @@
         self.n_qubits = 10
 
         self.vc = MinimumVertexCover(
             nw.circulant_graph(self.n_qubits, [1]), field=1.0, penalty=10
         ).qubo
 
     def testOsEnvironAssignment(self):
-
         qaoa_workflow = AWSJobs(algorithm="QaoA")
         assert qaoa_workflow.algorithm == "qaoa"
-        assert qaoa_workflow.input_dir == "./tests/jobs_test_input/"
+        assert qaoa_workflow.input_dir == "./src/openqaoa-braket/tests/jobs_test_input/"
         assert qaoa_workflow.device.device_name == os.environ["AMZN_BRAKET_DEVICE_ARN"]
 
         rqaoa_workflow = AWSJobs(algorithm="rqAoa")
         assert rqaoa_workflow.algorithm == "rqaoa"
         assert rqaoa_workflow.device.device_name == os.environ["AMZN_BRAKET_DEVICE_ARN"]
 
     @pytest.mark.docker_aws
@@ -79,45 +78,44 @@
 
         input_data_path = os.path.join(
             os.environ["AMZN_BRAKET_INPUT_DIR"], "input_data/"
         )
 
         # Create the qubo and the qaoa
         q = QAOA()
-        q.set_classical_optimizer(maxiter='5')
+        q.set_classical_optimizer(maxiter="5")
         q.set_device(
             create_device("aws", "arn:aws:braket:::device/quantum-simulator/amazon/sv1")
         )
-        
+
         ### The following lines are needed to fool the github actions into correctly executing q.compile() !!
-        q.device.check_connection = MagicMock(return_value = True)
+        q.device.check_connection = MagicMock(return_value=True)
         q.device.qpu_connected = True
         q.device.provider_connected = True
         q.device.n_qubits = self.n_qubits
-        q.device.backend_device = ''
-        q.device.aws_region = 'us-east-1'
+        q.device.backend_device = ""
+        q.device.aws_region = "us-east-1"
 
         q.compile(self.vc)
         q.dump(
             file_name="openqaoa_params.json",
             file_path=input_data_path,
             prepend_id=False,
             overwrite=True,
         )
 
         job = LocalQuantumJob.create(
             device="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
-            source_module="./tests/jobs_test_input/aws_braket_source_module/openqaoa_qaoa_script.py",
+            source_module="./src/openqaoa-braket/tests/jobs_test_input/aws_braket_source_module/openqaoa_qaoa_script.py",
             image_uri="amazon-braket-oq-dev",
             input_data={"input_data": input_data_path},
         )
 
         assert (job.state() == "COMPLETED") and (job.result() != None) == True
 
-
     @pytest.mark.docker_aws
     def testLocalJobRQAOA(self):
         """Test an end-to-end rqaoa running on a local docker instance"""
 
         input_data_path = os.path.join(
             os.environ["AMZN_BRAKET_INPUT_DIR"], "input_data/"
         )
@@ -125,34 +123,34 @@
         # Create the rqaoa
         r = RQAOA()
         r.set_rqaoa_parameters(n_cutoff=6)
         r.set_classical_optimizer(maxiter=3, save_intermediate=False)
         r.set_device(
             create_device("aws", "arn:aws:braket:::device/quantum-simulator/amazon/sv1")
         )
-        
+
         ### The following lines are needed to fool the github actions into correctly executing q.compile() !!
-        r.device.check_connection = MagicMock(return_value = True)
+        r.device.check_connection = MagicMock(return_value=True)
         r.device.qpu_connected = True
         r.device.provider_connected = True
         r.device.n_qubits = self.n_qubits
-        r.device.backend_device = ''
-        r.device.aws_region = 'us-east-1'
+        r.device.backend_device = ""
+        r.device.aws_region = "us-east-1"
 
         r.compile(self.vc)
         r.dump(
             file_name="openqaoa_params.json",
             file_path=input_data_path,
             prepend_id=False,
             overwrite=True,
         )
 
         job = LocalQuantumJob.create(
             device="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
-            source_module="./tests/jobs_test_input/aws_braket_source_module/openqaoa_rqaoa_script.py",
+            source_module="./src/openqaoa-braket/tests/jobs_test_input/aws_braket_source_module/openqaoa_rqaoa_script.py",
             image_uri="amazon-braket-oq-dev",
             input_data={"input_data": input_data_path},
         )
 
         assert (job.state() == "COMPLETED") and (job.result() != None) == True
```

### Comparing `openqaoa-0.1.3/tests/test_benchmark.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pytest
 import sys
 
 from openqaoa import QAOA, create_device, QAOABenchmark
 from openqaoa.problems import QUBO
+from openqaoa.backends.devices_core import SUPPORTED_LOCAL_SIMULATORS
 
 
 def there_is_an_error(function, **kwargs):
     error = False
     try:
         function(**kwargs)
     except:
         error = True
     return error
 
 
 class TestingBenchmark(unittest.TestCase):
+
     def test_simple_benchmark(self):
         "Test the simplest benchmark."
 
         qaoa = QAOA()
         qaoa.set_device(create_device(name="analytical_simulator", location="local"))
         qaoa.compile(QUBO.random_instance(5))
 
@@ -64,27 +66,27 @@
 
         qaoa_vectorized = QAOA()
         qaoa_vectorized.set_device(create_device(name="vectorized", location="local"))
         qaoa_vectorized.compile(QUBO.random_instance(5))
 
         # standard qaoa should have a analytical reference
         qaoa = QAOA()
-        qaoa.set_device(create_device(name="qiskit.shot_simulator", location="local"))
+        qaoa.set_device(create_device(name="vectorized", location="local"))
         qaoa.compile(QUBO.random_instance(5))
         benchmark = QAOABenchmark(qaoa)
         assert isinstance(
             benchmark.reference, QAOA
         ), "The qaoa reference should be a QAOA object."
         assert isinstance(
             benchmark.reference.backend, type(qaoa_analytical.backend)
         ), "The qaoa reference should have an analytical backend."
 
         # p>1 qaoa should have a vectorized reference
         qaoa = QAOA()
-        qaoa.set_device(create_device(name="qiskit.shot_simulator", location="local"))
+        qaoa.set_device(create_device(name="vectorized", location="local"))
         qaoa.set_circuit_properties(p=2)
         qaoa.compile(QUBO.random_instance(5))
         benchmark = QAOABenchmark(qaoa)
         assert isinstance(
             benchmark.reference, QAOA
         ), "The qaoa reference should be a QAOA object."
         assert isinstance(
@@ -305,14 +307,17 @@
     @pytest.mark.skipif(
         sys.platform == "darwin" or sys.platform.startswith("win"),
         reason="Test does not run on Mac and Windows currently",
     )
     def test_difference(self):
         "Test the property difference and difference_mean."
 
+        if "qiskit.shot_simulator" not in SUPPORTED_LOCAL_SIMULATORS:
+            self.skipTest(reason="The Qiskit Shot Simulator is currently not available. Please install the openqaoa-qiskit plugin.")
+
         # device shot-based
         qaoa = QAOA()
         qaoa.set_device(create_device(location="local", name="qiskit.shot_simulator"))
         qaoa.compile(QUBO.random_instance(5))
 
         benchmark = QAOABenchmark(qaoa)
         benchmark.run(n_points_axis=4, ranges=[(0, np.pi), (-5, 9)])
@@ -323,14 +328,17 @@
         assert np.all(
             benchmark.difference == benchmark.values - benchmark.values_reference
         ), "The difference matrix should be the difference between the values and the reference values."
         assert benchmark.difference_mean == np.mean(
             benchmark.difference
         ), "The difference mean should be the mean of the difference matrix."
 
+    def test_difference(self):
+        "Test the property difference and difference_mean."
+
         # test raise errors if not run main or run reference
         qaoa = QAOA()
         qaoa.compile(QUBO.random_instance(5))
         benchmark = QAOABenchmark(qaoa)
 
         error = False
         try:
```

### Comparing `openqaoa-0.1.3/tests/test_circuit_routing.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_circuit_routing_pyquil.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from openqaoa.qaoa_components import (
     create_qaoa_variational_params,
     QAOADescriptor,
     PauliOp,
     Hamiltonian,
 )
 from openqaoa.utilities import X_mixer_hamiltonian
-from openqaoa.problems import NumberPartition, Knapsack, MaximumCut, ShortestPath
+from openqaoa.backends import create_device
+from openqaoa.problems import MaximumCut, ShortestPath
 from openqaoa_pyquil.backends import DevicePyquil, QAOAPyQuilQPUBackend
 from openqaoa.backends.devices_core import DeviceBase
 from openqaoa.qaoa_components.ansatz_constructor.gatemap import SWAPGateMap
 
 
 class TestingQAOAPyquilQVM_QR(unittest.TestCase):
 
@@ -591,220 +592,14 @@
             self.initial_physical_to_logical_mapping,
             self.final_logical_qubit_order,
         )
 
 
 class TestingQubitRouting(unittest.TestCase):
     def setUp(self):
-        """
-        Test edge cases
-        """
-        # case qubits device > qubits problem (IBM NAIROBI)
-        self.IBM_NAIROBI_KNAPSACK = ExpectedRouting(
-            qubo=Knapsack.random_instance(n_items=3, seed=20).qubo,
-            device_location="ibmq",
-            device_name="ibm_nairobi",
-            qpu_credentials={
-                "hub": "ibm-q",
-                "group": "open",
-                "project": "main",
-                "as_emulator": True,
-            },
-            problem_to_solve=[
-                (0, 1),
-                (2, 3),
-                (2, 4),
-                (3, 4),
-                (0, 2),
-                (0, 3),
-                (0, 4),
-                (1, 2),
-                (1, 3),
-                (1, 4),
-            ],
-            initial_mapping=None,
-            gate_indices_list=[
-                [2, 4],
-                [1, 2],
-                [3, 5],
-                [0, 5],
-                [4, 5],
-                [4, 5],
-                [2, 4],
-                [0, 5],
-                [2, 4],
-                [1, 2],
-                [4, 5],
-                [0, 5],
-                [1, 2],
-                [2, 4],
-                [2, 4],
-                [0, 5],
-                [4, 5],
-            ],
-            swap_mask=[
-                False,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                True,
-                False,
-                True,
-                False,
-                True,
-                True,
-                False,
-            ],
-            initial_physical_to_logical_mapping={6: 0, 2: 1, 1: 2, 4: 3, 3: 4, 5: 5},
-            final_logical_qubit_order=[5, 4, 0, 1, 2, 3],
-        )
-
-        # case qubits problem == 2 (IBM OSLO)
-        self.IBM_OSLO_QUBO2 = ExpectedRouting(
-            qubo=QUBO.from_dict(
-                {
-                    "terms": [[0, 1], [1]],
-                    "weights": [9.800730090617392, 26.220558065741773],
-                    "n": 2,
-                }
-            ),
-            device_location="ibmq",
-            device_name="ibm_oslo",
-            qpu_credentials={
-                "hub": "ibm-q",
-                "group": "open",
-                "project": "main",
-                "as_emulator": True,
-            },
-            problem_to_solve=[(0, 1)],
-            initial_mapping=None,
-            gate_indices_list=[[0, 2], [1, 2]],
-            swap_mask=[True, False],
-            initial_physical_to_logical_mapping={2: 0, 3: 1, 1: 2},
-            final_logical_qubit_order=[2, 1, 0],
-        )
-
-        # case qubits device == qubits problem (IBM OSLO)
-        self.IBM_OSLO_NPARTITION = ExpectedRouting(
-            qubo=NumberPartition.random_instance(n_numbers=7, seed=2).qubo,
-            device_location="ibmq",
-            device_name="ibm_oslo",
-            qpu_credentials={
-                "hub": "ibm-q",
-                "group": "open",
-                "project": "main",
-                "as_emulator": True,
-            },
-            problem_to_solve=[
-                (0, 1),
-                (0, 2),
-                (0, 3),
-                (0, 4),
-                (0, 5),
-                (0, 6),
-                (1, 2),
-                (1, 3),
-                (1, 4),
-                (1, 5),
-                (1, 6),
-                (2, 3),
-                (2, 4),
-                (2, 5),
-                (2, 6),
-                (3, 4),
-                (3, 5),
-                (3, 6),
-                (4, 5),
-                (4, 6),
-                (5, 6),
-            ],
-            initial_mapping=None,
-            gate_indices_list=[
-                [0, 5],
-                [1, 5],
-                [3, 4],
-                [4, 5],
-                [2, 3],
-                [3, 6],
-                [4, 5],
-                [0, 5],
-                [1, 5],
-                [3, 4],
-                [3, 4],
-                [2, 3],
-                [3, 6],
-                [4, 5],
-                [0, 5],
-                [1, 5],
-                [2, 3],
-                [3, 6],
-                [3, 4],
-                [3, 4],
-                [3, 6],
-                [0, 5],
-                [1, 5],
-                [4, 5],
-                [4, 5],
-                [1, 5],
-                [3, 6],
-                [3, 4],
-                [3, 4],
-                [1, 5],
-                [4, 5],
-            ],
-            swap_mask=[
-                False,
-                False,
-                False,
-                False,
-                False,
-                False,
-                True,
-                False,
-                False,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                True,
-                False,
-                False,
-                True,
-                False,
-                True,
-                False,
-                True,
-                True,
-                False,
-            ],
-            initial_physical_to_logical_mapping={
-                0: 0,
-                2: 1,
-                4: 2,
-                5: 3,
-                3: 4,
-                1: 5,
-                6: 6,
-            },
-            final_logical_qubit_order=[3, 5, 1, 0, 6, 2, 4],
-        )
 
         # case qubits device > qubits problem (RIGETTI)
         self.RIGETTI_SHORTESTPATH = ExpectedRouting(
             qubo=ShortestPath.random_instance(
                 n_nodes=4, edge_probability=0.9, seed=20
             ).qubo,
             device_location="qcs",
```

### Comparing `openqaoa-0.1.3/tests/test_converters.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_custom_mixer.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_custom_mixer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 )
 from openqaoa.problems import MinimumVertexCover
 from openqaoa.qaoa_components.ansatz_constructor.gatemaplabel import GateMapType
 
 
 class TestingCustomMixer(unittest.TestCase):
     def setUp(self):
-
         nodes = 6
         edge_probability = 0.7
         g = nx.generators.fast_gnp_random_graph(n=nodes, p=edge_probability, seed=34)
         mini_cov = MinimumVertexCover(g, field=1.0, penalty=1.0)
         self.PROBLEM_QUBO = mini_cov.qubo
 
         # Case with Mixer with 1 AND 2-qubit terms
@@ -90,68 +89,61 @@
                 self.COMPLICATED_GATEMAP_LIST,
                 self.COMPLICATED_COEFFS,
                 self.COMPLICATED_SEQUENCE,
             ],
         ]
 
     def test_custom_mixer_basic_workflow(self):
-
         """
         Check that using custom mixers works.
         Custom Mixers are only available in Manual mode.
         """
 
         for each_gatemap_list, each_gatemap_coeffs, _ in self.TESTING_GATEMAPS:
-
             custom_mixer_block_gatemap = each_gatemap_list
             custom_mixer_block_coeffs = each_gatemap_coeffs
 
             qaoa_descriptor = QAOADescriptor(
                 self.PROBLEM_QUBO.hamiltonian,
                 custom_mixer_block_gatemap,
                 p=1,
                 mixer_coeffs=custom_mixer_block_coeffs,
             )
-            device_local = create_device(location="local", name="qiskit.shot_simulator")
+            device_local = create_device(location="local", name="vectorized")
             variate_params = create_qaoa_variational_params(
                 qaoa_descriptor, "standard", "rand"
             )
             backend_local = get_qaoa_backend(qaoa_descriptor, device_local, n_shots=500)
             optimizer = get_optimizer(
                 backend_local, variate_params, {"method": "cobyla", "maxiter": 10}
             )
             optimizer.optimize()
 
     def test_mixer_block_properties_sequence(self):
-
         """
         The custom mixers should have sequences that are correct.
         The sequence values are based on the position of the gate in the block
         relative to other gates of the same qubit count.
         """
 
         for (
             each_gatemap_list,
             each_gatemap_coeffs,
             correct_seq,
         ) in self.TESTING_GATEMAPS:
-
             gatemap_list_sequence = []
             one_qubit_count = 0
             two_qubit_count = 0
 
             for each_gatemap in each_gatemap_list:
-
                 if each_gatemap.gate_label.n_qubits == 1:
-
                     gatemap_list_sequence.append(one_qubit_count)
                     one_qubit_count += 1
 
                 elif each_gatemap.gate_label.n_qubits == 2:
-
                     gatemap_list_sequence.append(two_qubit_count)
                     two_qubit_count += 1
 
             # Test Equality between hand-written and programmatic assignment
             self.assertEqual(gatemap_list_sequence, correct_seq)
 
             qaoa_descriptor = QAOADescriptor(
@@ -166,61 +158,56 @@
                 for each_mixer_gatemap in qaoa_descriptor.mixer_block
             ]
 
             # Test Equality between OQ and hand-written sequence
             self.assertEqual(descriptor_mixer_seq, correct_seq)
 
     def test_set_block_sequence(self):
-
         """
         Check that the set block sequence method is correct.
         """
 
         for (
             each_gatemap_list,
             each_gatemap_coeffs,
             correct_seq,
         ) in self.TESTING_GATEMAPS:
-
             output_gatemap_list = QAOADescriptor.set_block_sequence(each_gatemap_list)
             output_seq = [
                 each_gatemap.gate_label.sequence for each_gatemap in output_gatemap_list
             ]
 
             self.assertEqual(output_seq, correct_seq)
 
     def test_set_block_sequence_error_raises(self):
-
         """
         Check that the set block sequence method raises the right error when the
         wrong type is passed. A TypeError should be raised if the input_gatemap_list
         if not a List of RotationGateMap Objects.
         """
 
         incorrect_input_iterable = [""], [1], [SWAPGateMap(0, 1)], [RXGateMap]
 
         for each_iterable in incorrect_input_iterable:
             with self.assertRaises(TypeError):
                 QAOADescriptor.set_block_sequence(each_iterable)
 
     def test_block_setter(self):
-
         """
         Check that block_setter method correctly maps the sequence and the type
         of the RotationGateMap Objects returned.
         """
 
         input_enum_type = GateMapType.MIXER
 
         for (
             each_gatemap_list,
             each_gatemap_coeffs,
             correct_seq,
         ) in self.TESTING_GATEMAPS:
-
             output_gatemap_list = QAOADescriptor.block_setter(
                 each_gatemap_list, input_enum_type
             )
 
             output_type = [
                 each_gatemap.gate_label.type for each_gatemap in output_gatemap_list
             ]
@@ -231,15 +218,14 @@
             # sequence and type should be labelled correctly.
             self.assertEqual(output_seq, correct_seq)
             self.assertEqual(
                 output_type, [input_enum_type for _ in range(len(correct_seq))]
             )
 
     def test_block_setter_error_raises(self):
-
         """
         The block_setter method should raise a ValueError if the input_object is
         not of the type Hamiltonian or List. It should also raise a TypeError if
         the List contains elements that are not of the type RotationGateMap.
         """
 
         incorrect_input_object = [(), "", 1]
@@ -259,15 +245,14 @@
         for each_input_iterable in incorrect_input_iterable:
             with self.assertRaises(TypeError):
                 QAOADescriptor.block_setter(
                     input_object=each_input_iterable, block_type=GateMapType.MIXER
                 )
 
     def test_block_setter_equivalence_simple(self):
-
         """
         A Hamiltonian Object and a list of RotationGateMap should have both their
         sequence and type assigned the same if they represent the same gate sequence.
         """
 
         # 1-Qubit
         test_hamiltonian = X_mixer_hamiltonian(3)
```

### Comparing `openqaoa-0.1.3/tests/test_derivative.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_derivative.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
             for i, grad in enumerate(grad_fd):
                 assert np.isclose(grad, grad_ps[i], rtol=1e-05, atol=1e-05)
                 assert np.isclose(grad, grad_sps[i], rtol=1e-05, atol=1e-05)
     """
 
     def setUp(self):
-
         self.log = Logger(
             {
                 "func_evals": {
                     "history_update_bool": False,
                     "best_update_string": "HighestOnly",
                 },
                 "jac_func_evals": {
@@ -188,19 +187,17 @@
             )
             for type_ in gradients_types_list
         ]
 
         test_points = [[0, 0], [np.pi / 2, np.pi / 3], [1, 2]]
 
         for point in test_points:
-
             for gradient_fun, gradient_name in zip(
                 gradients_fun_list, gradients_types_list
             ):
-
                 # compute gradient for each point with number of shots 1000 for ech function evaluation
                 grad, var, n_shots = gradient_fun(point, n_shots=1000)
 
                 # check if there is a gradient and variance (we can't check the value of the gradient and variance because it is randomly computed, since n_shots is 1000)
                 for g in grad:
                     assert (
                         np.abs(g) >= 0
```

### Comparing `openqaoa-0.1.3/tests/test_gate_applicators_braket.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_gate_applicators_pyquil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,255 +1,391 @@
 import unittest
 
-from braket.circuits import gates as brk_gate
-from braket.circuits import Circuit
+from pyquil import Program, gates
 
 import openqaoa
 import openqaoa.qaoa_components.ansatz_constructor.gates as oq_gate_mod
-from openqaoa_braket.backends.gates_braket import BraketGateApplicator
+from openqaoa_pyquil.backends.gates_pyquil import PyquilGateApplicator
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 
-class TestBraketGateApplicator(unittest.TestCase):
-    
+
+class TestPyquilGateApplicator(unittest.TestCase):
     def setUp(self):
-        
-        available_gates = [each_subclass_gate for each_subclass_gate in brk_gate.Gate.__subclasses__()]
-        available_gates.extend([each_subclass_gate for each_subclass_gate in brk_gate.AngledGate.__subclasses__()])
-        
-        available_braket_gates_name = [each_gate.__name__.lower() for each_gate in available_gates]
-        self.available_braket_gates = dict(zip(available_braket_gates_name, 
-                                               available_gates))
-        
-        self.oq_available_gates = tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+        available_gates = []
+        available_pyquil_gates_name = []
+        for each_gate_name, each_gate_function in gates.QUANTUM_GATES.items():
+            available_gates.append(each_gate_function)
+            available_pyquil_gates_name.append(each_gate_name.lower())
+        self.available_pyquil_gates = dict(
+            zip(available_pyquil_gates_name, available_gates)
+        )
+
+        self.oq_available_gates = (
+            tuple(
+                [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+                ]
+            )
+            + tuple(
+                [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+                ]
+            )
+        )
+
         # OneQubitGate, OneQubitRotationGate, TwoQubitGate, TwoQubitRotationGate are not acceptable inputs into the function even though they are of the Gate class
-        # RXY, RZX and RYZ are not supported by Braket library
-        self.braket_excluded_gates = [oq_gate_mod.OneQubitGate, oq_gate_mod.OneQubitRotationGate, 
-                          oq_gate_mod.TwoQubitGate, oq_gate_mod.TwoQubitRotationGate, 
-                          oq_gate_mod.RXY, oq_gate_mod.RZX, oq_gate_mod.RYZ]
-    
+        # RXX, RYY, RZZ, RXY, RZX and RYZ are not supported by Pyquil library
+        self.pyquil_excluded_gates = [
+            oq_gate_mod.OneQubitGate,
+            oq_gate_mod.OneQubitRotationGate,
+            oq_gate_mod.TwoQubitGate,
+            oq_gate_mod.TwoQubitRotationGate,
+            oq_gate_mod.RXX,
+            oq_gate_mod.RYY,
+            oq_gate_mod.RZZ,
+            oq_gate_mod.RXY,
+            oq_gate_mod.RZX,
+            oq_gate_mod.RYZ,
+        ]
+
     def test_gate_applicator_mapper(self):
-        
         """
         The mapper to the gate applicator should only contain gates that
         are trivially support by the library.
         """
 
-        for each_gate in BraketGateApplicator.BRAKET_OQ_GATE_MAPPER.values():
-            
-            self.assertTrue(each_gate.__name__ in self.available_braket_gates.keys(), '{}, {}'.format(each_gate.__name__, self.available_braket_gates.keys()))
-            
+        for each_gate in PyquilGateApplicator.PYQUIL_OQ_GATE_MAPPER.values():
+            self.assertTrue(
+                each_gate.__name__.lower() in self.available_pyquil_gates.keys(),
+                "{}, {}".format(each_gate.__name__, self.available_pyquil_gates.keys()),
+            )
+
     def test_gate_selector(self):
-        
         """
-        This method should return the Braket Gate object based on the input OQ 
+        This method should return the Pyquil Gate object based on the input OQ
         Gate object.
         """
-        
-        gate_applicator = BraketGateApplicator()
-        
-        oq_gate_list = tuple([each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()])
-        
-        oq_gate_list_1q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()])
-        
+
+        gate_applicator = PyquilGateApplicator()
+
+        oq_gate_list = tuple(
+            [each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()]
+        )
+
+        oq_gate_list_1q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_1q:
-            if each_gate not in self.braket_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None))
+            if each_gate not in self.pyquil_excluded_gates:
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None)
+                )
                 self.assertEqual(
-                    getattr(
-                        self.available_braket_gates[returned_gate.__name__], 
-                        returned_gate.__name__), 
-                    returned_gate
-                )
-        
-        oq_gate_list_1qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()])
-        
+                    self.available_pyquil_gates[returned_gate.__name__.lower()],
+                    returned_gate,
+                )
+
+        oq_gate_list_1qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_1qr:
-            if each_gate not in self.braket_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, rotation_object=None))
+            if each_gate not in self.pyquil_excluded_gates:
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, rotation_object=None)
+                )
                 self.assertEqual(
-                    getattr(
-                        self.available_braket_gates[returned_gate.__name__], 
-                        returned_gate.__name__), 
-                    returned_gate
-                )
-        
-        oq_gate_list_2q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()])
-        
+                    self.available_pyquil_gates[returned_gate.__name__.lower()],
+                    returned_gate,
+                )
+
+        oq_gate_list_2q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_2q:
-            if each_gate not in self.braket_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None))
+            if each_gate not in self.pyquil_excluded_gates:
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, qubit_2=None)
+                )
                 self.assertEqual(
-                    getattr(
-                        self.available_braket_gates[returned_gate.__name__], 
-                        returned_gate.__name__), 
-                    returned_gate
-                )
-        
-        oq_gate_list_2qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+                    self.available_pyquil_gates[returned_gate.__name__.lower()],
+                    returned_gate,
+                )
+
+        oq_gate_list_2qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_2qr:
-            if each_gate not in self.braket_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None, rotation_object=None))
+            if each_gate not in self.pyquil_excluded_gates:
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(
+                        applicator=None,
+                        qubit_1=None,
+                        qubit_2=None,
+                        rotation_object=None,
+                    )
+                )
                 self.assertEqual(
-                    getattr(
-                        self.available_braket_gates[returned_gate.__name__], 
-                        returned_gate.__name__), 
-                    returned_gate
+                    self.available_pyquil_gates[returned_gate.__name__.lower()],
+                    returned_gate,
                 )
-                
-    def test_not_supported_gates(self):
 
+    def test_not_supported_gates(self):
         """
-        If an unsupported Gate object is passed into the apply_gate method, 
+        If an unsupported Gate object is passed into the apply_gate method,
         a KeyError should be raised.
         The unsupported Gate object does not exist on the mapper.
         """
-        
-        unsupported_list = [oq_gate_mod.RXY, oq_gate_mod.RZX, oq_gate_mod.RYZ]
+
+        unsupported_list = [
+            oq_gate_mod.RXX,
+            oq_gate_mod.RYY,
+            oq_gate_mod.RZZ,
+            oq_gate_mod.RXY,
+            oq_gate_mod.RZX,
+            oq_gate_mod.RYZ,
+        ]
         qubit_1 = 0
         qubit_2 = 1
         rotation_object = None
-        circuit = Circuit()
-        
-        gate_applicator = BraketGateApplicator()
-        
+        circuit = Program()
+
+        gate_applicator = PyquilGateApplicator()
+
         for each_gate in unsupported_list:
             with self.assertRaises(KeyError):
-                gate_applicator.apply_gate(each_gate, qubit_1, qubit_2, 
-                                           rotation_object, circuit)
-                
+                gate_applicator.apply_gate(
+                    each_gate, qubit_1, qubit_2, rotation_object, circuit
+                )
+
     def test_wrong_argument(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
         incorrect set of arguments, a TypeError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 1
-                       }, 
-                       tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       },
-                       tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()):
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       }
-                      }
-        circuit = Circuit()
-        gate_applicator = BraketGateApplicator()
-        
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 1,
+            },
+            tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+            tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+        }
+        circuit = Program()
+        gate_applicator = PyquilGateApplicator()
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
-                if each_gate not in self.braket_excluded_gates:
+                each_gate.n_qubits = input_arguments["n_qubits"]
+                if each_gate not in self.pyquil_excluded_gates:
                     with self.assertRaises(TypeError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['wrong_args'], circuit)
-                        
+                        gate_applicator.apply_gate(
+                            each_gate, *input_arguments["wrong_args"], circuit
+                        )
+
     def test_wrong_n_qubits(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
-        n_qubits attribute that is not 1 or 2, a ValueError should be raised. 
+        n_qubits attribute that is not 1 or 2, a ValueError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'args': [0, None], 
-                        'n_qubits': 3
-                       }
-                      }
-        circuit = Circuit()
-        gate_applicator = BraketGateApplicator()
-        
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "args": [0, None],
+                "n_qubits": 3,
+            }
+        }
+        circuit = Program()
+        gate_applicator = PyquilGateApplicator()
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
-                if each_gate not in self.braket_excluded_gates:
+                each_gate.n_qubits = input_arguments["n_qubits"]
+                if each_gate not in self.pyquil_excluded_gates:
                     with self.assertRaises(ValueError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['args'], circuit)
+                        gate_applicator.apply_gate(
+                            each_gate, *input_arguments["args"], circuit
+                        )
                     break
-                    
+
     def test_static_methods_1q(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate to the circuit object.
         This method is check directly as there are currently no OQ Gate objects
         that call this method through apply_gate.
         """
-        
-        gate_applicator = BraketGateApplicator()
-        circuit = Circuit()
-        output_circuit = gate_applicator.apply_1q_fixed_gate(brk_gate.X.x, 0, circuit)
-
-        self.assertEqual([qubit for qubit in output_circuit.instructions[0].target], [0])
-        self.assertEqual(output_circuit.instructions[0].operator.name.lower(), 'x')
-                    
+
+        gate_applicator = PyquilGateApplicator()
+        circuit = Program()
+        output_circuit = gate_applicator.apply_1q_fixed_gate(gates.X, 0, circuit)
+
+        self.assertEqual(
+            [
+                each_instruction.get_qubits()
+                for each_instruction in circuit.instructions
+            ],
+            [{0}],
+        )
+        self.assertEqual(
+            [
+                each_instruction.name.lower()
+                for each_instruction in circuit.instructions
+            ],
+            ["x"],
+        )
+
     def test_static_methods_1qr(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate to the circuit object.
         """
 
-        gate_applicator = BraketGateApplicator()
+        gate_applicator = PyquilGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
-            circuit = Circuit()
-            
-            output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, rot_obj), 0, rot_obj, circuit)
-
-            self.assertEqual(output_circuit.instructions[0].operator.angle, input_angle)
-            self.assertEqual([qubit for qubit in output_circuit.instructions[0].target], [0])
-            self.assertEqual(output_circuit.instructions[0].operator.name.lower(), gate_applicator.BRAKET_OQ_GATE_MAPPER[each_gate.__name__].__name__)
-        
+            circuit = Program()
+            output_circuit = gate_applicator.apply_gate(
+                each_gate(gate_applicator, 0, rot_obj), 0, rot_obj, circuit
+            )
+
+            self.assertEqual(
+                [each_instruction.params for each_instruction in circuit.instructions],
+                [[input_angle]],
+            )
+            self.assertEqual(
+                [
+                    each_instruction.get_qubits()
+                    for each_instruction in circuit.instructions
+                ],
+                [{0}],
+            )
+            self.assertEqual(
+                [
+                    each_instruction.name.lower()
+                    for each_instruction in circuit.instructions
+                ],
+                [
+                    gate_applicator.PYQUIL_OQ_GATE_MAPPER[
+                        each_gate.__name__
+                    ].__name__.lower()
+                ],
+            )
+
     def test_static_methods_2q(self):
-        
         """
-        Checks that the static method, apply_2q_fixed_gate, apply the correct 
+        Checks that the static method, apply_2q_fixed_gate, apply the correct
         gate to the circuit object.
         """
-        
-        gate_applicator = BraketGateApplicator()
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
-        
+
+        gate_applicator = PyquilGateApplicator()
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
-            if each_gate not in self.braket_excluded_gates:
-                circuit = Circuit()
-                output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1), 0, 1, circuit)
-
-                self.assertEqual([qubit for qubit in output_circuit.instructions[0].target], [0, 1])
-                self.assertEqual(output_circuit.instructions[0].operator.name.lower(), gate_applicator.BRAKET_OQ_GATE_MAPPER[each_gate.__name__].__name__)
-                
+            if each_gate not in self.pyquil_excluded_gates:
+                circuit = Program()
+                output_circuit = gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1), 0, 1, circuit
+                )
+
+                self.assertEqual(
+                    [
+                        each_instruction.get_qubits()
+                        for each_instruction in circuit.instructions
+                    ],
+                    [{0, 1}],
+                )
+                self.assertEqual(
+                    [
+                        each_instruction.name.lower()
+                        for each_instruction in circuit.instructions
+                    ],
+                    [
+                        gate_applicator.PYQUIL_OQ_GATE_MAPPER[
+                            each_gate.__name__
+                        ].__name__.lower()
+                    ],
+                )
+
     def test_static_methods_2qr(self):
-        
         """
-        Checks that the static method, apply_2q_rotation_gate, apply the correct 
+        Checks that the static method, apply_2q_rotation_gate, apply the correct
         gate to the circuit object.
         """
-        
-        gate_applicator = BraketGateApplicator()
+
+        gate_applicator = PyquilGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
-            if each_gate not in self.braket_excluded_gates:
-                circuit = Circuit()
-                output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1, rot_obj), 0, 1, rot_obj, circuit)
-                
-                self.assertEqual(output_circuit.instructions[0].operator.angle, input_angle)
-                self.assertEqual([qubit for qubit in output_circuit.instructions[0].target], [0, 1])
-                self.assertEqual(output_circuit.instructions[0].operator.name.lower(), gate_applicator.BRAKET_OQ_GATE_MAPPER[each_gate.__name__].__name__)
-        
+            if each_gate not in self.pyquil_excluded_gates:
+                circuit = Program()
+                output_circuit = gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1, rot_obj), 0, 1, rot_obj, circuit
+                )
+
+                self.assertEqual(
+                    [
+                        each_instruction.params
+                        for each_instruction in circuit.instructions
+                    ],
+                    [[input_angle]],
+                )
+                self.assertEqual(
+                    [
+                        each_instruction.get_qubits()
+                        for each_instruction in circuit.instructions
+                    ],
+                    [{0, 1}],
+                )
+                self.assertEqual(
+                    [
+                        each_instruction.name.lower()
+                        for each_instruction in circuit.instructions
+                    ],
+                    [
+                        gate_applicator.PYQUIL_OQ_GATE_MAPPER[
+                            each_gate.__name__
+                        ].__name__.lower()
+                    ],
+                )
+
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_gate_applicators_qiskit.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_gate_applicators_qiskit.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,244 +6,397 @@
 from qiskit import QuantumCircuit
 
 import openqaoa
 import openqaoa.qaoa_components.ansatz_constructor.gates as oq_gate_mod
 from openqaoa_qiskit.backends.gates_qiskit import QiskitGateApplicator
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 
+
 class TestQiskitGateApplicator(unittest.TestCase):
-    
     def setUp(self):
-        
-        available_gates = [each_subclass_gate for each_subclass_gate in qsk_gate.Gate.__subclasses__()]
-        available_gates.extend([each_subclass_gate for each_subclass_gate in qsk_c_gate.ControlledGate.__subclasses__()])
-        
-        available_qiskit_gates_name = [each_gate.__name__.lower() for each_gate in available_gates]
-        self.available_qiskit_gates = dict(zip(available_qiskit_gates_name, 
-                                               available_gates))
-        
-        self.oq_available_gates = tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+        available_gates = [
+            each_subclass_gate for each_subclass_gate in qsk_gate.Gate.__subclasses__()
+        ]
+        available_gates.extend(
+            [
+                each_subclass_gate
+                for each_subclass_gate in qsk_c_gate.ControlledGate.__subclasses__()
+            ]
+        )
+
+        available_qiskit_gates_name = [
+            each_gate.__name__.lower() for each_gate in available_gates
+        ]
+        self.available_qiskit_gates = dict(
+            zip(available_qiskit_gates_name, available_gates)
+        )
+
+        self.oq_available_gates = (
+            tuple(
+                [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+                ]
+            )
+            + tuple(
+                [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+                ]
+            )
+        )
+
         # OneQubitGate, OneQubitRotationGate, TwoQubitGate, TwoQubitRotationGate are not acceptable inputs into the function even though they are of the Gate class
         # RXY, RiSWAP and RYZ are not supported by Qiskit library
-        self.qiskit_excluded_gates = [oq_gate_mod.OneQubitGate, oq_gate_mod.OneQubitRotationGate, 
-                          oq_gate_mod.TwoQubitGate, oq_gate_mod.TwoQubitRotationGate, 
-                          oq_gate_mod.RXY, oq_gate_mod.RiSWAP, oq_gate_mod.RYZ]
-    
+        self.qiskit_excluded_gates = [
+            oq_gate_mod.OneQubitGate,
+            oq_gate_mod.OneQubitRotationGate,
+            oq_gate_mod.TwoQubitGate,
+            oq_gate_mod.TwoQubitRotationGate,
+            oq_gate_mod.RXY,
+            oq_gate_mod.RiSWAP,
+            oq_gate_mod.RYZ,
+        ]
+
     def test_gate_applicator_mapper(self):
-        
         """
         The mapper to the gate applicator should only contain gates that
         are trivially support by the library.
         """
 
         for each_gate in QiskitGateApplicator.QISKIT_OQ_GATE_MAPPER.values():
+            self.assertTrue(
+                each_gate.__name__.lower() in self.available_qiskit_gates.keys(),
+                "{}, {}".format(each_gate.__name__, self.available_qiskit_gates.keys()),
+            )
 
-            self.assertTrue(each_gate.__name__.lower() in self.available_qiskit_gates.keys(), '{}, {}'.format(each_gate.__name__, self.available_qiskit_gates.keys()))
-            
     def test_gate_selector(self):
-        
         """
-        This method should return the Qiskit Gate object based on the input OQ 
+        This method should return the Qiskit Gate object based on the input OQ
         Gate object.
         """
-        
+
         gate_applicator = QiskitGateApplicator()
-        
-        oq_gate_list = tuple([each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()])
-        
-        oq_gate_list_1q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()])
-        
+
+        oq_gate_list = tuple(
+            [each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()]
+        )
+
+        oq_gate_list_1q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_1q:
             if each_gate not in self.qiskit_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None))
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None)
+                )
                 self.assertEqual(
                     self.available_qiskit_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-        
-        oq_gate_list_1qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()])
-        
+
+        oq_gate_list_1qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_1qr:
             if each_gate not in self.qiskit_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, rotation_object=None))
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, rotation_object=None)
+                )
                 self.assertEqual(
                     self.available_qiskit_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-        
-        oq_gate_list_2q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()])
-        
+
+        oq_gate_list_2q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_2q:
             if each_gate not in self.qiskit_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None))
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, qubit_2=None)
+                )
                 self.assertEqual(
                     self.available_qiskit_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-        
-        oq_gate_list_2qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+
+        oq_gate_list_2qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_2qr:
             if each_gate not in self.qiskit_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None, rotation_object=None))
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(
+                        applicator=None,
+                        qubit_1=None,
+                        qubit_2=None,
+                        rotation_object=None,
+                    )
+                )
                 self.assertEqual(
                     self.available_qiskit_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-                
-    def test_not_supported_gates(self):
 
+    def test_not_supported_gates(self):
         """
-        If an unsupported Gate object is passed into the apply_gate method, 
+        If an unsupported Gate object is passed into the apply_gate method,
         a KeyError should be raised.
         The unsupported Gate object does not exist on the mapper.
         """
-        
+
         unsupported_list = [oq_gate_mod.RXY, oq_gate_mod.RiSWAP, oq_gate_mod.RYZ]
         qubit_1 = 0
         qubit_2 = 1
         rotation_object = None
         circuit = QuantumCircuit(2)
-        
+
         gate_applicator = QiskitGateApplicator()
-        
+
         for each_gate in unsupported_list:
             with self.assertRaises(KeyError):
-                gate_applicator.apply_gate(each_gate, qubit_1, qubit_2, 
-                                           rotation_object, circuit)
-                
+                gate_applicator.apply_gate(
+                    each_gate, qubit_1, qubit_2, rotation_object, circuit
+                )
+
     def test_wrong_argument(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
         incorrect set of arguments, a TypeError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 1
-                       }, 
-                       tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       },
-                       tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()):
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       }
-                      }
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 1,
+            },
+            tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+            tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+        }
         circuit = QuantumCircuit(2)
         gate_applicator = QiskitGateApplicator()
-        
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
+                each_gate.n_qubits = input_arguments["n_qubits"]
                 if each_gate not in self.qiskit_excluded_gates:
                     with self.assertRaises(TypeError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['wrong_args'], circuit)
-                        
+                        gate_applicator.apply_gate(
+                            each_gate, *input_arguments["wrong_args"], circuit
+                        )
+
     def test_wrong_n_qubits(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
-        n_qubits attribute that is not 1 or 2, a ValueError should be raised. 
+        n_qubits attribute that is not 1 or 2, a ValueError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'args': [0, None], 
-                        'n_qubits': 3
-                       }
-                      }
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "args": [0, None],
+                "n_qubits": 3,
+            }
+        }
         circuit = QuantumCircuit(2)
         gate_applicator = QiskitGateApplicator()
-        
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
+                each_gate.n_qubits = input_arguments["n_qubits"]
                 if each_gate not in self.qiskit_excluded_gates:
                     with self.assertRaises(ValueError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['args'], circuit)
+                        gate_applicator.apply_gate(
+                            each_gate, *input_arguments["args"], circuit
+                        )
                     break
-                    
+
     def test_static_methods_1q(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate to the circuit object.
         This method is check directly as there are currently no OQ Gate objects
         that call this method through apply_gate.
         """
-        
+
         gate_applicator = QiskitGateApplicator()
         circuit = QuantumCircuit(1)
-        output_circuit = gate_applicator.apply_1q_fixed_gate(qsk_s_gate.XGate, 0, circuit)
+        output_circuit = gate_applicator.apply_1q_fixed_gate(
+            qsk_s_gate.XGate, 0, circuit
+        )
+
+        self.assertEqual(
+            [
+                each_qubit_ci.index
+                for circuit_instruction in output_circuit.data
+                for each_qubit_ci in circuit_instruction.qubits
+            ],
+            [0],
+        )
+        self.assertEqual(
+            [
+                circuit_instruction.operation.name
+                for circuit_instruction in output_circuit.data
+            ],
+            ["x"],
+        )
 
-        self.assertEqual([each_qubit_ci.index for circuit_instruction in output_circuit.data for each_qubit_ci in circuit_instruction.qubits], [0])
-        self.assertEqual([circuit_instruction.operation.name for circuit_instruction in output_circuit.data], ['x'])
-                    
     def test_static_methods_1qr(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate to the circuit object.
         """
 
         gate_applicator = QiskitGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             circuit = QuantumCircuit(1)
-            
-            output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, rot_obj), 0, rot_obj, circuit)
 
-            self.assertEqual([circuit_instruction.operation.params for circuit_instruction in output_circuit.data], [[input_angle]])
-            self.assertEqual([each_qubit_ci.index for circuit_instruction in output_circuit.data for each_qubit_ci in circuit_instruction.qubits], [0])
-            self.assertEqual([circuit_instruction.operation.name for circuit_instruction in output_circuit.data], [gate_applicator.QISKIT_OQ_GATE_MAPPER[each_gate.__name__].__name__.lower()[:-4]])
-        
+            output_circuit = gate_applicator.apply_gate(
+                each_gate(gate_applicator, 0, rot_obj), 0, rot_obj, circuit
+            )
+
+            self.assertEqual(
+                [
+                    circuit_instruction.operation.params
+                    for circuit_instruction in output_circuit.data
+                ],
+                [[input_angle]],
+            )
+            self.assertEqual(
+                [
+                    each_qubit_ci.index
+                    for circuit_instruction in output_circuit.data
+                    for each_qubit_ci in circuit_instruction.qubits
+                ],
+                [0],
+            )
+            self.assertEqual(
+                [
+                    circuit_instruction.operation.name
+                    for circuit_instruction in output_circuit.data
+                ],
+                [
+                    gate_applicator.QISKIT_OQ_GATE_MAPPER[
+                        each_gate.__name__
+                    ].__name__.lower()[:-4]
+                ],
+            )
+
     def test_static_methods_2q(self):
-        
         """
-        Checks that the static method, apply_2q_fixed_gate, apply the correct 
+        Checks that the static method, apply_2q_fixed_gate, apply the correct
         gate to the circuit object.
         """
-        
+
         gate_applicator = QiskitGateApplicator()
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             if each_gate not in self.qiskit_excluded_gates:
                 circuit = QuantumCircuit(2)
-                output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1), 0, 1, circuit)
+                output_circuit = gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1), 0, 1, circuit
+                )
+
+                self.assertEqual(
+                    [
+                        each_qubit_ci.index
+                        for circuit_instruction in output_circuit.data
+                        for each_qubit_ci in circuit_instruction.qubits
+                    ],
+                    [0, 1],
+                )
+                self.assertEqual(
+                    [
+                        circuit_instruction.operation.name
+                        for circuit_instruction in output_circuit.data
+                    ],
+                    [
+                        gate_applicator.QISKIT_OQ_GATE_MAPPER[
+                            each_gate.__name__
+                        ].__name__.lower()[:-4]
+                    ],
+                )
 
-                self.assertEqual([each_qubit_ci.index for circuit_instruction in output_circuit.data for each_qubit_ci in circuit_instruction.qubits], [0, 1])
-                self.assertEqual([circuit_instruction.operation.name for circuit_instruction in output_circuit.data], [gate_applicator.QISKIT_OQ_GATE_MAPPER[each_gate.__name__].__name__.lower()[:-4]])
-                
     def test_static_methods_2qr(self):
-        
         """
-        Checks that the static method, apply_2q_rotation_gate, apply the correct 
+        Checks that the static method, apply_2q_rotation_gate, apply the correct
         gate to the circuit object.
         """
-        
+
         gate_applicator = QiskitGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             if each_gate not in self.qiskit_excluded_gates:
                 circuit = QuantumCircuit(2)
-                output_circuit = gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1, rot_obj), 0, 1, rot_obj, circuit)
-                
-                self.assertEqual([circuit_instruction.operation.params for circuit_instruction in output_circuit.data], [[input_angle]])
-                self.assertEqual([each_qubit_ci.index for circuit_instruction in output_circuit.data for each_qubit_ci in circuit_instruction.qubits], [0, 1])
-                self.assertEqual([circuit_instruction.operation.name for circuit_instruction in output_circuit.data], [gate_applicator.QISKIT_OQ_GATE_MAPPER[each_gate.__name__].__name__.lower()[:-4]])
-        
+                output_circuit = gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1, rot_obj), 0, 1, rot_obj, circuit
+                )
+
+                self.assertEqual(
+                    [
+                        circuit_instruction.operation.params
+                        for circuit_instruction in output_circuit.data
+                    ],
+                    [[input_angle]],
+                )
+                self.assertEqual(
+                    [
+                        each_qubit_ci.index
+                        for circuit_instruction in output_circuit.data
+                        for each_qubit_ci in circuit_instruction.qubits
+                    ],
+                    [0, 1],
+                )
+                self.assertEqual(
+                    [
+                        circuit_instruction.operation.name
+                        for circuit_instruction in output_circuit.data
+                    ],
+                    [
+                        gate_applicator.QISKIT_OQ_GATE_MAPPER[
+                            each_gate.__name__
+                        ].__name__.lower()[:-4]
+                    ],
+                )
+
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_gate_applicators_vectorized.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_gate_applicators_vectorized.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,246 +3,358 @@
 
 import openqaoa
 from openqaoa.backends.qaoa_vectorized import QAOAvectorizedBackendSimulator
 import openqaoa.qaoa_components.ansatz_constructor.gates as oq_gate_mod
 from openqaoa.backends.gates_vectorized import VectorizedGateApplicator
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 
+
 class TestVectorizedGateApplicator(unittest.TestCase):
-    
     def setUp(self):
-        
-        available_vectorized_gates_name = [each_name for each_name in dir(QAOAvectorizedBackendSimulator) if 'apply' in each_name]
-        available_gates = [getattr(QAOAvectorizedBackendSimulator, each_name) for each_name in available_vectorized_gates_name]
-        
-        self.available_vectorized_gates = dict(zip(available_vectorized_gates_name, 
-                                                   available_gates))
-        
-        self.oq_available_gates = tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]) + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+        available_vectorized_gates_name = [
+            each_name
+            for each_name in dir(QAOAvectorizedBackendSimulator)
+            if "apply" in each_name
+        ]
+        available_gates = [
+            getattr(QAOAvectorizedBackendSimulator, each_name)
+            for each_name in available_vectorized_gates_name
+        ]
+
+        self.available_vectorized_gates = dict(
+            zip(available_vectorized_gates_name, available_gates)
+        )
+
+        self.oq_available_gates = (
+            tuple(
+                [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+                ]
+            )
+            + tuple(
+                [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+            )
+            + tuple(
+                [
+                    each_gate
+                    for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+                ]
+            )
+        )
+
         # OneQubitGate, OneQubitRotationGate, TwoQubitGate, TwoQubitRotationGate are not acceptable inputs into the function even though they are of the Gate class
         # CZ, CX, RXY and CPhase are not supported by Vectorized library
-        self.vectorized_excluded_gates = [oq_gate_mod.OneQubitGate, 
-                                          oq_gate_mod.OneQubitRotationGate, 
-                                          oq_gate_mod.TwoQubitGate, oq_gate_mod.TwoQubitRotationGate, 
-                                          oq_gate_mod.CZ, oq_gate_mod.CX, 
-                                          oq_gate_mod.RXY, oq_gate_mod.CPHASE]
-    
+        self.vectorized_excluded_gates = [
+            oq_gate_mod.OneQubitGate,
+            oq_gate_mod.OneQubitRotationGate,
+            oq_gate_mod.TwoQubitGate,
+            oq_gate_mod.TwoQubitRotationGate,
+            oq_gate_mod.X,
+            oq_gate_mod.CZ,
+            oq_gate_mod.CX,
+            oq_gate_mod.RXY,
+            oq_gate_mod.CPHASE,
+        ]
+
     def test_gate_applicator_mapper(self):
-        
         """
         The mapper to the gate applicator should only contain gates that
         are trivially support by the library.
         """
 
-        for each_gate in VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(QAOAvectorizedBackendSimulator).values():
+        for each_gate in VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(
+            QAOAvectorizedBackendSimulator
+        ).values():
+            self.assertTrue(
+                each_gate.__name__.lower() in self.available_vectorized_gates.keys(),
+                "{}, {}".format(
+                    each_gate.__name__, self.available_vectorized_gates.keys()
+                ),
+            )
 
-            self.assertTrue(each_gate.__name__.lower() in self.available_vectorized_gates.keys(), '{}, {}'.format(each_gate.__name__, self.available_vectorized_gates.keys()))
-            
     def test_gate_selector(self):
-        
         """
-        This method should apply the Vectorized Gate Function based on the input OQ 
+        This method should apply the Vectorized Gate Function based on the input OQ
         Gate object.
         """
-        
+
         gate_applicator = VectorizedGateApplicator()
-        
-        oq_gate_list = tuple([each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()])
-        
+
+        oq_gate_list = tuple(
+            [each_gate for each_gate in oq_gate_mod.Gate.__subclasses__()]
+        )
+
         # Vectorized Gate Function for 1 Qubit Gates without Rotation Angle
-        oq_gate_list_1q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()])
-        
+        oq_gate_list_1q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.OneQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_1q:
             if each_gate not in self.vectorized_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, vectorized_backend=None), QAOAvectorizedBackendSimulator)
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, vectorized_backend=None),
+                    QAOAvectorizedBackendSimulator,
+                )
                 self.assertEqual(
-                    self.available_vectorized_gates[returned_gate._extract_mock_name.lower()],
-                    returned_gate
+                    self.available_vectorized_gates[
+                        returned_gate._extract_mock_name.lower()
+                    ],
+                    returned_gate,
                 )
-        
+
         # Vectorized Gate Function for 1 Qubit Gates with Rotation Angle
-        oq_gate_list_1qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()])
-        
+        oq_gate_list_1qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_1qr:
             if each_gate not in self.vectorized_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, rotation_object=None), QAOAvectorizedBackendSimulator)
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, rotation_object=None),
+                    QAOAvectorizedBackendSimulator,
+                )
                 self.assertEqual(
                     self.available_vectorized_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-        
+
         # Vectorized Gate Function for 2 Qubit Gate without Rotation Angle
-        oq_gate_list_2q = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()])
-        
+        oq_gate_list_2q = oq_gate_list + tuple(
+            [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
+        )
+
         for each_gate in oq_gate_list_2q:
             if each_gate not in self.vectorized_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None), QAOAvectorizedBackendSimulator)
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(applicator=None, qubit_1=None, qubit_2=None),
+                    QAOAvectorizedBackendSimulator,
+                )
                 self.assertEqual(
                     self.available_vectorized_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-        
+
         # Vectorized Gate Function for 2 Qubit Gate with Rotation Angle
-        oq_gate_list_2qr = oq_gate_list + tuple([each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()])
-        
+        oq_gate_list_2qr = oq_gate_list + tuple(
+            [
+                each_gate
+                for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+            ]
+        )
+
         for each_gate in oq_gate_list_2qr:
             if each_gate not in self.vectorized_excluded_gates:
-                returned_gate = gate_applicator.gate_selector(each_gate(applicator=None, qubit_1=None, qubit_2=None, rotation_object=None), QAOAvectorizedBackendSimulator)
+                returned_gate = gate_applicator.gate_selector(
+                    each_gate(
+                        applicator=None,
+                        qubit_1=None,
+                        qubit_2=None,
+                        rotation_object=None,
+                    ),
+                    QAOAvectorizedBackendSimulator,
+                )
                 self.assertEqual(
                     self.available_vectorized_gates[returned_gate.__name__.lower()],
-                    returned_gate
+                    returned_gate,
                 )
-                
-    def test_not_supported_gates(self):
 
+    def test_not_supported_gates(self):
         """
-        If an unsupported Gate object is passed into the apply_gate method, 
+        If an unsupported Gate object is passed into the apply_gate method,
         a KeyError should be raised.
         The unsupported Gate object does not exist on the mapper.
         """
-        
-        unsupported_list = [oq_gate_mod.CZ, oq_gate_mod.CX, oq_gate_mod.RXY, 
-                            oq_gate_mod.CPHASE]
+
+        unsupported_list = [
+            oq_gate_mod.CZ,
+            oq_gate_mod.CX,
+            oq_gate_mod.RXY,
+            oq_gate_mod.CPHASE,
+        ]
         qubit_1 = 0
         qubit_2 = 1
         rotation_object = None
-        
+
         gate_applicator = VectorizedGateApplicator()
-        
+
         for each_gate in unsupported_list:
             with self.assertRaises(KeyError):
-                gate_applicator.apply_gate(each_gate, qubit_1, qubit_2, 
-                                           rotation_object, QAOAvectorizedBackendSimulator)
-                
+                gate_applicator.apply_gate(
+                    each_gate,
+                    qubit_1,
+                    qubit_2,
+                    rotation_object,
+                    QAOAvectorizedBackendSimulator,
+                )
+
     def test_wrong_argument(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
         incorrect set of arguments, a TypeError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 1
-                       }, 
-                       tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): 
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       },
-                       tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()):
-                       {'wrong_args': [0, 1, None], 
-                        'n_qubits': 2
-                       }
-                      }
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 1,
+            },
+            tuple(oq_gate_mod.TwoQubitGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+            tuple(oq_gate_mod.TwoQubitRotationGate.__subclasses__()): {
+                "wrong_args": [0, 1, None],
+                "n_qubits": 2,
+            },
+        }
         gate_applicator = VectorizedGateApplicator()
-        
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
+                each_gate.n_qubits = input_arguments["n_qubits"]
                 if each_gate not in self.vectorized_excluded_gates:
                     with self.assertRaises(TypeError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['wrong_args'], QAOAvectorizedBackendSimulator)
-                        
+                        gate_applicator.apply_gate(
+                            each_gate,
+                            *input_arguments["wrong_args"],
+                            QAOAvectorizedBackendSimulator
+                        )
+
     def test_wrong_n_qubits(self):
-        
         """
         If a supported Gate object is passed into the apply_gate method with the
-        n_qubits attribute that is not 1 or 2, a ValueError should be raised. 
+        n_qubits attribute that is not 1 or 2, a ValueError should be raised.
         """
-        
-        input_gates = {tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): 
-                       {'args': [0, None], 
-                        'n_qubits': 3
-                       }
-                      }
+
+        input_gates = {
+            tuple(oq_gate_mod.OneQubitRotationGate.__subclasses__()): {
+                "args": [0, None],
+                "n_qubits": 3,
+            }
+        }
         gate_applicator = VectorizedGateApplicator()
-        
+
         for each_gate_set, input_arguments in input_gates.items():
             for each_gate in each_gate_set:
-                each_gate.n_qubits = input_arguments['n_qubits']
+                each_gate.n_qubits = input_arguments["n_qubits"]
                 if each_gate not in self.vectorized_excluded_gates:
                     with self.assertRaises(ValueError):
-                        gate_applicator.apply_gate(each_gate, *input_arguments['args'], QAOAvectorizedBackendSimulator)
+                        gate_applicator.apply_gate(
+                            each_gate,
+                            *input_arguments["args"],
+                            QAOAvectorizedBackendSimulator
+                        )
                     break
-                    
+
     def test_static_methods_1q(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate function.
         This method is check directly as there are currently no OQ Gate objects
         that call this method through apply_gate.
         """
-        
+
         gate_applicator = VectorizedGateApplicator()
         QAOAvectorizedBackendSimulator.apply_x = Mock()
         gate_applicator.apply_1q_fixed_gate(QAOAvectorizedBackendSimulator.apply_x, 0)
-        
+
         QAOAvectorizedBackendSimulator.apply_x.assert_called_with(0)
-                    
+
     def test_static_methods_1qr(self):
-        
         """
-        Checks that the static method, apply_1q_rotation_gate, apply the correct 
+        Checks that the static method, apply_1q_rotation_gate, apply the correct
         gate function.
         """
 
         gate_applicator = VectorizedGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.OneQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             mock_vectorized_backend = Mock()
-            gate_applicator.apply_gate(each_gate(gate_applicator, 0, rot_obj), 0, rot_obj, mock_vectorized_backend)
-            
-            method_name = (VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(mock_vectorized_backend)[each_gate.__name__]._extract_mock_name()[5:])
+            gate_applicator.apply_gate(
+                each_gate(gate_applicator, 0, rot_obj),
+                0,
+                rot_obj,
+                mock_vectorized_backend,
+            )
+
+            method_name = VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(
+                mock_vectorized_backend
+            )[each_gate.__name__]._extract_mock_name()[5:]
             # Check that the method is called with the right arguments
-            getattr(mock_vectorized_backend, method_name).assert_called_with(0, rot_obj.rotation_angle)
+            getattr(mock_vectorized_backend, method_name).assert_called_with(
+                0, rot_obj.rotation_angle
+            )
 
     def test_static_methods_2q(self):
-        
         """
-        Checks that the static method, apply_2q_fixed_gate, apply the correct 
+        Checks that the static method, apply_2q_fixed_gate, apply the correct
         gate function.
         """
-        
+
         gate_applicator = VectorizedGateApplicator()
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             if each_gate not in self.vectorized_excluded_gates:
                 mock_vectorized_backend = Mock()
-                gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1), 0, 1, mock_vectorized_backend)
-                
-                method_name = (VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(mock_vectorized_backend)[each_gate.__name__]._extract_mock_name()[5:])
+                gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1), 0, 1, mock_vectorized_backend
+                )
+
+                method_name = VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(
+                    mock_vectorized_backend
+                )[each_gate.__name__]._extract_mock_name()[5:]
                 # Check that the method is called with the right arguments
                 getattr(mock_vectorized_backend, method_name).assert_called_with(0, 1)
-                
+
     def test_static_methods_2qr(self):
-        
         """
-        Checks that the static method, apply_2q_rotation_gate, apply the correct 
+        Checks that the static method, apply_2q_rotation_gate, apply the correct
         gate function.
         """
-        
+
         gate_applicator = VectorizedGateApplicator()
         input_angle = 1
         rot_obj = RotationAngle(lambda x: x, None, input_angle)
-        
-        each_sub_gate = [each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()]
-        
+
+        each_sub_gate = [
+            each_gate for each_gate in oq_gate_mod.TwoQubitRotationGate.__subclasses__()
+        ]
+
         for each_gate in each_sub_gate:
             if each_gate not in self.vectorized_excluded_gates:
                 mock_vectorized_backend = Mock()
-                gate_applicator.apply_gate(each_gate(gate_applicator, 0, 1, rot_obj), 0, 1, rot_obj, mock_vectorized_backend)
-                
-                method_name = (VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(mock_vectorized_backend)[each_gate.__name__]._extract_mock_name()[5:])
+                gate_applicator.apply_gate(
+                    each_gate(gate_applicator, 0, 1, rot_obj),
+                    0,
+                    1,
+                    rot_obj,
+                    mock_vectorized_backend,
+                )
+
+                method_name = VectorizedGateApplicator.VECTORIZED_OQ_GATE_MAPPER(
+                    mock_vectorized_backend
+                )[each_gate.__name__]._extract_mock_name()[5:]
                 # Check that the method is called with the right arguments
-                getattr(mock_vectorized_backend, method_name).assert_called_with(0, 1, rot_obj.rotation_angle)
-        
+                getattr(mock_vectorized_backend, method_name).assert_called_with(
+                    0, 1, rot_obj.rotation_angle
+                )
+
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_imports.py` & `openqaoa-0.1.3rc1/tests/test_imports.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,33 @@
 import unittest
 import importlib
+import os
 
 from setuptools import find_namespace_packages
 
 
 class TestImports(unittest.TestCase):
 
     """
     Test module imports within OpenQAOA
     """
 
     def test_all_module_import(self):
         """
         Test all the main module imports for OQ
         """
-
-        package_names = [
-            "openqaoa",
-            "openqaoa_braket",
-            "openqaoa_qiskit",
-            "openqaoa_pyquil",
-            "openqaoa_azure",
-        ]
-        folder_names = [
-            "openqaoa-core",
-            "openqaoa-braket",
-            "openqaoa-qiskit",
-            "openqaoa-pyquil",
-            "openqaoa-azure",
-        ]
-        packages_import = find_namespace_packages(where="./src")
-        updated_packages = []
-        for each_package_name in packages_import:
-            for _index, each_folder_name in enumerate(folder_names):
-                if each_folder_name in each_package_name:
-                    updated_packages.append(
-                        each_package_name.replace(
-                            each_folder_name, package_names[_index]
-                        )
-                    )
-                    continue
-
-        for each_package in updated_packages:
+        
+        folder_names = [each_file for each_file in os.listdir('src') if 'openqaoa-' in each_file]
+        
+        packages_import = []
+        for each_file_name in folder_names:
+            packages_import.extend(find_namespace_packages(where="./src/"+each_file_name, exclude=['dist', 'build', 'build.*', 'tests', 'tests.*']))
+        print(packages_import)
+        packages_import = sorted(packages_import)
+        for each_package in packages_import:
             try:
                 importlib.import_module(each_package)
             except Exception as e:
                 raise Exception(e)
 
 
 if __name__ == "__main__":
```

### Comparing `openqaoa-0.1.3/tests/test_logger.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,44 +10,40 @@
     IfLowerDo,
     IfHigherDo,
 )
 
 
 class TestingLoggerClass(unittest.TestCase):
     def test_logger_var_setting_1(self):
-
         test_var = LoggerVariable("test_var", EmptyValue, EmptyValue)
 
         test_var.update(10)
 
         self.assertEqual(test_var.history, [])
         self.assertEqual(test_var.best, [])
 
     def test_logger_var_setting_2(self):
-
         test_var = LoggerVariable("test_var", AppendValue, AppendValue)
 
         test_var.update(5)
         test_var.update(10)
 
         self.assertEqual(test_var.history, [5, 10])
         self.assertEqual(test_var.best, [5, 10])
 
     def test_logger_var_setting_3(self):
-
         test_var = LoggerVariable("test_var", ReplaceValue, ReplaceValue)
 
         test_var.update(5)
         test_var.update(10)
 
         self.assertEqual(test_var.history, [10])
         self.assertEqual(test_var.best, [10])
 
     def test_logger_var_setting_4(self):
-
         test_var = LoggerVariable(
             "test_var", IfLowerDo(EmptyValue), IfLowerDo(EmptyValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(10)
 
@@ -56,15 +52,14 @@
 
         test_var.update(1)
 
         self.assertEqual(test_var.history, [])
         self.assertEqual(test_var.best, [])
 
     def test_logger_var_setting_5(self):
-
         test_var = LoggerVariable(
             "test_var", IfLowerDo(AppendValue), IfLowerDo(AppendValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(10)
 
@@ -73,15 +68,14 @@
 
         test_var.update(1)
 
         self.assertEqual(test_var.history, [5, 1])
         self.assertEqual(test_var.best, [5, 1])
 
     def test_logger_var_setting_6(self):
-
         test_var = LoggerVariable(
             "test_var", IfLowerDo(ReplaceValue), IfLowerDo(ReplaceValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(10)
 
@@ -90,15 +84,14 @@
 
         test_var.update(1)
 
         self.assertEqual(test_var.history, [1])
         self.assertEqual(test_var.best, [1])
 
     def test_logger_var_setting_7(self):
-
         test_var = LoggerVariable(
             "test_var", IfHigherDo(EmptyValue), IfHigherDo(EmptyValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(1)
 
@@ -107,15 +100,14 @@
 
         test_var.update(10)
 
         self.assertEqual(test_var.history, [])
         self.assertEqual(test_var.best, [])
 
     def test_logger_var_setting_8(self):
-
         test_var = LoggerVariable(
             "test_var", IfHigherDo(AppendValue), IfHigherDo(AppendValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(1)
 
@@ -124,15 +116,14 @@
 
         test_var.update(10)
 
         self.assertEqual(test_var.history, [5, 10])
         self.assertEqual(test_var.best, [5, 10])
 
     def test_logger_var_setting_9(self):
-
         test_var = LoggerVariable(
             "test_var", IfHigherDo(ReplaceValue), IfHigherDo(ReplaceValue)
         )
 
         test_var.update(5)  # First value gets appended regardless
         test_var.update(1)
 
@@ -141,28 +132,26 @@
 
         test_var.update(10)
 
         self.assertEqual(test_var.history, [10])
         self.assertEqual(test_var.best, [10])
 
     def test_logger_var_methods(self):
-
         test_var = LoggerVariable("test_var", ReplaceValue, ReplaceValue)
         test_var_2 = LoggerVariable("test_var", ReplaceValue, ReplaceValue)
 
         test_var.update(1)
 
         test_var_2.update_history(1)
         test_var_2.update_best(1)
 
         self.assertEqual(test_var.history, test_var_2.history)
         self.assertEqual(test_var.best, test_var_2.best)
 
     def test_logger_var_fact_hist_bool(self):
-
         var_1 = LoggerVariableFactory.create_logger_variable(
             "new_attribute", True, "Replace"
         )
         var_2 = LoggerVariableFactory.create_logger_variable(
             "new_attribute", False, "Replace"
         )
 
@@ -174,15 +163,14 @@
 
         self.assertEqual(var_1.name, "new_attribute")
         self.assertEqual(var_2.name, "new_attribute")
         self.assertEqual(var_1.history, [1, 2])
         self.assertEqual(var_2.history, [])
 
     def test_logger_var_fact_best_str(self):
-
         """
         Testing all possible settings of a variable created through the Factory
         Class
         """
 
         var_1 = LoggerVariableFactory.create_logger_variable(
             "new_attribute", True, "Append"
@@ -217,15 +205,14 @@
         self.assertEqual(var_2.best, [1])
         self.assertEqual(var_3.best, [5, 1])
         self.assertEqual(var_4.best, [1])
         self.assertEqual(var_5.best, [5, 7, 10])
         self.assertEqual(var_6.best, [10])
 
     def test_logger_obj_update_struct_1(self):
-
         """
         The best update structure ensures that the best value for that particular
         attribute respects a relation with another attribute.
 
         In the code below, the following can be observed:
         Even though the lowest in attribute 2 is 10. The best of attribute 2 is
         15 instead. This is because the best value of attribute 2 depends on whether
@@ -306,15 +293,14 @@
         self.assertEqual(logger_obj.attribute_3.history, [])
 
         self.assertEqual(logger_obj.attribute_1.best, [20])
         self.assertEqual(logger_obj.attribute_2.best, [3, 2])
         self.assertEqual(logger_obj.attribute_3.best, ["string 4"])
 
     def test_logger_obj_update_struct_2(self):
-
         """
         Single layer test
         """
 
         logger_obj = Logger(
             {
                 "attribute_1": {
@@ -381,15 +367,14 @@
         self.assertEqual(logger_obj.attribute_3.history, [])
 
         self.assertEqual(logger_obj.attribute_1.best, [20])
         self.assertEqual(logger_obj.attribute_2.best, [3, 1])
         self.assertEqual(logger_obj.attribute_3.best, ["string 4"])
 
     def test_logger_obj_update_struct_3(self):
-
         """
         Multi layer test
         """
 
         logger_obj = Logger(
             {
                 "attribute_1": {
```

### Comparing `openqaoa-0.1.3/tests/test_notebooks.py` & `openqaoa-0.1.3rc1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_operators.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             (0, 1, 5, 3, 7, 6),
             (6, 5, 4, 3, 2, 1, 0),
         ]
         input_exc_strings = ["XY", "XZZYZXYZ", "YXZZ", "XYZZX", "Z"]
 
         # Test the exceptions are raised
         for string, index in zip(input_exc_strings, input_exc_indices):
-
             # Attempt construction of Pauli operator
             with self.assertRaises(AssertionError) as context:
                 pauli = PauliOp(string, index)
 
             # Check exception message
             self.assertEqual(
                 f"Each Pauli operator must have a unique qubit index",
@@ -132,15 +131,14 @@
         input_exc_strings = ["LXY", "Q", "ZYXZR", "FYZZXX", "ZYXYZYN"]
 
         # Pauli set
         PAULIS_SET = set("XYZI")
 
         # Test the exceptions are raised
         for string, index in zip(input_exc_strings, input_exc_indices):
-
             # Extract exception from string
             non_pauli_operator = list(set(string) - PAULIS_SET)[0]
 
             # Attempt construction of Pauli operator
             with self.assertRaises(ValueError) as context:
                 pauli = PauliOp(string, index)
 
@@ -894,15 +892,14 @@
         """
 
         # Initialize lists containing correct and computed lengths
         correct_lengths = []
         lengths = []
 
         for n_qubits in range(3, 10):
-
             # Compute correct lengths
             correct_lengths.append(n_qubits + n_qubits * (n_qubits - 1) / 2)
 
             # Define Pauli terms
             singlet_indices = [(i,) for i in range(n_qubits)]
             pair_indices = [(i, j) for j in range(n_qubits) for i in range(j)]
             linear_terms = [PauliOp("Z", indices) for indices in singlet_indices]
@@ -1039,15 +1036,14 @@
         correct_hamiltonian_dict = {
             term.qubit_indices: coeff
             for term, coeff in zip(input_terms, input_coefficients)
         }
 
         # Add terms and coefficients from the other hamiltonian
         for term, coeff in zip(other_input_terms, other_input_coefficients):
-
             # If term was absent add it together with coefficient
             if correct_hamiltonian_dict.get(term.qubit_indices) is None:
                 correct_hamiltonian_dict.update({term.qubit_indices: coeff})
 
             # If term was present add coefficient to current term
             else:
                 correct_hamiltonian_dict[term.qubit_indices] += coeff
@@ -1220,15 +1216,14 @@
         constant_exc = 2
 
         # Define different types of coefficients containing exceptions
         coefficients_exc_types = [[-1j, 1, -1j], [2, 3, 0.1 * 1j]]
 
         # Check for every coefficient type
         for coefficients_exc in coefficients_exc_types:
-
             # Test the exception is raised - Attempt construction of Hamiltonian
             with self.assertRaises(ValueError) as context:
                 hamiltonian_exc = Hamiltonian.classical_hamiltonian(
                     terms_exc, coefficients_exc, constant_exc
                 )
 
         # Check exception message
```

### Comparing `openqaoa-0.1.3/tests/test_optimizers.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     [1, 1.1, 1.5, 2, -0.8],
     0.8,
 )
 
 
 class TestQAOACostBaseClass(unittest.TestCase):
     def setUp(self):
-
         self.log = Logger(
             {
                 "func_evals": {
                     "history_update_bool": False,
                     "best_update_string": "HighestOnly",
                 },
                 "jac_func_evals": {
@@ -144,15 +143,14 @@
         optimizer_dicts = []
         for method in MINIMIZE_METHODS:
             optimizer_dicts.append(
                 {"method": method, "maxiter": niter, "tol": 10 ** (-9)}
             )
 
         for i, optimizer_dict in enumerate(optimizer_dicts):
-
             optimizer_dict["jac"] = derivative(
                 backend_obj_vectorized,
                 variate_params,
                 self.log,
                 "gradient",
                 "finite_difference",
             )
@@ -229,15 +227,14 @@
                 "jac": "finite_difference",
                 "maxiter": niter,
                 "optimizer_options": {"stepsize": stepsize, "decay": 0.9, "eps": 1e-07},
             }
         )
 
         for i, optimizer_dict in enumerate(optimizer_dicts):
-
             # Optimize
             vector_optimizer = get_optimizer(
                 backend_obj_vectorized, variate_params, optimizer_dict=optimizer_dict
             )
             vector_optimizer()
 
             y_opt = vector_optimizer.qaoa_result.intermediate["cost"]
@@ -543,15 +540,14 @@
 
         y = [y0, y1, y2]
 
         for i, yi in enumerate(y):
             assert np.isclose(yi, y_opt[i], rtol=1e-05, atol=1e-05)
 
     def test_optimize_loop_crash(self):
-
         """
         This tests that the optimization loop doesnt crash silently.
         An Exception gets raised.
         """
 
         cost_hamil = Hamiltonian(
             [
@@ -586,22 +582,20 @@
         self.assertRaises(Exception, lambda: vector_optimizer.optimize())
 
         # Check that QAOA Result exists
         self.assertEqual(type(vector_optimizer.qaoa_result), QAOAResult)
 
     @classmethod
     def tearDownClass(cls):
-
         output_csv = ["oq_saved_info_job_ids.csv", "oq_saved_info_param_log.csv"]
         for each_csv in output_csv:
-            if os.path.exists(each_csv):
-                os.remove(each_csv)
-            else:
-                raise FileNotFoundError(
-                    "Unable to remove the generated csv file: {}".format(each_csv)
-                )
+            try:
+                if os.path.exists(each_csv):
+                    os.remove(each_csv)
+            except Exception:
+                continue
 
 
 if __name__ == "__main__":
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=PendingDeprecationWarning)
         unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_optimizers_pennylane.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_optimizers_pennylane.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 qubo_problem_1 = problem.qubo
 qubo_problem_2 = QUBO.random_instance(5)
 qubo_problem_3 = QUBO.random_instance(6)
 
 
 class TestPennylaneOptimizers(unittest.TestCase):
     def setUp(self):
-
         self.log = Logger(
             {
                 "func_evals": {
                     "history_update_bool": False,
                     "best_update_string": "HighestOnly",
                 },
                 "jac_func_evals": {
@@ -204,15 +203,14 @@
 
         def cost(params):
             variate_params.update_from_raw(params)
             return np.real(backend_obj_vectorized.expectation(variate_params))
 
         i = 0
         for method in list_optimizers:
-
             pennylane_method = method
 
             # copy the parameters
             x0 = copy.deepcopy(variate_params.raw().copy())
 
             # Optimize with the implemented optimizer in OpenQAOA
             vector_optimizer = get_optimizer(
```

### Comparing `openqaoa-0.1.3/tests/test_parameters.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     terms_wo_bias, weights_wo_bias, constant=0.7
 )
 mixer_hamiltonian = X_mixer_hamiltonian(len(register))
 
 
 class TestingQAOADescriptor(unittest.TestCase):
     def setUp(self):
-
         self.p = 2
         self.cost_hamil = Hamiltonian(
             [
                 PauliOp("ZZ", (0, 1)),
                 PauliOp("ZZ", (1, 2)),
                 PauliOp("ZZ", (0, 2)),
                 PauliOp("Z", (0,)),
@@ -42,15 +41,14 @@
             1,
         )
         self.mixer_hamil = X_mixer_hamiltonian(n_qubits=3)
         self.mixer_gatemap = [RXGateMap(0), RXGateMap(1), RXGateMap(2)]
         self.mixer_gatemap_coeffs = self.mixer_hamil.coeffs
 
     def test_QAOADescriptor(self):
-
         """
         QAOADescriptor accept 2 types of inputs for mixer_blocks argument on initilisation. This test checks that the same mixer block when presented in Hamiltonian or as a List of RotationGateMap, plus the appropriate mixer coefficients, produces similar internal attributes.
         """
 
         qaoa_descriptor = QAOADescriptor(self.cost_hamil, self.mixer_hamil, p=self.p)
 
         qaoa_descriptor_gm = QAOADescriptor(
@@ -80,15 +78,14 @@
             qaoa_descriptor_gm.mixer_qubits_singles,
         )
         self.assertEqual(
             qaoa_descriptor.mixer_qubits_pairs, qaoa_descriptor_gm.mixer_qubits_pairs
         )
 
     def test_QAOADescriptor_mixer_coeffs_selector_hamiltonian(self):
-
         """
         If a mixer hamiltonian is used for mixer_block, the coefficients will be obtained from it. Even if the user inputs his own mixer coefficient, it will be ignored.
         """
 
         verify_mixer_coeffs = [-1, -1, -1]
 
         mixer_hamil = X_mixer_hamiltonian(n_qubits=3)
@@ -98,15 +95,14 @@
             self.cost_hamil, self.mixer_hamil, p=self.p, mixer_coeffs=[1, 0, 1]
         )
 
         self.assertEqual(qaoa_descriptor.mixer_block_coeffs, verify_mixer_coeffs)
         self.assertEqual(qaoa_descriptor_2.mixer_block_coeffs, verify_mixer_coeffs)
 
     def test_QAOADescriptor_mixer_coeffs_selector_gatemap(self):
-
         """
         If a mixer gatemap is used for mixer_block, the user is required to input his own mixer coefficients, there should be an error message if the user does not input the appropriate number of mixer coefficients.
         """
 
         verify_mixer_coeffs = [-1, -1, -1]
 
         qaoa_descriptor = QAOADescriptor(
@@ -122,15 +118,14 @@
             QAOADescriptor(self.cost_hamil, self.mixer_gatemap, self.p, [])
             self.assertEqual(
                 "The number of terms/gatemaps must match the number of coefficients provided.",
                 str(cm.exception),
             )
 
     def test_QAOADescriptor_assign_coefficients(self):
-
         """
         The method should split the coefficients and gatemaps in the proper order. Regardless of their positions within the hamiltonian or gatemap list.
         """
 
         verify_mixer_coeffs = [-1, -1, -1, -0.5]
 
         # TestCase 1: GateMap Mixer
@@ -183,15 +178,14 @@
                 "RYYGateMap",
                 "RXXGateMap",
                 "RYYGateMap",
             ],
         )
 
     def test_QAOADescriptor_cost_blocks(self):
-
         """
         cost_blocks property should always return a list of RotationGateMaps based on the input cost hamiltonian.
         """
 
         mixer_gatemap = [RXGateMap(0), RXGateMap(1), RXGateMap(2), RXXGateMap(0, 2)]
 
         qaoa_descriptor = QAOADescriptor(
@@ -206,15 +200,14 @@
 
             self.assertEqual(
                 [each_item.gate_label.sequence for each_item in each_p_block],
                 [0, 1, 2, 0],
             )
 
     def test_QAOADescriptor_mixer_blocks(self):
-
         """
         mixer_blocks property should always return a list of RotationGateMaps based on the input cost hamiltonian.
         """
 
         mixer_gatemap = [RXGateMap(0), RXGateMap(1), RXGateMap(2), RXXGateMap(0, 2)]
 
         qaoa_descriptor = QAOADescriptor(
@@ -229,15 +222,14 @@
 
             self.assertEqual(
                 [each_item.gate_label.sequence for each_item in each_p_block],
                 [0, 1, 2, 0],
             )
 
     def test_QAOADescriptor_weird_cases(self):
-
         """
         Testing various weird cases
         """
 
         # TestCase 1: Empty List Mixer Block
         qaoa_descriptor = QAOADescriptor(self.cost_hamil, [], p=self.p)
 
@@ -249,15 +241,14 @@
 
         # TestCase 3: p is not an int
         self.assertRaises(
             TypeError, QAOADescriptor, self.cost_hamil, self.mixer_hamil, "test"
         )
 
     def test_QAOADescriptor_abstract_circuit(self):
-
         """
         The abstract circuit should be consistent with the cost hamiltonian, mixer block and the p value.
         """
 
         mixer_hamil = X_mixer_hamiltonian(n_qubits=3)
         mixer_gatemap = [RXGateMap(0), RXGateMap(1), RXGateMap(2)]
 
@@ -346,36 +337,33 @@
         assert np.allclose(params.mixer_1q_angles, mixer_1q_angles)
         assert np.allclose(params.mixer_2q_angles, mixer_2q_angles)
         assert np.allclose(params.cost_1q_angles, cost_1q_angles)
         assert np.allclose(params.cost_2q_angles, cost_2q_angles)
         assert type(params) == QAOAVariationalStandardWithBiasParams
 
     def test_QAOAVariationalAnnealingParamsCustomInitialisation(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         schedule = [0.4, 1.0]
         annealing_params = QAOAVariationalAnnealingParams(
             qaoa_descriptor, total_annealing_time=5, schedule=schedule
         )
 
         assert type(annealing_params) == QAOAVariationalAnnealingParams
 
     def test_QAOAVariationalFourierParamsCustomInitialisation(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         v = [0.4, 1.0]
         u = [0.5, 1.2]
         fourier_params = QAOAVariationalFourierParams(qaoa_descriptor, q=2, v=v, u=u)
 
         assert np.allclose(fourier_params.betas, dct(v, n=qaoa_descriptor.p, axis=0))
         assert np.allclose(fourier_params.gammas, dst(u, n=qaoa_descriptor.p, axis=0))
         assert type(fourier_params) == QAOAVariationalFourierParams
 
     def test_QAOAVariationalFourierExtendedParamsCustomInitialisation(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         v_singles = [[0.4] * 3, [1.0] * 3]
         v_pairs = []
         u_singles = [[0.5], [1.2]]
         u_pairs = [[4.5] * 2, [123] * 2]
         fourier_params = QAOAVariationalFourierExtendedParams(
             qaoa_descriptor, 2, v_singles, v_pairs, u_singles, u_pairs
@@ -390,15 +378,14 @@
         assert np.allclose(
             fourier_params.gammas_pairs, dst(u_pairs, n=qaoa_descriptor.p, axis=0)
         )
 
         assert type(fourier_params) == QAOAVariationalFourierExtendedParams
 
     def test_QAOAVariationalAnnealingParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         params = QAOAVariationalAnnealingParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, total_annealing_time=2
         )
 
         assert np.allclose(qaoa_descriptor.qureg, [0, 1, 2])
         assert np.allclose(params.mixer_1q_angles, [[-2 * 0.75] * 3, [-2 * 0.25] * 3])
@@ -409,15 +396,14 @@
 
         # Test updating and raw output
         raw = np.random.rand(len(params))
         params.update_from_raw(raw)
         assert np.allclose(raw, params.raw())
 
     def test_QAOAVariationalStandardWithBiasParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         params = QAOAVariationalStandardWithBiasParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, time=2
         )
         assert np.allclose(qaoa_descriptor.qureg, [0, 1, 2])
         assert np.allclose(params.mixer_1q_angles, [[-2 * 0.75] * 3, [-2 * 0.25] * 3])
         assert np.allclose(params.cost_1q_angles, [[2 * 0.125], [2 * 0.375]])
@@ -427,15 +413,14 @@
 
         # Test updating and raw output
         raw = np.random.rand(len(params))
         params.update_from_raw(raw)
         assert np.allclose(raw, params.raw())
 
     def test_QAOAVariationalStandardParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
         params = QAOAVariationalStandardParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, time=2
         )
 
         assert np.allclose(qaoa_descriptor.qureg, [0, 1, 2])
         assert np.allclose(params.mixer_1q_angles, [[-2 * 0.75] * 3, [-2 * 0.25] * 3])
@@ -468,15 +453,14 @@
         assert np.allclose(p2.mixer_1q_angles, p3.mixer_1q_angles)
         assert np.allclose(p1.cost_1q_angles, p2.cost_1q_angles)
         assert np.allclose(p2.cost_1q_angles, p3.cost_1q_angles)
         assert np.allclose(p1.cost_2q_angles, p2.cost_2q_angles)
         assert np.allclose(p2.cost_2q_angles, p3.cost_2q_angles)
 
     def test_QAOAVariationalFourierParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=3)
         params = QAOAVariationalFourierParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, q=2, time=2
         )
 
         # just access the angles, to check that it actually creates them
         assert len(params.cost_1q_angles) == len(params.cost_2q_angles)
@@ -484,15 +468,14 @@
         assert np.allclose(params.u, [1 / 3, 0])
         # Test updating and raw output
         raw = np.random.rand(len(params))
         params.update_from_raw(raw)
         assert np.allclose(raw, params.raw())
 
     def test_QAOAVariationalFourierWithBiasParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=3)
         params = QAOAVariationalFourierWithBiasParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, q=2, time=2
         )
 
         # just access the angles, to check that it actually creates them
         assert len(params.cost_1q_angles) == len(params.cost_2q_angles)
@@ -501,15 +484,14 @@
         assert np.allclose(params.u_pairs, [1 / 3, 0])
         # Test updating and raw output
         raw = np.random.rand(len(params))
         params.update_from_raw(raw)
         assert np.allclose(raw, params.raw())
 
     def test_QAOAVariationalFourierExtendedParams(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=3)
         params = QAOAVariationalFourierExtendedParams.linear_ramp_from_hamiltonian(
             qaoa_descriptor, q=2, time=2
         )
 
         # just access the angles, to check that it actually creates them
         assert len(params.cost_1q_angles) == len(params.cost_2q_angles)
@@ -543,15 +525,14 @@
         assert np.allclose(params1.cost_1q_angles, params2.cost_1q_angles)
         assert np.allclose(params1.cost_2q_angles, params2.cost_2q_angles)
         assert np.allclose(params1.mixer_1q_angles, params3.mixer_1q_angles)
         assert np.allclose(params1.cost_1q_angles, params3.cost_1q_angles)
         assert np.allclose(params1.cost_2q_angles, params3.cost_2q_angles)
 
     def test_inputChecking(self):
-
         # Check that an error is raised if we pass in an extra angle in `betas` (depth is 3, here we give 4 beta values)
         reg = [0, 1]
         terms = [[0, 1]]
         weights = [0.7]
         n_layers = 3
         betas_singles = [1, 2, 3, 4]
         betas_pairs = []
@@ -567,30 +548,28 @@
             betas_singles,
             betas_pairs,
             gammas_singles,
             gammas_pairs,
         )
 
     def test_str_and_repr(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
 
         for each_key_value in PARAMS_CLASSES_MAPPER.keys():
             variate_params = create_qaoa_variational_params(
                 qaoa_descriptor,
                 params_type=each_key_value,
                 init_type="rand",
                 q=1,
                 total_annealing_time=1,
             )
 
             self.assertEqual(variate_params.__str__(), variate_params.__repr__())
 
     def test_qaoa_variational_params_asdict(self):
-
         p = 4
         q = 2
 
         number_of_params = {
             "standard": {"betas": p, "gammas": p},
             "standard_w_bias": {"betas": p, "gammas_singles": p, "gammas_pairs": p},
             "extended": {
@@ -609,15 +588,14 @@
             "fourier_w_bias": {"v": q, "u_singles": q, "u_pairs": q},
             "annealing": {"schedule": p},
         }
 
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=p)
 
         for each_key_value in PARAMS_CLASSES_MAPPER.keys():
-
             # create the variational params object
             variate_params = create_qaoa_variational_params(
                 qaoa_descriptor,
                 params_type=each_key_value,
                 init_type="rand",
                 q=q,
                 total_annealing_time=2,
@@ -654,15 +632,14 @@
                 list_params_raw += value.flatten().tolist()
 
             assert np.allclose(
                 list_params_raw, variate_params.raw().tolist()
             ), f"asdict() should return a dict with the correct values, it did not for type: '{each_key_value}'."
 
     def test_qaoa_variational_params_update_from_dict(self):
-
         qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
 
         for each_key_value in PARAMS_CLASSES_MAPPER.keys():
             variate_params = create_qaoa_variational_params(
                 qaoa_descriptor,
                 params_type=each_key_value,
                 init_type="rand",
```

### Comparing `openqaoa-0.1.3/tests/test_parameters_plots.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_parameters_plots.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_pyquil_qvm.py` & `openqaoa-0.1.3rc1/src/openqaoa-pyquil/tests/test_pyquil_qvm.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     backend. `as_qvm` is set to be True throughout.
 
     For all of these tests, qvm and quilc must be running.
     """
 
     @pytest.mark.qvm
     def test_connection(self):
-
         """
         Checks if connection to qvm and quilc is successful.
         TODO : improve test
         """
 
         # Check connection to qvm
         device_pyquil = DevicePyquil(
@@ -44,15 +43,14 @@
         program = Program().inst(RX(np.pi, 0))
         device_pyquil.quantum_computer.compiler.quil_to_native_quil(program)
 
         pass
 
     @pytest.mark.qvm
     def test_active_reset(self):
-
         """
         Test if active_reset works fine.
         Check for RESET instruction in parametric circuit when active_reset = True / False
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
@@ -87,15 +85,14 @@
         )
         assert "RESET" not in [
             str(instr) for instr in backend_obj_pyquil.parametric_circuit
         ]
 
     @pytest.mark.qvm
     def test_rewiring(self):
-
         """
         Test if rewiring works fine.
 
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
@@ -147,15 +144,14 @@
         )
         assert 'PRAGMA INITIAL_REWIRING "PARTIAL"' in [
             str(instr) for instr in backend_obj_pyquil.parametric_circuit
         ]
 
     @pytest.mark.qvm
     def test_qaoa_pyquil_expectation(self):
-
         """
         Checks if expectation value agrees with known values. Since angles are selected such that the final state is one of the computational basis states, shots do not matter (there is no statistical variance).
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
         )
@@ -182,27 +178,27 @@
         )
         backend_obj_pyquil.expectation(variate_params)
 
         assert np.isclose(backend_obj_pyquil.expectation(variate_params), -1)
 
     @pytest.mark.qvm
     def test_qaoa_pyquil_gate_names(self):
-
         """
         Checks if names of gates are correct, and no. of measurement gates match the no. of qubits.
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
         )
 
         # Without interaction terms
         cost_hamil = Hamiltonian([PauliOp("Z", (0,)), PauliOp("Z", (1,))], [1, 1], 1)
         mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=1)
+        params = create_qaoa_variational_params(qaoa_descriptor, "standard", "ramp")
         backend_obj_pyquil = QAOAPyQuilQPUBackend(
             qaoa_descriptor=qaoa_descriptor,
             device=device_pyquil,
             prepend_state=None,
             append_state=None,
             init_hadamard=True,
             cvar_alpha=1,
@@ -228,28 +224,29 @@
             "RX",
             "RX",
         ]
 
         measurement_gate_no = len(
             [
                 instr
-                for instr in backend_obj_pyquil.parametric_circuit
+                for instr in backend_obj_pyquil.qaoa_circuit(params)
                 if type(instr) == quilbase.Measurement
             ]
         )
         assert measurement_gate_no == 2
 
         # With interaction terms
         cost_hamil = Hamiltonian(
             [PauliOp("Z", (0,)), PauliOp("Z", (1,)), PauliOp("ZZ", (0, 1))],
             [1, 1, 1],
             1,
         )
         mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=1)
+        params = create_qaoa_variational_params(qaoa_descriptor, "standard", "ramp")
         backend_obj_pyquil = QAOAPyQuilQPUBackend(
             qaoa_descriptor=qaoa_descriptor,
             device=device_pyquil,
             prepend_state=None,
             append_state=None,
             init_hadamard=True,
             cvar_alpha=1,
@@ -278,23 +275,22 @@
             "RX",
             "RX",
         ]
 
         measurement_gate_no = len(
             [
                 instr
-                for instr in backend_obj_pyquil.parametric_circuit
+                for instr in backend_obj_pyquil.qaoa_circuit(params)
                 if type(instr) == quilbase.Measurement
             ]
         )
         assert measurement_gate_no == 2
 
     @pytest.mark.qvm
     def test_circuit_init_hadamard(self):
-
         """
         Checks correctness of circuit for the argument `init_hadamard`.
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
         )
@@ -358,18 +354,17 @@
         )
 
         assert ["RZ", "RZ", "RZ", "RZ", "CPHASE", "RX", "RX"] == [
             instr.name
             for instr in pyquil_backend.parametric_circuit
             if type(instr) == quilbase.Gate
         ]
-
+        
     @pytest.mark.qvm
     def test_circuit_append_state(self):
-
         """
         Checks correctness of circuit for the argument `append_state`.
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
         )
@@ -379,35 +374,73 @@
             [PauliOp("Z", (0,)), PauliOp("Z", (1,)), PauliOp("ZZ", (0, 1))],
             [1, 1, 1],
             1,
         )
         mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=1)
 
+        params = create_qaoa_variational_params(qaoa_descriptor, "standard", "ramp")
+
         append_circuit = Program().inst(RX(np.pi, 0), RY(np.pi / 2, 1), RZ(np.pi, 0))
 
         pyquil_backend = QAOAPyQuilQPUBackend(
             device_pyquil,
             qaoa_descriptor,
             n_shots=10,
             prepend_state=None,
-            append_state=append_circuit,
+            append_state=append_circuit,  
             init_hadamard=False,
             cvar_alpha=1,
         )
 
-        assert ["RZ", "RZ", "RZ", "RZ", "CPHASE", "RX", "RX", "RX", "RY", "RZ"] == [
+        assert set([
+            "RZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "CZ",
+            "RZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "CZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RZ",
+            "RX",
+            "RZ",
+            "RX",
+            "RZ",
+        ]) == set([
             instr.name
-            for instr in pyquil_backend.parametric_circuit
+            for instr in pyquil_backend.qaoa_circuit(params)
             if type(instr) == quilbase.Gate
-        ]
+        ])
 
     @pytest.mark.qvm
     def test_circuit_prepend_state(self):
-
         """
         Checks correctness of circuit for the argument `prepend_state`.
         """
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
         )
@@ -452,15 +485,14 @@
                 cvar_alpha=1,
                 n_shots=1,
             ),
         )
 
     @pytest.mark.qvm
     def test_pyquil_vectorized_agreement(self):
-
         """
         Checks correctness of expectation values with vectorized backend, up to a tolerance of delta = std.dev.
         """
 
         # Without interaction terms
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=3, compiler_timeout=3
```

### Comparing `openqaoa-0.1.3/tests/test_qpu_braket.py` & `openqaoa-0.1.3rc1/src/openqaoa-braket/tests/test_qpu_braket.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_qpu_qiskit.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_qpu_qiskit.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import pytest
 import subprocess
 
 from qiskit import QuantumCircuit
 from qiskit.quantum_info import Operator
 from qiskit.tools.monitor import job_monitor
 
-
-from openqaoa_azure.backends import DeviceAzure
 from openqaoa.qaoa_components import (
     create_qaoa_variational_params,
     PauliOp,
     Hamiltonian,
     QAOADescriptor,
     QAOAVariationalStandardParams,
 )
@@ -25,160 +23,14 @@
     QAOAQiskitBackendStatevecSimulator,
 )
 from openqaoa.utilities import X_mixer_hamiltonian
 from openqaoa.problems import NumberPartition
 from openqaoa import QAOA, create_device
 
 
-class TestingQAOAQiskitQPUBackendAzure(unittest.TestCase):
-
-    """This Object tests the QAOA Qiskit QPU Backend object with the Azure
-    Device object. This checks that the use of qiskit to send circuits to Azure
-    is working as intended.
-
-    The Azure CLI has to be configured beforehand to run these tests.
-    """
-
-    @pytest.mark.api
-    def setUp(self):
-        """
-        Setting up the credentials
-        """
-        bashCommand = "az resource list"
-        process = subprocess.Popen(bashCommand.split(), stdout=subprocess.PIPE)
-        output, error = process.communicate()
-
-        if error is not None:
-            print(error)
-            raise Exception(
-                "You must have the Azure CLI installed and must be logged in to use the Azure Quantum Backends"
-            )
-        else:
-            output_json = json.loads(output)
-            output_json_s = [
-                each_json
-                for each_json in output_json
-                if each_json["name"] == "TestingOpenQAOA"
-            ][0]
-            self.RESOURCE_ID = output_json_s["id"]
-            self.AZ_LOCATION = output_json_s["location"]
-
-    @pytest.mark.sim
-    def check_shots_tally(self):
-        """
-        There is a known bug in the qiskit backend for azure where if the shots
-        argument might be ignored. This test checks that the output from the azure
-        computation matches the input requirements.
-        """
-
-        shots = 1024
-        problem_qubo = NumberPartition([1, 2, 3]).qubo
-        azure_device = create_device(
-            location="azure",
-            name="rigetti.sim.qvm",
-            resource_id=self.RESOURCE_ID,
-            az_location=self.AZ_LOCATION,
-        )
-
-        q = QAOA()
-        q.set_device(azure_device)
-        q.set_backend_properties(n_shots=shots)
-        q.set_classical_optimizer(maxiter=1)
-        q.compile(problem_qubo)
-        q.optimize()
-
-        q.dump(file_name="check_shots_tally", prepend_id=False, overwrite=True)
-
-        comp_shots = sum(q.result.optimized["optimized measurement outcomes"].values())
-
-        self.assertEqual(shots, comp_shots)
-
-    @pytest.mark.api
-    def test_expectations_in_init(self):
-        """
-        Testing the Exceptions in the init function of the QiskitQPUShotBasedBackend
-        """
-
-        nqubits = 3
-        p = 1
-        weights = [1, 1, 1]
-        gammas = [1 / 8 * np.pi]
-        betas = [1 / 8 * np.pi]
-        shots = 10000
-
-        cost_hamil = Hamiltonian(
-            [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
-            weights,
-            1,
-        )
-        mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits)
-        qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=p)
-
-        # Try to compute the variate params
-        _ = QAOAVariationalStandardParams(qaoa_descriptor, betas, gammas)
-
-        # We mock the potential Exception that could occur in the Device class
-        azure_device = DeviceAzure("", "", "")
-        azure_device._check_provider_connection = Mock(return_value=False)
-
-        try:
-            QAOAQiskitQPUBackend(qaoa_descriptor, azure_device, shots, None, None, True)
-        except Exception as e:
-            self.assertEqual(str(e), "Error connecting to AZURE.")
-
-        with self.assertRaises(Exception):
-            QAOAQiskitQPUBackend(qaoa_descriptor, azure_device, shots, None, None, True)
-
-        azure_device = DeviceAzure(
-            device_name="", resource_id=self.RESOURCE_ID, az_location=self.AZ_LOCATION
-        )
-
-        try:
-            QAOAQiskitQPUBackend(qaoa_descriptor, azure_device, shots, None, None, True)
-        except Exception as e:
-            self.assertEqual(
-                str(e),
-                "Connection to AZURE was made. Error connecting to the specified backend.",
-            )
-
-        with self.assertRaises(Exception):
-            QAOAQiskitQPUBackend(qaoa_descriptor, azure_device, shots, None, None, True)
-
-    @pytest.mark.api
-    def test_remote_qubit_overflow(self):
-        """
-        If the user creates a circuit that is larger than the maximum circuit size
-        that is supported by the QPU. An Exception should be raised with the
-        appropriate error message alerting the user to the error.
-        """
-
-        shots = 100
-
-        set_of_numbers = np.random.randint(1, 10, 6).tolist()
-        qubo = NumberPartition(set_of_numbers).qubo
-
-        mixer_hamil = X_mixer_hamiltonian(n_qubits=6)
-        qaoa_descriptor = QAOADescriptor(qubo.hamiltonian, mixer_hamil, p=1)
-
-        # Check the creation of the varitional parms
-        _ = create_qaoa_variational_params(qaoa_descriptor, "standard", "rand")
-
-        azure_device = DeviceAzure(
-            "rigetti.sim.qvm", self.RESOURCE_ID, self.AZ_LOCATION
-        )
-
-        try:
-            QAOAQiskitQPUBackend(qaoa_descriptor, azure_device, shots, None, None, True)
-        except Exception as e:
-            self.assertEqual(
-                str(e),
-                "There are lesser qubits on the device than the number of qubits required for the circuit.",
-            )
-
-
 class TestingQAOAQiskitQPUBackend(unittest.TestCase):
 
     """This Object tests the QAOA Qiskit QPU Backend objects, which is tasked with the
     creation and execution of a QAOA circuit for the selected QPU provider and
     backend.
 
     IBMQ Account has to be saved locally to run these tests.
```

### Comparing `openqaoa-0.1.3/tests/test_result_object.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_result_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         q.optimize()
 
         assert set(
             ["most_probable_states", "evals", "intermediate", "optimized"]
         ) <= set([a for a in dir(q.result) if not a.startswith("__")])
 
     def test_most_probable_bitstring(self):
-
         cost_hamil = Hamiltonian(
             [
                 PauliOp("ZZ", (0, 3)),
                 PauliOp("ZZ", (0, 1)),
                 PauliOp("ZZ", (1, 2)),
                 PauliOp("ZZ", (2, 3)),
                 PauliOp("Z", (0,)),
@@ -100,52 +99,39 @@
             mps_sv["solutions_bitstrings"]
         )  # Equality for sv
         assert set(["0101", "1010"]) >= set(
             mps_shot["solutions_bitstrings"]
         )  # Subset for shot/qpu
 
     def test_plot_cost(self):
-
         # Create the problem
         g = nx.circulant_graph(6, [1])
         vc = MinimumVertexCover(g, field=1.0, penalty=10).qubo
 
         q = QAOA()
         q.compile(vc, verbose=False)
         q.optimize()
 
         q.result.plot_cost()
 
     def test_plot_probabilities(self):
-
         # Create the problem
         g = nx.circulant_graph(6, [1])
         vc = MinimumVertexCover(g, field=1.0, penalty=10).qubo
 
         # first for state-vector based simulator:
         q_sv = QAOA()
         q_sv.set_circuit_properties(p=3, init_type="ramp")
         q_sv.compile(vc)
 
         q_sv.optimize()
 
         q_sv.result.plot_probabilities()
 
-        # then for shot based simulator:
-        q_shot = QAOA()
-        q_shot_dev = create_device(location="local", name="qiskit.shot_simulator")
-        q_shot.set_device(q_shot_dev)
-
-        q_shot.compile(vc)
-        q_shot.optimize()
-
-        q_shot.result.plot_probabilities()
-
     def test_plot_n_shots(self):
-
         # Create the problem
         g = nx.circulant_graph(6, [1])
         vc = MinimumVertexCover(g, field=1.0, penalty=10).qubo
 
         for method in ["cans", "icans"]:
             q = QAOA()
             q.set_classical_optimizer(
@@ -237,15 +223,14 @@
                 argument="label", inputs_to_try=[0, ["one", "two", "three"], [1, "two"]]
             )
             test_incorrect_arguments(
                 argument="color", inputs_to_try=[0, ["b", "c", "g"], [1, "g"]]
             )
 
     def test_get_counts(self):
-
         # measurement outcome from a statevector_simulator backend
         optimized_measurement_outcomes_sv = np.array(
             [
                 0.18256422 - 0.1296918j,
                 -0.03786405 - 0.13158363j,
                 -0.03786405 - 0.13158363j,
                 -0.01910622 + 0.3151214j,
```

### Comparing `openqaoa-0.1.3/tests/test_results.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_results.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,19 +11,16 @@
 )
 from openqaoa.backends import create_device
 from openqaoa.backends.basebackend import QAOABaseBackendStatevector
 from openqaoa.backends.devices_core import SUPPORTED_LOCAL_SIMULATORS
 from openqaoa.problems import MinimumVertexCover, QUBO, MaximumCut
 from openqaoa.qaoa_components import Hamiltonian
 
-ALLOWED_LOCAL_SIMUALTORS = SUPPORTED_LOCAL_SIMULATORS
-
 
 def _compare_qaoa_results(dict_old, dict_new, bool_cmplx_str):
-
     for key in dict_old.keys():
         if key == "cost_hamiltonian":  ## CHECK WHAT DO WITH THIS
             pass
         elif key == "_QAOAResult__type_backend":
             if issubclass(dict_old[key], QAOABaseBackendStatevector):
                 assert (
                     dict_new[key] == QAOABaseBackendStatevector
@@ -94,15 +91,14 @@
 class TestingResultOutputs(unittest.TestCase):
 
     """
     Test the Results Output after an optimization loop
     """
 
     def test_flags_result_outputs_workflow(self):
-
         """
         Run an optimization problem for 5 iterations.
         Should expect certain fields of the results output to be filled based
         on some of the users inputs. (Default settings)
         Can be checked for cobyla.
 
         Check for all available supported local backends.
@@ -112,27 +108,26 @@
         vc = MinimumVertexCover(g, field=1.0, penalty=10).qubo
 
         choice_combination = list(
             itertools.product([True, False], [True, False], [True, False])
         )
         recorded_evals = [0, 5]
 
-        for device_name in ALLOWED_LOCAL_SIMUALTORS:
-
+        for device_name in SUPPORTED_LOCAL_SIMULATORS:
             for each_choice in choice_combination:
-
                 q = QAOA()
                 q.set_classical_optimizer(
                     method="cobyla",
                     parameter_log=each_choice[0],
                     cost_progress=each_choice[1],
                     optimization_progress=each_choice[2],
                     maxiter=5,
                 )
                 device = create_device("local", device_name)
+                print(device.device_name)
                 q.set_device(device)
                 q.compile(vc)
                 q.optimize()
                 self.assertEqual(
                     recorded_evals[each_choice[0]], len(q.result.intermediate["angles"])
                 )
                 self.assertEqual(
@@ -324,21 +319,21 @@
         """
 
         # problem
         maxcut_qubo = MaximumCut(
             nw.generators.fast_gnp_random_graph(n=6, p=0.6, seed=42)
         ).qubo
 
-        # run qaoa with different devices, and save the objcets in a list
+        # run qaoa with different devices, and save the objects in a list
         qaoas = []
         for device in [
-            create_device(location="local", name="qiskit.shot_simulator"),
-            create_device(location="local", name="vectorized"),
+            create_device(location="local", name=each_device_name)
+            for each_device_name in SUPPORTED_LOCAL_SIMULATORS
+            if each_device_name != "analytical_simulator"
         ]:
-
             q = QAOA()
             q.set_device(device)
             q.set_circuit_properties(
                 p=1, param_type="extended", init_type="rand", mixer_hamiltonian="x"
             )
             q.set_backend_properties(prepend_state=None, append_state=None)
             q.set_classical_optimizer(maxiter=10, optimization_progress=True)
@@ -361,14 +356,108 @@
                     results_from_dict, QAOAResult
                 ), "results_from_dict is not an instance of Result"
 
                 _compare_qaoa_results(
                     results.__dict__, results_from_dict.__dict__, bool_cmplx_str
                 )
 
+    def test_qaoa_results_calculate_statistics_full(self):
+
+        maxcut_qubo = MaximumCut(
+            nw.generators.fast_gnp_random_graph(n=6, p=0.6, seed=42)
+        ).qubo
+
+        qaoas = []
+        for device_name in SUPPORTED_LOCAL_SIMULATORS:
+            if device_name == "analytical_simulator":
+                continue
+
+            qaoa = QAOA()
+
+            qaoa.set_device(create_device("local", device_name))
+            qaoa.set_classical_optimizer(optimization_progress=True)
+
+            qaoa.compile(maxcut_qubo)
+            qaoa.optimize()
+
+            qaoas.append(qaoa)
+
+        for qaoa in qaoas:
+            result = qaoa.result.calculate_statistics(include_intermediate=True)
+            result_optimized = result['optimized']
+            result_intermediate = result['intermediate']
+            optimized_sorted, optimized_mean, optimized_std_deviation = list(result_optimized['sorted'].values()), \
+                result_optimized['mean'], result_optimized['std_deviation']
+
+            for ri in result_intermediate:
+                intermediate_sorted, intermediate_mean, intermediate_std_deviation = list(ri['sorted'].values()), ri['mean'], ri['std_deviation']
+
+                assert all(intermediate_sorted[i] >= intermediate_sorted[i + 1] for i in range(len(intermediate_sorted) - 1)), "Counts in descending order."
+                assert intermediate_mean > 0, "Mean is greater then zero."
+                assert intermediate_std_deviation > 0, "Standard deviation is greater than zero."
+
+            assert all(optimized_sorted[i] >= optimized_sorted[i + 1] for i in range(len(optimized_sorted) - 1)), "Counts in descending order."
+            assert optimized_mean > 0, "Mean is greater then zero."
+            assert optimized_std_deviation > 0, "Standard deviation is greater than zero."
+
+    def test_qaoa_results_calculate_statistics_without_intermediate(self):
+
+        maxcut_qubo = MaximumCut(
+            nw.generators.fast_gnp_random_graph(n=6, p=0.6, seed=42)
+        ).qubo
+
+        qaoas = []
+        for device_name in SUPPORTED_LOCAL_SIMULATORS:
+            if device_name == "analytical_simulator":
+                continue
+
+            qaoa = QAOA()
+            qaoa.set_device(create_device("local", device_name))
+            qaoa.set_classical_optimizer(optimization_progress=False)
+
+            qaoa.compile(maxcut_qubo)
+            qaoa.optimize()
+
+            qaoas.append(qaoa)
+
+        for qaoa in qaoas:
+            result = qaoa.result.calculate_statistics(include_intermediate=False)
+            result_optimized = result['optimized']
+            optimized_sorted, optimized_mean, optimized_std_deviation = list(result_optimized['sorted'].values()), \
+                result_optimized['mean'], result_optimized['std_deviation']
+
+            assert result['intermediate'] == [], "Statistics for intermediate measurements are empty."
+            assert all(optimized_sorted[i] >= optimized_sorted[i + 1] for i in range(len(optimized_sorted) - 1)), "Counts in descending order."
+            assert optimized_mean > 0, "Mean is greater then zero."
+            assert optimized_std_deviation > 0, "Standard deviation is greater than zero."
+
+    def test_qaoa_results_calculate_statistics_raise_value_error(self):
+        """
+        The method raise an error if the user requires statistics on all 
+        intermediate measurement outcomes but hasn't specified saving them during optimization.
+        """
+        maxcut_qubo = MaximumCut(
+            nw.generators.fast_gnp_random_graph(n=6, p=0.6, seed=42)
+        ).qubo
+
+        qaoa = QAOA()
+        qaoa.set_device(create_device(location="local", name="vectorized"))
+        qaoa.set_classical_optimizer(optimization_progress=False)
+
+        qaoa.compile(maxcut_qubo)
+        qaoa.optimize()
+
+        try:
+            qaoa.result.calculate_statistics(include_intermediate=True)
+        except ValueError as e:
+            self.assertEqual(
+                str(e),
+                "The underlying QAOA object does not seem to have any intermediate measurement result. Please, consider saving intermediate measurements during optimization by setting `optimization_progress=True` in your workflow.",
+            )
+
 
 class TestingRQAOAResultOutputs(unittest.TestCase):
     """
     Test the  Results Output after a full RQAOA loop
     """
 
     def __run_rqaoa(
@@ -376,15 +465,15 @@
         type="custom",
         eliminations=1,
         p=1,
         param_type="standard",
         mixer="x",
         method="cobyla",
         maxiter=15,
-        name_device="qiskit.statevector_simulator",
+        name_device="vectorized",
     ):
         """
         private function to run the RQAOA
         """
 
         n_qubits = 6
         n_cutoff = 3
@@ -501,15 +590,14 @@
         # test the solution method
         assert (
             results.get_solution() == results["solution"]
         ), "get_solution method is not correct"
 
         # test the methods for the intermediate steps
         for i in range(results["number_steps"]):
-
             # methods for intermediate qaao results
             assert (
                 results.get_qaoa_results(i)
                 == results["intermediate_steps"][i]["qaoa_results"]
             ), "get_qaoa_results method is not correct"
             assert (
                 results.get_qaoa_optimized_angles(i)
@@ -683,19 +771,20 @@
         # problem
         maxcut_qubo = MaximumCut(
             nw.generators.fast_gnp_random_graph(n=6, p=0.6, seed=42)
         ).qubo
 
         # run rqaoa with different devices, and save the objcets in a list
         rqaoas = []
+
         for device in [
-            create_device(location="local", name="qiskit.shot_simulator"),
-            create_device(location="local", name="vectorized"),
+            create_device(location="local", name=each_device_name)
+            for each_device_name in SUPPORTED_LOCAL_SIMULATORS
+            if each_device_name != "analytical_simulator"
         ]:
-
             r = RQAOA()
             r.set_device(device)
             r.set_circuit_properties(
                 p=1, param_type="extended", init_type="rand", mixer_hamiltonian="x"
             )
             r.set_backend_properties(prepend_state=None, append_state=None)
             r.set_classical_optimizer(maxiter=10, optimization_progress=True)
@@ -704,15 +793,14 @@
 
             r.optimize()
 
             rqaoas.append(r)
 
         # for each rqaoa object, we check that we can create a new results object from the dictionary of the old one
         for r in rqaoas:
-
             new_results = RQAOAResult.from_dict(r.result.asdict())
             old_results = r.result
 
             # assert that new_results is an instance of RQAOAResult
             assert isinstance(
                 new_results, RQAOAResult
             ), "new_results is not an instance of RQAOAResult"
```

### Comparing `openqaoa-0.1.3/tests/test_rqaoa.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_rqaoa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.3/tests/test_sample_from_wavefunction.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_sample_from_wavefunction_qiskit.py`

 * *Files 24% similar despite different names*

```diff
@@ -129,43 +129,9 @@
         samples_prob_qiskit = np.array(list(samples_dict_qiskit.values()), dtype=float)
 
         np.testing.assert_array_almost_equal(prob_wf_vec, samples_prob_vec, decimal=3)
         np.testing.assert_array_almost_equal(
             prob_wf_qiskit, samples_prob_qiskit, decimal=3
         )
 
-    # def testing_w_init_prog(self):
-    # 	"""
-    # 	This function creates an init_prog and then implements a Hamiltonian
-    # 	with zero betas and gammas.
-    # 	"""
-    # 	reg = [0,1,2,3,4,5]
-    # 	init_terms = [(i,) for i in reg]
-    # 	init_weights = [1]*len(init_terms)
-    # 	init_p=2
-
-    # 	init_params = ([[np.pi/4]*len(reg),
-    # 					[np.pi/2,0,0,0,0,np.pi/2]],
-    # 					[[-np.pi/4]*len(init_terms),
-    # 					[0]*len(reg)],
-    # 					[[],[]])
-    # 	hyperparams_init = HyperParams(init_terms,init_weights,reg,init_p)
-    # 	init_prog = ExtendedParams(hyperparams_init,init_params)
-
-    # 	terms,weights = zip(*random_hamiltonian(reg).items())
-    # 	terms, weights = list(terms),list(weights)
-    # 	p=1
-    # 	trainable_params = ([0],[0])
-    # 	hyperparams = HyperParams(terms,weights,reg,p)
-
-    # 	qaoa_params = StandardParams(hyperparams,trainable_params)
-    # 	cost_fn = QAOACostVector(qaoa_params,init_prog=init_prog)
-
-    # 	solution = '100001'
-    # 	shot_results = cost_fn.get_samples(qaoa_params.raw(), nshots=15)
-    # 	bool_list = [x == solution for x in shot_results]
-
-    # 	assert all(bool_list)
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_sim_qiskit.py` & `openqaoa-0.1.3rc1/src/openqaoa-qiskit/tests/test_sim_qiskit.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
     """This Object tests the QAOA Qiskit Simulator Backend objects, which is
     tasked with the creation and execution of a QAOA circuit for the qiskit
     library and its local backends.
     """
 
     def test_circuit_angle_assignment_statevec_backend(self):
-
         """
         A tests that checks if the circuit created by the Qiskit Backend
         has the appropriate angles assigned before the circuit is executed.
         Checks the circuit created on IBM Simulator Backends.
         """
 
         ntrials = 10
@@ -41,15 +40,14 @@
             [np.random.rand(), np.random.rand(), np.random.rand()]
             for i in range(ntrials)
         ]
         init_hadamards = [np.random.choice([True, False]) for i in range(ntrials)]
         constants = [np.random.rand() for i in range(ntrials)]
 
         for i in range(ntrials):
-
             gammas = [np.random.rand() * np.pi for i in range(p)]
             betas = [np.random.rand() * np.pi for i in range(p)]
 
             print(gammas)
             print(betas)
 
             cost_hamil = Hamiltonian(
@@ -86,15 +84,14 @@
 
             self.assertEqual(
                 main_circuit.to_instruction().definition,
                 statevec_circuit.to_instruction().definition,
             )
 
     def test_circuit_angle_assignment_statevec_backend_w_hadamard(self):
-
         """
         Checks for consistent if init_hadamard is set to True.
         """
 
         ntrials = 10
 
         nqubits = 3
@@ -103,15 +100,14 @@
             [np.random.rand(), np.random.rand(), np.random.rand()]
             for i in range(ntrials)
         ]
         init_hadamards = [np.random.choice([True, False]) for i in range(ntrials)]
         constants = [np.random.rand() for i in range(ntrials)]
 
         for i in range(ntrials):
-
             gammas = [np.random.rand() * np.pi for i in range(p)]
             betas = [np.random.rand() * np.pi for i in range(p)]
 
             cost_hamil = Hamiltonian(
                 [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
                 weights[i],
                 constants[i],
@@ -146,15 +142,14 @@
 
             self.assertEqual(
                 main_circuit.to_instruction().definition,
                 statevec_circuit.to_instruction().definition,
             )
 
     def test_prepend_circuit(self):
-
         """
         Checks if prepended circuit has been prepended correctly.
         """
 
         nqubits = 3
         p = 1
         weights = [1, 1, 1]
@@ -203,15 +198,14 @@
         )
         self.assertEqual(
             main_circuit.to_instruction().definition,
             shot_circuit.to_instruction().definition,
         )
 
     def test_append_circuit(self):
-
         """
         Checks if appended circuit is appropriately appended to the back of the
         QAOA Circuit.
         """
 
         nqubits = 3
         p = 1
@@ -261,15 +255,14 @@
         )
         self.assertEqual(
             main_circuit.to_instruction().definition,
             shot_circuit.to_instruction().definition,
         )
 
     def test_qaoa_circuit_wavefunction_expectation_equivalence_1(self):
-
         """
         The following tests with a similar naming scheme check for consistency
         between the outputs of the qiskit statevector simulator and the
         vectorized backend.
         We compare both the wavefunctions returned by the Backends and the
         expectation values.
         """
@@ -277,15 +270,14 @@
         nqubits = 3
         p = 1
         weights = [1, 2, 3]
         gammas = [[3], [2]]
         betas = [[1], [1 / 8]]
 
         for i in range(2):
-
             cost_hamil = Hamiltonian(
                 [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
                 weights,
                 1,
             )
             mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits)
             qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=p)
@@ -313,30 +305,28 @@
                     qiskit_wavefunction[j].real, vector_wavefunction[j].real
                 )
                 self.assertAlmostEqual(
                     qiskit_wavefunction[j].imag, vector_wavefunction[j].imag
                 )
 
     def test_qaoa_circuit_wavefunction_expectation_equivalence_2(self):
-
         """Due to the difference in the constructions of the statevector simulators,
         there is a global phase difference between the results obtained from
         qiskit's statevector simulator and OpenQAOA's vectorised simulator. In order to
         show the equivalence between the wavefunctions produced, the expectation
         of a random operator is computed.
         """
 
         nqubits = 3
         p = 1
         weights = [1, 2, 3]
         gammas = [[1 / 8 * np.pi], [1 / 8 * np.pi]]
         betas = [[1], [1 / 8 * np.pi]]
 
         for i in range(2):
-
             cost_hamil = Hamiltonian(
                 [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
                 weights,
                 1,
             )
 
             mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits)
@@ -375,15 +365,14 @@
             )
 
             self.assertAlmostEqual(expect_qiskit.real, expect_vector.real)
             self.assertAlmostEqual(expect_qiskit.imag, expect_vector.imag)
             self.assertAlmostEqual(qiskit_expectation, vector_expectation)
 
     def test_qaoa_circuit_wavefunction_expectation_equivalence_3(self):
-
         """Due to the difference in the constructions of the statevector simulators,
         there is a global phase difference between the results obtained from
         qiskit's statevector simulator and OpenQAOA's vectorised simulator. In order to
         show the equivalence between the wavefunctions produced, the expectation
         of a random operator is computed.
 
         Nonuniform mixer weights.
@@ -392,15 +381,14 @@
         nqubits = 3
         p = 1
         weights = [1, 2, 3]
         gammas = [[1 / 8 * np.pi], [1 / 8 * np.pi]]
         betas = [[1], [1 / 8 * np.pi]]
 
         for i in range(2):
-
             cost_hamil = Hamiltonian(
                 [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
                 weights,
                 1,
             )
 
             mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits, coeffs=[1, 2, 3])
@@ -439,15 +427,14 @@
             )
 
             self.assertAlmostEqual(expect_qiskit.real, expect_vector.real)
             self.assertAlmostEqual(expect_qiskit.imag, expect_vector.imag)
             self.assertAlmostEqual(qiskit_expectation, vector_expectation)
 
     def test_qaoa_circuit_wavefunction_expectation_equivalence_4(self):
-
         """Due to the difference in the constructions of the statevector simulators,
         there is a global phase difference between the results obtained from
         qiskit's statevector simulator and OpenQAOA's vectorised simulator. In order to
         show the equivalence between the wavefunctions produced, the expectation
         of a random operator is computed.
 
         Y, YY and XX mixers with nonuniform weights.
@@ -456,15 +443,14 @@
         nqubits = 3
         p = 1
         weights = [1, 2, 3]
         gammas = [[1 / 8 * np.pi], [1 / 8 * np.pi]]
         betas = [[1], [1 / 8 * np.pi]]
 
         for i in range(2):
-
             cost_hamil = Hamiltonian(
                 [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
                 weights,
                 1,
             )
             mixer_hamil = Hamiltonian(
                 [
@@ -540,15 +526,14 @@
         exp_qiskit_statevec = backend_qiskit_statevec.expectation(
             (variational_params_std)
         )
 
         assert np.isclose(exp_qiskit_statevec, -6)
 
     def test_get_wavefunction(self):
-
         n_qubits = 3
         terms = [[0, 1], [0, 2], [0]]
         weights = [1, 1, -0.5]
         p = 1
 
         betas_singles = [np.pi, 0, 0]
         betas_pairs = []
@@ -623,15 +608,14 @@
         assert np.isclose(energy_qiskit, correct_energy)
 
         config_qiskit = [config.tolist() for config in config_qiskit]
 
         assert correct_config in config_qiskit
 
     def test_expectation_w_uncertainty(self):
-
         """
         Test the standard deviation equality. Expectation w uncertainty.
         """
 
         n_qubits = 8
         register = range(n_qubits)
         p = 1
@@ -683,15 +667,14 @@
         # Standard deviation
         exp_2 = np.dot(probs, ham_matrix)
         std_dev2 = np.sqrt(np.dot(probs, ham_matrix_sq) - exp_2**2)
 
         assert np.isclose(exp_unc_qiskit_statevec, std_dev2)
 
     def test_expectation_w_randomizing_variables(self):
-
         """
         Run ntrials sets of randomized input parameters and compares the
         expectation value output between the qiskit statevector simulator and
         vectorized simulator.
         """
 
         ntrials = 100
@@ -702,15 +685,14 @@
             [np.random.rand(), np.random.rand(), np.random.rand(), np.random.rand()]
             for i in range(ntrials)
         ]
         init_hadamards = [np.random.choice([True, False]) for i in range(ntrials)]
         constants = [np.random.rand() for i in range(ntrials)]
 
         for i in range(ntrials):
-
             gammas = [np.random.rand() * np.pi for i in range(p[i])]
             betas = [np.random.rand() * np.pi for i in range(p[i])]
 
             cost_hamil = Hamiltonian(
                 [
                     PauliOp("Z", (0,)),
                     PauliOp("ZZ", (0, 1)),
@@ -736,15 +718,14 @@
                 qaoa_descriptor, None, None, init_hadamards[i]
             )
             vector_expectation = vector_backend.expectation(variate_params)
 
             self.assertAlmostEqual(qiskit_expectation, vector_expectation)
 
     def test_shot_based_simulator(self):
-
         """
         Test get_counts in shot-based qiskit simulator.
         """
 
         nqubits = 3
         p = 1
         weights = [1, 1, 1]
@@ -766,15 +747,14 @@
         )
 
         shot_result = qiskit_shot_backend.get_counts(variate_params)
 
         self.assertEqual(type(shot_result), dict)
 
     def test_cvar_alpha_expectation(self):
-
         """
         Test computing the expectation value by changing the alpha of the cvar.
         """
 
         nqubits = 3
         p = 1
         weights = [1, -1, 1]
@@ -804,15 +784,14 @@
         qiskit_shot_backend.cvar_alpha = 0.75
         expectation_value_075 = qiskit_shot_backend.expectation(variate_params)
         self.assertNotEqual(expectation_value_05, expectation_value_075)
         self.assertEqual(type(float(expectation_value_05)), float)
         self.assertEqual(type(float(expectation_value_075)), float)
 
     def test_standard_decomposition_branch_in_circuit_construction(self):
-
         """
         XY Pauli is not an implemented low level gate. Produces NotImplementedError
         as the standard decomposition for the XY PauliGate doesnt exist.
         """
 
         nqubits = 3
         p = 1
```

### Comparing `openqaoa-0.1.3/tests/test_simulators.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_simulators.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         """
 
         # define problem
         problem = QUBO.random_instance(3)
 
         # loop over all simulators
         for n in SUPPORTED_LOCAL_SIMULATORS:
-
             # initialize
             q = QAOA()
 
             # device
             device = create_device(location="local", name=n)
             q.set_device(device)
```

### Comparing `openqaoa-0.1.3/tests/test_utilities.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         """
 
         # Set of sizes
         sizes = range(1, 10)
 
         # Test for different sizes
         for n_qubits in sizes:
-
             # Define input coefficients
             input_coefficients = [-1 for _ in range(n_qubits)]
 
             # Define mixer Hamiltonian
             mixer_hamiltonian = X_mixer_hamiltonian(n_qubits, input_coefficients)
 
             # Extract mixer Hamiltonian attributes
@@ -80,21 +79,18 @@
         terms_strings = ["XX", "YY"]
 
         # Set of uses
         input_type = ["string", "custom"]
 
         # Test for different sizes
         for n_qubits in sizes:
-
             # Test for different connectivities
             for connectivity in connectivities:
-
                 # Test for different input types
                 for input in input_type:
-
                     # Define connectivity explicit indexing
                     if connectivity == "full":
                         terms_indices = list(itertools.combinations(range(n_qubits), 2))
 
                     elif connectivity == "chain":
                         terms_indices = [(i, i + 1) for i in range(n_qubits - 1)]
 
@@ -170,15 +166,14 @@
         # Define number of qubits
         n_qubits = 10
 
         # Define a qubit connectivity for X, and a connectivity for XY mixers
         connectivities = [None, "star", "full", "chain"]
 
         for connectivity in connectivities:
-
             # Define connectivity explicit indexing
             if connectivity == "full":
                 terms_indices = list(itertools.combinations(range(n_qubits), 2))
                 input_coefficients = 2 * [1 for _ in range(len(terms_indices))]
                 mixer_type = "xy"
 
             elif connectivity == "chain":
@@ -305,15 +300,14 @@
         singlet_edges = [(i,) for i in range(n_qubits)]
         edges = singlet_edges + pair_edges
 
         graph = nx.Graph()
 
         # Populate the graph with weighted nodes and weighted edges
         for edge in edges:
-
             # Weighted node
             if len(edge) == 1:
                 graph.add_node(edge[0], weight=-1)
 
             # Weighted edge
             else:
                 graph.add_edge(edge[0], edge[1], weight=0.5)
@@ -358,20 +352,17 @@
         n_nodes = 6
 
         # Set of degrees
         degrees = [2, 3, 4, 5]
 
         # Check for every degree
         for degree in degrees:
-
             # Check for weighted and unweighted
             for weighted in [False, True]:
-
                 for biases in [False, True]:
-
                     # Generate graph
                     graph = random_k_regular_graph(
                         degree, list(range(n_nodes)), weighted=weighted, biases=biases
                     )
 
                     # Test it has the correct number of edges for a regular graph
                     assert np.allclose(
@@ -393,15 +384,14 @@
         """
 
         # Number of qubits
         sizes = list(range(2, 10))
 
         # Test for different qubit numbers
         for n_qubits in sizes:
-
             hamiltonian = random_classical_hamiltonian(reg=list(range(n_qubits)))
 
             # Test the hamiltonian is a Hamiltonian object
             assert isinstance(
                 hamiltonian, Hamiltonian
             ), f"The object is not Hamiltonian object"
 
@@ -488,15 +478,14 @@
         states = ["0101010101", [1, 0, 1, 0, 1, 0, 1, 0, 1, 0]]
 
         # Correct energies
         correct_energy = -10
 
         # Test for each string
         for state in states:
-
             # Compute energies for the given trial states
             energy = bitstring_energy(hamiltonian, state)
 
             # Test computed solution is correcrt
             assert np.allclose(correct_energy, energy), f"Computed energy is incorrect"
 
     def test_energy_expectation(self):
@@ -699,15 +688,14 @@
         """
 
         # Set of sizes
         sizes = range(3, 10)
 
         # Uniform case
         for n_qubits in sizes:
-
             # Generate ring of disagrees and extract attributes
             rod_hamiltonian = ring_of_disagrees(reg=list(range(n_qubits)))
 
             rod_terms = rod_hamiltonian.terms
             rod_coefficients = rod_hamiltonian.coeffs
             rod_constant = rod_hamiltonian.constant
 
@@ -773,15 +761,14 @@
             (np.pi / 4, np.pi / 4): (0, 0),
             (np.pi / 4, np.pi / 8): (-np.sqrt(2) / 4, -0.25),
             (np.pi / 8, 0): (0, 0),
         }  # (beta,gamma):(exp_val,corr)
 
         # Compute singlet expectation values and correlations for each set of angles
         for qaoa_angles in qaoa_angles_cases.keys():
-
             # Extract correct solution
             exp_val = np.round(qaoa_angles_cases[qaoa_angles][0], 16)
             corr = np.round(qaoa_angles_cases[qaoa_angles][1], 16)
 
             # Compute expectation values and correlations
             comp_exp_val = np.round(
                 exp_val_single_analytical(spin, hamiltonian, qaoa_angles), 16
@@ -814,16 +801,14 @@
             ]
         )
 
         corr_matrix -= np.outer(exp_val_list, exp_val_list)
 
         # Compute list of expectation values and correlation matrix
         comp_exp_val_list, comp_corr_matrix = exp_val_hamiltonian_termwise(
-            variational_params=None,
-            qaoa_backend=None,
             hamiltonian=hamiltonian,
             p=1,
             mixer_type="x",
             qaoa_optimized_angles=fixed_angles,
             analytical=True,
         )
 
@@ -887,28 +872,24 @@
 
         qaoa_results_optimized = qaoa_results.optimized
         qaoa_optimized_angles = qaoa_results_optimized["angles"]
         qaoa_optimized_counts = qaoa_results.get_counts(
             qaoa_results_optimized["measurement_outcomes"]
         )
         num_exp_vals_z, num_corr_matrix = exp_val_hamiltonian_termwise(
-            variational_params,
-            qaoa_backend,
             hamiltonian,
             "x",
             p,
             qaoa_optimized_angles,
             qaoa_optimized_counts,
             analytical=False,
         )
 
         # Analytical expectation values
         exp_vals_z, corr_matrix = exp_val_hamiltonian_termwise(
-            variational_params,
-            qaoa_backend,
             hamiltonian,
             "x",
             p,
             qaoa_optimized_angles,
             qaoa_optimized_counts,
             analytical=True,
         )
@@ -919,14 +900,176 @@
         ), f"Computed singlet expectation values are incorrect"
 
         for j in range(len(num_corr_matrix)):
             assert np.allclose(
                 corr_matrix[j], num_corr_matrix[j]
             ), f"Computed correlation matrix is incorrect"
 
+    def test_calculate_calibration_factors(self):
+        """
+        Tests the function that computes the calibration factors.
+
+        The test consists in creating a simple hamiltonian, and a variety of calibration registers, qubit mappings and calibration measurements for different edge cases. See the comments before every case for more information.
+
+        """
+        # Create a Hamiltonian
+        n_qubits = 4
+        edges = (
+            [(i, i + 1) for i in range(n_qubits - 1)]
+            + [(0, n_qubits - 1)]
+            + [(i,) for i in range(n_qubits)]
+        )
+        weights = [1 for _ in range(len(edges))]
+        hamiltonian = Hamiltonian.classical_hamiltonian(edges, weights, constant=10)
+
+        # Create mock registers and mapping, on a 7 qubits device
+        calibration_registers = [120, 121, 131, 132, 133, 134, 140]
+        qubit_mapping = [131, 132, 133, 134]
+
+        ### no errors, all factors should be equal to 1, i.e. no correction needed
+        calibration_measurements = {"0000000": 100}
+
+        output_calibration_factors = calculate_calibration_factors(
+            hamiltonian, calibration_measurements, calibration_registers, qubit_mapping
+        )
+
+        expected_calibration_factors = {
+            (0, 1): 1.0,
+            (1, 2): 1.0,
+            (2, 3): 1.0,
+            (0, 3): 1.0,
+            (0,): 1.0,
+            (1,): 1.0,
+            (2,): 1.0,
+            (3,): 1.0,
+        }
+
+        assert (
+            output_calibration_factors == expected_calibration_factors
+        ), f"Calibration factors have not been calculated correctly in the absense of errors."
+
+        ### some of the physical qubits always get flipped
+        ##### in this case the physical qubits 131 and 132 where 0 and 1 problem qubits are mapped to
+        ##### note that the flipping of both 0 and 1 cancels, resulting in a calibration factor = 1 for the term [0,1].
+        calibration_measurements = {"0011000": 100}
+
+        output_calibration_factors = calculate_calibration_factors(
+            hamiltonian, calibration_measurements, calibration_registers, qubit_mapping
+        )
+        expected_calibration_factors = {
+            (0, 1): 1.0,
+            (0, 3): -1.0,
+            (1, 2): -1.0,
+            (2, 3): 1.0,
+            (0,): -1.0,
+            (1,): -1.0,
+            (2,): 1.0,
+            (3,): 1.0,
+        }
+
+        assert (
+            output_calibration_factors == expected_calibration_factors
+        ), f"Calibration factors have not been calculated correctly for bit flip errors."
+
+        ### Bit flip errors happen on all qubits vut the ones we embed the problem onto
+        ##### in this example device qubits 120, 121 and 140 are faulty but this should nt affect the rest
+        calibration_measurements = {"1100001": 100}
+
+        output_calibration_factors = calculate_calibration_factors(
+            hamiltonian, calibration_measurements, calibration_registers, qubit_mapping
+        )
+        expected_calibration_factors = {
+            (0, 1): 1.0,
+            (0, 3): 1.0,
+            (1, 2): 1.0,
+            (2, 3): 1.0,
+            (0,): 1.0,
+            (1,): 1.0,
+            (2,): 1.0,
+            (3,): 1.0,
+        }
+
+        assert (
+            output_calibration_factors == expected_calibration_factors
+        ), f"Calibration factors have not been calculated correctly for errors happening on irrelevant qubits."
+
+        ### A bitflip error on the 131 physical register
+        ##### but now the 1st problem qubit has been mapped to register after the routing
+        qubit_mapping = [133, 131, 132, 134]
+        calibration_measurements = {"0010000": 100}
+
+        output_calibration_factors = calculate_calibration_factors(
+            hamiltonian, calibration_measurements, calibration_registers, qubit_mapping
+        )
+
+        expected_calibration_factors = {
+            (0, 1): -1.0,
+            (1, 2): -1.0,
+            (2, 3): 1.0,
+            (0, 3): 1.0,
+            (0,): 1.0,
+            (1,): -1.0,
+            (2,): 1.0,
+            (3,): 1.0,
+        }
+
+        assert (
+            output_calibration_factors == expected_calibration_factors
+        ), f"Calibration factors have not been calculated correctly when routed."
+
+        ### A bitflip error happen with probability 0.25 on the 131 and 132 physical registers
+        ##### which results in more entries in the measurements dict
+        ##### and affects the 0th and 1st problem qubits
+        qubit_mapping = [133, 131, 132, 134]
+        calibration_measurements = {
+            "0000000": 10000 * 0.75 * 0.75,
+            "0001000": 10000 * 0.25 * 0.75,
+            "0010000": 10000 * 0.75 * 25,
+            "0011000": 10000 * 0.25 * 0.25,
+        }
+
+        output_calibration_factors = calculate_calibration_factors(
+            hamiltonian, calibration_measurements, calibration_registers, qubit_mapping
+        )
+
+        expected_calibration_factors = {
+            (0, 1): -0.923322683706,
+            (1, 2): -0.936102236422,
+            (2, 3): 0.974440894569,
+            (0, 3): 1.0,
+            (0,): 1.0,
+            (1,): -0.923322683706,
+            (2,): 0.974440894569,
+            (3,): 1.0,
+        }
+
+        assert (
+            output_calibration_factors == expected_calibration_factors
+        ), f"Calibration factors have not been calculated correctly in the presense of probabalistic errors."
+
+        ### Calibration factors are 0 as a result of a faulty measurement (probability of an error is 0.5)
+        ##### Raise a ValueError
+        calibration_measurements = {
+            "0000000": 10000 * 0.5,
+            "0001000": 10000 * 0.5,
+        }
+
+        exception = False
+        try:
+            output_calibration_factors = calculate_calibration_factors(
+                hamiltonian,
+                calibration_measurements,
+                calibration_registers,
+                qubit_mapping,
+            )
+        except:
+            exception = True
+
+        assert exception, "Calibration factors 0 didn't fail"
+
     def test_energy_expectation_analytical(self):
         """
         Tests the function that computed the expectation value of the Hamiltonian from an
         analytical function valid for a single layer QAOA Ansatz with the X mixer.
 
         The test consists in computing the expectation value of an example Hamiltonian for different angles.
         """
@@ -1059,15 +1202,14 @@
                 "110": 0,
                 "111": 0,
             },
         ]
 
         # Test that each probability dictionary has been generated correctly
         for idx, prob_dict in enumerate(prob_dicts):
-
             # Check each string has the same probability associated
             for string in prob_dict.keys():
                 assert np.allclose(
                     prob_dicts[idx][string], correct_prob_dicts[idx][string]
                 ), f"Probablity have not been generated correctly"
 
     def test_delete_keys_from_dict(self):
@@ -1202,15 +1344,15 @@
 
         # Test that the uuid has been generated correctly
         assert is_valid_uuid(generated_uuid), f"UUID has not been generated correctly"
 
     def test_generate_timestamp(self):
         """
         Tests the function that generates a timestamp: generate_timestamp.
-        It checks if the reutned string is a valid timestamp of format YYYY-MM-DDTHH:MM:SS.
+        It checks if the returned string is a valid timestamp of format YYYY-MM-DDTHH:MM:SS.
         """
 
         def is_valid_timestamp(s):
             try:
                 datetime.datetime.strptime(s, "%Y-%m-%dT%H:%M:%S")
                 return True
             except ValueError:
@@ -1241,10 +1383,29 @@
         expected_dict = {"110011": 1, "111000": 2, "000000": 3}
 
         # Test that the dictionary has been permuted correctly
         assert (
             output_dict == expected_dict
         ), f"Dictionary has not been permuted correctly"
 
+    def test_negate_counts_dictionary(self):
+        """
+        Tests the function that negates the counts dictionary used for SPAM Twirling.
+
+        13 => 001101 in binary => negate the 3rd, 4th, and 6th qubit
+        """
+        # Input dictionary
+        input_dict = {"011011": 1, "000111": 2, "000000": 3}
+
+        # Expected dictionary
+        expected_dict = {"010110": 1, "001010": 2, "001101": 3}
+
+        output_dict = negate_counts_dictionary(input_dict, s=13)
+
+        # Test that the dictionary has been permuted correctly
+        assert (
+            output_dict == expected_dict
+        ), f"Dictionary has not been negated correctly"
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.3/tests/test_vectorized.py` & `openqaoa-0.1.3rc1/src/openqaoa-core/tests/test_vectorized.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,29 +78,27 @@
 
 class TestingQAOAvectorizedBackend(unittest.TestCase):
     """
     Unittest based testing of QAOACostVector
     """
 
     def test_permute(self):
-
         nqubits = 3
 
         arr = np.arange(2**nqubits)
         arr.shape = [2] * nqubits
         # reshaped_arr = backend._reshape_qubits(nqubits, arr)
         perm = [2, 0, 1]
         permuted_arr = _permute_qubits(arr, perm)
 
         expected_arr = np.array([[[0, 2], [4, 6]], [[1, 3], [5, 7]]])
 
         assert np.array_equal(permuted_arr, expected_arr)
 
     def test_get_perm(self):
-
         nqubits = 4
 
         perm1, perminv1 = _get_perm(nqubits, [1, 3])
         perm2, perminv2 = _get_perm(nqubits, [0, 2])
 
         perm1_expected = np.array([2, 0, 1, 3])
         perminv1_expected = np.array([1, 2, 0, 3])
@@ -114,15 +112,14 @@
         assert np.array_equal(perminv2, perminv2_expected)
 
     ##########################################################
     # TESTS OF BASIC CIRCUIT OPERATIONS (SAME AS FOR PROJECTQ)
     ##########################################################
 
     def test_qaoa_circuit(self):
-
         # Test circuit with p = 1 on 3 qubits
         # Performs a round of ZZ rotations through pi, and a round of X mixer rotations through pi
         nqubits = 3
         register = [i for i in range(nqubits)]
         p = 1
         bias_qubits = []
         bias_angles = []
@@ -148,15 +145,14 @@
         wf = wf / wf[0]
 
         expected_wf = np.array([1, 1, 1, 1, 1, 1, 1, 1])
 
         assert np.allclose(wf, expected_wf)
 
     def test_wavefunction_single_terms(self):
-
         # Test wavefunction and expectation values with hamiltonian object, without 2-qubit terms
         cost_hamil = Hamiltonian([PauliOp("Z", (0,)), PauliOp("Z", (1,))], [1, 1], 1)
         mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=1)
         variate_params = create_qaoa_variational_params(
             qaoa_descriptor, "standard", "ramp"
         )
@@ -165,15 +161,14 @@
         args = [np.pi / 4, np.pi / 4]  # beta, gamma
         variate_params.update_from_raw(args)
 
         assert np.allclose(backend_obj.wavefunction(variate_params), [0, 0, 0, 1j])
         assert np.isclose(backend_obj.expectation(variate_params), -1)
 
     def test_wavefunction(self):
-
         nqubits = 3
 
         # Test circuit with p = 1 on 3 qubits
         terms = [[0, 1], [0, 2], [0]]
         weights = [1, 1, -0.5]
         register = [0, 1, 2]
         p = 1
@@ -209,15 +204,14 @@
 
         expected_wf = -1j * np.array([-1, 1, 1, -1, 1, -1, -1, 1]) / (2 * np.sqrt(2))
 
         assert np.allclose(wf, direct_wf)
         assert np.allclose(wf, expected_wf)
 
     def test_execute_exp_val(self):
-
         n_qubits = 8
         register, cost_hamil, qaoa_descriptor, variate_params = Disagrees_SetUp(
             n_qubits
         )
 
         backend_vectorized = QAOAvectorizedBackendSimulator(
             qaoa_descriptor, prepend_state=None, append_state=None, init_hadamard=True
@@ -278,15 +272,14 @@
         )
 
         exp_vec = backend_vectorized.expectation(variational_params_std)
 
         assert np.isclose(exp_vec, -6)
 
     def test_get_wavefunction(self):
-
         n_qubits = 3
         terms = [[0, 1], [0, 2], [0]]
         weights = [1, 1, -0.5]
         p = 1
 
         betas_singles = [np.pi, 0, 0]
         betas_pairs = []
@@ -363,15 +356,14 @@
 
         assert correct_config in config_vec
 
     def test_afunction_throws_exception(self):
         # Make sure that exception is raised when Hamiltonian contains nonclassical (non-Z or ZZ terms)
 
         def test_nonclassical_hamiltonian_error():
-
             cost_hamil = Hamiltonian(
                 [PauliOp("Y", (0,)), PauliOp("Z", (1,))], [1, 1], 1
             )
             mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
             qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=1)
             variate_params = create_qaoa_variational_params(
                 qaoa_descriptor, "standard", "ramp"
@@ -383,15 +375,14 @@
         self.assertRaises(Exception, test_nonclassical_hamiltonian_error)
 
     ##########################################################
     # TESTS OF APPLY GATE METHODS
     ##########################################################
 
     def test_apply_rx(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rx method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -405,15 +396,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_ry(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_ry method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -427,15 +417,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rz(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rz method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -449,15 +438,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rxx(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rxx method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -471,15 +459,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_ryy(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_ryy method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -493,15 +480,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rzz(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rzz method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -515,15 +501,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rzx(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rzx method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -537,15 +522,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rxz(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rxz method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -559,15 +543,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rxy(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_rxy method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -581,15 +564,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_ryx(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_ryx method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -603,15 +585,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_ryz(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_ryz method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
@@ -625,15 +606,14 @@
             res_wfn = np.matmul(unitary, wavefn).reshape([2] * n_qubits)
 
             assert np.allclose(
                 vector_backend.wavefn, res_wfn
             ), f"angle = {angle} failed, {vector_backend.wavefn} != {res_wfn}"
 
     def test_apply_rzy(self):
-
         constI, constX, constY, constZ = pauli_matrix_SetUp()
 
         # Result from apply_ryz method
         angles = [0.1, np.pi / 2, np.pi / 4]
 
         for angle in angles:
             n_qubits, vector_backend = apply_gate_problem_SetUp()
```

