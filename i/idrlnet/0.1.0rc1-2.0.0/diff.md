# Comparing `tmp/idrlnet-0.1.0rc1.tar.gz` & `tmp/idrlnet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/idrlnet-0.1.0rc1.tar", last modified: Fri Aug 12 09:27:02 2022, max compression
+gzip compressed data, was "dist/idrlnet-2.0.0.tar", last modified: Fri Jun 30 08:50:18 2023, max compression
```

## Comparing `idrlnet-0.1.0rc1.tar` & `idrlnet-2.0.0.tar`

### file list

```diff
@@ -1,102 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/modules/idrlnet.architecture.rst
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/modules/idrlnet.geo_utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/modules/idrlnet.pde_op.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/modules/idrlnet.rst
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/modules/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/docs/user/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/cite_idrlnet.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/docs/user/get_started/
--rw-r--r--   0 runner    (1001) docker     (121)     8978 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/1_simple_poisson.md
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/2_euler_beam.md
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/3_burgers_equation.md
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/4_allen_cahn.md
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/5_inverse_wave_equation.md
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/6_parameterized_poisson.md
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/7_minimal_surface.md
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/8_volterra_ide.md
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/get_started/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/installation.md
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/docs/user/team.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/Volterra_IDE/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/Volterra_IDE/readme.md
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/Volterra_IDE/volterra_ide.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/allen_cahn/
--rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/allen_cahn/allen_cahn.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/allen_cahn/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/burgers_equation/
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/burgers_equation/burgers_equation.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/burgers_equation/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/consolidation/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/consolidation/Aana.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/consolidation/Boneside_pinn.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/consolidation/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/euler_beam/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/euler_beam/euler_beam.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/euler_beam/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/holes_heat_flux/
--rw-r--r--   0 runner    (1001) docker     (121)     8324 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/holes_heat_flux/holes_heat_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/inverse_wave_equation/
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/inverse_wave_equation/inverse_wave_equation.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/inverse_wave_equation/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/ldc/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4427 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/ldc/ldc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/minimal_surface_of_revolution.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/minimal_surface_of_revolution_pretrain.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/parameterized_poisson/
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/parameterized_poisson/parameterized_poisson.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/parameterized_poisson/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/examples/simple_poisson/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/simple_poisson/readme.md
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/examples/simple_poisson/simple_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet/architecture/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/architecture/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/architecture/layer.py
--rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/architecture/mlp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6926 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14373 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/geo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/geo_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    26096 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/geo_obj.py
--rw-r--r--   0 runner    (1001) docker     (121)     4856 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/geo_utils/sympy_np.py
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/net.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/optim.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/pde.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet/pde_op/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/pde_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6184 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/pde_op/equations.py
--rw-r--r--   0 runner    (1001) docker     (121)    12956 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/pde_op/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/receivers.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (121)    19799 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/torch_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     9469 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/idrlnet/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/idrlnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 09:27:02.000000 idrlnet-0.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-08-12 09:26:54.000000 idrlnet-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-30 08:50:04.000000 idrlnet-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 08:50:04.000000 idrlnet-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-30 08:50:18.000000 idrlnet-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-30 08:50:04.000000 idrlnet-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/modules/idrlnet.architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/modules/idrlnet.geo_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/modules/idrlnet.pde_op.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/modules/idrlnet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/modules/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/cite_idrlnet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/docs/user/get_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/10_deepritz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/1_simple_poisson.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/2_euler_beam.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/3_burgers_equation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/4_allen_cahn.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/5_inverse_wave_equation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/6_parameterized_poisson.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/7_minimal_surface.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/8_volterra_ide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/9_navier_stokes_equation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/get_started/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 08:50:04.000000 idrlnet-2.0.0/docs/user/team.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/Volterra_IDE/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/Volterra_IDE/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/Volterra_IDE/volterra_ide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/allen_cahn/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/allen_cahn/allen_cahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/allen_cahn/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/burgers_equation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/burgers_equation/burgers_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/burgers_equation/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/consolidation/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/consolidation/Aana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/consolidation/Boneside_pinn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/consolidation/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/deepritz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/deepritz/deepritz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/euler_beam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/euler_beam/euler_beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/euler_beam/euler_beam_lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/euler_beam/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/holes_heat_flux/
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/holes_heat_flux/holes_heat_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/inverse_wave_equation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/inverse_wave_equation/inverse_wave_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/inverse_wave_equation/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/ldc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ldc/ldc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/minimal_surface_of_revolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/minimal_surface_of_revolution/minimal_surface_of_revolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/minimal_surface_of_revolution/minimal_surface_of_revolution_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/minimal_surface_of_revolution/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/ns_steady/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_steady/NS_steady.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332902 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_steady/NSexternel_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1284985 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_steady/NSexternel_test.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/ns_unsteady/
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_unsteady/NS_unsteady.py
+-rw-r--r--   0 runner    (1001) docker     (123)   636411 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_unsteady/NSexternel_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   615806 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/ns_unsteady/NSexternel_test.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/parameterized_poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/parameterized_poisson/parameterized_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/parameterized_poisson/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/examples/simple_poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/simple_poisson/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-30 08:50:04.000000 idrlnet-2.0.0/examples/simple_poisson/simple_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/architecture/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/architecture/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/architecture/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet/geo_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/geo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/geo_utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/geo_utils/geo_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26096 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/geo_utils/geo_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/geo_utils/sympy_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet/pde_op/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/pde_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/pde_op/equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/pde_op/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/torch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-06-30 08:50:04.000000 idrlnet-2.0.0/idrlnet/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 08:50:18.000000 idrlnet-2.0.0/idrlnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:50:18.000000 idrlnet-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-30 08:50:04.000000 idrlnet-2.0.0/setup.py
```

### Comparing `idrlnet-0.1.0rc1/LICENSE` & `idrlnet-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/PKG-INFO` & `idrlnet-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: idrlnet
-Version: 0.1.0rc1
+Version: 2.0.0
 Summary: IDRLnet
 Home-page: https://github.com/idrl-lab/idrlnet
 Author: Intelligent Design & Robust Learning lab
 Author-email: weipeng@deepinfar.cn
 License: UNKNOWN
 Description: # IDRLnet
         
         [![License](https://img.shields.io/github/license/analysiscenter/pydens.svg)](https://www.apache.org/licenses/LICENSE-2.0)
         [![Python](https://img.shields.io/badge/python-3.7/3.8/3.9-blue.svg)](https://python.org)
         [![Documentation Status](https://readthedocs.org/projects/idrlnet/badge/?version=latest)](https://idrlnet.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/idrlnet.svg)](https://badge.fury.io/py/idrlnet)
         [![DockerHub](https://img.shields.io/docker/pulls/idrl/idrlnet.svg)](https://hub.docker.com/r/idrl/idrlnet)
         [![CodeFactor](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/badge/master)](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/overview/master)
         
-        
-        **IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine
-        learning library that solves both forward and inverse differential equations via physics-informed neural
-        networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
+        **IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine learning library that solves both forward and inverse differential equations via physics-informed neural networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
         
         ## Docs
         
         - [Full docs](https://idrlnet.readthedocs.io/en/latest/)
         - [Tutorial](https://idrlnet.readthedocs.io/en/latest/user/get_started/tutorial.html)
         - Paper:
            - IDRLnet: A Physics-Informed Neural Network Library. [arXiv](https://arxiv.org/abs/2107.04320)
@@ -70,29 +67,35 @@
         ```
         
         
         ## Features
         
         IDRLnet supports
         
-        -  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon,
-           circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and
-           intersection;
-        
-        -  sampling in the interior of the defined geometry or on the boundary with given conditions.
-        
-        -  enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph
-           will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via
-           explicit expressions, users model problems more naturally.
+        -  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon, circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and intersection;
+           ![Geometry](https://raw.githubusercontent.com/weipeng0098/picture/master/20210617081809.png)
+           
+        - sampling in the interior of the defined geometry or on the boundary with given conditions.
         
-        -  solving variational minimization problem;
+        - enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via explicit expressions, users model problems more naturally.
         
-        -  solving integral differential equation;
+        - builds computational graph automatically;
         
-        -  adaptive resampling;
+           ![computationDomain](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142531.png)
+        
+        -  user-defined callbacks;
+           
+           ![callback](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142621.png)
+           
+        -  solving variational minimization problem;
+           <img src="https://raw.githubusercontent.com/weipeng0098/picture/master/20210617082331.gif" alt="miniface" style="zoom:33%;" />
+           
+        - solving integral differential equation;
+        
+        - adaptive resampling;
         
         -  recover unknown parameters of PDEs from noisy measurement data.
         
         It is also easy to customize IDRLnet to meet new demands.
         
         -  Main Dependencies
         
@@ -103,20 +106,18 @@
         
         ## Contributing to IDRLnet
         
         First off, thanks for taking the time to contribute!
         
         -  **Reporting bugs.** To report a bug, simply open an issue in the GitHub "Issues" section.
         
-        -  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and
-           minor improvements to existing functionality, let us know by opening an issue.
-        
-        -  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a
-           pull-request.
-        
+        -  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and minor improvements to existing functionality, let us know by opening an issue.
+           
+        -  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a pull-request.
+           
         -  **Asking questions.** To get help on how to use IDRLnet or its functionalities, you can as well open an issue.
         
         -  **Answering questions.** If you know the answer to any question in the "Issues", you are welcomed to answer.
         
         ## The Team
         
         IDRLnet was originally developed by IDRL lab.
```

### Comparing `idrlnet-0.1.0rc1/README.md` & `idrlnet-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 [![License](https://img.shields.io/github/license/analysiscenter/pydens.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![Python](https://img.shields.io/badge/python-3.7/3.8/3.9-blue.svg)](https://python.org)
 [![Documentation Status](https://readthedocs.org/projects/idrlnet/badge/?version=latest)](https://idrlnet.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/idrlnet.svg)](https://badge.fury.io/py/idrlnet)
 [![DockerHub](https://img.shields.io/docker/pulls/idrl/idrlnet.svg)](https://hub.docker.com/r/idrl/idrlnet)
 [![CodeFactor](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/badge/master)](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/overview/master)
 
-
-**IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine
-learning library that solves both forward and inverse differential equations via physics-informed neural
-networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
+**IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine learning library that solves both forward and inverse differential equations via physics-informed neural networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
 
 ## Docs
 
 - [Full docs](https://idrlnet.readthedocs.io/en/latest/)
 - [Tutorial](https://idrlnet.readthedocs.io/en/latest/user/get_started/tutorial.html)
 - Paper:
    - IDRLnet: A Physics-Informed Neural Network Library. [arXiv](https://arxiv.org/abs/2107.04320)
@@ -62,29 +59,35 @@
 ```
 
 
 ## Features
 
 IDRLnet supports
 
--  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon,
-   circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and
-   intersection;
-
--  sampling in the interior of the defined geometry or on the boundary with given conditions.
-
--  enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph
-   will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via
-   explicit expressions, users model problems more naturally.
+-  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon, circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and intersection;
+   ![Geometry](https://raw.githubusercontent.com/weipeng0098/picture/master/20210617081809.png)
+   
+- sampling in the interior of the defined geometry or on the boundary with given conditions.
 
--  solving variational minimization problem;
+- enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via explicit expressions, users model problems more naturally.
 
--  solving integral differential equation;
+- builds computational graph automatically;
 
--  adaptive resampling;
+   ![computationDomain](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142531.png)
+
+-  user-defined callbacks;
+   
+   ![callback](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142621.png)
+   
+-  solving variational minimization problem;
+   <img src="https://raw.githubusercontent.com/weipeng0098/picture/master/20210617082331.gif" alt="miniface" style="zoom:33%;" />
+   
+- solving integral differential equation;
+
+- adaptive resampling;
 
 -  recover unknown parameters of PDEs from noisy measurement data.
 
 It is also easy to customize IDRLnet to meet new demands.
 
 -  Main Dependencies
 
@@ -95,20 +98,18 @@
 
 ## Contributing to IDRLnet
 
 First off, thanks for taking the time to contribute!
 
 -  **Reporting bugs.** To report a bug, simply open an issue in the GitHub "Issues" section.
 
--  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and
-   minor improvements to existing functionality, let us know by opening an issue.
-
--  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a
-   pull-request.
-
+-  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and minor improvements to existing functionality, let us know by opening an issue.
+   
+-  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a pull-request.
+   
 -  **Asking questions.** To get help on how to use IDRLnet or its functionalities, you can as well open an issue.
 
 -  **Answering questions.** If you know the answer to any question in the "Issues", you are welcomed to answer.
 
 ## The Team
 
 IDRLnet was originally developed by IDRL lab.
```

### Comparing `idrlnet-0.1.0rc1/docs/Makefile` & `idrlnet-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/conf.py` & `idrlnet-2.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
 
 project = "idrlnet"
-copyright = "2021, IDRL"
+copyright = "2023, IDRL"
 author = "IDRL"
 
 # The full version, including alpha/beta/rc tags
-release = "0.1.0-rc1"
+release = "2.0.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `idrlnet-0.1.0rc1/docs/index.rst` & `idrlnet-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/make.bat` & `idrlnet-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/modules/idrlnet.architecture.rst` & `idrlnet-2.0.0/docs/modules/idrlnet.architecture.rst`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/modules/idrlnet.geo_utils.rst` & `idrlnet-2.0.0/docs/modules/idrlnet.geo_utils.rst`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/modules/idrlnet.rst` & `idrlnet-2.0.0/docs/modules/idrlnet.rst`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/1_simple_poisson.md` & `idrlnet-2.0.0/docs/user/get_started/1_simple_poisson.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/2_euler_beam.md` & `idrlnet-2.0.0/docs/user/get_started/2_euler_beam.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/3_burgers_equation.md` & `idrlnet-2.0.0/docs/user/get_started/3_burgers_equation.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/4_allen_cahn.md` & `idrlnet-2.0.0/docs/user/get_started/4_allen_cahn.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/5_inverse_wave_equation.md` & `idrlnet-2.0.0/docs/user/get_started/5_inverse_wave_equation.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/6_parameterized_poisson.md` & `idrlnet-2.0.0/docs/user/get_started/6_parameterized_poisson.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/7_minimal_surface.md` & `idrlnet-2.0.0/docs/user/get_started/7_minimal_surface.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/8_volterra_ide.md` & `idrlnet-2.0.0/docs/user/get_started/8_volterra_ide.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/docs/user/get_started/tutorial.rst` & `idrlnet-2.0.0/docs/user/get_started/tutorial.rst`

 * *Files 17% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 3. :ref:`Burgers' Equation <Burgers' Equation>`. The case presents how to include ``time`` in the sampling domains.
 4. :ref:`Allen-Cahn Equation <Allen-Cahn Equation>`. The example introduces the representation of periodic boundary conditions.
    ``Receiver`` acting as ``callbacks`` are also introduced, including implementing user-defined algorithms and post-processing during the training.
 5. :ref:`Inverse wave equation <Inverse Wave Equation>`. The example introduces how to discover unknown parameters in PDEs.
 6. :ref:`Parameterized poisson equation <Parameterized Poisson>`. The example introduces how to train a surrogate with parameters.
 7. :ref:`Variational Minimization <Variational Minimization>`. The example introduces how to solve variational minimization problems.
 8. :ref:`Volterra integral differential equation <Volterra Integral Differential Equation>`. The example introduces the way to solve IDEs.
+9. :ref:`Navier-Stokes equation <Navier-Stokes equations>`. The example introduces how to use the LBFGS optimizer.
+10. :ref:`Deepritz method <Deepritz>`. The example introduces the way to solve PDEs with the Deepritz method.
 
 
 
 .. toctree::
    :maxdepth: 2
 
    1_simple_poisson
    2_euler_beam
    3_burgers_equation
    4_allen_cahn
    5_inverse_wave_equation
    6_parameterized_poisson
    7_minimal_surface
    8_volterra_ide
+   9_navier_stokes_equation
+   10_deepritz
```

### Comparing `idrlnet-0.1.0rc1/docs/user/installation.md` & `idrlnet-2.0.0/docs/user/installation.md`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/Volterra_IDE/volterra_ide.py` & `idrlnet-2.0.0/examples/Volterra_IDE/volterra_ide.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/allen_cahn/allen_cahn.py` & `idrlnet-2.0.0/examples/allen_cahn/allen_cahn.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/burgers_equation/burgers_equation.py` & `idrlnet-2.0.0/examples/burgers_equation/burgers_equation.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/consolidation/Aana.py` & `idrlnet-2.0.0/examples/consolidation/Aana.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/consolidation/Boneside_pinn.py` & `idrlnet-2.0.0/examples/consolidation/Boneside_pinn.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/euler_beam/euler_beam.py` & `idrlnet-2.0.0/examples/euler_beam/euler_beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         LeftBoundary1(),
         LeftBoundary2(),
         RightBoundary1(),
         RightBoundary2(),
     ),
     netnodes=[net],
     pdes=[pde1, pde2, pde3, pde4],
-    max_iter=2000,
-)
+    max_iter=2000)
 solver.solve()
 
 
 # inference
 def exact(x):
     return -(x ** 4) / 24 + x ** 3 / 6 - x ** 2 / 4
```

### Comparing `idrlnet-0.1.0rc1/examples/holes_heat_flux/holes_heat_flux.py` & `idrlnet-2.0.0/examples/holes_heat_flux/holes_heat_flux.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/inverse_wave_equation/inverse_wave_equation.py` & `idrlnet-2.0.0/examples/inverse_wave_equation/inverse_wave_equation.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/ldc/ldc.py` & `idrlnet-2.0.0/examples/ldc/ldc.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/minimal_surface_of_revolution.py` & `idrlnet-2.0.0/examples/minimal_surface_of_revolution/minimal_surface_of_revolution.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/minimal_surface_of_revolution/minimal_surface_of_revolution_pretrain.py` & `idrlnet-2.0.0/examples/minimal_surface_of_revolution/minimal_surface_of_revolution_pretrain.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/parameterized_poisson/parameterized_poisson.py` & `idrlnet-2.0.0/examples/parameterized_poisson/parameterized_poisson.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/examples/simple_poisson/simple_poisson.py` & `idrlnet-2.0.0/examples/simple_poisson/simple_poisson.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/__init__.py` & `idrlnet-2.0.0/idrlnet/__init__.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/architecture/grid.py` & `idrlnet-2.0.0/idrlnet/architecture/grid.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/architecture/layer.py` & `idrlnet-2.0.0/idrlnet/architecture/layer.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/architecture/mlp.py` & `idrlnet-2.0.0/idrlnet/architecture/mlp.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/callbacks.py` & `idrlnet-2.0.0/idrlnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/data.py` & `idrlnet-2.0.0/idrlnet/data.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/geo_utils/geo.py` & `idrlnet-2.0.0/idrlnet/geo_utils/geo.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/geo_utils/geo_builder.py` & `idrlnet-2.0.0/idrlnet/geo_utils/geo_builder.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/geo_utils/geo_obj.py` & `idrlnet-2.0.0/idrlnet/geo_utils/geo_obj.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/geo_utils/sympy_np.py` & `idrlnet-2.0.0/idrlnet/geo_utils/sympy_np.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/graph.py` & `idrlnet-2.0.0/idrlnet/graph.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/header.py` & `idrlnet-2.0.0/idrlnet/header.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/net.py` & `idrlnet-2.0.0/idrlnet/net.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/node.py` & `idrlnet-2.0.0/idrlnet/node.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/optim.py` & `idrlnet-2.0.0/idrlnet/optim.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/pde.py` & `idrlnet-2.0.0/idrlnet/pde.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/pde_op/equations.py` & `idrlnet-2.0.0/idrlnet/pde_op/equations.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/pde_op/operator.py` & `idrlnet-2.0.0/idrlnet/pde_op/operator.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/receivers.py` & `idrlnet-2.0.0/idrlnet/receivers.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/shortcut.py` & `idrlnet-2.0.0/idrlnet/shortcut.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/solver.py` & `idrlnet-2.0.0/idrlnet/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -308,26 +308,45 @@
 
     def train_pipe(self):
         """Sample once; calculate the loss once; backward propagation once
         :return: None
         """
         self.notify(self, message={Signal.TRAIN_PIPE_START: "defaults"})
         for opt in self.optimizers:
-            opt.zero_grad()
+            # print('Running optimization with %s'%(self.optimizer_config['optimizer']))
+            if self.optimizer_config['optimizer'] == 'LBFGS':
+                def closure():
+                    opt.zero_grad()
+                    samples = self.sample_variables_from_domains()
+                    in_var, true_out, lambda_out = self.generate_in_out_dict(samples)
+                    pred_out_sample = self.forward_through_all_graph(in_var, self.outvar_dict_index)
+                    loss = self.compute_loss(in_var, pred_out_sample, true_out, lambda_out)
+                    self.notify(self, message={Signal.BEFORE_BACKWARD: 'defaults'})
+                    loss.backward()
+                    return loss
+                opt.step(closure)
+
+            else:
+                opt.zero_grad()
+                samples = self.sample_variables_from_domains()
+                in_var, true_out, lambda_out = self.generate_in_out_dict(samples)
+                pred_out_sample = self.forward_through_all_graph(in_var, self.outvar_dict_index)
+                try:
+                    loss = self.compute_loss(in_var, pred_out_sample, true_out, lambda_out)
+                except RuntimeError:
+                    raise
+                self.notify(self, message={Signal.BEFORE_BACKWARD: 'defaults'})
+                loss.backward()
+                opt.step()
+                
         samples = self.sample_variables_from_domains()
         in_var, true_out, lambda_out = self.generate_in_out_dict(samples)
         pred_out_sample = self.forward_through_all_graph(in_var, self.outvar_dict_index)
-        try:
-            loss = self.compute_loss(in_var, pred_out_sample, true_out, lambda_out)
-        except RuntimeError:
-            raise
-        self.notify(self, message={Signal.BEFORE_BACKWARD: "defaults"})
-        loss.backward()
-        for opt in self.optimizers:
-            opt.step()
+        loss = self.compute_loss(in_var, pred_out_sample, true_out, lambda_out)
+        
         self.global_step += 1
 
         for scheduler in self.schedulers:
             scheduler.step(self.global_step)
         self.notify(self, message={Signal.TRAIN_PIPE_END: "defaults"})
         return loss
```

### Comparing `idrlnet-0.1.0rc1/idrlnet/torch_util.py` & `idrlnet-2.0.0/idrlnet/torch_util.py`

 * *Files identical despite different names*

### Comparing `idrlnet-0.1.0rc1/idrlnet/variable.py` & `idrlnet-2.0.0/idrlnet/variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 
 
 class Loss(enum.Enum):
     """Enumerate loss functions"""
 
     L1 = "L1"
     square = "square"
+    Identity = "Identity"
 
 
 class LossFunction:
     """Manage loss functions"""
 
     @staticmethod
     def weighted_loss(variables, loss_function, name):
         if loss_function == Loss.L1.name or loss_function == Loss.L1:
             return LossFunction.weighted_L1_loss(variables, name=name)
         elif loss_function == Loss.square.name or loss_function == Loss.square:
             return LossFunction.weighted_square_loss(variables, name=name)
+        elif loss_function == Loss.Identity.name or loss_function == Loss.Identity:
+            return LossFunction.weighted_identity_loss(variables, name=name)
         raise NotImplementedError(f"loss function {loss_function} is not defined!")
 
     @staticmethod
     def weighted_L1_loss(variables: "Variables", name: str) -> "Variables":
         loss = 0.0
         for key, val in variables.items():
             if key.startswith("lambda_") or key == "area":
@@ -58,14 +61,28 @@
                 loss += torch.sum(
                     (val ** 2) * variables["lambda_" + key] * variables["area"]
                 )
             else:
                 loss += torch.sum((val ** 2) * variables["area"])
         return Variables({name: loss})
 
+    @staticmethod
+    def weighted_identity_loss(variables: "Variables", name: str) -> "Variables":
+        loss = 0.0
+        for key, val in variables.items():
+            if key.startswith("lambda_") or key == "area":
+                continue
+            elif "lambda_" + key in variables.keys():
+                loss += torch.sum(
+                    val * variables["lambda_" + key] * variables["area"]
+                )
+            else:
+                loss += torch.sum(val * variables["area"])
+        return Variables({name: loss})
+
 
 class Variables(dict):
     def __sub__(self, other: "Variables") -> "Variables":
         return Variables(
             {
                 key: (self[key] if key in self else 0)
                 - (other[key] if key in other else 0)
```

### Comparing `idrlnet-0.1.0rc1/idrlnet.egg-info/PKG-INFO` & `idrlnet-2.0.0/idrlnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: idrlnet
-Version: 0.1.0rc1
+Version: 2.0.0
 Summary: IDRLnet
 Home-page: https://github.com/idrl-lab/idrlnet
 Author: Intelligent Design & Robust Learning lab
 Author-email: weipeng@deepinfar.cn
 License: UNKNOWN
 Description: # IDRLnet
         
         [![License](https://img.shields.io/github/license/analysiscenter/pydens.svg)](https://www.apache.org/licenses/LICENSE-2.0)
         [![Python](https://img.shields.io/badge/python-3.7/3.8/3.9-blue.svg)](https://python.org)
         [![Documentation Status](https://readthedocs.org/projects/idrlnet/badge/?version=latest)](https://idrlnet.readthedocs.io/en/latest/?badge=latest)
         [![PyPI version](https://badge.fury.io/py/idrlnet.svg)](https://badge.fury.io/py/idrlnet)
         [![DockerHub](https://img.shields.io/docker/pulls/idrl/idrlnet.svg)](https://hub.docker.com/r/idrl/idrlnet)
         [![CodeFactor](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/badge/master)](https://www.codefactor.io/repository/github/idrl-lab/idrlnet/overview/master)
         
-        
-        **IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine
-        learning library that solves both forward and inverse differential equations via physics-informed neural
-        networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
+        **IDRLnet** is a machine learning library on top of [PyTorch](https://pytorch.org/). Use IDRLnet if you need a machine learning library that solves both forward and inverse differential equations via physics-informed neural networks (PINN). IDRLnet is a flexible framework inspired by [Nvidia Simnet](https://developer.nvidia.com/simnet>).
         
         ## Docs
         
         - [Full docs](https://idrlnet.readthedocs.io/en/latest/)
         - [Tutorial](https://idrlnet.readthedocs.io/en/latest/user/get_started/tutorial.html)
         - Paper:
            - IDRLnet: A Physics-Informed Neural Network Library. [arXiv](https://arxiv.org/abs/2107.04320)
@@ -70,29 +67,35 @@
         ```
         
         
         ## Features
         
         IDRLnet supports
         
-        -  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon,
-           circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and
-           intersection;
-        
-        -  sampling in the interior of the defined geometry or on the boundary with given conditions.
-        
-        -  enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph
-           will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via
-           explicit expressions, users model problems more naturally.
+        -  complex domain geometries without mesh generation. Provided geometries include interval, triangle, rectangle, polygon, circle, sphere... Other geometries can be constructed using three boolean operations: union, difference, and intersection;
+           ![Geometry](https://raw.githubusercontent.com/weipeng0098/picture/master/20210617081809.png)
+           
+        - sampling in the interior of the defined geometry or on the boundary with given conditions.
         
-        -  solving variational minimization problem;
+        - enables the user code to be structured. Data sources, operations, constraints are all represented by ``Node``. The graph will be automatically constructed via label symbols of each node. Getting rid of the explicit construction via explicit expressions, users model problems more naturally.
         
-        -  solving integral differential equation;
+        - builds computational graph automatically;
         
-        -  adaptive resampling;
+           ![computationDomain](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142531.png)
+        
+        -  user-defined callbacks;
+           
+           ![callback](https://raw.githubusercontent.com/weipeng0098/picture/master/20220815142621.png)
+           
+        -  solving variational minimization problem;
+           <img src="https://raw.githubusercontent.com/weipeng0098/picture/master/20210617082331.gif" alt="miniface" style="zoom:33%;" />
+           
+        - solving integral differential equation;
+        
+        - adaptive resampling;
         
         -  recover unknown parameters of PDEs from noisy measurement data.
         
         It is also easy to customize IDRLnet to meet new demands.
         
         -  Main Dependencies
         
@@ -103,20 +106,18 @@
         
         ## Contributing to IDRLnet
         
         First off, thanks for taking the time to contribute!
         
         -  **Reporting bugs.** To report a bug, simply open an issue in the GitHub "Issues" section.
         
-        -  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and
-           minor improvements to existing functionality, let us know by opening an issue.
-        
-        -  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a
-           pull-request.
-        
+        -  **Suggesting enhancements.** To submit an enhancement suggestion for IDRLnet, including completely new features and minor improvements to existing functionality, let us know by opening an issue.
+           
+        -  **Pull requests.** If you made improvements to IDRLnet, fixed a bug, or had a new example, feel free to send us a pull-request.
+           
         -  **Asking questions.** To get help on how to use IDRLnet or its functionalities, you can as well open an issue.
         
         -  **Answering questions.** If you know the answer to any question in the "Issues", you are welcomed to answer.
         
         ## The Team
         
         IDRLnet was originally developed by IDRL lab.
```

### Comparing `idrlnet-0.1.0rc1/idrlnet.egg-info/SOURCES.txt` & `idrlnet-2.0.0/idrlnet.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,41 +10,51 @@
 docs/modules/idrlnet.geo_utils.rst
 docs/modules/idrlnet.pde_op.rst
 docs/modules/idrlnet.rst
 docs/modules/modules.rst
 docs/user/cite_idrlnet.md
 docs/user/installation.md
 docs/user/team.md
+docs/user/get_started/10_deepritz.md
 docs/user/get_started/1_simple_poisson.md
 docs/user/get_started/2_euler_beam.md
 docs/user/get_started/3_burgers_equation.md
 docs/user/get_started/4_allen_cahn.md
 docs/user/get_started/5_inverse_wave_equation.md
 docs/user/get_started/6_parameterized_poisson.md
 docs/user/get_started/7_minimal_surface.md
 docs/user/get_started/8_volterra_ide.md
+docs/user/get_started/9_navier_stokes_equation.md
 docs/user/get_started/tutorial.rst
 examples/Volterra_IDE/readme.md
 examples/Volterra_IDE/volterra_ide.py
 examples/allen_cahn/allen_cahn.py
 examples/allen_cahn/readme.md
 examples/burgers_equation/burgers_equation.py
 examples/burgers_equation/readme.md
 examples/consolidation/Aana.py
 examples/consolidation/Boneside_pinn.py
 examples/consolidation/readme.md
+examples/deepritz/deepritz.py
 examples/euler_beam/euler_beam.py
+examples/euler_beam/euler_beam_lbfgs.py
 examples/euler_beam/readme.md
 examples/holes_heat_flux/holes_heat_flux.py
 examples/inverse_wave_equation/inverse_wave_equation.py
 examples/inverse_wave_equation/readme.md
 examples/ldc/ldc.py
 examples/minimal_surface_of_revolution/minimal_surface_of_revolution.py
 examples/minimal_surface_of_revolution/minimal_surface_of_revolution_pretrain.py
 examples/minimal_surface_of_revolution/readme.md
+examples/ns_steady/NS_steady.py
+examples/ns_steady/NSexternel_sample.csv
+examples/ns_steady/NSexternel_test.csv
+examples/ns_unsteady/NS_unsteady.py
+examples/ns_unsteady/NSexternel_sample.csv
+examples/ns_unsteady/NSexternel_test.csv
 examples/parameterized_poisson/parameterized_poisson.py
 examples/parameterized_poisson/readme.md
 examples/simple_poisson/readme.md
 examples/simple_poisson/simple_poisson.py
 idrlnet/__init__.py
 idrlnet/callbacks.py
 idrlnet/data.py
```

### Comparing `idrlnet-0.1.0rc1/setup.py` & `idrlnet-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if line:  # if requirement is not empty
             requirements.append(line)
     return requirements
 
 
 setuptools.setup(
     name="idrlnet",  # Replace with your own username
-    version="0.1.0-rc1",
+    version="2.0.0",
     author="Intelligent Design & Robust Learning lab",
     author_email="weipeng@deepinfar.cn",
     description="IDRLnet",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/idrl-lab/idrlnet",
     packages=setuptools.find_packages(),
```

