# Comparing `tmp/jaxsim-0.1.dev164.tar.gz` & `tmp/jaxsim-0.1.dev185.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev164.tar", last modified: Fri Jun  9 10:24:56 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev185.tar", last modified: Fri Jun 30 14:39:38 2023, max compression
```

## Comparing `jaxsim-0.1.dev164.tar` & `jaxsim-0.1.dev185.tar`

### file list

```diff
@@ -1,83 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.898701 jaxsim-0.1.dev164/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.898701 jaxsim-0.1.dev164/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.906701 jaxsim-0.1.dev164/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.910701 jaxsim-0.1.dev164/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-09 10:24:41.000000 jaxsim-0.1.dev164/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:24:56.902701 jaxsim-0.1.dev164/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 10:24:56.000000 jaxsim-0.1.dev164/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.030300 jaxsim-0.1.dev185/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.030300 jaxsim-0.1.dev185/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44682 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.038300 jaxsim-0.1.dev185/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.034300 jaxsim-0.1.dev185/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-30 14:39:38.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 14:39:37.000000 jaxsim-0.1.dev185/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:38.042300 jaxsim-0.1.dev185/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/test_eom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/test_forward_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_idyntree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 14:39:22.000000 jaxsim-0.1.dev185/tests/utils_rng.py
```

### Comparing `jaxsim-0.1.dev164/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev185/.github/workflows/ci_cd.yml`

 * *Files 22% similar despite different names*

```diff
@@ -57,36 +57,64 @@
           - macos-latest
           # https://github.com/google/jax/issues/5795
           # - windows-latest
         python:
           - "3.8"
           - "3.9"
           - "3.10"
-          # - "3.11"
+          - "3.11"
 
     steps:
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
       - name: Download Python packages
         uses: actions/download-artifact@v3
         with:
           path: dist
           name: dist
 
-      - name: Install wheel
+      # Workaround: install iDynTree for Python 3.11
+      - name: iDynTree on Python 3.11
+        if: contains(matrix.os, 'ubuntu') && matrix.python == '3.11'
         shell: bash
-        run: pip install dist/*.whl
+        run: pip install --pre idyntree
+
+      - name: Install wheel (ubuntu)
+        if: contains(matrix.os, 'ubuntu')
+        shell: bash
+        run: pip install "$(find dist/ -type f -name '*.whl')[all]"
+
+      - name: Install wheel (macos)
+        if: contains(matrix.os, 'macos')
+        shell: bash
+        run: pip install "$(find dist/ -type f -name '*.whl')"
 
       - name: Import the package
         run: python -c "import jaxsim"
 
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - name: Install Gazebo Classic
+        if: contains(matrix.os, 'ubuntu') && (matrix.python == '3.10' || matrix.python == '3.11')
+        run: |
+          sudo apt-get update
+          sudo apt-get install gazebo
+
+      - name: Run the Python tests
+        if: contains(matrix.os, 'ubuntu') && (matrix.python == '3.10' || matrix.python == '3.11')
+        run: pytest
+        env:
+          JAX_PLATFORM_NAME: cpu
+
   publish:
     name: Publish to PyPI
     needs: test
     runs-on: ubuntu-22.04
 
     steps:
```

### Comparing `jaxsim-0.1.dev164/.github/workflows/style.yml` & `jaxsim-0.1.dev185/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/.gitignore` & `jaxsim-0.1.dev185/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/LICENSE` & `jaxsim-0.1.dev185/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/PKG-INFO` & `jaxsim-0.1.dev185/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev164
+Version: 0.1.dev185
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev164/README.md` & `jaxsim-0.1.dev185/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/setup.cfg` & `jaxsim-0.1.dev185/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = jaxsim
 description = A physics engine in reduced coordinates implemented with JAX.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diego Ferigo
 author_email = diego.ferigo@iit.it
 license = BSD
-license_file = LICENSE
+license_files = LICENSE
 platforms = any
 url = https://github.com/ami-iit/jaxsim
 project_urls = 
 	Changelog = https://github.com/ami-iit/jaxsim/releases
 	Source = https://github.com/ami-iit/jaxsim
 	Tracker = https://github.com/ami-iit/jaxsim/issues
 keywords = 
@@ -48,34 +48,34 @@
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	coloredlogs
-	distrax
-	flax
-	jax >=0.3.14, <0.3.16
-	jaxlib == 0.3.15
+	jax >= 0.4.1
+	jaxlib
 	jaxlie
-	jax_dataclasses >= 1.2.2, < 1.4.0
+	jax_dataclasses >= 1.4.0
 	pptree
 	rod
 	scipy
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 style = 
 	black
 	isort
 testing = 
+	idyntree
 	pytest
 	pytest-icdiff
+	robot-descriptions
 all = 
 	%(style)s
 	%(testing)s
 
 [tool:pytest]
 addopts = -rsxX -v --strict-markers
 testpaths = tests
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/__init__.py` & `jaxsim-0.1.dev185/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev185/src/jaxsim/high_level/joint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from typing import Tuple
+import dataclasses
+from typing import Any, Tuple
 
 import jax_dataclasses
+from jax_dataclasses import Static
 
-import jaxsim.high_level
-import jaxsim.parsers.descriptions as descriptions
+import jaxsim.parsers
 import jaxsim.typing as jtp
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class Joint(JaxsimDataclass):
     """
     High-level class to operate on a single joint of a simulated model.
     """
 
-    joint_description: descriptions.JointDescription = jax_dataclasses.static_field()
-    parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
-        default=None, repr=False, compare=False
-    )
+    joint_description: Static[jaxsim.parsers.descriptions.JointDescription]
+
+    _parent_model: Any = dataclasses.field(default=None, repr=False, compare=False)
+
+    @property
+    def parent_model(self) -> "jaxsim.high_level.model.Model":
+        return self._parent_model
 
     def valid(self) -> bool:
         return self.parent_model is not None
 
     def index(self) -> int:
         return self.joint_description.index
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev185/src/jaxsim/high_level/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+import dataclasses
+from typing import Any
+
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
+from jax_dataclasses import Static
 
-import jaxsim.high_level
-import jaxsim.parsers.descriptions as descriptions
+import jaxsim.parsers
 import jaxsim.sixd as sixd
 import jaxsim.typing as jtp
 from jaxsim.physics.algos.jacobian import jacobian
 from jaxsim.utils import JaxsimDataclass
 
 from .common import VelRepr
 
 
 @jax_dataclasses.pytree_dataclass
 class Link(JaxsimDataclass):
     """
     High-level class to operate on a single link of a simulated model.
     """
 
-    link_description: descriptions.LinkDescription = jax_dataclasses.static_field()
-    parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
-        default=None, repr=False, compare=False
-    )
+    link_description: Static[jaxsim.parsers.descriptions.LinkDescription]
+
+    _parent_model: Any = dataclasses.field(default=None, repr=False, compare=False)
+
+    @property
+    def parent_model(self) -> "jaxsim.high_level.model.Model":
+        return self._parent_model
 
     def valid(self) -> bool:
         return self.parent_model is not None
 
     # ==========
     # Properties
     # ==========
@@ -139,30 +145,30 @@
             LW_X_L = sixd.se3.SE3.from_matrix(LW_H_L).adjoint()
             return LW_X_L @ L_J_WL_target
 
         else:
             raise ValueError(output_vel_repr)
 
     def external_force(self) -> jtp.Vector:
-        W_f_ext = self.parent_model.data.model_input.f_ext[self.index()]
-
-        if self.parent_model.velocity_representation is VelRepr.Inertial:
-            return W_f_ext
-
-        elif self.parent_model.velocity_representation is VelRepr.Body:
-            W_H_B = self.parent_model.base_transform()
-            W_X_B = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
+        """
+        Return the active external force acting on the link.
 
-            return W_X_B.transpose() @ W_f_ext
+        This external force is a user input and is not computed by the physics engine.
+        During the simulation, this external force is summed to other terms like those
+        related to enforce contact constraints.
+
+        Returns:
+            The active external 6D force acting on the link in the active representation.
+        """
 
-        elif self.parent_model.velocity_representation is VelRepr.Mixed:
-            raise NotImplementedError
+        W_f_ext = self.parent_model.data.model_input.f_ext[self.index()]
 
-        else:
-            raise ValueError(self.parent_model.velocity_representation)
+        return self.parent_model.inertial_to_active_representation(
+            array=W_f_ext, is_force=True
+        )
 
     def add_external_force(
         self, force: jtp.Array = None, torque: jtp.Array = None
     ) -> None:
         force = force if force is not None else jnp.zeros(3)
         torque = torque if torque is not None else jnp.zeros(3)
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev185/src/jaxsim/high_level/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import dataclasses
 import pathlib
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-import jax.experimental.ode
+import jax
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
+from jax_dataclasses import Static
 
-import jaxsim
 import jaxsim.physics.algos.aba
 import jaxsim.physics.algos.crba
 import jaxsim.physics.algos.forward_kinematics
 import jaxsim.physics.algos.rnea
 import jaxsim.physics.model.physics_model
 import jaxsim.physics.model.physics_model_state
 import jaxsim.typing as jtp
@@ -19,14 +19,16 @@
 from jaxsim.physics.algos import soft_contacts
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.simulation import ode_data, ode_integration
 from jaxsim.simulation.ode_integration import IntegratorType
 from jaxsim.utils import JaxsimDataclass, Mutability
 
 from .common import VelRepr
+from .joint import Joint
+from .link import Link
 
 
 @jax_dataclasses.pytree_dataclass
 class ModelData(JaxsimDataclass):
     """
     Class used to store the model state and input at a given time.
     """
@@ -95,31 +97,31 @@
 
 @jax_dataclasses.pytree_dataclass
 class Model(JaxsimDataclass):
     """
     High-level class to operate on a simulated model.
     """
 
-    model_name: str = jax_dataclasses.static_field()
+    model_name: Static[str]
+
     physics_model: physics.model.physics_model.PhysicsModel = dataclasses.field(
         repr=False
     )
 
-    velocity_representation: VelRepr = jax_dataclasses.static_field(
-        default=VelRepr.Mixed
-    )
+    velocity_representation: Static[VelRepr] = dataclasses.field(default=VelRepr.Mixed)
 
-    _links: Dict[str, "high_level.link.Link"] = jax_dataclasses.static_field(
+    _links: Static[Dict[str, Link]] = dataclasses.field(
         default_factory=list, repr=False
     )
-    _joints: Dict[str, "high_level.joint.Joint"] = jax_dataclasses.static_field(
+
+    _joints: Static[Dict[str, Joint]] = dataclasses.field(
         default_factory=list, repr=False
     )
 
-    data: ModelData = jax_dataclasses.field(default=None, repr=False)
+    data: ModelData = dataclasses.field(default=None, repr=False)
 
     # ========================
     # Initialization and state
     # ========================
 
     @staticmethod
     def build_from_model_description(
@@ -264,18 +266,18 @@
     def __post_init__(self):
         """Post-init logic. Use the static methods to build high-level models."""
 
         original_mutability = self._mutability()
         self._set_mutability(Mutability.MUTABLE_NO_VALIDATION)
 
         for l in self._links.values():
-            l.mutable(validate=False).parent_model = self
+            l.mutable(validate=False)._parent_model = self
 
         for j in self._joints.values():
-            j.mutable(validate=False).parent_model = self
+            j.mutable(validate=False)._parent_model = self
 
         self._links: Dict[str, high_level.link.Link] = {
             k: v for k, v in sorted(self._links.items(), key=lambda kv: kv[1].index())
         }
 
         self._joints: Dict[str, high_level.joint.Joint] = {
             k: v for k, v in sorted(self._joints.items(), key=lambda kv: kv[1].index())
@@ -538,14 +540,28 @@
                 self.data.model_state.base_angular_velocity,
             ]
         )
 
         return self.inertial_to_active_representation(array=W_v_WB)
 
     def external_forces(self) -> jtp.Matrix:
+        """
+        Return the active external forces acting on the robot.
+
+        The external forces are a user input and are not computed by the physics engine.
+        During the simulation, these external forces are summed to other terms like
+        the external forces due to the contact with the environment.
+
+        Returns:
+            A matrix of shape (n_links, 6) containing the external forces acting on the
+            robot links. The forces are expressed in the active representation.
+        """
+
+        # Get the active external forces that are always stored internally
+        # in Inertial representation
         W_f_ext = self.data.model_input.f_ext
 
         inertial_to_active = lambda f: self.inertial_to_active_representation(
             f, is_force=True
         )
 
         return jax.vmap(inertial_to_active, in_axes=0)(W_f_ext)
@@ -556,24 +572,62 @@
 
     def generalized_position(self) -> Tuple[jtp.Matrix, jtp.Vector]:
         return self.base_transform(), self.joint_positions()
 
     def generalized_velocity(self) -> jtp.Vector:
         return jnp.hstack([self.base_velocity(), self.joint_velocities()])
 
-    def generalized_jacobian(self, output_vel_repr: VelRepr = None) -> jtp.Matrix:
-        return jnp.vstack(
+    def generalized_free_floating_jacobian(
+        self, output_vel_repr: VelRepr = None
+    ) -> jtp.Matrix:
+        """"""
+
+        if output_vel_repr is None:
+            output_vel_repr = self.velocity_representation
+
+        # The body frame of the Link.jacobian method is the link frame L.
+        # In this method, we want instead to use the base link B as body frame.
+        # Therefore, we always get the link jacobian having Inertial as output
+        # representation, and then we convert it to the desired output representation.
+        if output_vel_repr is VelRepr.Inertial:
+            to_output = lambda J: J
+
+        elif output_vel_repr is VelRepr.Body:
+
+            def to_output(W_J_Wi):
+                W_H_B = self.base_transform()
+                B_X_W = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
+                return B_X_W @ W_J_Wi
+
+        elif output_vel_repr is VelRepr.Mixed:
+
+            def to_output(W_J_Wi):
+                W_H_B = self.base_transform()
+                W_H_BW = jnp.array(W_H_B).at[0:3, 0:3].set(jnp.eye(3))
+                BW_X_W = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
+                return BW_X_W @ W_J_Wi
+
+        else:
+            raise ValueError(output_vel_repr)
+
+        # Get the link jacobians in Inertial representation and convert them to the
+        # target output representation in which the body frame is the base link B
+        J_free_floating = jnp.vstack(
             [
-                self.get_link(link_name=link_name).jacobian(
-                    output_vel_repr=output_vel_repr
+                to_output(
+                    self.get_link(link_name=link_name).jacobian(
+                        output_vel_repr=VelRepr.Inertial
+                    )
                 )
                 for link_name in self.link_names()
             ]
         )
 
+        return J_free_floating
+
     def free_floating_mass_matrix(self) -> jtp.Matrix:
         M_body = jaxsim.physics.algos.crba.crba(
             model=self.physics_model,
             q=self.data.model_state.joint_positions,
         )
 
         if self.velocity_representation is VelRepr.Body:
@@ -595,38 +649,48 @@
             invT = jnp.block([[BW_X_W, zero_6n], [zero_6n.T, jnp.eye(self.dofs())]])
 
             return invT.T @ M_body @ invT
 
         else:
             raise ValueError(self.velocity_representation)
 
-    def free_floating_generalized_forces(self) -> jtp.Vector:
-        model_state = self.data.model_state
-        model = self.copy().mutable(validate=True)
-
-        model.zero()
-        model.data.model_state.base_position = model_state.base_position
-        model.data.model_state.base_quaternion = model_state.base_quaternion
-        model.data.model_state.joint_positions = model_state.joint_positions
-        model.data.model_state.base_linear_velocity = model_state.base_linear_velocity
-        model.data.model_state.base_angular_velocity = model_state.base_angular_velocity
-        model.data.model_state.joint_velocities = model_state.joint_velocities
+    def free_floating_bias_forces(self) -> jtp.Vector:
+        with self.editable(validate=True) as model:
+            model.zero()
 
-        return jnp.hstack(model.inverse_dynamics())
+            state = self.data.model_state.copy()
+            model.data.model_state.base_position = state.base_position
+            model.data.model_state.base_quaternion = state.base_quaternion
+            model.data.model_state.joint_positions = state.joint_positions
+            model.data.model_state.base_linear_velocity = state.base_linear_velocity
+            model.data.model_state.base_angular_velocity = state.base_angular_velocity
+            model.data.model_state.joint_velocities = state.joint_velocities
+
+        return jnp.hstack(
+            model.inverse_dynamics(
+                base_acceleration=jnp.zeros(6),
+                joint_accelerations=jnp.zeros(model.dofs()),
+            )
+        )
 
     def free_floating_gravity_forces(self) -> jtp.Vector:
-        model_state = self.data.model_state
-        model = self.copy().mutable(validate=True)
-
-        model.zero()
-        model.data.model_state.base_position = model_state.base_position
-        model.data.model_state.base_quaternion = model_state.base_quaternion
-        model.data.model_state.joint_positions = model_state.joint_positions
+        with self.editable(validate=True) as model:
+            model.zero()
 
-        return jnp.hstack(model.inverse_dynamics())
+            state = self.data.model_state.copy()
+            model.data.model_state.base_position = state.base_position
+            model.data.model_state.base_quaternion = state.base_quaternion
+            model.data.model_state.joint_positions = state.joint_positions
+
+        return jnp.hstack(
+            model.inverse_dynamics(
+                base_acceleration=jnp.zeros(6),
+                joint_accelerations=jnp.zeros(model.dofs()),
+            )
+        )
 
     def momentum(self) -> jtp.Vector:
         with self.editable(validate=True) as m:
             m.set_velocity_representation(vel_repr=VelRepr.Body)
 
         # Compute the momentum in body-fixed velocity representation.
         # Note: the first 6 rows of the mass matrix define the jacobian of the
@@ -673,46 +737,86 @@
         return W_H_i
 
     def inverse_dynamics(
         self,
         joint_accelerations: jtp.Vector = None,
         base_acceleration: jtp.Vector = jnp.zeros(6),
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-        if (
-            self.velocity_representation is VelRepr.Mixed
-            and self.floating_base()
-            and not jnp.allclose(self.data.model_state.base_angular_velocity, 0)
-        ):
-            msg = "This method has to be fixed in Mixed representation"
-            raise ValueError(msg)
+        """
+        Compute inverse dynamics with the RNEA algorithm.
+
+        Args:
+            joint_accelerations: the joint accelerations to consider.
+            base_acceleration:  the base acceleration in the active representation to consider.
+
+        Returns:
+            A tuple containing the 6D force in active representation applied to the base
+            to obtain the considered base acceleration, and the joint torques to apply
+            to obtain the considered joint accelerations.
+        """
 
         # Build joint accelerations if not provided
         joint_accelerations = (
             joint_accelerations
             if joint_accelerations is not None
             else jnp.zeros_like(self.joint_positions())
         )
 
         if joint_accelerations.size != self.dofs():
             raise ValueError(joint_accelerations.size)
 
         if base_acceleration.size != 6:
             raise ValueError(base_acceleration.size)
 
-        # Express base_acceleration in inertial representation
-        W_a_WB = self.active_to_inertial_representation(array=base_acceleration)
+        def to_inertial(C_vd_WB, W_H_C, C_v_WB, W_vl_WC):
+            W_X_C = sixd.se3.SE3.from_matrix(W_H_C).adjoint()
+            C_X_W = sixd.se3.SE3.from_matrix(W_H_C).inverse().adjoint()
+
+            if self.velocity_representation != VelRepr.Mixed:
+                return W_X_C @ C_vd_WB
+            else:
+                from jaxsim.math.cross import Cross
+
+                C_v_WC = C_X_W @ jnp.hstack([W_vl_WC, jnp.zeros(3)])
+                return W_X_C @ (C_vd_WB + Cross.vx(C_v_WC) @ C_v_WB)
+
+        if self.velocity_representation is VelRepr.Inertial:
+            W_H_C = W_H_W = jnp.eye(4)
+            W_vl_WC = W_vl_WW = jnp.zeros(3)
+
+        elif self.velocity_representation is VelRepr.Body:
+            W_H_C = W_H_B = self.base_transform()
+            W_vl_WC = W_vl_WB = self.base_velocity()[0:3]
+
+        elif self.velocity_representation is VelRepr.Mixed:
+            W_H_B = self.base_transform()
+            W_H_C = W_H_BW = W_H_B.at[0:3, 0:3].set(jnp.eye(3))
+            W_vl_WC = W_vl_W_BW = self.base_velocity()[0:3]
+
+        else:
+            raise ValueError(self.velocity_representation)
+
+        # We need to convert the derivative of the base acceleration to the Inertial
+        # representation. In Mixed representation, this conversion is not a plain
+        # transformation with just X, but it also involves a cross product in ℝ⁶.
+        W_v̇_WB = to_inertial(
+            C_vd_WB=base_acceleration,
+            W_H_C=W_H_C,
+            C_v_WB=self.base_velocity(),
+            W_vl_WC=W_vl_WC,
+        )
 
         # Compute RNEA
         W_f_B, tau = jaxsim.physics.algos.rnea.rnea(
             model=self.physics_model,
             xfb=self.data.model_state.xfb(),
             q=self.data.model_state.joint_positions,
             qd=self.data.model_state.joint_velocities,
             qdd=joint_accelerations,
-            a0fb=W_a_WB,
+            a0fb=W_v̇_WB,
             f_ext=self.data.model_input.f_ext,
         )
 
         # Adjust shape
         tau = jnp.atleast_1d(tau.squeeze())
 
         # Express W_f_B in the active representation
@@ -728,70 +832,103 @@
             if prefer_aba
             else self.forward_dynamics_crb(tau=tau)
         )
 
     def forward_dynamics_aba(
         self, tau: jtp.Vector = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-        if (
-            self.velocity_representation is not VelRepr.Inertial
-            and (self.data.model_input.f_ext != 0).any()
-        ):
-            msg1 = "This method has to be fixed for Body and Mixed representation, "
-            msg2 = "use forward_dynamics_crb instead."
-            raise ValueError(msg1 + msg2)
-
         # Build joint torques if not provided
         tau = tau if tau is not None else jnp.zeros_like(self.joint_positions())
 
         # Compute ABA
-        W_a_WB, sdd = jaxsim.physics.algos.aba.aba(
+        W_v̇_WB, sdd = jaxsim.physics.algos.aba.aba(
             model=self.physics_model,
             xfb=self.data.model_state.xfb(),
             q=self.data.model_state.joint_positions,
             qd=self.data.model_state.joint_velocities,
             tau=tau,
             f_ext=self.data.model_input.f_ext,
         )
 
+        def to_active(W_vd_WB, W_H_C, W_v_WB, W_vl_WC):
+            C_X_W = sixd.se3.SE3.from_matrix(W_H_C).inverse().adjoint()
+
+            if self.velocity_representation != VelRepr.Mixed:
+                return C_X_W @ W_vd_WB
+            else:
+                from jaxsim.math.cross import Cross
+
+                W_v_WC = jnp.hstack([W_vl_WC, jnp.zeros(3)])
+                return C_X_W @ (W_vd_WB - Cross.vx(W_v_WC) @ W_v_WB)
+
+        if self.velocity_representation is VelRepr.Inertial:
+            W_H_C = W_H_W = jnp.eye(4)
+            W_vl_WC = W_vl_WW = jnp.zeros(3)
+
+        elif self.velocity_representation is VelRepr.Body:
+            W_H_C = W_H_B = self.base_transform()
+            W_vl_WC = W_vl_WB = self.base_velocity()[0:3]
+
+        elif self.velocity_representation is VelRepr.Mixed:
+            W_H_B = self.base_transform()
+            W_H_C = W_H_BW = W_H_B.at[0:3, 0:3].set(jnp.eye(3))
+            W_vl_WC = W_vl_W_BW = self.base_velocity()[0:3]
+
+        else:
+            raise ValueError(self.velocity_representation)
+
+        # We need to convert the derivative of the base acceleration to the active
+        # representation. In Mixed representation, this conversion is not a plain
+        # transformation with just X, but it also involves a cross product in ℝ⁶.
+        C_v̇_WB = to_active(
+            W_vd_WB=W_v̇_WB.squeeze(),
+            W_H_C=W_H_C,
+            W_v_WB=jnp.hstack(
+                [
+                    self.data.model_state.base_linear_velocity,
+                    self.data.model_state.base_angular_velocity,
+                ]
+            ),
+            W_vl_WC=W_vl_WC,
+        )
+
         # Adjust shape
         sdd = jnp.atleast_1d(sdd.squeeze())
 
-        # Express W_a_WB in the active representation
-        a_WB = self.inertial_to_active_representation(array=W_a_WB)
-
-        return a_WB, sdd
+        return C_v̇_WB, sdd
 
     def forward_dynamics_crb(
         self, tau: jtp.Vector = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
         # Build joint torques if not provided
-        tau = tau if tau is not None else jnp.zeros_like(self.joint_positions())
-        tau = jnp.atleast_1d(tau.squeeze())
-        tau = jnp.vstack(tau) if tau.size > 0 else jnp.empty(shape=(0, 1))
+        τ = tau if tau is not None else jnp.zeros_like(self.joint_positions())
+        τ = jnp.atleast_1d(τ.squeeze())
+        τ = jnp.vstack(τ) if τ.size > 0 else jnp.empty(shape=(0, 1))
 
         # Compute terms of the floating-base EoM
         M = self.free_floating_mass_matrix()
-        h = jnp.vstack(self.free_floating_generalized_forces())
-        J = self.generalized_jacobian()
+        h = jnp.vstack(self.free_floating_bias_forces())
+        J = self.generalized_free_floating_jacobian()
         f_ext = jnp.vstack(self.external_forces().flatten())
         S = jnp.block([jnp.zeros(shape=(self.dofs(), 6)), jnp.eye(self.dofs())]).T
 
-        if self.floating_base():
-            nu_dot = jnp.linalg.inv(M) @ (S @ tau - h + J.T @ f_ext)
-            sdd = nu_dot[6:]
-            a_WB = nu_dot[0:6]
+        # Configure the slice for fixed/floating base robots
+        sl = np.s_[0:] if self.floating_base() else np.s_[6:]
 
-        else:
-            hss = h[6:]
-            Jss = J[:, 6:]
-            Mss = M[6:, 6:]
+        # Compute the generalized acceleration by inverting the EoM
+        ν̇ = jnp.linalg.inv(M[sl, sl]) @ ((S @ τ)[sl] - h[sl] + J[:, sl].T @ f_ext)
 
-            a_WB = jnp.zeros(6)
-            sdd = jnp.linalg.inv(Mss) @ (tau - hss + Jss.T @ f_ext)
+        # Extract the base acceleration in the active representation.
+        # Note that this is an apparent acceleration (relevant in Mixed representation),
+        # therefore it cannot be always expressed in different frames with just a
+        # 6D transformation X.
+        a_WB = ν̇[0:6] if self.floating_base() else jnp.zeros(6)
+
+        # Extract the joint accelerations
+        sdd = ν̇[6:] if self.floating_base() else ν̇
 
         # Adjust shape and convert to lin-ang serialization
         a_WB = a_WB.squeeze()
         sdd = jnp.atleast_1d(sdd.squeeze())
 
         return a_WB, sdd
 
@@ -1065,33 +1202,33 @@
         if self.velocity_representation is VelRepr.Inertial:
             return W_array
 
         elif self.velocity_representation is VelRepr.Body:
             W_H_B = self.base_transform()
 
             if not is_force:
-                B_X_W: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
-                B_array = B_X_W @ W_array
+                B_Xv_W = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
+                B_array = B_Xv_W @ W_array
 
             else:
-                W_X_B: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
-                B_array = W_X_B.T @ W_array
+                B_Xf_W = sixd.se3.SE3.from_matrix(W_H_B).adjoint().T
+                B_array = B_Xf_W @ W_array
 
             return B_array
 
         elif self.velocity_representation is VelRepr.Mixed:
             W_H_BW = jnp.eye(4).at[0:3, 3].set(self.base_position())
 
             if not is_force:
-                BW_X_W = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
-                BW_array = BW_X_W @ W_array
+                BW_Xv_W = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
+                BW_array = BW_Xv_W @ W_array
 
             else:
-                W_X_BW = sixd.se3.SE3.from_matrix(W_H_BW).adjoint()
-                BW_array = W_X_BW.transpose() @ W_array
+                BW_Xf_W = sixd.se3.SE3.from_matrix(W_H_BW).adjoint().T
+                BW_array = BW_Xf_W @ W_array
 
             return BW_array
 
         else:
             raise ValueError(self.velocity_representation)
 
     def active_to_inertial_representation(
@@ -1107,34 +1244,34 @@
             return W_array
 
         elif self.velocity_representation is VelRepr.Body:
             B_array = array
             W_H_B = self.base_transform()
 
             if not is_force:
-                W_X_B: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
-                W_array = W_X_B @ B_array
+                W_Xv_B: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
+                W_array = W_Xv_B @ B_array
 
             else:
-                B_X_W: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
-                W_array = B_X_W.T @ B_array
+                W_Xf_B = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint().T
+                W_array = W_Xf_B @ B_array
 
             return W_array
 
         elif self.velocity_representation is VelRepr.Mixed:
             BW_array = array
             W_H_BW = jnp.eye(4).at[0:3, 3].set(self.base_position())
 
             if not is_force:
-                W_X_BW: jtp.Array = sixd.se3.SE3.from_matrix(W_H_BW).adjoint()
-                W_array = W_X_BW @ BW_array
+                W_Xv_BW: jtp.Array = sixd.se3.SE3.from_matrix(W_H_BW).adjoint()
+                W_array = W_Xv_BW @ BW_array
 
             else:
-                BW_X_W: jtp.Array = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
-                W_array = BW_X_W.T @ BW_array
+                W_Xf_BW = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint().T
+                W_array = W_Xf_BW @ BW_array
 
             return W_array
 
         else:
             raise ValueError(self.velocity_representation)
 
     def _joint_indices(self, joint_names: List[str] = None) -> jtp.Vector:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/logging.py` & `jaxsim-0.1.dev185/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev185/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev185/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev185/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev185/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev185/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev185/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev185/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev185/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev185/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import copy
 import dataclasses
 from typing import List, Optional
 
 import jax.numpy as jnp
 import jax_dataclasses
+from jax_dataclasses import Static
 
 import jaxsim.typing as jtp
 from jaxsim.sixd import se3
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class LinkDescription(JaxsimDataclass):
-    name: str = jax_dataclasses.static_field()
+    """
+    In-memory description of a robot link.
+    """
+
+    name: Static[str]
     mass: float
     inertia: jtp.Matrix
     index: Optional[int] = None
-    parent: "LinkDescription" = jax_dataclasses.static_field(default=None, repr=False)
+    parent: Static["LinkDescription"] = dataclasses.field(default=None, repr=False)
     pose: jtp.Matrix = dataclasses.field(default_factory=lambda: jnp.eye(4), repr=False)
-    children: List["LinkDescription"] = jax_dataclasses.static_field(
+    children: Static[List["LinkDescription"]] = dataclasses.field(
         default_factory=list, repr=False
     )
 
     def __hash__(self) -> int:
         return hash(self.__repr__())
 
     @property
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev185/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/jacobian.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 import jaxsim.typing as jtp
+from jaxsim.math.adjoint import Adjoint
 from jaxsim.physics.model.physics_model import PhysicsModel
 
 from . import utils
 
 
 def jacobian(model: PhysicsModel, body_index: jtp.Int, q: jtp.Vector) -> jtp.Matrix:
     _, q, _, _, _, _ = utils.process_inputs(physics_model=model, q=q)
@@ -33,17 +34,21 @@
     propagate_kinematics_carry = (i_X_λi, i_X_0)
 
     def propagate_kinematics(
         carry: PropagateKinematicsCarry, i: jtp.Int
     ) -> Tuple[PropagateKinematicsCarry, None]:
         i_X_λi, i_X_0 = carry
 
+        # For each body (i), compute the parent (λi) to body (i) adjoint matrix
         i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
         i_X_λi = i_X_λi.at[i].set(i_X_λi_i)
 
+        # Compute the base (0) to body (i) adjoint matrix.
+        # This works fine since we traverse the kinematic tree following the link
+        # indices assigned with BFS.
         i_X_0_i = i_X_λi[i] @ i_X_0[λ[i]]
         i_X_0 = i_X_0.at[i].set(i_X_0_i)
 
         return (i_X_λi, i_X_0), None
 
     (i_X_λi, i_X_0), _ = jax.lax.scan(
         f=propagate_kinematics,
@@ -63,15 +68,15 @@
     # To make JIT happy, we operate on a boolean version of κ(i).
     # Checking if j ∈ κ(i) is equivalent to: κ_bool(j) is True.
     κ_bool = model.support_body_array_bool(body_index=body_index)
 
     def compute_jacobian(J: jtp.MatrixJax, i: jtp.Int) -> Tuple[jtp.MatrixJax, None]:
         def update_jacobian(J: jtp.MatrixJax, i: jtp.Int) -> jtp.MatrixJax:
             ii = i - 1
-            Js_i = i_X_0[body_index] @ jnp.linalg.inv(i_X_0[i]) @ S[i]
+            Js_i = i_X_0[body_index] @ Adjoint.inverse(i_X_0[i]) @ S[i]
             J = J.at[0:6, 6 + ii].set(Js_i.squeeze())
 
             return J
 
         J = jax.lax.select(pred=κ_bool[i], on_true=update_jacobian(J, i), on_false=J)
         return J, None
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import dataclasses
 from typing import Tuple
 
 import jax
-import jax.experimental.loops
 import jax.flatten_util
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
 
 import jaxsim.physics.model.physics_model
 import jaxsim.typing as jtp
@@ -52,14 +51,18 @@
 
 def collidable_points_pos_vel(
     model: PhysicsModel,
     q: jtp.Vector,
     qd: jtp.Vector,
     xfb: jtp.Vector = None,
 ) -> Tuple[jtp.Matrix, jtp.Matrix]:
+    """
+    Compute the position and linear velocity of collidable points in the world frame.
+    """
+
     # Make sure that shape and size are correct
     xfb, q, qd, _, _, _ = utils.process_inputs(physics_model=model, xfb=xfb, q=q, qd=qd)
 
     # Initialize buffers of link transforms (W_X_i) and 6D inertial velocities (W_v_Wi)
     W_X_i = jnp.zeros(shape=[model.NB, 6, 6])
     W_v_Wi = jnp.zeros(shape=[model.NB, 6, 1])
 
@@ -178,19 +181,19 @@
     )
 
     return W_p_Ci.transpose(), CW_v_WC.transpose()
 
 
 @jax_dataclasses.pytree_dataclass
 class SoftContactsParams:
-    """"""
+    """Parameters of the soft contacts model."""
 
-    K: float = dataclasses.field(default=jnp.array(1e6, dtype=float))
-    D: float = dataclasses.field(default=jnp.array(2000, dtype=float))
-    mu: float = dataclasses.field(default=jnp.array(0.5, dtype=float))
+    K: float = dataclasses.field(default_factory=lambda: jnp.array(1e6, dtype=float))
+    D: float = dataclasses.field(default_factory=lambda: jnp.array(2000, dtype=float))
+    mu: float = dataclasses.field(default_factory=lambda: jnp.array(0.5, dtype=float))
 
     @staticmethod
     def build(
         K: float = 1e6, D: float = 2_000, mu: float = 0.5
     ) -> "SoftContactsParams":
         """"""
 
@@ -199,14 +202,16 @@
             D=jnp.array(D, dtype=float),
             mu=jnp.array(mu, dtype=float),
         )
 
 
 @jax_dataclasses.pytree_dataclass
 class SoftContacts:
+    """Soft contacts model."""
+
     parameters: SoftContactsParams = dataclasses.field(
         default_factory=SoftContactsParams
     )
 
     terrain: Terrain = dataclasses.field(default_factory=FlatTerrain)
 
     def contact_model(
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/terrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 class FlatTerrain(Terrain):
     def height(self, x: float, y: float) -> float:
         return 0.0
 
 
 @jax_dataclasses.pytree_dataclass
 class PlaneTerrain(Terrain):
-    plane_normal: jtp.Vector = jax_dataclasses.field(default=jnp.array([0, 0, 1.0]))
+    plane_normal: jtp.Vector = jax_dataclasses.field(
+        default_factory=lambda: jnp.array([0, 0, 1.0])
+    )
 
     @staticmethod
     def build(plane_normal: jtp.Vector) -> "PlaneTerrain":
         """"""
 
         return PlaneTerrain(plane_normal=jnp.array(plane_normal, dtype=float))
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/model/ground_contact.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+import dataclasses
+
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
 import numpy.typing as npt
+from jax_dataclasses import Static
 
 from jaxsim.parsers.descriptions import ModelDescription
 
 
 @jax_dataclasses.pytree_dataclass
 class GroundContact:
-    point: npt.NDArray = jax_dataclasses.field(default_factory=lambda: jnp.array([]))
-    body: npt.NDArray = jax_dataclasses.static_field(
+    """
+    Class to store the collidable points of a robot model.
+    """
+
+    point: npt.NDArray = dataclasses.field(default_factory=lambda: jnp.array([]))
+    body: Static[npt.NDArray] = dataclasses.field(
         default_factory=lambda: np.array([], dtype=int)
     )
 
     @staticmethod
     def build_from(
         model_description: ModelDescription,
     ) -> "GroundContact":
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import dataclasses
 from typing import Dict, Union
 
 import jax.lax
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
-from jax_dataclasses import pytree_dataclass, static_field
+from jax_dataclasses import Static
 
 import jaxsim.parsers
 import jaxsim.physics
 import jaxsim.typing as jtp
 from jaxsim.parsers.descriptions import JointDescriptor, JointType
 from jaxsim.physics import default_gravity
 from jaxsim.sixd import se3
 from jaxsim.utils import JaxsimDataclass, not_tracing
 
 from .ground_contact import GroundContact
 from .physics_model_state import PhysicsModelState
 
 
-@pytree_dataclass
+@jax_dataclasses.pytree_dataclass
 class PhysicsModel(JaxsimDataclass):
-    NB: int = static_field()
-    initial_state: PhysicsModelState = jax_dataclasses.field(default=None)
+    """
+    A read-only class to store all the information necessary to run RBDAs on a model.
+    """
+
+    NB: Static[int]
+    initial_state: PhysicsModelState = dataclasses.field(default=None)
     gravity: jtp.Vector = dataclasses.field(
         default_factory=lambda: jnp.hstack(
             [np.zeros(3), jaxsim.physics.default_gravity()]
         )
     )
-    is_floating_base: bool = static_field(default_factory=lambda: False)
+    is_floating_base: Static[bool] = dataclasses.field(default=False)
     gc: GroundContact = dataclasses.field(default_factory=lambda: GroundContact())
-    description: jaxsim.parsers.descriptions.model.ModelDescription = static_field(
-        default=None
-    )
-
-    _parent_array_dict: Dict[int, int] = static_field(default_factory=dict)
-    _jtype_dict: Dict[int, Union[JointType, JointDescriptor]] = static_field(
-        default_factory=dict
-    )
+    description: Static[
+        jaxsim.parsers.descriptions.model.ModelDescription
+    ] = dataclasses.field(default=None)
+
+    _parent_array_dict: Static[Dict[int, int]] = dataclasses.field(default_factory=dict)
+    _jtype_dict: Static[
+        Dict[int, Union[JointType, JointDescriptor]]
+    ] = dataclasses.field(default_factory=dict)
     _tree_transforms_dict: Dict[int, jtp.Matrix] = dataclasses.field(
         default_factory=dict
     )
     _link_inertias_dict: Dict[int, jtp.Matrix] = dataclasses.field(default_factory=dict)
 
     _joint_friction_static: Dict[int, float] = dataclasses.field(default_factory=dict)
     _joint_friction_viscous: Dict[int, float] = dataclasses.field(default_factory=dict)
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev185/src/jaxsim/physics/model/physics_model_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             valid=valid,
         )
 
         return valid
 
 
 @jax_dataclasses.pytree_dataclass
-class PhysicsModelInput:
+class PhysicsModelInput(JaxsimDataclass):
     tau: jtp.VectorJax
     f_ext: jtp.MatrixJax
 
     @staticmethod
     def zero(
         physics_model: "jaxsim.physics.model.physics_model.PhysicsModel",
     ) -> "PhysicsModelInput":
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import functools
 import pathlib
 from typing import Dict, List, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax_dataclasses
+from jax_dataclasses import Static
 
 import jaxsim.high_level
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.physics
 import jaxsim.simulation.simulator_callbacks as scb
 import jaxsim.typing as jtp
 from jaxsim import logging
@@ -27,49 +28,51 @@
     """
     Data used by the simulator.
 
     It can be used as JaxSim state in a functional programming style.
     """
 
     # Simulation time stored in ns in order to prevent floats approximation
-    time_ns: jtp.Int = jnp.array(0, dtype=jnp.uint64)
+    time_ns: jtp.Int = dataclasses.field(
+        default_factory=lambda: jnp.array(0, dtype=jnp.uint64)
+    )
 
     # Terrain and contact parameters
-    terrain: Terrain = jax_dataclasses.field(default_factory=lambda: FlatTerrain())
-    contact_parameters: SoftContactsParams = jax_dataclasses.field(
+    terrain: Terrain = dataclasses.field(default_factory=lambda: FlatTerrain())
+    contact_parameters: SoftContactsParams = dataclasses.field(
         default_factory=lambda: SoftContactsParams()
     )
 
     # Dictionary containing all handled models
-    models: Dict[str, Model] = jax_dataclasses.field(default_factory=dict)
+    models: Dict[str, Model] = dataclasses.field(default_factory=dict)
 
     # Default gravity vector (could be overridden for individual models)
-    gravity: jtp.Vector = jax_dataclasses.field(
+    gravity: jtp.Vector = dataclasses.field(
         default_factory=lambda: jaxsim.physics.default_gravity()
     )
 
 
 @jax_dataclasses.pytree_dataclass
 class JaxSim(JaxsimDataclass):
     """The JaxSim simulator."""
 
     # Step size stored in ns in order to prevent floats approximation
-    step_size_ns: jtp.Int = jax_dataclasses.field(
+    step_size_ns: jtp.Int = dataclasses.field(
         default_factory=lambda: jnp.array(1_000_000, dtype=jnp.uint64)
     )
 
     # Number of sub-steps performed at each integration step.
     # Note: there is no collision detection performed in sub-steps.
-    steps_per_run: jtp.Int = jax_dataclasses.static_field(default=1)
+    steps_per_run: Static[jtp.Int] = dataclasses.field(default=1)
 
     # Default velocity representation (could be overridden for individual models)
-    velocity_representation: VelRepr = jax_dataclasses.field(default=VelRepr.Inertial)
+    velocity_representation: VelRepr = dataclasses.field(default=VelRepr.Inertial)
 
     # Integrator type
-    integrator_type: ode_integration.IntegratorType = jax_dataclasses.static_field(
+    integrator_type: Static[ode_integration.IntegratorType] = dataclasses.field(
         default=ode_integration.IntegratorType.EulerForward
     )
 
     # Simulator data
     data: SimulatorData = dataclasses.field(default_factory=lambda: SimulatorData())
 
     @staticmethod
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev185/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/typing.py` & `jaxsim-0.1.dev185/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev164/src/jaxsim/utils.py` & `jaxsim-0.1.dev185/src/jaxsim/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
 
     def mutable(self: T, mutable: bool = True, validate: bool = False) -> T:
         self.set_mutability(mutable=mutable, validate=validate)
         return self
 
     def copy(self: T) -> T:
-        obj = jax.tree_util.tree_map(lambda leaf: leaf, self)
+        obj = copy.deepcopy(self)
         obj._set_mutability(mutability=self._mutability())
         return obj
 
     def replace(self: T, validate: bool = True, **kwargs) -> T:
         with self.editable(validate=validate) as obj:
             _ = [obj.__setattr__(k, copy.copy(v)) for k, v in kwargs.items()]
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev185/src/jaxsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev164
+Version: 0.1.dev185
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev164/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev185/src/jaxsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,14 @@
 src/jaxsim/simulation/integrators.py
 src/jaxsim/simulation/ode.py
 src/jaxsim/simulation/ode_data.py
 src/jaxsim/simulation/ode_integration.py
 src/jaxsim/simulation/simulator.py
 src/jaxsim/simulation/simulator_callbacks.py
 src/jaxsim/simulation/utils.py
-src/jaxsim/sixd/__init__.py
+src/jaxsim/sixd/__init__.py
+tests/__init__.py
+tests/test_eom.py
+tests/test_forward_dynamics.py
+tests/utils_idyntree.py
+tests/utils_models.py
+tests/utils_rng.py
```

