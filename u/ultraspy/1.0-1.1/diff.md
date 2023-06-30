# Comparing `tmp/ultraspy-1.0.tar.gz` & `tmp/ultraspy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultraspy-1.0.tar", last modified: Wed Jun  7 12:52:52 2023, max compression
+gzip compressed data, was "ultraspy-1.1.tar", last modified: Fri Jun 30 16:46:58 2023, max compression
```

## Comparing `ultraspy-1.0.tar` & `ultraspy-1.1.tar`

### file list

```diff
@@ -1,461 +1,632 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:52.008041 ultraspy-1.0/
--rw-rw-rw-   0        0        0      256 2023-06-07 09:00:51.000000 ultraspy-1.0/.readthedocs.yml
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.766073 ultraspy-1.0/.tox/docs/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.767591 ultraspy-1.0/.tox/docs/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.771598 ultraspy-1.0/.tox/docs/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.767591 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.905684 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.767591 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.929788 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.767591 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.935372 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-07 10:50:22.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.949459 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-07 10:49:44.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-07 10:49:44.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.955547 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-07 10:49:45.000000 ultraspy-1.0/.tox/docs/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/py310-cpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.776332 ultraspy-1.0/.tox/py310-cpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.780477 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.780477 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.957559 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.780477 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.966077 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.780477 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.969587 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-06 15:39:23.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.784487 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.784487 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.973595 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-06 15:38:45.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-06 15:38:45.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.975607 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-06 15:38:46.000000 ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/py38-cpu_tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.785499 ultraspy-1.0/.tox/py38-cpu_tests/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.789837 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.788549 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.977660 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.789837 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.986172 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.789837 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.989680 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-07 10:42:48.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.792846 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.789837 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.789837 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.993688 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-07 10:42:10.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-07 10:42:10.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.792846 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.792846 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.995695 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-07 10:42:11.000000 ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
--rw-rw-rw-   0        0        0       68 2022-08-03 15:17:56.000000 ultraspy-1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0       90 2023-06-07 11:12:32.000000 ultraspy-1.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2367 2023-04-20 15:30:24.000000 ultraspy-1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1091 2022-06-22 12:40:44.000000 ultraspy-1.0/LICENSE
--rw-rw-rw-   0        0        0      278 2023-04-20 15:30:24.000000 ultraspy-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3545 2023-06-07 12:52:52.008041 ultraspy-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2023-06-07 11:18:20.000000 ultraspy-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.001737 ultraspy-1.0/docs/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.001737 ultraspy-1.0/docs/_static/
--rw-rw-rw-   0        0        0      235 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/_static/custom.css
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.032444 ultraspy-1.0/docs/algorithms/
--rw-rw-rw-   0        0        0     3530 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/algorithms/das_algo.rst
--rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/algorithms/fdmas_algo.rst
--rw-rw-rw-   0        0        0      187 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/algorithms/index.rst
--rw-rw-rw-   0        0        0     2452 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/algorithms/pdas_algo.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.070102 ultraspy-1.0/docs/api_references/
--rw-rw-rw-   0        0        0      488 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/api_references/beamformers.rst
--rw-rw-rw-   0        0        0      905 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/api_references/classes.rst
--rw-rw-rw-   0        0        0       94 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/api_references/gpu_utils.rst
--rw-rw-rw-   0        0        0      143 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/api_references/index.rst
--rw-rw-rw-   0        0        0       88 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/api_references/metrics.rst
--rw-rw-rw-   0        0        0     1624 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/api_references/ultraspy.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.117390 ultraspy-1.0/docs/architecture/
--rw-rw-rw-   0        0        0    11787 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/architecture/beamformer_class.rst
--rw-rw-rw-   0        0        0     4254 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/architecture/common_methods.rst
--rw-rw-rw-   0        0        0     1987 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/architecture/index.rst
--rw-rw-rw-   0        0        0      421 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/architecture/probe_class.rst
--rw-rw-rw-   0        0        0       65 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/architecture/reader_class.rst
--rw-rw-rw-   0        0        0       60 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/architecture/scan_class.rst
--rw-rw-rw-   0        0        0     2750 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.155722 ultraspy-1.0/docs/contribute/
--rw-rw-rw-   0        0        0     2037 2023-06-07 11:48:18.000000 ultraspy-1.0/docs/contribute/devops_routine.rst
--rw-rw-rw-   0        0        0      625 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/index.rst
--rw-rw-rw-   0        0        0     3923 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/own_beamformer.rst
--rw-rw-rw-   0        0        0      677 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/own_methods.rst
--rw-rw-rw-   0        0        0      911 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/own_setups_options.rst
--rw-rw-rw-   0        0        0     2456 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/preparation.rst
--rw-rw-rw-   0        0        0     1594 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/contribute/tdd.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.197526 ultraspy-1.0/docs/examples/
--rw-rw-rw-   0        0        0     9976 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/examples/das.rst
--rw-rw-rw-   0        0        0     6125 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/examples/doppler.rst
--rw-rw-rw-   0        0        0      327 2023-06-07 09:00:51.000000 ultraspy-1.0/docs/examples/index.rst
--rw-rw-rw-   0        0        0    12052 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/examples/metrics.rst
--rw-rw-rw-   0        0        0     7211 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/examples/simu_data.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.241735 ultraspy-1.0/docs/images/
--rw-rw-rw-   0        0        0    34289 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/block_grid.png
--rw-rw-rw-   0        0        0   132410 2023-01-25 18:21:44.000000 ultraspy-1.0/docs/images/convex_delays.png
--rw-rw-rw-   0        0        0   114606 2023-01-25 18:21:44.000000 ultraspy-1.0/docs/images/convex_probe.png
--rw-rw-rw-   0        0        0    35256 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/das_algo.png
--rw-rw-rw-   0        0        0    32371 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/das_bmode.png
--rw-rw-rw-   0        0        0    54387 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/das_dam.png
--rw-rw-rw-   0        0        0   229452 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/images/doppler.png
--rw-rw-rw-   0        0        0    87019 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/fdmas_optim_gpu.png
--rw-rw-rw-   0        0        0   180354 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/fdmas_spectra.png
--rw-rw-rw-   0        0        0    12459 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/fnumber.png
--rw-rw-rw-   0        0        0    99220 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/gpu_architecture.png
--rw-rw-rw-   0        0        0    87661 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/interpolation_beamforming.png
--rw-rw-rw-   0        0        0    66458 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_lobes.png
--rw-rw-rw-   0        0        0    31442 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_lobes_axial.png
--rw-rw-rw-   0        0        0    46092 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_lobes_lateral.png
--rw-rw-rw-   0        0        0    51462 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_masks.png
--rw-rw-rw-   0        0        0    74436 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_raw_data.png
--rw-rw-rw-   0        0        0    41500 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_snr_correct.png
--rw-rw-rw-   0        0        0    31289 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_snr_wrong.png
--rw-rw-rw-   0        0        0   260166 2022-08-03 15:17:56.000000 ultraspy-1.0/docs/images/metrics_spectra.png
--rw-rw-rw-   0        0        0   299480 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/images/pdas_spectra.png
--rw-rw-rw-   0        0        0    24721 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/images/polar_system.png
--rw-rw-rw-   0        0        0   114889 2023-04-20 15:30:24.000000 ultraspy-1.0/docs/images/ultraspy_classes.png
--rw-rw-rw-   0        0        0     2701 2023-06-07 11:21:30.000000 ultraspy-1.0/docs/index.rst
--rw-rw-rw-   0        0        0     4063 2023-06-07 11:21:30.000000 ultraspy-1.0/docs/installation.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.274448 ultraspy-1.0/docs/tech_choices/
--rw-rw-rw-   0        0        0     3692 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/tech_choices/beamforming_choices.rst
--rw-rw-rw-   0        0        0     2436 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/tech_choices/gpu_beamformers.rst
--rw-rw-rw-   0        0        0     5834 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/tech_choices/gpu_configs.rst
--rw-rw-rw-   0        0        0      248 2023-04-26 14:04:14.000000 ultraspy-1.0/docs/tech_choices/index.rst
--rw-rw-rw-   0        0        0      110 2023-04-20 15:30:24.000000 ultraspy-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 12:52:52.008041 ultraspy-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-06-07 11:13:48.000000 ultraspy-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.275513 ultraspy-1.0/src/
--rw-rw-rw-   0        0        0        0 2022-06-22 12:40:44.000000 ultraspy-1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.325343 ultraspy-1.0/src/ultraspy/
--rw-rw-rw-   0        0        0      892 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/TODO.md
--rw-rw-rw-   0        0        0     1068 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.447873 ultraspy-1.0/src/ultraspy/beamformers/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/beamformers/__init__.py
--rw-rw-rw-   0        0        0    30358 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/beamformers/beamformer.py
--rw-rw-rw-   0        0        0    17908 2023-06-06 13:22:47.000000 ultraspy-1.0/src/ultraspy/beamformers/das.py
--rw-rw-rw-   0        0        0    26096 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/beamformers/fdmas.py
--rw-rw-rw-   0        0        0     2381 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/beamformers/options.py
--rw-rw-rw-   0        0        0    22921 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/beamformers/pdas.py
--rw-rw-rw-   0        0        0     1105 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/beamformers/setups.py
--rw-rw-rw-   0        0        0      786 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/config.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.519810 ultraspy-1.0/src/ultraspy/cpu/
--rw-rw-rw-   0        0        0      642 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/cpu/__init__.py
--rw-rw-rw-   0        0        0     2702 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/display.py
--rw-rw-rw-   0        0        0     9390 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/cpu/doppler.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.800876 ultraspy-1.0/src/ultraspy/cpu/kernels/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.591697 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/__init__.py
--rw-rw-rw-   0        0        0     2804 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py
--rw-rw-rw-   0        0        0     1960 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/apodization.py
--rw-rw-rw-   0        0        0    13231 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/das.py
--rw-rw-rw-   0        0        0    16093 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/fdmas.py
--rw-rw-rw-   0        0        0     1808 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/interpolation.py
--rw-rw-rw-   0        0        0      457 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/maths_utils.py
--rw-rw-rw-   0        0        0    15618 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/pdas.py
--rw-rw-rw-   0        0        0     1133 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.651911 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/__init__.py
--rw-rw-rw-   0        0        0     2117 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py
--rw-rw-rw-   0        0        0     5983 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/das.py
--rw-rw-rw-   0        0        0     8235 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py
--rw-rw-rw-   0        0        0     5075 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py
--rw-rw-rw-   0        0        0     8892 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/pdas.py
--rw-rw-rw-   0        0        0     1097 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py
--rw-rw-rw-   0        0        0     2663 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/cpu/post_processing.py
--rw-rw-rw-   0        0        0     7395 2023-04-26 16:33:32.000000 ultraspy-1.0/src/ultraspy/cpu/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.719137 ultraspy-1.0/src/ultraspy/gpu/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/display.py
--rw-rw-rw-   0        0        0    12887 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/doppler.py
--rw-rw-rw-   0        0        0     3032 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/gpu_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.793648 ultraspy-1.0/src/ultraspy/gpu/kernels/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.861616 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/
--rw-rw-rw-   0        0        0     1742 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
--rw-rw-rw-   0        0        0     2656 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/apodization.cu
--rw-rw-rw-   0        0        0    18518 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/das.cu
--rw-rw-rw-   0        0        0    22384 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/fdmas.cu
--rw-rw-rw-   0        0        0     4039 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/interpolation.cu
--rw-rw-rw-   0        0        0    23418 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/pdas.cu
--rw-rw-rw-   0        0        0     2435 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu
--rw-rw-rw-   0        0        0     4641 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
--rw-rw-rw-   0        0        0     2298 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.893705 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/
--rw-rw-rw-   0        0        0     1600 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/color_map.cu
--rw-rw-rw-   0        0        0     2188 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
--rw-rw-rw-   0        0        0     3096 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
--rw-rw-rw-   0        0        0     4122 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
--rw-rw-rw-   0        0        0     1558 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/power_map.cu
--rw-rw-rw-   0        0        0     3749 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/doppler_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.897747 ultraspy-1.0/src/ultraspy/gpu/kernels/headers/
--rw-rw-rw-   0        0        0      124 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/headers/cupy_header.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.957525 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/
--rw-rw-rw-   0        0        0     1737 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/by2.cu
--rw-rw-rw-   0        0        0     7248 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/convolve.cu
--rw-rw-rw-   0        0        0     1681 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/divide_by.cu
--rw-rw-rw-   0        0        0     8193 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/flip.cu
--rw-rw-rw-   0        0        0     1274 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/get_modulo.cu
--rw-rw-rw-   0        0        0     3695 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/median_filter.cu
--rw-rw-rw-   0        0        0     1552 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators/to_db.cu
--rw-rw-rw-   0        0        0     4802 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/operators_kernels.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.009758 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/
--rw-rw-rw-   0        0        0     2288 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/down_mix.cu
--rw-rw-rw-   0        0        0     4618 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/filter0.cu
--rw-rw-rw-   0        0        0     2460 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_end_sig.cu
--rw-rw-rw-   0        0        0     2906 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_filter.cu
--rw-rw-rw-   0        0        0     2512 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_start_sig.cu
--rw-rw-rw-   0        0        0     2432 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/signal_kernels.py
--rw-rw-rw-   0        0        0     3413 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/kernels/utils.py
--rw-rw-rw-   0        0        0     2801 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/gpu/post_processing.py
--rw-rw-rw-   0        0        0    12741 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/gpu/signal.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.073759 ultraspy-1.0/src/ultraspy/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/helpers/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/helpers/doppler_helpers.py
--rw-rw-rw-   0        0        0     4037 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/helpers/metrics_helpers.py
--rw-rw-rw-   0        0        0     6240 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/helpers/signal_helpers.py
--rw-rw-rw-   0        0        0     3816 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/helpers/transmit_delays_helpers.py
--rw-rw-rw-   0        0        0      530 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/helpers/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.085364 ultraspy-1.0/src/ultraspy/io/
--rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.145629 ultraspy-1.0/src/ultraspy/io/file_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/factory.py
--rw-rw-rw-   0        0        0     1267 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/file_loader.py
--rw-rw-rw-   0        0        0     1922 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/h5_loader.py
--rw-rw-rw-   0        0        0     2063 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/mat_loader.py
--rw-rw-rw-   0        0        0     7828 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/file_loaders/rff256_loader.py
--rw-rw-rw-   0        0        0    23998 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/io/reader.py
--rw-rw-rw-   0        0        0    15946 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.193545 ultraspy-1.0/src/ultraspy/probes/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/probes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.221702 ultraspy-1.0/src/ultraspy/probes/configs/
--rw-rw-rw-   0        0        0      182 2023-01-25 18:21:44.000000 ultraspy-1.0/src/ultraspy/probes/configs/c5-2v.ini
--rw-rw-rw-   0        0        0      164 2023-01-25 18:21:44.000000 ultraspy-1.0/src/ultraspy/probes/configs/l11-4v.ini
--rw-rw-rw-   0        0        0      165 2023-01-25 18:21:44.000000 ultraspy-1.0/src/ultraspy/probes/configs/l11-5v.ini
--rw-rw-rw-   0        0        0      170 2023-01-25 18:21:44.000000 ultraspy-1.0/src/ultraspy/probes/configs/l14-5w.ini
--rw-rw-rw-   0        0        0      160 2023-01-25 18:21:44.000000 ultraspy-1.0/src/ultraspy/probes/configs/l7-4.ini
--rw-rw-rw-   0        0        0      198 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/probes/configs/mux_1024_8MHz.ini
--rw-rw-rw-   0        0        0      164 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/probes/configs/p4-2v.ini
--rw-rw-rw-   0        0        0     2635 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/probes/convex_probe.py
--rw-rw-rw-   0        0        0     5082 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/probes/factory.py
--rw-rw-rw-   0        0        0     1571 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/probes/linear_probe.py
--rw-rw-rw-   0        0        0     2344 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/probes/matricial_probe.py
--rw-rw-rw-   0        0        0     8325 2023-04-26 14:04:14.000000 ultraspy-1.0/src/ultraspy/probes/probe.py
--rw-rw-rw-   0        0        0    17720 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/scan.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.275525 ultraspy-1.0/src/ultraspy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/__init__.py
--rw-rw-rw-   0        0        0      585 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/beamformers.py
--rw-rw-rw-   0        0        0     3648 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/linear_decomposition.py
--rw-rw-rw-   0        0        0     2331 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/masks.py
--rw-rw-rw-   0        0        0     1292 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/matplot.py
--rw-rw-rw-   0        0        0     3336 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/print.py
--rw-rw-rw-   0        0        0      495 2023-06-07 09:00:51.000000 ultraspy-1.0/src/ultraspy/utils/scan.py
--rw-rw-rw-   0        0        0      711 2023-04-20 15:30:24.000000 ultraspy-1.0/src/ultraspy/utils/string.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:50.356053 ultraspy-1.0/src/ultraspy.egg-info/
--rw-rw-rw-   0        0        0     3545 2023-06-07 12:52:44.000000 ultraspy-1.0/src/ultraspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14882 2023-06-07 12:52:49.000000 ultraspy-1.0/src/ultraspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:52:44.000000 ultraspy-1.0/src/ultraspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-07 12:52:44.000000 ultraspy-1.0/src/ultraspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 12:52:44.000000 ultraspy-1.0/src/ultraspy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.281559 ultraspy-1.0/tests/
--rw-rw-rw-   0        0        0     6137 2023-06-07 09:02:02.000000 ultraspy-1.0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.337663 ultraspy-1.0/tests/test_cpu/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.375527 ultraspy-1.0/tests/test_cpu/beamformers/
--rw-rw-rw-   0        0        0     7493 2023-06-07 09:00:51.000000 ultraspy-1.0/tests/test_cpu/beamformers/test_beamformer.py
--rw-rw-rw-   0        0        0    51386 2023-06-07 09:00:51.000000 ultraspy-1.0/tests/test_cpu/beamformers/test_das.py
--rw-rw-rw-   0        0        0    14986 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/beamformers/test_fdmas.py
--rw-rw-rw-   0        0        0    18333 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/beamformers/test_pdas.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.401851 ultraspy-1.0/tests/test_cpu/helpers/
--rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/helpers/test_doppler_helpers.py
--rw-rw-rw-   0        0        0      674 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/helpers/test_signal_helpers.py
--rw-rw-rw-   0        0        0      295 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/helpers/test_transmit_delays_helpers.py
--rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/helpers/test_windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.409404 ultraspy-1.0/tests/test_cpu/io/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.429578 ultraspy-1.0/tests/test_cpu/io/file_loaders/
--rw-rw-rw-   0        0        0      183 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/io/file_loaders/test_h5_loaders.py
--rw-rw-rw-   0        0        0      191 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/io/file_loaders/test_mat_loader.py
--rw-rw-rw-   0        0        0      203 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/io/file_loaders/test_rff256_loader.py
--rw-rw-rw-   0        0        0     1453 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/io/test_reader.py
--rw-rw-rw-   0        0        0    11386 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/test_doppler.py
--rw-rw-rw-   0        0        0     8264 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_cpu/test_metrics.py
--rw-rw-rw-   0        0        0     1093 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/test_post_processing.py
--rw-rw-rw-   0        0        0     1074 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/test_probes.py
--rw-rw-rw-   0        0        0     4333 2023-06-07 09:00:51.000000 ultraspy-1.0/tests/test_cpu/test_scan.py
--rw-rw-rw-   0        0        0     6287 2023-04-26 16:33:32.000000 ultraspy-1.0/tests/test_cpu/test_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.458110 ultraspy-1.0/tests/test_cpu/utils/
--rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/utils/test_linear_decomposition.py
--rw-rw-rw-   0        0        0     1478 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/utils/test_masks.py
--rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/utils/test_print_utils.py
--rw-rw-rw-   0        0        0      261 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/utils/test_scans_utils.py
--rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_cpu/utils/test_string.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.501502 ultraspy-1.0/tests/test_gpu/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.537869 ultraspy-1.0/tests/test_gpu/beamformers/
--rw-rw-rw-   0        0        0     6486 2023-06-07 09:00:51.000000 ultraspy-1.0/tests/test_gpu/beamformers/test_beamformer.py
--rw-rw-rw-   0        0        0    16206 2023-06-07 09:00:51.000000 ultraspy-1.0/tests/test_gpu/beamformers/test_das.py
--rw-rw-rw-   0        0        0     7610 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_gpu/beamformers/test_fdmas.py
--rw-rw-rw-   0        0        0     6963 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_gpu/beamformers/test_pdas.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.546373 ultraspy-1.0/tests/test_gpu/helpers/
--rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/helpers/test_doppler_helpers.py
--rw-rw-rw-   0        0        0      872 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/helpers/test_signal_helpers.py
--rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/helpers/test_windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.576170 ultraspy-1.0/tests/test_gpu/kernels/
--rw-rw-rw-   0        0        0      112 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/kernels/test_beamformers_kernels.py
--rw-rw-rw-   0        0        0     4328 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/kernels/test_doppler_kernels.py
--rw-rw-rw-   0        0        0     8108 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/kernels/test_operators_kernels.py
--rw-rw-rw-   0        0        0     3203 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/kernels/test_signal_kernels.py
--rw-rw-rw-   0        0        0      248 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/test_display.py
--rw-rw-rw-   0        0        0     4997 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/test_doppler.py
--rw-rw-rw-   0        0        0     3960 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_gpu/test_filtfilts.py
--rw-rw-rw-   0        0        0     1881 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/test_gpu_utils.py
--rw-rw-rw-   0        0        0      176 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/test_post_processing.py
--rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.0/tests/test_gpu/test_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.582723 ultraspy-1.0/tests/test_gpu/utils/
--rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/utils/test_linear_decomposition.py
--rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/utils/test_print_utils.py
--rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.0/tests/test_gpu/utils/test_string_utils.py
--rw-rw-rw-   0        0        0      797 2023-06-07 10:52:39.000000 ultraspy-1.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.825507 ultraspy-1.0/venv/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.825507 ultraspy-1.0/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.849955 ultraspy-1.0/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.835683 ultraspy-1.0/venv/Lib/site-packages/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.825507 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.825507 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.833656 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.833656 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.829615 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.607401 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
--rw-rw-rw-   0        0        0    11047 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
--rw-rw-rw-   0        0        0     9934 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
--rw-rw-rw-   0        0        0    11663 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
--rw-rw-rw-   0        0        0     1611 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.676350 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
--rw-rw-rw-   0        0        0     8406 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
--rw-rw-rw-   0        0        0     8480 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
--rw-rw-rw-   0        0        0     8529 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
--rw-rw-rw-   0        0        0     6005 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
--rw-rw-rw-   0        0        0     6193 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
--rw-rw-rw-   0        0        0     8389 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
--rw-rw-rw-   0        0        0     8452 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
--rw-rw-rw-   0        0        0     7714 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
--rw-rw-rw-   0        0        0    13661 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.692883 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.711726 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
--rw-rw-rw-   0        0        0    38255 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
--rw-rw-rw-   0        0        0    97459 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
--rw-rw-rw-   0        0        0    22413 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
--rw-rw-rw-   0        0        0    31573 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.879438 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/
--rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
--rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
--rw-rw-rw-   0        0        0    17023 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
--rw-rw-rw-   0        0        0     9933 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
--rw-rw-rw-   0        0        0    20045 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
--rw-rw-rw-   0        0        0    26109 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
--rw-rw-rw-   0        0        0    27450 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
--rw-rw-rw-   0        0        0    35739 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
--rw-rw-rw-   0        0        0    71982 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
--rw-rw-rw-   0        0        0    47767 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
--rw-rw-rw-   0        0        0    51261 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
--rw-rw-rw-   0        0        0    31216 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
--rw-rw-rw-   0        0        0    32082 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
--rw-rw-rw-   0        0        0    34615 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
--rw-rw-rw-   0        0        0    38679 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
--rw-rw-rw-   0        0        0    22169 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
--rw-rw-rw-   0        0        0     5284 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
--rw-rw-rw-   0        0        0    26354 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
--rw-rw-rw-   0        0        0    28026 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
--rw-rw-rw-   0        0        0    21011 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.887491 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
--rw-rw-rw-   0        0        0    28426 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.899517 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/
--rw-rw-rw-   0        0        0    42322 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.919597 ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/
--rw-rw-rw-   0        0        0    31907 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu
--rw-rw-rw-   0        0        0     2900 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
--rw-rw-rw-   0        0        0    18156 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.927736 ultraspy-1.0/venv/Lib/site-packages/cupy/random/
--rw-rw-rw-   0        0        0    29209 2023-02-22 11:49:00.000000 ultraspy-1.0/venv/Lib/site-packages/cupy/random/cupy_distributions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.835683 ultraspy-1.0/venv/Lib/site-packages/numba/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.931743 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/
--rw-rw-rw-   0        0        0     1000 2023-06-02 15:39:03.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.837710 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.945338 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/
--rw-rw-rw-   0        0        0      299 2023-06-02 15:39:04.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
--rw-rw-rw-   0        0        0      145 2023-06-02 15:39:04.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/error.cu
--rw-rw-rw-   0        0        0      564 2023-06-02 15:39:04.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
--rw-rw-rw-   0        0        0      179 2023-06-02 15:39:04.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.837710 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.947860 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      926 2023-06-02 15:39:04.000000 ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/numpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.837710 ultraspy-1.0/venv/Lib/site-packages/numpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.837710 ultraspy-1.0/venv/Lib/site-packages/numpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.951868 ultraspy-1.0/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-02 15:39:09.000000 ultraspy-1.0/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-02 15:39:09.000000 ultraspy-1.0/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/numpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/numpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.955383 ultraspy-1.0/venv/Lib/site-packages/numpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-02 15:39:10.000000 ultraspy-1.0/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/~-mpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/~-mpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.841717 ultraspy-1.0/venv/Lib/site-packages/~-mpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.959395 ultraspy-1.0/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-06-02 15:35:42.000000 ultraspy-1.0/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-06-02 15:35:42.000000 ultraspy-1.0/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.845717 ultraspy-1.0/venv/Lib/site-packages/~-mpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.845717 ultraspy-1.0/venv/Lib/site-packages/~-mpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.963395 ultraspy-1.0/venv/Lib/site-packages/~-mpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-06-02 15:35:43.000000 ultraspy-1.0/venv/Lib/site-packages/~-mpy/typing/tests/data/mypy.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.845717 ultraspy-1.0/venv/Lib/site-packages/~umba/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.845717 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.849955 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.845717 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.991555 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/
--rw-rw-rw-   0        0        0      294 2022-08-02 14:53:44.000000 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/cuda_include.cu
--rw-rw-rw-   0        0        0      138 2022-08-02 14:53:44.000000 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/error.cu
--rw-rw-rw-   0        0        0      214 2022-08-02 14:53:44.000000 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/jitlink.cu
--rw-rw-rw-   0        0        0      172 2022-08-02 14:53:44.000000 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/warn.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.849955 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:51.995557 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/
--rw-rw-rw-   0        0        0      292 2022-08-02 14:53:44.000000 ultraspy-1.0/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/functions.cu
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.853958 ultraspy-1.0/venv/Lib/site-packages/~umpy/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.853958 ultraspy-1.0/venv/Lib/site-packages/~umpy/core/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.853958 ultraspy-1.0/venv/Lib/site-packages/~umpy/core/lib/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:52.004004 ultraspy-1.0/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/
--rw-rw-rw-   0        0        0      151 2023-05-03 12:33:57.000000 ultraspy-1.0/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/mlib.ini
--rw-rw-rw-   0        0        0      380 2023-05-03 12:33:57.000000 ultraspy-1.0/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/npymath.ini
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.855464 ultraspy-1.0/venv/Lib/site-packages/~umpy/typing/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:49.855464 ultraspy-1.0/venv/Lib/site-packages/~umpy/typing/tests/
-drwxrwxrwx   0        0        0        0 2023-06-07 12:52:52.005511 ultraspy-1.0/venv/Lib/site-packages/~umpy/typing/tests/data/
--rw-rw-rw-   0        0        0      176 2023-05-03 12:33:57.000000 ultraspy-1.0/venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.026367 ultraspy-1.1/
+-rw-rw-rw-   0        0        0      256 2023-06-07 09:00:51.000000 ultraspy-1.1/.readthedocs.yml
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.124384 ultraspy-1.1/.tox/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.042948 ultraspy-1.1/.tox/docs/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.043849 ultraspy-1.1/.tox/docs/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.047892 ultraspy-1.1/.tox/docs/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.043849 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.271403 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 10:38:14.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.046882 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.309397 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.046882 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.319587 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 10:38:15.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.049959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.047892 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.048959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.340518 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 10:37:24.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 10:37:24.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.049959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.050959 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.351050 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 10:37:25.000000 ultraspy-1.1/.tox/docs/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.051960 ultraspy-1.1/.tox/py310-cpu_tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.051960 ultraspy-1.1/.tox/py310-cpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.052959 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.355168 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 10:45:09.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.367471 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.054961 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.371548 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 10:45:10.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.092481 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.091421 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.091421 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.378622 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 10:44:26.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 10:44:26.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.093519 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.093519 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.380717 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 10:44:27.000000 ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.095517 ultraspy-1.1/.tox/py310-gpu_tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.095517 ultraspy-1.1/.tox/py310-gpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.110788 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.105182 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.097035 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.098127 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.104134 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.103129 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.100127 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.423269 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.533382 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.557319 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.582777 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.794513 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.806202 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.816915 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-06-21 12:46:31.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.844151 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-06-21 12:46:32.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.852347 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-06-21 12:46:33.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.107700 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.856858 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.109790 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.869560 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.109790 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.872644 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 12:46:14.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.112787 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.111788 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.112787 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.878716 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 12:45:19.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 12:45:19.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.113863 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.113863 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.881766 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 12:45:21.000000 ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.114863 ultraspy-1.1/.tox/py38-cpu_tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.114863 ultraspy-1.1/.tox/py38-cpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.120386 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.116373 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.884808 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.118383 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.899297 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.119380 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.902334 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 11:28:38.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.122384 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.121385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.121385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.908453 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.122384 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.123385 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.911577 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 11:27:53.000000 ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.124384 ultraspy-1.1/.tox/py38-gpu_tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.125386 ultraspy-1.1/.tox/py38-gpu_tests/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.140890 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.135675 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.126382 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.127505 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.133587 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.133587 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.130580 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.956167 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.086785 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.118214 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.147184 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.363725 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.376220 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.386321 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-06-21 12:59:06.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.408625 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-06-21 12:59:07.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.419670 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-06-21 12:59:08.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.136671 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.419670 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-21 12:59:16.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.139845 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.430997 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.139845 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.436506 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-21 12:59:17.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.143888 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.141887 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.142895 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.442127 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-21 12:58:24.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-21 12:58:24.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.144892 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.144892 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.446133 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-21 12:58:25.000000 ultraspy-1.1/.tox/py38-gpu_tests/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+-rw-rw-rw-   0        0        0       68 2022-08-03 15:17:56.000000 ultraspy-1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0      217 2023-06-30 16:44:31.000000 ultraspy-1.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2367 2023-04-20 15:30:24.000000 ultraspy-1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1091 2022-06-22 12:40:44.000000 ultraspy-1.1/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-04-20 15:30:24.000000 ultraspy-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3545 2023-06-30 16:46:58.026367 ultraspy-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2023-06-07 11:18:20.000000 ultraspy-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.464228 ultraspy-1.1/docs/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.466234 ultraspy-1.1/docs/_static/
+-rw-rw-rw-   0        0        0      235 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1119 2023-06-30 15:44:47.000000 ultraspy-1.1/docs/acknowledgements.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.497892 ultraspy-1.1/docs/algorithms/
+-rw-rw-rw-   0        0        0     3530 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/das_algo.rst
+-rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/fdmas_algo.rst
+-rw-rw-rw-   0        0        0      187 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/index.rst
+-rw-rw-rw-   0        0        0     2452 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/algorithms/pdas_algo.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.536139 ultraspy-1.1/docs/api_references/
+-rw-rw-rw-   0        0        0      488 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/beamformers.rst
+-rw-rw-rw-   0        0        0      905 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/api_references/classes.rst
+-rw-rw-rw-   0        0        0       94 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/gpu_utils.rst
+-rw-rw-rw-   0        0        0      143 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/index.rst
+-rw-rw-rw-   0        0        0       88 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/api_references/metrics.rst
+-rw-rw-rw-   0        0        0     1624 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/api_references/ultraspy.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.587452 ultraspy-1.1/docs/architecture/
+-rw-rw-rw-   0        0        0    11787 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/architecture/beamformer_class.rst
+-rw-rw-rw-   0        0        0     4254 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/common_methods.rst
+-rw-rw-rw-   0        0        0     1987 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/index.rst
+-rw-rw-rw-   0        0        0      421 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/probe_class.rst
+-rw-rw-rw-   0        0        0       65 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/reader_class.rst
+-rw-rw-rw-   0        0        0       60 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/architecture/scan_class.rst
+-rw-rw-rw-   0        0        0     2884 2023-06-21 10:05:36.000000 ultraspy-1.1/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.654499 ultraspy-1.1/docs/contribute/
+-rw-rw-rw-   0        0        0     2037 2023-06-07 11:48:18.000000 ultraspy-1.1/docs/contribute/devops_routine.rst
+-rw-rw-rw-   0        0        0      625 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/index.rst
+-rw-rw-rw-   0        0        0     3923 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_beamformer.rst
+-rw-rw-rw-   0        0        0      677 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_methods.rst
+-rw-rw-rw-   0        0        0      911 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/own_setups_options.rst
+-rw-rw-rw-   0        0        0     2456 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/preparation.rst
+-rw-rw-rw-   0        0        0     1594 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/contribute/tdd.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.706507 ultraspy-1.1/docs/examples/
+-rw-rw-rw-   0        0        0     9976 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/das.rst
+-rw-rw-rw-   0        0        0     6125 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/doppler.rst
+-rw-rw-rw-   0        0        0      327 2023-06-07 09:00:51.000000 ultraspy-1.1/docs/examples/index.rst
+-rw-rw-rw-   0        0        0    12052 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/examples/metrics.rst
+-rw-rw-rw-   0        0        0     7211 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/examples/simu_data.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.816570 ultraspy-1.1/docs/images/
+-rw-rw-rw-   0        0        0    34289 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/block_grid.png
+-rw-rw-rw-   0        0        0   132410 2023-01-25 18:21:44.000000 ultraspy-1.1/docs/images/convex_delays.png
+-rw-rw-rw-   0        0        0   114606 2023-01-25 18:21:44.000000 ultraspy-1.1/docs/images/convex_probe.png
+-rw-rw-rw-   0        0        0    18675 2023-06-21 10:27:54.000000 ultraspy-1.1/docs/images/creatis_logo.png
+-rw-rw-rw-   0        0        0    35256 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/das_algo.png
+-rw-rw-rw-   0        0        0    32371 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/das_bmode.png
+-rw-rw-rw-   0        0        0    54387 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/das_dam.png
+-rw-rw-rw-   0        0        0   229452 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/doppler.png
+-rw-rw-rw-   0        0        0    87019 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fdmas_optim_gpu.png
+-rw-rw-rw-   0        0        0   180354 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fdmas_spectra.png
+-rw-rw-rw-   0        0        0    12459 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/fnumber.png
+-rw-rw-rw-   0        0        0    99220 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/gpu_architecture.png
+-rw-rw-rw-   0        0        0   110727 2023-06-21 10:17:27.000000 ultraspy-1.1/docs/images/image4us.png
+-rw-rw-rw-   0        0        0    64454 2023-06-21 10:27:24.000000 ultraspy-1.1/docs/images/image4us_logo.png
+-rw-rw-rw-   0        0        0    87661 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/interpolation_beamforming.png
+-rw-rw-rw-   0        0        0    66458 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes.png
+-rw-rw-rw-   0        0        0    31442 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes_axial.png
+-rw-rw-rw-   0        0        0    46092 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_lobes_lateral.png
+-rw-rw-rw-   0        0        0    51462 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_masks.png
+-rw-rw-rw-   0        0        0    74436 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_raw_data.png
+-rw-rw-rw-   0        0        0    41500 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_snr_correct.png
+-rw-rw-rw-   0        0        0    31289 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_snr_wrong.png
+-rw-rw-rw-   0        0        0   260166 2022-08-03 15:17:56.000000 ultraspy-1.1/docs/images/metrics_spectra.png
+-rw-rw-rw-   0        0        0   299480 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/images/pdas_spectra.png
+-rw-rw-rw-   0        0        0    24721 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/polar_system.png
+-rw-rw-rw-   0        0        0    96279 2023-06-21 10:28:29.000000 ultraspy-1.1/docs/images/tpac_logo.jpg
+-rw-rw-rw-   0        0        0   114889 2023-04-20 15:30:24.000000 ultraspy-1.1/docs/images/ultraspy_classes.png
+-rw-rw-rw-   0        0        0     3166 2023-06-21 10:31:57.000000 ultraspy-1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     4063 2023-06-07 11:21:30.000000 ultraspy-1.1/docs/installation.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.856184 ultraspy-1.1/docs/tech_choices/
+-rw-rw-rw-   0        0        0     3692 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/beamforming_choices.rst
+-rw-rw-rw-   0        0        0     2436 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/gpu_beamformers.rst
+-rw-rw-rw-   0        0        0     5834 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/gpu_configs.rst
+-rw-rw-rw-   0        0        0      248 2023-04-26 14:04:14.000000 ultraspy-1.1/docs/tech_choices/index.rst
+-rw-rw-rw-   0        0        0      110 2023-04-20 15:30:24.000000 ultraspy-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 16:46:58.026367 ultraspy-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-06-30 16:44:39.000000 ultraspy-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.856184 ultraspy-1.1/src/
+-rw-rw-rw-   0        0        0        0 2022-06-22 12:40:44.000000 ultraspy-1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.866115 ultraspy-1.1/src/ultraspy/
+-rw-rw-rw-   0        0        0      892 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/TODO.md
+-rw-rw-rw-   0        0        0     1068 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.906328 ultraspy-1.1/src/ultraspy/beamformers/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/beamformers/__init__.py
+-rw-rw-rw-   0        0        0    30236 2023-06-26 16:05:31.000000 ultraspy-1.1/src/ultraspy/beamformers/beamformer.py
+-rw-rw-rw-   0        0        0    17908 2023-06-06 13:22:47.000000 ultraspy-1.1/src/ultraspy/beamformers/das.py
+-rw-rw-rw-   0        0        0    26096 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/fdmas.py
+-rw-rw-rw-   0        0        0     2381 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/options.py
+-rw-rw-rw-   0        0        0    22921 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/beamformers/pdas.py
+-rw-rw-rw-   0        0        0     1105 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/beamformers/setups.py
+-rw-rw-rw-   0        0        0      786 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/config.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.909850 ultraspy-1.1/src/ultraspy/cpu/
+-rw-rw-rw-   0        0        0      642 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/__init__.py
+-rw-rw-rw-   0        0        0     2702 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/display.py
+-rw-rw-rw-   0        0        0     9390 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/doppler.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.156486 ultraspy-1.1/src/ultraspy/cpu/kernels/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.926119 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/__init__.py
+-rw-rw-rw-   0        0        0     2804 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py
+-rw-rw-rw-   0        0        0     1960 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/apodization.py
+-rw-rw-rw-   0        0        0    13231 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/das.py
+-rw-rw-rw-   0        0        0    16093 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/fdmas.py
+-rw-rw-rw-   0        0        0     1808 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/interpolation.py
+-rw-rw-rw-   0        0        0      457 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/maths_utils.py
+-rw-rw-rw-   0        0        0    15618 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/pdas.py
+-rw-rw-rw-   0        0        0     1133 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.943302 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py
+-rw-rw-rw-   0        0        0     5983 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/das.py
+-rw-rw-rw-   0        0        0     8235 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py
+-rw-rw-rw-   0        0        0     5075 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py
+-rw-rw-rw-   0        0        0     8892 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/pdas.py
+-rw-rw-rw-   0        0        0     1097 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py
+-rw-rw-rw-   0        0        0     2663 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/cpu/post_processing.py
+-rw-rw-rw-   0        0        0     7395 2023-04-26 16:33:32.000000 ultraspy-1.1/src/ultraspy/cpu/signal.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.956318 ultraspy-1.1/src/ultraspy/gpu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/__init__.py
+-rw-rw-rw-   0        0        0     3257 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/display.py
+-rw-rw-rw-   0        0        0    12887 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/doppler.py
+-rw-rw-rw-   0        0        0     3032 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/gpu_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.966356 ultraspy-1.1/src/ultraspy/gpu/kernels/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.977531 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/
+-rw-rw-rw-   0        0        0     1742 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu
+-rw-rw-rw-   0        0        0     2656 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/apodization.cu
+-rw-rw-rw-   0        0        0    18518 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/das.cu
+-rw-rw-rw-   0        0        0    22384 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/fdmas.cu
+-rw-rw-rw-   0        0        0     4039 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/interpolation.cu
+-rw-rw-rw-   0        0        0    23418 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/pdas.cu
+-rw-rw-rw-   0        0        0     2435 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu
+-rw-rw-rw-   0        0        0     4641 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu
+-rw-rw-rw-   0        0        0     2298 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers_kernels.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.988573 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/
+-rw-rw-rw-   0        0        0     1600 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/color_map.cu
+-rw-rw-rw-   0        0        0     2188 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu
+-rw-rw-rw-   0        0        0     3096 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu
+-rw-rw-rw-   0        0        0     4122 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu
+-rw-rw-rw-   0        0        0     1558 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/power_map.cu
+-rw-rw-rw-   0        0        0     3749 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/doppler_kernels.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.988573 ultraspy-1.1/src/ultraspy/gpu/kernels/headers/
+-rw-rw-rw-   0        0        0      124 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/headers/cupy_header.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.004622 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/
+-rw-rw-rw-   0        0        0     1737 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/by2.cu
+-rw-rw-rw-   0        0        0     7248 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/convolve.cu
+-rw-rw-rw-   0        0        0     1681 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/divide_by.cu
+-rw-rw-rw-   0        0        0     8193 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/flip.cu
+-rw-rw-rw-   0        0        0     1274 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/get_modulo.cu
+-rw-rw-rw-   0        0        0     3695 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/median_filter.cu
+-rw-rw-rw-   0        0        0     1552 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators/to_db.cu
+-rw-rw-rw-   0        0        0     4802 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/operators_kernels.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.010925 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/
+-rw-rw-rw-   0        0        0     2288 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/down_mix.cu
+-rw-rw-rw-   0        0        0     4618 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/filter0.cu
+-rw-rw-rw-   0        0        0     2460 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_end_sig.cu
+-rw-rw-rw-   0        0        0     2906 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_filter.cu
+-rw-rw-rw-   0        0        0     2512 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_start_sig.cu
+-rw-rw-rw-   0        0        0     2432 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/signal_kernels.py
+-rw-rw-rw-   0        0        0     3413 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/kernels/utils.py
+-rw-rw-rw-   0        0        0     2801 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/gpu/post_processing.py
+-rw-rw-rw-   0        0        0    12741 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/gpu/signal.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.022239 ultraspy-1.1/src/ultraspy/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/doppler_helpers.py
+-rw-rw-rw-   0        0        0     4037 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/metrics_helpers.py
+-rw-rw-rw-   0        0        0     6240 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/signal_helpers.py
+-rw-rw-rw-   0        0        0    11815 2023-06-26 16:21:58.000000 ultraspy-1.1/src/ultraspy/helpers/transmit_delays_helpers.py
+-rw-rw-rw-   0        0        0      530 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/helpers/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.026248 ultraspy-1.1/src/ultraspy/io/
+-rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.041217 ultraspy-1.1/src/ultraspy/io/file_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/factory.py
+-rw-rw-rw-   0        0        0     1267 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/file_loader.py
+-rw-rw-rw-   0        0        0     2023 2023-06-26 15:49:38.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/h5_loader.py
+-rw-rw-rw-   0        0        0     2063 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/mat_loader.py
+-rw-rw-rw-   0        0        0     7828 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/io/file_loaders/rff256_loader.py
+-rw-rw-rw-   0        0        0    26165 2023-06-29 12:01:56.000000 ultraspy-1.1/src/ultraspy/io/reader.py
+-rw-rw-rw-   0        0        0    15946 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.046233 ultraspy-1.1/src/ultraspy/probes/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/probes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.056595 ultraspy-1.1/src/ultraspy/probes/configs/
+-rw-rw-rw-   0        0        0      182 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/c5-2v.ini
+-rw-rw-rw-   0        0        0      164 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l11-4v.ini
+-rw-rw-rw-   0        0        0      165 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l11-5v.ini
+-rw-rw-rw-   0        0        0      170 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l14-5w.ini
+-rw-rw-rw-   0        0        0      160 2023-01-25 18:21:44.000000 ultraspy-1.1/src/ultraspy/probes/configs/l7-4.ini
+-rw-rw-rw-   0        0        0      208 2023-06-19 15:40:23.000000 ultraspy-1.1/src/ultraspy/probes/configs/mux_1024_8MHz.ini
+-rw-rw-rw-   0        0        0      164 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/probes/configs/p4-2v.ini
+-rw-rw-rw-   0        0        0     2635 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/convex_probe.py
+-rw-rw-rw-   0        0        0     5382 2023-06-19 15:41:35.000000 ultraspy-1.1/src/ultraspy/probes/factory.py
+-rw-rw-rw-   0        0        0     1571 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/linear_probe.py
+-rw-rw-rw-   0        0        0     2359 2023-06-16 13:59:32.000000 ultraspy-1.1/src/ultraspy/probes/matricial_probe.py
+-rw-rw-rw-   0        0        0     8325 2023-04-26 14:04:14.000000 ultraspy-1.1/src/ultraspy/probes/probe.py
+-rw-rw-rw-   0        0        0    17720 2023-06-07 09:00:51.000000 ultraspy-1.1/src/ultraspy/scan.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.076306 ultraspy-1.1/src/ultraspy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/__init__.py
+-rw-rw-rw-   0        0        0      585 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/beamformers.py
+-rw-rw-rw-   0        0        0     3648 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/linear_decomposition.py
+-rw-rw-rw-   0        0        0     2331 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/masks.py
+-rw-rw-rw-   0        0        0     1292 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/matplot.py
+-rw-rw-rw-   0        0        0     3336 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/print.py
+-rw-rw-rw-   0        0        0      495 2023-06-07 14:21:21.000000 ultraspy-1.1/src/ultraspy/utils/scan.py
+-rw-rw-rw-   0        0        0      711 2023-04-20 15:30:24.000000 ultraspy-1.1/src/ultraspy/utils/string.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:56.887743 ultraspy-1.1/src/ultraspy.egg-info/
+-rw-rw-rw-   0        0        0     3545 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    24698 2023-06-30 16:46:55.000000 ultraspy-1.1/src/ultraspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 16:46:44.000000 ultraspy-1.1/src/ultraspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.086353 ultraspy-1.1/tests/
+-rw-rw-rw-   0        0        0     6137 2023-06-07 09:02:02.000000 ultraspy-1.1/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.146471 ultraspy-1.1/tests/test_cpu/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.216366 ultraspy-1.1/tests/test_cpu/beamformers/
+-rw-rw-rw-   0        0        0     7493 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_beamformer.py
+-rw-rw-rw-   0        0        0    51386 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_das.py
+-rw-rw-rw-   0        0        0    14986 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_fdmas.py
+-rw-rw-rw-   0        0        0    18333 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/beamformers/test_pdas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.267958 ultraspy-1.1/tests/test_cpu/helpers/
+-rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_doppler_helpers.py
+-rw-rw-rw-   0        0        0      674 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_signal_helpers.py
+-rw-rw-rw-   0        0        0      295 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_transmit_delays_helpers.py
+-rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/helpers/test_windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.277541 ultraspy-1.1/tests/test_cpu/io/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.306916 ultraspy-1.1/tests/test_cpu/io/file_loaders/
+-rw-rw-rw-   0        0        0      183 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_h5_loaders.py
+-rw-rw-rw-   0        0        0      191 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_mat_loader.py
+-rw-rw-rw-   0        0        0      203 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/file_loaders/test_rff256_loader.py
+-rw-rw-rw-   0        0        0     1453 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/io/test_reader.py
+-rw-rw-rw-   0        0        0    11386 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/test_doppler.py
+-rw-rw-rw-   0        0        0     8264 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_cpu/test_metrics.py
+-rw-rw-rw-   0        0        0     1093 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/test_post_processing.py
+-rw-rw-rw-   0        0        0     1074 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/test_probes.py
+-rw-rw-rw-   0        0        0     4333 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_cpu/test_scan.py
+-rw-rw-rw-   0        0        0     6287 2023-04-26 16:33:32.000000 ultraspy-1.1/tests/test_cpu/test_signal.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.357591 ultraspy-1.1/tests/test_cpu/utils/
+-rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_linear_decomposition.py
+-rw-rw-rw-   0        0        0     1478 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_masks.py
+-rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_print_utils.py
+-rw-rw-rw-   0        0        0      261 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_scans_utils.py
+-rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_cpu/utils/test_string.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.419695 ultraspy-1.1/tests/test_gpu/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.466396 ultraspy-1.1/tests/test_gpu/beamformers/
+-rw-rw-rw-   0        0        0     6486 2023-06-07 09:00:51.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_beamformer.py
+-rw-rw-rw-   0        0        0    16206 2023-06-27 12:49:38.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_das.py
+-rw-rw-rw-   0        0        0     7610 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_fdmas.py
+-rw-rw-rw-   0        0        0     6963 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/beamformers/test_pdas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.476539 ultraspy-1.1/tests/test_gpu/helpers/
+-rw-rw-rw-   0        0        0     1752 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_doppler_helpers.py
+-rw-rw-rw-   0        0        0      872 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_signal_helpers.py
+-rw-rw-rw-   0        0        0      642 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/helpers/test_windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.519386 ultraspy-1.1/tests/test_gpu/kernels/
+-rw-rw-rw-   0        0        0      112 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_beamformers_kernels.py
+-rw-rw-rw-   0        0        0     4328 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_doppler_kernels.py
+-rw-rw-rw-   0        0        0     8108 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_operators_kernels.py
+-rw-rw-rw-   0        0        0     3203 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/kernels/test_signal_kernels.py
+-rw-rw-rw-   0        0        0      248 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_display.py
+-rw-rw-rw-   0        0        0     4997 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_doppler.py
+-rw-rw-rw-   0        0        0     3960 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/test_filtfilts.py
+-rw-rw-rw-   0        0        0     1881 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_gpu_utils.py
+-rw-rw-rw-   0        0        0      176 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/test_post_processing.py
+-rw-rw-rw-   0        0        0     3874 2023-04-26 14:04:14.000000 ultraspy-1.1/tests/test_gpu/test_signal.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.526397 ultraspy-1.1/tests/test_gpu/utils/
+-rw-rw-rw-   0        0        0     2121 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_linear_decomposition.py
+-rw-rw-rw-   0        0        0      245 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_print_utils.py
+-rw-rw-rw-   0        0        0      251 2023-04-20 15:30:24.000000 ultraspy-1.1/tests/test_gpu/utils/test_string_utils.py
+-rw-rw-rw-   0        0        0      798 2023-06-30 15:51:44.000000 ultraspy-1.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.178639 ultraspy-1.1/venv/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.178639 ultraspy-1.1/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.209871 ultraspy-1.1/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.191260 ultraspy-1.1/venv/Lib/site-packages/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.180640 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.180640 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.189267 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.188251 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.183729 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.563619 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/
+-rw-rw-rw-   0        0        0    11047 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu
+-rw-rw-rw-   0        0        0     9934 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu
+-rw-rw-rw-   0        0        0    11663 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu
+-rw-rw-rw-   0        0        0     1611 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.646607 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/
+-rw-rw-rw-   0        0        0     8406 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu
+-rw-rw-rw-   0        0        0     8480 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu
+-rw-rw-rw-   0        0        0     8529 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu
+-rw-rw-rw-   0        0        0     6005 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu
+-rw-rw-rw-   0        0        0     6193 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu
+-rw-rw-rw-   0        0        0     8389 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu
+-rw-rw-rw-   0        0        0     8452 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu
+-rw-rw-rw-   0        0        0     7714 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu
+-rw-rw-rw-   0        0        0    13661 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.665398 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.676482 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/
+-rw-rw-rw-   0        0        0    38255 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu
+-rw-rw-rw-   0        0        0    97459 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu
+-rw-rw-rw-   0        0        0    22413 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu
+-rw-rw-rw-   0        0        0    31573 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.886616 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/
+-rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_a.cu
+-rw-rw-rw-   0        0        0      326 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/link_b.cu
+-rw-rw-rw-   0        0        0    17023 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu
+-rw-rw-rw-   0        0        0     9933 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu
+-rw-rw-rw-   0        0        0    20045 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu
+-rw-rw-rw-   0        0        0    26109 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu
+-rw-rw-rw-   0        0        0    27450 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu
+-rw-rw-rw-   0        0        0    35739 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu
+-rw-rw-rw-   0        0        0    71982 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu
+-rw-rw-rw-   0        0        0    47767 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu
+-rw-rw-rw-   0        0        0    51261 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu
+-rw-rw-rw-   0        0        0    31216 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu
+-rw-rw-rw-   0        0        0    32082 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu
+-rw-rw-rw-   0        0        0    34615 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu
+-rw-rw-rw-   0        0        0    38679 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu
+-rw-rw-rw-   0        0        0    22169 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu
+-rw-rw-rw-   0        0        0     5284 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu
+-rw-rw-rw-   0        0        0    26354 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu
+-rw-rw-rw-   0        0        0    28026 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu
+-rw-rw-rw-   0        0        0    21011 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.898019 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/
+-rw-rw-rw-   0        0        0    28426 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.906567 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/
+-rw-rw-rw-   0        0        0    42322 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.926133 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/
+-rw-rw-rw-   0        0        0    31907 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu
+-rw-rw-rw-   0        0        0     2900 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu
+-rw-rw-rw-   0        0        0    18156 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.936167 ultraspy-1.1/venv/Lib/site-packages/cupy/random/
+-rw-rw-rw-   0        0        0    29209 2023-02-22 11:49:00.000000 ultraspy-1.1/venv/Lib/site-packages/cupy/random/cupy_distributions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.193259 ultraspy-1.1/venv/Lib/site-packages/numba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.946589 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/
+-rw-rw-rw-   0        0        0     1000 2023-06-02 15:39:03.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.195541 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.962426 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/
+-rw-rw-rw-   0        0        0      299 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      145 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/error.cu
+-rw-rw-rw-   0        0        0      564 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu
+-rw-rw-rw-   0        0        0      179 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.195541 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.965490 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      926 2023-06-02 15:39:04.000000 ultraspy-1.1/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.199655 ultraspy-1.1/venv/Lib/site-packages/numpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.197651 ultraspy-1.1/venv/Lib/site-packages/numpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.198652 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.969894 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-02 15:39:09.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-02 15:39:09.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.199655 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.200650 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.969894 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-02 15:39:10.000000 ultraspy-1.1/venv/Lib/site-packages/numpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.204212 ultraspy-1.1/venv/Lib/site-packages/~-mpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.202649 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.202649 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.976402 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-06-02 15:35:42.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-06-02 15:35:42.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.204212 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.205238 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:57.981145 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-06-02 15:35:43.000000 ultraspy-1.1/venv/Lib/site-packages/~-mpy/typing/tests/data/mypy.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.205238 ultraspy-1.1/venv/Lib/site-packages/~umba/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.206751 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.208772 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.207759 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.006554 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/
+-rw-rw-rw-   0        0        0      294 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/cuda_include.cu
+-rw-rw-rw-   0        0        0      138 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/error.cu
+-rw-rw-rw-   0        0        0      214 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/jitlink.cu
+-rw-rw-rw-   0        0        0      172 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/cudadrv/data/warn.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.208772 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.016536 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/
+-rw-rw-rw-   0        0        0      292 2022-08-02 14:53:44.000000 ultraspy-1.1/venv/Lib/site-packages/~umba/cuda/tests/doc_examples/ffi/functions.cu
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.212910 ultraspy-1.1/venv/Lib/site-packages/~umpy/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.210911 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.211910 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.025862 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/
+-rw-rw-rw-   0        0        0      151 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/mlib.ini
+-rw-rw-rw-   0        0        0      380 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/core/lib/npy-pkg-config/npymath.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.212910 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:55.213909 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/
+drwxrwxrwx   0        0        0        0 2023-06-30 16:46:58.026367 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/data/
+-rw-rw-rw-   0        0        0      176 2023-05-03 12:33:57.000000 ultraspy-1.1/venv/Lib/site-packages/~umpy/typing/tests/data/mypy.ini
```

### Comparing `ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.1/.tox/docs/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.1/.tox/py310-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/CONTRIBUTING.rst` & `ultraspy-1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/LICENSE` & `ultraspy-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/PKG-INFO` & `ultraspy-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultraspy
-Version: 1.0
+Version: 1.1
 Summary: Ultrasound toolbox for GPU
 Home-page: https://gitlab.com/pecarlat/ultraspy
 Author: Pierre Ecarlat
 Author-email: pierre.ecarlat@gmail.com
 Project-URL: Documentation, https://ultraspy.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/pecarlat/ultraspy/-/issues/
 Keywords: ultrasound,python,beamforming,doppler
```

### Comparing `ultraspy-1.0/README.rst` & `ultraspy-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/algorithms/das_algo.rst` & `ultraspy-1.1/docs/algorithms/das_algo.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/algorithms/fdmas_algo.rst` & `ultraspy-1.1/docs/algorithms/fdmas_algo.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/algorithms/pdas_algo.rst` & `ultraspy-1.1/docs/algorithms/pdas_algo.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/api_references/classes.rst` & `ultraspy-1.1/docs/api_references/classes.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/api_references/ultraspy.rst` & `ultraspy-1.1/docs/api_references/ultraspy.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/architecture/beamformer_class.rst` & `ultraspy-1.1/docs/architecture/beamformer_class.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/architecture/common_methods.rst` & `ultraspy-1.1/docs/architecture/common_methods.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/architecture/index.rst` & `ultraspy-1.1/docs/architecture/index.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/conf.py` & `ultraspy-1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,21 @@
 html_theme = 'sphinx_rtd_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+# Logo title
+html_logo = "images/image4us.png"
+html_theme_options = {
+    'logo_only': False,
+    'display_version': False,
+}
+
 
 # -- Options for LaTex output -------------------------------------------------
 
 # Avoid blank page used for duplex printing.
 latex_elements = {
   'extraclassoptions': 'openany,oneside'
 }
```

### Comparing `ultraspy-1.0/docs/contribute/devops_routine.rst` & `ultraspy-1.1/docs/contribute/devops_routine.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/index.rst` & `ultraspy-1.1/docs/contribute/index.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/own_beamformer.rst` & `ultraspy-1.1/docs/contribute/own_beamformer.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/own_methods.rst` & `ultraspy-1.1/docs/contribute/own_methods.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/own_setups_options.rst` & `ultraspy-1.1/docs/contribute/own_setups_options.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/preparation.rst` & `ultraspy-1.1/docs/contribute/preparation.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/contribute/tdd.rst` & `ultraspy-1.1/docs/contribute/tdd.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/examples/das.rst` & `ultraspy-1.1/docs/examples/das.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/examples/doppler.rst` & `ultraspy-1.1/docs/examples/doppler.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/examples/metrics.rst` & `ultraspy-1.1/docs/examples/metrics.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/examples/simu_data.rst` & `ultraspy-1.1/docs/examples/simu_data.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/block_grid.png` & `ultraspy-1.1/docs/images/block_grid.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/convex_delays.png` & `ultraspy-1.1/docs/images/convex_delays.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/convex_probe.png` & `ultraspy-1.1/docs/images/convex_probe.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/das_algo.png` & `ultraspy-1.1/docs/images/das_algo.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/das_bmode.png` & `ultraspy-1.1/docs/images/das_bmode.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/das_dam.png` & `ultraspy-1.1/docs/images/das_dam.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/doppler.png` & `ultraspy-1.1/docs/images/doppler.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/fdmas_optim_gpu.png` & `ultraspy-1.1/docs/images/fdmas_optim_gpu.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/fdmas_spectra.png` & `ultraspy-1.1/docs/images/fdmas_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/fnumber.png` & `ultraspy-1.1/docs/images/fnumber.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/gpu_architecture.png` & `ultraspy-1.1/docs/images/gpu_architecture.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/interpolation_beamforming.png` & `ultraspy-1.1/docs/images/interpolation_beamforming.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_lobes.png` & `ultraspy-1.1/docs/images/metrics_lobes.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_lobes_axial.png` & `ultraspy-1.1/docs/images/metrics_lobes_axial.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_lobes_lateral.png` & `ultraspy-1.1/docs/images/metrics_lobes_lateral.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_masks.png` & `ultraspy-1.1/docs/images/metrics_masks.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_raw_data.png` & `ultraspy-1.1/docs/images/metrics_raw_data.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_snr_correct.png` & `ultraspy-1.1/docs/images/metrics_snr_correct.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_snr_wrong.png` & `ultraspy-1.1/docs/images/metrics_snr_wrong.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/metrics_spectra.png` & `ultraspy-1.1/docs/images/metrics_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/pdas_spectra.png` & `ultraspy-1.1/docs/images/pdas_spectra.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/polar_system.png` & `ultraspy-1.1/docs/images/polar_system.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/images/ultraspy_classes.png` & `ultraspy-1.1/docs/images/ultraspy_classes.png`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/index.rst` & `ultraspy-1.1/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .. ultraspy documentation master file
 
 What is `ultraspy`?
 -------------------
-`ultraspy` is a package designed to efficiently manipulate ultrasound data
-using GPU. The most common beamforming or Doppler methods are implemented (such
-as DAS, RF to I/Qs, Color/Power Doppler, ...), along with some state-of-the-art
-methods (Capon beamforming, Vector Doppler, alias-free Doppler velocity, ...).
-A set of metrics (PSL, FWHM, SNR) is also provided so anyone can validate the
-quality of their ultrasound data and beamforming operations.
+`ultraspy` is a package developed by
+`CREATIS <https://www.creatis.insa-lyon.fr>`_ and
+`TPAC <https://thephasedarraycompany.com>`_, as part of the ANR Labcom Image4US.
+It is designed to efficiently manipulate ultrasound data using GPU. The most
+common beamforming or Doppler methods are implemented (such as DAS, RF to I/Qs,
+Color/Power Doppler, ...), along with some state-of-the-art methods (Capon
+beamforming, Vector Doppler, alias-free Doppler velocity, ...). A set of
+metrics (PSL, FWHM, SNR) is also provided so anyone can validate the quality of
+their ultrasound data and beamforming operations.
 
 The package is designed to work with both RF and I/Q signals, in 2D or 3D, and
 with any type of probe (linear, convex, or matrix). The core code can run both
 on CPU and GPU, making it ideal for any real-time application. All beamforming
 parameters (f-number, compounding, apodization…) can be freely customized at
 any time for research purposes.
 
@@ -48,20 +51,36 @@
 
 Great, I'm in! What should I do?
 --------------------------------
 First thing first, you'll have to :ref:`install it<installation>`, then you can
 have a look to the :ref:`examples<examples>`. Enjoy! :-)
 
 
+Special thanks
+--------------
+The list of contributors and advisors can be found in the :ref:`dedicated
+section<thanks>`.
+
+.. image:: images/creatis_logo.png
+   :height: 40
+
+.. image:: images/image4us_logo.png
+   :height: 100
+
+.. image:: images/tpac_logo.jpg
+   :height: 75
+
+
 Index
 -----
 
 .. toctree::
    :maxdepth: 2
 
    installation
    examples/index
    architecture/index
    algorithms/index
    tech_choices/index
    contribute/index
    api_references/index
+   acknowledgements
```

### Comparing `ultraspy-1.0/docs/installation.rst` & `ultraspy-1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/tech_choices/beamforming_choices.rst` & `ultraspy-1.1/docs/tech_choices/beamforming_choices.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/tech_choices/gpu_beamformers.rst` & `ultraspy-1.1/docs/tech_choices/gpu_beamformers.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/docs/tech_choices/gpu_configs.rst` & `ultraspy-1.1/docs/tech_choices/gpu_configs.rst`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/setup.py` & `ultraspy-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Contents of local files
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 
 setup(
     name='ultraspy',
-    version='1.0',
+    version='1.1',
     author='Pierre Ecarlat',
     author_email='pierre.ecarlat@gmail.com',
     description='Ultrasound toolbox for GPU',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pecarlat/ultraspy',
     project_urls={
```

### Comparing `ultraspy-1.0/src/ultraspy/TODO.md` & `ultraspy-1.1/src/ultraspy/TODO.md`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/__init__.py` & `ultraspy-1.1/src/ultraspy/__init__.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/beamformer.py` & `ultraspy-1.1/src/ultraspy/beamformers/beamformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         :param str name: The name of the parameter
         :param int, float, list, numpy.ndarray value: The value to attribute
         """
         if name not in bf_setups.INFO:
             raise AttributeError("Unknown setup name. Please pick one in "
                                  f"{bf_setups.INFO.keys()}.")
 
-        if name is 'f_number' and isinstance(value, (int, float)):
+        if name == 'f_number' and isinstance(value, (int, float)):
             # Duplicate the f-number in both directions
             value = [value, value]
 
         self.setups[name] = self._convert_given_info(value,
                                                      bf_setups.INFO[name])
 
         if name in ['emitted_probe', 'received_probe'] and \
@@ -279,17 +279,15 @@
             self.update_setup('prf', acquisition_info['prf'])
         seq = acquisition_info['sequence_elements']
         self.update_setup('emitted_probe', probe.geometry[:, seq['emitted']])
         self.update_setup('received_probe', probe.geometry[:, seq['received']])
         self._is_same_probe = np.all([seq['emitted'] == seq['received']])
         self.update_setup('transmissions_idx',
                           list(range(acquisition_info['delays'].shape[0])))
-        delays = acquisition_info['delays']
-        self.update_setup('delays', delays[np.arange(delays.shape[0])[:, None],
-                                           seq['emitted']])
+        self.update_setup('delays', acquisition_info['delays'])
         th = probe.get_thetas()
         self.update_setup('emitted_thetas', th[seq['emitted']])
         self.update_setup('received_thetas', th[seq['received']])
 
     def init_from_beamformer(self, beamformer):
         """Updates the setups and options using a previously initialized
         beamformer.
```

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/das.py` & `ultraspy-1.1/src/ultraspy/beamformers/das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/fdmas.py` & `ultraspy-1.1/src/ultraspy/beamformers/fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/options.py` & `ultraspy-1.1/src/ultraspy/beamformers/options.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/pdas.py` & `ultraspy-1.1/src/ultraspy/beamformers/pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/beamformers/setups.py` & `ultraspy-1.1/src/ultraspy/beamformers/setups.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/config.py` & `ultraspy-1.1/src/ultraspy/config.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/__init__.py` & `ultraspy-1.1/src/ultraspy/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/display.py` & `ultraspy-1.1/src/ultraspy/cpu/display.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/doppler.py` & `ultraspy-1.1/src/ultraspy/cpu/doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/aperture_ratio.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/apodization.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/apodization.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/das.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/fdmas.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/interpolation.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/interpolation.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/pdas.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numba_cores/probe_distances.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/aperture_ratio.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/das.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/interpolation.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/pdas.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py` & `ultraspy-1.1/src/ultraspy/cpu/kernels/numpy_cores/probe_distances.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/post_processing.py` & `ultraspy-1.1/src/ultraspy/cpu/post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/cpu/signal.py` & `ultraspy-1.1/src/ultraspy/cpu/signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/display.py` & `ultraspy-1.1/src/ultraspy/gpu/display.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/doppler.py` & `ultraspy-1.1/src/ultraspy/gpu/doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/gpu_utils.py` & `ultraspy-1.1/src/ultraspy/gpu/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/aperture_ratio.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/apodization.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/apodization.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/das.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/das.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/fdmas.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/fdmas.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/interpolation.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/interpolation.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/pdas.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/pdas.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/probe_distances.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers/transmit_delays.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/beamformers_kernels.py` & `ultraspy-1.1/src/ultraspy/gpu/kernels/beamformers_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/color_map.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/color_map.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/correlation_matrix.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/mean_wall_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/poly_wall_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler/power_map.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler/power_map.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/doppler_kernels.py` & `ultraspy-1.1/src/ultraspy/gpu/kernels/doppler_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/by2.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/by2.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/convolve.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/convolve.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/divide_by.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/divide_by.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/flip.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/flip.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/get_modulo.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/get_modulo.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/median_filter.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/median_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators/to_db.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators/to_db.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/operators_kernels.py` & `ultraspy-1.1/src/ultraspy/gpu/kernels/operators_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal/down_mix.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/down_mix.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal/filter0.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/filter0.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_end_sig.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_end_sig.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_filter.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_filter.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal/init_start_sig.cu` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal/init_start_sig.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/signal_kernels.py` & `ultraspy-1.1/src/ultraspy/gpu/kernels/signal_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/kernels/utils.py` & `ultraspy-1.1/src/ultraspy/gpu/kernels/utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/post_processing.py` & `ultraspy-1.1/src/ultraspy/gpu/post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/gpu/signal.py` & `ultraspy-1.1/src/ultraspy/gpu/signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/helpers/doppler_helpers.py` & `ultraspy-1.1/src/ultraspy/helpers/doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/helpers/metrics_helpers.py` & `ultraspy-1.1/src/ultraspy/helpers/metrics_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/helpers/signal_helpers.py` & `ultraspy-1.1/src/ultraspy/helpers/signal_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/helpers/windows_helpers.py` & `ultraspy-1.1/src/ultraspy/helpers/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/io/file_loaders/factory.py` & `ultraspy-1.1/src/ultraspy/io/file_loaders/factory.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/io/file_loaders/file_loader.py` & `ultraspy-1.1/src/ultraspy/io/file_loaders/file_loader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/io/file_loaders/h5_loader.py` & `ultraspy-1.1/src/ultraspy/io/file_loaders/h5_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,12 +41,15 @@
             container[name] = {}
             for k, v in element.items():
                 self.store_element(v, container[name], k, skip)
         elif type(element) is h5py.Dataset:
             if name in skip:
                 logger.info(f"Skipped {name} while reading {self.filepath}.")
                 return
-            container[name] = np.array(element)
+            if element.shape:
+                container[name] = np.array(element)
+            else:
+                container[name] = element[()]
         else:
             raise TypeError(
                 f"Unknown data type while reading {self.filepath}: {name}, of "
                 f"type {type(element)}.")
```

### Comparing `ultraspy-1.0/src/ultraspy/io/file_loaders/mat_loader.py` & `ultraspy-1.1/src/ultraspy/io/file_loaders/mat_loader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/io/file_loaders/rff256_loader.py` & `ultraspy-1.1/src/ultraspy/io/file_loaders/rff256_loader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/io/reader.py` & `ultraspy-1.1/src/ultraspy/io/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     data_info, and the probe class, which can be used directly in the Beamformer
     class. Check their getters to learn more about them. You also can call
     :code:`Reader.available_systems` to have the list of the implemented
     ultrasound systems.
 
     Currently, the supported systems are:
 
+        - ultraspy: reads data formatted for the ultraspy library
         - picmus: reads data issued from the PICMUS challenge (
           creatis.insa-lyon.fr/Challenge/IEEE_IUS_2016)
         - must: reads the rotating disk data from MUST (biomecardio.com/MUST)
         - simus: data generated using the simulation tool SIMUS (biomecardio),
           contained RF and param
         - simu_3d: reads simulated 3d data from FieldII
         - dbsas: reads the data saved with the PA2 system of the company
@@ -46,29 +47,31 @@
         nb_elements, nb_time_samples). The number of elements can be 1D or
         2D when we are using a 3D probe
     :ivar dict data_info: The information about the data
     :ivar dict acquisition_info: The information about the acquisition setup
     :ivar dict probe: The probe class
     """
     available_systems = [
+        'ultraspy',
         'picmus',
         'must',
         'simus',
         'simu_3d',
         'dbsas',
         'vera',
         'ulaop',
     ]
 
-    def __init__(self, data_file, system, verbose=True):
+    def __init__(self, data_file, system='ultraspy', verbose=True):
         """It initializes the Reader class, using a given data file, known for
         being recorded using a given system.
 
         :param str data_file: The path where to find the data
-        :param str system: The name of the system to use
+        :param str system: The name of the system to use, default is the data
+            formatted for this library
         :param bool verbose: If True, we print a recap of the loaded data and
             of what has been extracted
         """
         if system not in self.available_systems:
             raise AttributeError(
                 f"Unknown system ({system}), please pick one among: "
                 f"{self.available_systems}.")
@@ -161,37 +164,90 @@
             file
         :param str system: The name of the system that has been used options
 
         :returns: The proper method to extract data
         :return type: function
         """
         return {
+            'ultraspy': self.__extract_ultraspy_data,
             'picmus': self.__extract_picmus_data,
             'must': self.__extract_must_data,
             'simus': self.__extract_simus_data,
             'simu_3d': self.__extract_simu_3d_data,
             'dbsas': self.__extract_dbsas_data,
             'vera': self.__extract_vera_data,
             'ulaop': self.__extract_ulaop_data,
         }[system](loaded_dict)
 
+    def __extract_ultraspy_data(self, loaded_dict):
+        """Extracts the relevant data, considering it has the format of the
+        ultraspy lib.
+
+        :param dict loaded_dict: The dictionary extracted from the data file
+        """
+        # Get the output data
+        data = loaded_dict['output']['data']
+
+        # Build the probe
+        probe_name = loaded_dict['probe']['name'].decode('utf-8')
+        if probe_name is not None:
+            probe = get_probe(probe_name)
+        else:
+            geometry = loaded_dict['probe']['geometry']
+            probe = build_probe_from_geometry(
+                geometry[0, :], geometry[1, :], geometry[2, :],
+                loaded_dict['probe']['central_freq'],
+                loaded_dict['probe']['bandwidth'])
+
+        # Sequences
+        emitted_sequence = loaded_dict['sequence']['emitted']
+        received_sequence = loaded_dict['sequence']['received']
+
+        # Acquisition
+        sampling_freq = loaded_dict['acquisition']['sampling_freq']
+        t0 = loaded_dict['acquisition']['t0']
+        prf = loaded_dict['acquisition']['prf']
+        signal_dur = loaded_dict['acquisition']['signal_duration']
+        sound_speed = loaded_dict['acquisition']['sound_speed']
+        delays = loaded_dict['acquisition']['delays']
+
+        # self.data = data.astype(np.int32)
+        self.data = data.astype(np.float32)
+        self.data_info = {
+            'data_shape': data.shape,
+            'data_type': np.float32,
+            'is_iq': False,
+        }
+        self.acquisition_info = {
+            'sampling_freq': sampling_freq,
+            't0': t0,
+            'prf': prf,
+            'signal_duration': signal_dur,
+            'delays': delays,
+            'sound_speed': sound_speed,
+            'sequence_elements': {
+                'emitted': emitted_sequence,
+                'received': received_sequence,
+            }
+        }
+        self.probe = probe
+
     def __extract_picmus_data(self, loaded_dict):
         """Extracts the relevant data, considering it is coming from Picmus.
 
         :param dict loaded_dict: The dictionary extracted from the data file
         """
         dataset = loaded_dict['US']['US_DATASET0000']
 
         # Identify the type of the data
         is_iq = dataset['data']['imag'].any()
 
         # Recover the data based on the format (I/Q, or RF)
         data = dataset['data']['real']
-        angles = np.concatenate([dataset['angles'][None, :],
-                                 np.zeros_like(dataset['angles'][None, :])])
+        angles = dataset['angles']
 
         probe = get_probe('L11-4v')
         file_f0 = dataset['sampling_frequency'][0] / 4
         if probe.central_freq != file_f0:
             logger.warning("The central frequency does not match the probe, "
                            f"update to {file_f0}, was {probe.central_freq}.")
             probe.set_central_freq(file_f0)
@@ -204,15 +260,16 @@
                                "is not a fourth of the sampling frequency.")
                 probe.set_central_freq(dataset['modulation_frequency'][0])
 
         # Compute the delays, in PICMUS, they are centered 2D plane waves
         speed_of_sound = dataset['sound_speed'][0]
         delays = compute_pw_delays(angles, probe,
                                    speed_of_sound=speed_of_sound,
-                                   transmission_mode='centered')
+                                   transmission_mode='centered',
+                                   smallest=False)
 
         # Adds an extra dimension for the number of frames (only one here)
         data = data[None, :]
         nb_transmissions = delays.shape[0]
         elements_indices = np.arange(probe.nb_elements)
 
         self.data = data
@@ -426,15 +483,15 @@
             'is_iq': False,
         }
         self.acquisition_info = {
             'sampling_freq': loaded_dict['setup']['Fs'][0, 0] * 1e6,
             't0': loaded_dict['setup']['startTime'][0, 0] * 1e-6,
             'prf': int(1 / (loaded_dict['setup']['timeSlot'][0, 0] * 1e-6)),
             'signal_duration': sig_dur,
-            'delays': delays,
+            'delays': np.take(delays, emitted),
             'sound_speed': speed_of_sound,
             'sequence_elements': {
                 'emitted': emitted,
                 'received': received,
             }
         }
         self.probe = probe
```

### Comparing `ultraspy-1.0/src/ultraspy/metrics.py` & `ultraspy-1.1/src/ultraspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/probes/convex_probe.py` & `ultraspy-1.1/src/ultraspy/probes/convex_probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/probes/factory.py` & `ultraspy-1.1/src/ultraspy/probes/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,61 +47,67 @@
     # Geometry of the probe must be supported
     assert geometry_type in ['linear', 'convex', 'matricial'], \
         "Unknown geometry type, please pick either 'linear', 'convex' or " \
         "'matricial'."
 
     if geometry_type == 'matricial':
         nb_elements = json.loads(config.get('Geometry', 'nb_elements'))
+        pitches = json.loads(config.get('Geometry', 'pitch'))
         empty_lines = json.loads(config.get('Geometry', 'empty_lines'))
         nb_elements = list(map(int, nb_elements))
+        pitch = list(pitches)
         empty_lines = list(map(int, empty_lines))
     else:
         nb_elements = config.getint('Geometry', 'nb_elements')
+        pitch = config.getfloat('Geometry', 'pitch')
         empty_lines = None
 
     config_dict = {
         'name': config.get('General', 'name'),
         'nb_elements': nb_elements,
-        'pitch': config.getfloat('Geometry', 'pitch'),
+        'pitch': pitch,
         'radius': config.getfloat('Geometry', 'radius', fallback=None),
         'empty_lines': empty_lines,
         'central_freq': config.getfloat('Transmission', 'central_freq'),
         'bandwidth': config.getfloat('Transmission', 'bandwidth'),
     }
 
     return {
         'linear': LinearProbe,
         'convex': ConvexProbe,
         'matricial': MatricialProbe,
     }[geometry_type](config_dict)
 
 
 def build_probe(geometry_type, nb_elements, pitch, central_freq,
-                bandwidth=None, radius=None):
+                bandwidth=None, radius=None, empty_lines=None):
     """Builds a probe based on its characteristics, is used when we load data
     from a file with unknown probe name. Not so clean tho.
 
     :ivar str geometry_type: The type of the probe (either linear, convex or
         matricial). Is defined by child
-    :ivar int nb_elements: The total number of piezo-electric elements in
-        the probe
-    :ivar float pitch: The space, in m, between two piezo-electric components
+    :ivar int, list nb_elements: The total number of piezo-electric elements in
+        the probe, 2D if matricial
+    :ivar float, list pitch: The space, in m, between two piezo-electric
+        components, 2D if matricial
     :ivar float central_freq: The central frequency of the probe, in Hz
     :ivar float bandwidth: The bandwidth of the probe (should be between 0 and
         200%), in %
     :ivar float radius: The radius of the curvature, in m
+    :ivar list empty_lines: The steps for the matricial empty lines, 2D
 
     :returns: The Probe class with the main info (central freq, coordinates of
         elements, etc)
     :return type: LinearProbe, ConvexProbe, MatricialProbe
     """
     config_dict = {
         'nb_elements': nb_elements,
         'pitch': pitch,
         'radius': radius,
+        'empty_lines': empty_lines,
         'central_freq': central_freq,
         'bandwidth': bandwidth,
     }
 
     return {
         'linear': LinearProbe,
         'convex': ConvexProbe,
```

### Comparing `ultraspy-1.0/src/ultraspy/probes/linear_probe.py` & `ultraspy-1.1/src/ultraspy/probes/linear_probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/probes/matricial_probe.py` & `ultraspy-1.1/src/ultraspy/probes/matricial_probe.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,17 @@
             gap_y = 0
             if ex > 0:
                 gap_x = nx // ex - (1 if nx // ex == nx / ex else 0)
             if ey > 0:
                 gap_y = ny // ey - (1 if ny // ey == ny / ey else 0)
             real_x = nx + gap_x
             real_y = ny + gap_y
-            pitch = config['pitch']
-            xnbs = (np.arange(real_x) - ((real_x - 1) / 2)) * pitch
-            ynbs = (np.arange(real_y) - ((real_y - 1) / 2)) * pitch
+            pitch_x, pitch_y = config['pitch']
+            xnbs = (np.arange(real_x) - ((real_x - 1) / 2)) * pitch_x
+            ynbs = (np.arange(real_y) - ((real_y - 1) / 2)) * pitch_y
             empty_x = [ex * (i + 1) + i for i in range(gap_x)]
             empty_y = [ey * (i + 1) + i for i in range(gap_y)]
             xnbs = np.delete(xnbs, empty_x)
             ynbs = np.delete(ynbs, empty_y)
             xx, yy = np.meshgrid(xnbs, ynbs)
             self._geometry[0, :] = xx.flatten()
             self._geometry[1, :] = yy.flatten()
```

### Comparing `ultraspy-1.0/src/ultraspy/probes/probe.py` & `ultraspy-1.1/src/ultraspy/probes/probe.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/scan.py` & `ultraspy-1.1/src/ultraspy/scan.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/beamformers.py` & `ultraspy-1.1/src/ultraspy/utils/beamformers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/linear_decomposition.py` & `ultraspy-1.1/src/ultraspy/utils/linear_decomposition.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/masks.py` & `ultraspy-1.1/src/ultraspy/utils/masks.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/matplot.py` & `ultraspy-1.1/src/ultraspy/utils/matplot.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/print.py` & `ultraspy-1.1/src/ultraspy/utils/print.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy/utils/string.py` & `ultraspy-1.1/src/ultraspy/utils/string.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/src/ultraspy.egg-info/PKG-INFO` & `ultraspy-1.1/src/ultraspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultraspy
-Version: 1.0
+Version: 1.1
 Summary: Ultrasound toolbox for GPU
 Home-page: https://gitlab.com/pecarlat/ultraspy
 Author: Pierre Ecarlat
 Author-email: pierre.ecarlat@gmail.com
 Project-URL: Documentation, https://ultraspy.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/pecarlat/ultraspy/-/issues/
 Keywords: ultrasound,python,beamforming,doppler
```

### Comparing `ultraspy-1.0/tests/conftest.py` & `ultraspy-1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/beamformers/test_beamformer.py` & `ultraspy-1.1/tests/test_cpu/beamformers/test_beamformer.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/beamformers/test_das.py` & `ultraspy-1.1/tests/test_cpu/beamformers/test_das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/beamformers/test_fdmas.py` & `ultraspy-1.1/tests/test_cpu/beamformers/test_fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/beamformers/test_pdas.py` & `ultraspy-1.1/tests/test_cpu/beamformers/test_pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/helpers/test_doppler_helpers.py` & `ultraspy-1.1/tests/test_cpu/helpers/test_doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/helpers/test_signal_helpers.py` & `ultraspy-1.1/tests/test_cpu/helpers/test_signal_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/helpers/test_windows_helpers.py` & `ultraspy-1.1/tests/test_cpu/helpers/test_windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/io/test_reader.py` & `ultraspy-1.1/tests/test_cpu/io/test_reader.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_doppler.py` & `ultraspy-1.1/tests/test_cpu/test_doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_metrics.py` & `ultraspy-1.1/tests/test_cpu/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_post_processing.py` & `ultraspy-1.1/tests/test_cpu/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_probes.py` & `ultraspy-1.1/tests/test_cpu/test_probes.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_scan.py` & `ultraspy-1.1/tests/test_cpu/test_scan.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/test_signal.py` & `ultraspy-1.1/tests/test_cpu/test_signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/utils/test_linear_decomposition.py` & `ultraspy-1.1/tests/test_cpu/utils/test_linear_decomposition.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_cpu/utils/test_masks.py` & `ultraspy-1.1/tests/test_cpu/utils/test_masks.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/beamformers/test_beamformer.py` & `ultraspy-1.1/tests/test_gpu/beamformers/test_beamformer.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/beamformers/test_das.py` & `ultraspy-1.1/tests/test_gpu/beamformers/test_das.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/beamformers/test_fdmas.py` & `ultraspy-1.1/tests/test_gpu/beamformers/test_fdmas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/beamformers/test_pdas.py` & `ultraspy-1.1/tests/test_gpu/beamformers/test_pdas.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/helpers/test_doppler_helpers.py` & `ultraspy-1.1/tests/test_gpu/helpers/test_doppler_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/helpers/test_signal_helpers.py` & `ultraspy-1.1/tests/test_gpu/helpers/test_signal_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/helpers/test_windows_helpers.py` & `ultraspy-1.1/tests/test_gpu/helpers/test_windows_helpers.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/kernels/test_doppler_kernels.py` & `ultraspy-1.1/tests/test_gpu/kernels/test_doppler_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/kernels/test_operators_kernels.py` & `ultraspy-1.1/tests/test_gpu/kernels/test_operators_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/kernels/test_signal_kernels.py` & `ultraspy-1.1/tests/test_gpu/kernels/test_signal_kernels.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/test_doppler.py` & `ultraspy-1.1/tests/test_gpu/test_doppler.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/test_filtfilts.py` & `ultraspy-1.1/tests/test_gpu/test_filtfilts.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/test_gpu_utils.py` & `ultraspy-1.1/tests/test_gpu/test_gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/test_signal.py` & `ultraspy-1.1/tests/test_gpu/test_signal.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tests/test_gpu/utils/test_linear_decomposition.py` & `ultraspy-1.1/tests/test_gpu/utils/test_linear_decomposition.py`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/tox.ini` & `ultraspy-1.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 000000e0: 203d 0d0a 2020 2020 5059 5448 4f4e 5041   =..    PYTHONPA
 000000f0: 5448 3d7b 746f 7869 6e69 6469 727d 2f73  TH={toxinidir}/s
 00000100: 7263 0d0a 2020 2020 3b20 556e 636f 6d6d  rc..    ; Uncomm
 00000110: 656e 7420 7468 6973 206c 696e 6520 746f  ent this line to
 00000120: 2074 6573 7420 7468 6520 4350 5520 7665   test the CPU ve
 00000130: 7273 696f 6e20 7573 696e 6720 4e75 6d70  rsion using Nump
 00000140: 7920 696e 7374 6561 6420 6f66 204e 756d  y instead of Num
-00000150: 6261 0d0a 2020 2020 554c 5452 4153 5059  ba..    ULTRASPY
-00000160: 5f43 5055 5f4c 4942 3d6e 756d 7079 0d0a  _CPU_LIB=numpy..
-00000170: 2020 2020 3b20 556e 636f 6d6d 656e 7420      ; Uncomment 
-00000180: 7468 6973 206c 696e 6520 746f 2073 6b69  this line to ski
-00000190: 7020 7468 6520 6d6f 7374 2068 6561 7679  p the most heavy
-000001a0: 2074 6573 7473 0d0a 2020 2020 3b48 4541   tests..    ;HEA
-000001b0: 5659 5f54 4553 543d 4661 6c73 650d 0a0d  VY_TEST=False...
-000001c0: 0a69 6e73 7461 6c6c 5f63 6f6d 6d61 6e64  .install_command
-000001d0: 203d 0d0a 2020 2020 7069 7020 696e 7374   =..    pip inst
-000001e0: 616c 6c20 7b6f 7074 737d 207b 7061 636b  all {opts} {pack
-000001f0: 6167 6573 7d0d 0a0d 0a64 6570 7320 3d0d  ages}....deps =.
-00000200: 0a20 2020 2063 7075 5f74 6573 7473 2c67  .    cpu_tests,g
-00000210: 7075 5f74 6573 7473 2c64 6f63 733a 202d  pu_tests,docs: -
-00000220: 727b 746f 7869 6e69 6469 727d 2f72 6571  r{toxinidir}/req
-00000230: 7569 7265 6d65 6e74 735f 6370 752e 7478  uirements_cpu.tx
-00000240: 740d 0a20 2020 2067 7075 5f74 6573 7473  t..    gpu_tests
-00000250: 3a20 2d72 7b74 6f78 696e 6964 6972 7d2f  : -r{toxinidir}/
-00000260: 7265 7175 6972 656d 656e 7473 5f67 7075  requirements_gpu
-00000270: 2e74 7874 0d0a 0d0a 636f 6d6d 616e 6473  .txt....commands
-00000280: 203d 0d0a 2020 2020 6370 755f 7465 7374   =..    cpu_test
-00000290: 733a 2070 7974 6573 7420 7465 7374 732f  s: pytest tests/
-000002a0: 7465 7374 5f63 7075 0d0a 2020 2020 6770  test_cpu..    gp
-000002b0: 755f 7465 7374 733a 2070 7974 6573 7420  u_tests: pytest 
-000002c0: 7465 7374 732f 7465 7374 5f67 7075 0d0a  tests/test_gpu..
-000002d0: 2020 2020 646f 6373 3a20 7370 6869 6e78      docs: sphinx
-000002e0: 2d62 7569 6c64 202d 5720 2d62 2068 746d  -build -W -b htm
-000002f0: 6c20 2d64 2064 6973 742f 646f 6373 2f64  l -d dist/docs/d
-00000300: 6f63 7472 6565 7320 646f 6373 2064 6973  octrees docs dis
-00000310: 742f 646f 6373 2f68 746d 6c0d 0a         t/docs/html..
+00000150: 6261 0d0a 2020 2020 3b55 4c54 5241 5350  ba..    ;ULTRASP
+00000160: 595f 4350 555f 4c49 423d 6e75 6d70 790d  Y_CPU_LIB=numpy.
+00000170: 0a20 2020 203b 2055 6e63 6f6d 6d65 6e74  .    ; Uncomment
+00000180: 2074 6869 7320 6c69 6e65 2074 6f20 736b   this line to sk
+00000190: 6970 2074 6865 206d 6f73 7420 6865 6176  ip the most heav
+000001a0: 7920 7465 7374 730d 0a20 2020 203b 4845  y tests..    ;HE
+000001b0: 4156 595f 5445 5354 3d46 616c 7365 0d0a  AVY_TEST=False..
+000001c0: 0d0a 696e 7374 616c 6c5f 636f 6d6d 616e  ..install_comman
+000001d0: 6420 3d0d 0a20 2020 2070 6970 2069 6e73  d =..    pip ins
+000001e0: 7461 6c6c 207b 6f70 7473 7d20 7b70 6163  tall {opts} {pac
+000001f0: 6b61 6765 737d 0d0a 0d0a 6465 7073 203d  kages}....deps =
+00000200: 0d0a 2020 2020 6370 755f 7465 7374 732c  ..    cpu_tests,
+00000210: 6770 755f 7465 7374 732c 646f 6373 3a20  gpu_tests,docs: 
+00000220: 2d72 7b74 6f78 696e 6964 6972 7d2f 7265  -r{toxinidir}/re
+00000230: 7175 6972 656d 656e 7473 5f63 7075 2e74  quirements_cpu.t
+00000240: 7874 0d0a 2020 2020 6770 755f 7465 7374  xt..    gpu_test
+00000250: 733a 202d 727b 746f 7869 6e69 6469 727d  s: -r{toxinidir}
+00000260: 2f72 6571 7569 7265 6d65 6e74 735f 6770  /requirements_gp
+00000270: 752e 7478 740d 0a0d 0a63 6f6d 6d61 6e64  u.txt....command
+00000280: 7320 3d0d 0a20 2020 2063 7075 5f74 6573  s =..    cpu_tes
+00000290: 7473 3a20 7079 7465 7374 2074 6573 7473  ts: pytest tests
+000002a0: 2f74 6573 745f 6370 750d 0a20 2020 2067  /test_cpu..    g
+000002b0: 7075 5f74 6573 7473 3a20 7079 7465 7374  pu_tests: pytest
+000002c0: 2074 6573 7473 2f74 6573 745f 6770 750d   tests/test_gpu.
+000002d0: 0a20 2020 2064 6f63 733a 2073 7068 696e  .    docs: sphin
+000002e0: 782d 6275 696c 6420 2d57 202d 6220 6874  x-build -W -b ht
+000002f0: 6d6c 202d 6420 6469 7374 2f64 6f63 732f  ml -d dist/docs/
+00000300: 646f 6374 7265 6573 2064 6f63 7320 6469  doctrees docs di
+00000310: 7374 2f64 6f63 732f 6874 6d6c 0d0a       st/docs/html..
```

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/cub/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/_core/include/cupy/jitify/jitify_test.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_cub.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cub.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_cufftXt.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/cuda/cupy_thrust.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/cuda/cupy_thrust.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/cupy/random/cupy_distributions.cu` & `ultraspy-1.1/.tox/py310-gpu_tests/Lib/site-packages/cupy/random/cupy_distributions.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu` & `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/cpp_function_wrappers.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/data/jitlink.cu` & `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/data/jitlink.cu`

 * *Files identical despite different names*

### Comparing `ultraspy-1.0/venv/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu` & `ultraspy-1.1/.tox/py38-cpu_tests/Lib/site-packages/numba/cuda/tests/doc_examples/ffi/functions.cu`

 * *Files identical despite different names*

