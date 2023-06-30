# Comparing `tmp/jaxsim-0.1.dev185.tar.gz` & `tmp/jaxsim-0.1.dev191.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev185.tar", last modified: Fri Jun 30 14:39:38 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev191.tar", last modified: Fri Jun 30 21:04:34 2023, max compression
```

## Comparing `jaxsim-0.1.dev185.tar` & `jaxsim-0.1.dev191.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.030300 jaxsim-0.1.dev185/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.030300 jaxsim-0.1.dev185/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    44682 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-30 14:39:38.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/test_eom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/test_forward_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_idyntree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.739724 jaxsim-0.1.dev191/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:04:34.759724 jaxsim-0.1.dev191/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.739724 jaxsim-0.1.dev191/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45600 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/test_eom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/test_forward_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_idyntree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_rng.py
```

### Comparing `jaxsim-0.1.dev185/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev191/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/.github/workflows/style.yml` & `jaxsim-0.1.dev191/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/.gitignore` & `jaxsim-0.1.dev191/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/LICENSE` & `jaxsim-0.1.dev191/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/PKG-INFO` & `jaxsim-0.1.dev191/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev185
+Version: 0.1.dev191
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev185/README.md` & `jaxsim-0.1.dev191/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/setup.cfg` & `jaxsim-0.1.dev191/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/__init__.py` & `jaxsim-0.1.dev191/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev191/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev191/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev191/src/jaxsim/high_level/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,23 +281,28 @@
 
         self._joints: Dict[str, high_level.joint.Joint] = {
             k: v for k, v in sorted(self._joints.items(), key=lambda kv: kv[1].index())
         }
 
         self._set_mutability(original_mutability)
 
-    def reduce(self, considered_joints: List[str]) -> None:
+    def reduce(
+        self, considered_joints: List[str], keep_base_pose: bool = False
+    ) -> None:
         """
         Reduce the model by lumping together the links connected by removed joints.
 
         Args:
             considered_joints: The list of joints to consider.
+            keep_base_pose: A flag indicating whether to keep the base pose or not.
         """
 
-        # Reduce the model description
+        # Reduce the model description.
+        # If considered_joints contains joints not existing in the model, the method
+        # will raise an exception.
         reduced_model_description = self.physics_model.description.reduce(
             considered_joints=considered_joints
         )
 
         # Create the physics model from the reduced model description
         physics_model = jaxsim.physics.model.physics_model.PhysicsModel.build_from(
             model_description=reduced_model_description,
@@ -307,22 +312,30 @@
         # Build the reduced high-level model
         reduced_model = Model.build(
             physics_model=physics_model,
             model_name=self.name(),
             vel_repr=self.velocity_representation,
         )
 
-        # Replace the current model with the reduced one
-        original_mutability = self._mutability()
-        self._set_mutability(mutability=self._mutability().MUTABLE_NO_VALIDATION)
-        self.physics_model = reduced_model.physics_model
-        self.data = reduced_model.data
-        self._links = reduced_model._links
-        self._joints = reduced_model._joints
-        self._set_mutability(original_mutability)
+        # Extract the base pose
+        W_p_B = self.base_position()
+        W_Q_B = self.base_orientation(dcm=False)
+
+        # Replace the current model with the reduced model.
+        # Since the structure of the PyTree changes, we disable validation.
+        with self.mutable_context(mutability=Mutability.MUTABLE_NO_VALIDATION):
+            self.physics_model = reduced_model.physics_model
+            self.data = reduced_model.data
+            self._links = reduced_model._links
+            self._joints = reduced_model._joints
+
+        if keep_base_pose:
+            with self.mutable_context(mutability=Mutability.MUTABLE):
+                self.reset_base_position(position=W_p_B)
+                self.reset_base_orientation(orientation=W_Q_B, dcm=False)
 
     def zero(self) -> None:
         self.data = ModelData.zero(physics_model=self.physics_model)
         self.data._set_mutability(self._mutability())
 
     def zero_input(self) -> None:
         self.data.model_input = ModelData.zero(
@@ -989,18 +1002,21 @@
             raise ValueError("Wrong arguments size", positions.size, len(joint_names))
 
         if positions.size == 0:
             return
 
         # TODO: joint position limits
 
-        self.data.model_state.joint_positions = (
-            self.data.model_state.joint_positions.at[
-                self._joint_indices(joint_names=joint_names)
-            ].set(positions)
+        self.data.model_state.joint_positions = jnp.atleast_1d(
+            jnp.array(
+                self.data.model_state.joint_positions.at[
+                    self._joint_indices(joint_names=joint_names)
+                ].set(positions),
+                dtype=float,
+            )
         )
 
     def reset_joint_velocities(
         self, velocities: jtp.Vector, joint_names: List[str] = None
     ) -> None:
         if joint_names is None:
             joint_names = self.joint_names()
@@ -1009,32 +1025,35 @@
             raise ValueError("Wrong arguments size", velocities.size, len(joint_names))
 
         if velocities.size == 0:
             return
 
         # TODO: joint velocity limits
 
-        self.data.model_state.joint_velocities = (
-            self.data.model_state.joint_velocities.at[
-                self._joint_indices(joint_names=joint_names)
-            ].set(velocities)
+        self.data.model_state.joint_velocities = jnp.atleast_1d(
+            jnp.array(
+                self.data.model_state.joint_velocities.at[
+                    self._joint_indices(joint_names=joint_names)
+                ].set(velocities),
+                dtype=float,
+            )
         )
 
     def reset_base_position(self, position: jtp.Vector) -> None:
-        self.data.model_state.base_position = position
+        self.data.model_state.base_position = jnp.array(position, dtype=float)
 
     def reset_base_orientation(self, orientation: jtp.Array, dcm: bool = False) -> None:
         if dcm:
             to_wxyz = np.array([3, 0, 1, 2])
             orientation_xyzw = sixd.so3.SO3.from_matrix(
                 orientation
             ).as_quaternion_xyzw()
             orientation = orientation_xyzw[to_wxyz]
 
-        self.data.model_state.base_quaternion = orientation
+        self.data.model_state.base_quaternion = jnp.array(orientation, dtype=float)
 
     def reset_base_transform(self, transform: jtp.Matrix) -> None:
         if transform.shape != (4, 4):
             raise ValueError(transform.shape)
 
         self.reset_base_position(position=transform[0:3, 3])
         self.reset_base_orientation(orientation=transform[0:3, 0:3], dcm=True)
@@ -1070,16 +1089,21 @@
             ).adjoint()
 
             base_velocity_inertial = w_X_bw @ base_velocity
 
         else:
             raise ValueError(self.velocity_representation)
 
-        self.data.model_state.base_linear_velocity = base_velocity_inertial[0:3]
-        self.data.model_state.base_angular_velocity = base_velocity_inertial[3:6]
+        self.data.model_state.base_linear_velocity = jnp.array(
+            base_velocity_inertial[0:3], dtype=float
+        )
+
+        self.data.model_state.base_angular_velocity = jnp.array(
+            base_velocity_inertial[3:6], dtype=float
+        )
 
     # ===========
     # Integration
     # ===========
 
     def integrate(
         self,
```

### Comparing `jaxsim-0.1.dev185/src/jaxsim/logging.py` & `jaxsim-0.1.dev191/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev191/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev191/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev191/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev191/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev191/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev191/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev191/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev191/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev191/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev191/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/aba.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         i_X_λi, v, c, MA, pA, i_X_0 = carry
 
         # Compute parent-to-child transform
         i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
         i_X_λi = i_X_λi.at[i].set(i_X_λi_i)
 
         # Propagate link velocity
-        vJ = S[i] * qd[ii]
+        vJ = S[i] * qd[ii] if qd.size != 0 else S[i] * 0
 
         v_i = i_X_λi[i] @ v[λ[i]] + vJ
         v = v.at[i].set(v_i)
 
         c_i = Cross.vx(v[i]) @ vJ
         c = c.at[i].set(c_i)
```

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     )
 
     # Number of sub-steps performed at each integration step.
     # Note: there is no collision detection performed in sub-steps.
     steps_per_run: Static[jtp.Int] = dataclasses.field(default=1)
 
     # Default velocity representation (could be overridden for individual models)
-    velocity_representation: VelRepr = dataclasses.field(default=VelRepr.Inertial)
+    velocity_representation: Static[VelRepr] = dataclasses.field(
+        default=VelRepr.Inertial
+    )
 
     # Integrator type
     integrator_type: Static[ode_integration.IntegratorType] = dataclasses.field(
         default=ode_integration.IntegratorType.EulerForward
     )
 
     # Simulator data
```

### Comparing `jaxsim-0.1.dev185/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev191/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/typing.py` & `jaxsim-0.1.dev191/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/src/jaxsim/utils.py` & `jaxsim-0.1.dev191/src/jaxsim/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         #
         # self_rw._set_mutability(self._mutability())
 
     @contextlib.contextmanager
     def mutable_context(self: T, mutability: Mutability) -> ContextManager[T]:
         """"""
 
-        original_mutability = self._mutability
+        original_mutability = self._mutability()
 
         self._set_mutability(mutability)
         yield self
 
         self._set_mutability(original_mutability)
 
     def is_mutable(self: T, validate: bool = False) -> bool:
```

### Comparing `jaxsim-0.1.dev185/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev191/src/jaxsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev185
+Version: 0.1.dev191
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev185/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev191/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/tests/test_eom.py` & `jaxsim-0.1.dev191/tests/test_eom.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/tests/test_forward_dynamics.py` & `jaxsim-0.1.dev191/tests/test_forward_dynamics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/tests/utils_idyntree.py` & `jaxsim-0.1.dev191/tests/utils_idyntree.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/tests/utils_models.py` & `jaxsim-0.1.dev191/tests/utils_models.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev185/tests/utils_rng.py` & `jaxsim-0.1.dev191/tests/utils_rng.py`

 * *Files identical despite different names*

