# Comparing `tmp/yaecs-3.2.5.tar.gz` & `tmp/yaecs-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.2.5.tar", last modified: Thu May  4 23:33:24 2023, max compression
+gzip compressed data, was "yaecs-4.0.2.tar", last modified: Fri Jun 30 12:12:49 2023, max compression
```

## Comparing `yaecs-3.2.5.tar` & `yaecs-4.0.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.621513 yaecs-3.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 23:33:05.000000 yaecs-3.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.605512 yaecs-3.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.609513 yaecs-3.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 23:33:05.000000 yaecs-3.2.5/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 23:33:05.000000 yaecs-3.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 23:33:05.000000 yaecs-3.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-04 23:33:05.000000 yaecs-3.2.5/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 23:33:05.000000 yaecs-3.2.5/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-04 23:33:05.000000 yaecs-3.2.5/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 23:33:05.000000 yaecs-3.2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 23:33:05.000000 yaecs-3.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 23:33:24.621513 yaecs-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-04 23:33:05.000000 yaecs-3.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/yaecs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/yaecs_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 23:33:05.000000 yaecs-3.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 23:33:05.000000 yaecs-3.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 23:33:05.000000 yaecs-3.2.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-04 23:33:05.000000 yaecs-3.2.5/resources/yaecs_constructor_overview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/scipts/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 23:33:05.000000 yaecs-3.2.5/scipts/build_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 23:33:05.000000 yaecs-3.2.5/scipts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:33:24.621513 yaecs-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 23:33:05.000000 yaecs-3.2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 23:33:05.000000 yaecs-3.2.5/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.621513 yaecs-3.2.5/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    47697 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33565 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35237 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 12:12:34.000000 yaecs-4.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.950137 yaecs-4.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.954137 yaecs-4.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 12:12:34.000000 yaecs-4.0.2/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 12:12:34.000000 yaecs-4.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-30 12:12:34.000000 yaecs-4.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-30 12:12:34.000000 yaecs-4.0.2/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-06-30 12:12:34.000000 yaecs-4.0.2/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-06-30 12:12:34.000000 yaecs-4.0.2/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-06-30 12:12:34.000000 yaecs-4.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:12:34.000000 yaecs-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-30 12:12:49.962137 yaecs-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-30 12:12:34.000000 yaecs-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/yaecs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-30 12:12:34.000000 yaecs-4.0.2/docs/yaecs_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-30 12:12:34.000000 yaecs-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 12:12:34.000000 yaecs-4.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 12:12:34.000000 yaecs-4.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-06-30 12:12:34.000000 yaecs-4.0.2/resources/yaecs_constructor_overview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/scipts/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 12:12:34.000000 yaecs-4.0.2/scipts/build_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 12:12:34.000000 yaecs-4.0.2/scipts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:12:49.962137 yaecs-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 12:12:34.000000 yaecs-4.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 12:12:34.000000 yaecs-4.0.2/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37943 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-30 12:12:34.000000 yaecs-4.0.2/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-30 12:12:34.000000 yaecs-4.0.2/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.958137 yaecs-4.0.2/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33849 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-06-30 12:12:34.000000 yaecs-4.0.2/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:12:49.962137 yaecs-4.0.2/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:12:49.000000 yaecs-4.0.2/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.2.5/.github/workflows/pipy_deployment.yaml` & `yaecs-4.0.2/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/.gitignore` & `yaecs-4.0.2/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -150,7 +150,11 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 .vscode/
 
 # Setuptools SCM
 yaecs/_version.py
+
+# private_tests
+unittests/config/test_project_config/
+unittests/config/test_config_project.py
```

### Comparing `yaecs-3.2.5/.pylintrc` & `yaecs-4.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/COPYING.LESSER.md` & `yaecs-4.0.2/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/COPYING.md` & `yaecs-4.0.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/DOCUMENTATION_WIP.md` & `yaecs-4.0.2/DOCUMENTATION_WIP.md`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
 #### 1) Creating the default config
 
 To use YAECS in a project, the very first thing to always do is to prepare the default config. The default config needs to be a YAML file, which will contain **all the parameters for your project** and their default values. We have decided to enforce the requirement that every single param be in the defaults, because it is both safer and desirable for you.
 
 It is **safer** because if you want to change a parameter and miss-spell its name, YAECS will know that the parameter name is wrong because it is not in the default config. Therefore instead of starting your experiment with incorrect values, YAECS will throw an error.
 
-It is **desirable** because it gives you a centralized place where you can look up all the values, all the hyper-parameters, all the magic numbers, without going through dozens of source files. YAECS is designed so that having a very large default config never becomes a burden for clarity. Therefore, no need to shy away from having **a lot** of parameters in there.
+It is **desirable** because it gives you a centralised place where you can look up all the values, all the hyper-parameters, all the magic numbers, without going through dozens of source files. YAECS is designed so that having a very large default config never becomes a burden for clarity. Therefore, no need to shy away from having **a lot** of parameters in there.
 
 YAML is a very intuitive config format. We chose it for its elegance, flexibility and the fact that it supports comments (which is not the case in JSON for example). If you need, you can find the YAML documentation here : TODO. Here is the config example we choose to use in this tutorial :
 
 ```yaml
 ---  # Default config - configs/default.yaml
 
 experiment_path: null
@@ -543,15 +543,15 @@
 
 ```bash
 python main.py --do_test
 ```
 
 #### 3) Parameter processing is awesome
 
-Here we present what we believe to be one of YAECS' main improvement over its competitors : parameters processing.  The idea is quite simple : most of the time, it is really useful to be able to perform some kind of processing on your parameters before using them, and it only makes sense that these operations should be performed by the config system. Here is why. The config should be prepared such that the code can access it in a simple, reliable and well-organized well. But at the same time, the config should be prepared by a human in a clear interface using the YAML language. In many cases, those two conditions do not fully align, and therefore it makes sense that the config system should be tasked with translating the config as seen by the human operator into the config as used by the code.
+Here we present what we believe to be one of YAECS' main improvement over its competitors : parameters processing.  The idea is quite simple : most of the time, it is really useful to be able to perform some kind of processing on your parameters before using them, and it only makes sense that these operations should be performed by the config system. Here is why. The config should be prepared such that the code can access it in a simple, reliable and well-organised well. But at the same time, the config should be prepared by a human in a clear interface using the YAML language. In many cases, those two conditions do not fully align, and therefore it makes sense that the config system should be tasked with translating the config as seen by the human operator into the config as used by the code.
 
 Here are a few example use cases :
 
 - if you want to check the value of a param for safety (see `check` in example below)
 - if you want to convert a param to another format (degrees to radians, human-readable to machine-readable etc.) (see `convert`)
 - if you want to use the info in your YAML-supported values to create custom objects (see `instanciate`)
 - if you want to control how the config is created via parameters in the config itself (see next section TODO)
@@ -693,15 +693,15 @@
         return {
             "*_config_file": self.register_as_additional_config_file,
         }
 
     def parameters_post_processing(self):
         return {}
 ```
-And there you go ! Now all parameters that end with `_config_file` will be recognized as you trying to add the corresponding paths to the config.
+And there you go ! Now all parameters that end with `_config_file` will be recognised as you trying to add the corresponding paths to the config.
 
 This ends the Intermediate section of our tutorial. By now, you already know most of what you need to work efficiently with YAECS. To become a real pro, there is only one section left !
 
 ### Advanced tips for larger projects
 
 Now that you might feel better acquainted with the core features of YAECS we can give you more details about a couple of very nice features which can save you a lot of time in certain particular situations.
 
@@ -1094,15 +1094,15 @@
     }
 ```
 
 ### Defining a config over several files
 
 It can often be very useful to split your config into several files to access
 the parameter you are looking for more efficiently. In combination with some
-nice features of the YAML syntax, the Configuration class allows to organize
+nice features of the YAML syntax, the Configuration class allows to organise
 your config more efficiently.
 
 #### 1. Several documents in a single file
 
 The Configuration class supports being fed YAML files with several documents.
 All documents are then concatenated together to create the config. As an
 example, the following YAML file :
@@ -1191,16 +1191,16 @@
 interpreted as a path to a new config file.
 
 ### Defining nested configs
 
 Another desirable property of our configuration is the ability to nest
 configurations inside other configurations. Reusing the example of section 2.
 of the previous advanced feature, it is easy to see that as the number of
-parameters grows, it would be nice to not only organize those parameters in
-different files on the disk, but also organize them in different “sub-configs”
+parameters grows, it would be nice to not only organise those parameters in
+different files on the disk, but also organise them in different “sub-configs”
 in our Configuration object. That way, a function that requires access to
 parameters of a certain nature can be passed only the parameters
 relevant to this function.
 
 Notifying the config that a certain subset of parameters needs to form a
 sub-config of the current config can be done using yaml tags. A yaml tag
 starts with “!” and is then followed by the name of the tag, for
```

### Comparing `yaecs-3.2.5/LICENSE.md` & `yaecs-4.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/PKG-INFO` & `yaecs-4.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-Metadata-Version: 2.1
-Name: yaecs
-Version: 3.2.5
-Summary: A Config System designed for experimental purposes
-Author: Reactive Reality AG
-Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
-Keywords: template,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: COPYING.LESSER.md
-License-File: COPYING.md
-
 # YAECS (Yet Another Experiment Config System)
 
 [![Offial repo](https://img.shields.io/badge/official%20repo-YAECS-%23ff9626?logo=gitlab)](https://gitlab.com/reactivereality/public/yaecs)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
 [![License](https://img.shields.io/badge/license-LGPLV3%2B-%23c4c2c2)](https://www.gnu.org/licenses/)
 
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
+[![PyPI version](https://badge.fury.io/py/yaecs.svg)](https://badge.fury.io/py/yaecs)
+
+[![Documentation Status](https://readthedocs.org/projects/yaecs/badge/?version=latest)](https://yaecs.readthedocs.io/en/latest/?badge=latest)
+
 ---
 
+## Documentation: [here](https://yaecs.readthedocs.io/en/stable/)
+
 **DISCLAIMER: This repository is the public version of a repository that is the
 property of [Reactive Reality](https://www.reactivereality.com/). This
 repository IS NOT OFFICIAL and might not be maintained in the future. Some
 minor changes * are applied from the
 [official repository (GitLab)](https://gitlab.com/reactivereality/public/yaecs)
 (under lesser GNU license).**
 
 This package is a Config System which allows easy manipulation of config files
 for safe, clear and repeatable experiments. In a few words, it is:
 
 - built for Machine Learning with its constraints in mind, but also usable
 out-of-the-box for other kinds of projects;
 - built with scalability in mind and can adapt just as easily to large projects
-investigating hundreds of well-organized parameters across many experiments;
+investigating hundreds of well-organised parameters across many experiments;
 - designed to encourage good coding practices for research purposes, and if
 used rigorously will ensure a number of highly desirable properties such that
 **maintenance-less forward-compatibility** of old configs, **easy
 reproducibility** of any experiment, and **extreme clarity** of former
 experiments for your future self or collaborators.
 
 [LINK TO DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home)
 
 ## Installation
 
-The package can be installed from pipy: `pip install yaecs`
+The package can be installed from pipy:
+
+```bash
+pip install yaecs
+```
 
 ## Getting started
 
 This package is adapted to a *project* where you need to run a number of
 experiments. In this setup, it can be useful to gather all the parameters in
 the project to a common location, some "config files", so you can access and
 modify them easily. This package is based on YAML, therefore your config files
@@ -78,15 +74,15 @@
         return {}
 ```
 
 That's all there is to it! Now if we use
 `config = ProjectSpecific.load_config()`, we can then call `config.data_path`
 or `config.learning_rate` to get their values as defined in the default config.
 We don't need to specify where to get the default config because a project
-should only ever have one default config, which centralizes all the parameters
+should only ever have one default config, which centralises all the parameters
 in that project. Since the location of the default config is a project
 constant, it is defined in your project-specific subclass and there is no need
 to clutter your main code with it. Now, for example, your main.py could look
 like:
 
 ```python
 from project_config import ProjectSpecific
@@ -111,28 +107,28 @@
  - data_path : ./data
  - learning_rate : 0.001
 ```
 
 The Configuration hierarchy tells you about the creation history of the config,
 in this case only the default config was used. Then, all parameters are
 displayed. There are of course many other features in this package which you
-can use to organize your parameters, hierarchise your experiments etc. The
+can use to organise your parameters, hierarchise your experiments etc. The
 idea being that once the bare minimum presented above is set up, scaling up
 is just as simple.
 
 You can learn more about all these features in our
 [DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home).
 
 ## config_history
 
 The Config History is a side-feature of the main Config System. It can be
 configured for any project which uses the Config System and provides a
 flexible framework to easily build graphs representing past experiments. In
 these graphs, each node represents an experiment, and vertices are drawn
-between your experiments to visualize easily which parameters changed from one
+between your experiments to visualise easily which parameters changed from one
 node to another.
 
 The graph can be coloured to show your most successful experiments, or grouped
 by parameters to see how well they have been explored in your experiment
 history. This makes it very useful to review your past work, share it with
 colleagues or make unexpected correlations appear.
```

### Comparing `yaecs-3.2.5/README.md` & `yaecs-4.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,64 @@
+Metadata-Version: 2.1
+Name: yaecs
+Version: 4.0.2
+Summary: A Config System designed for experimental purposes
+Author: Reactive Reality AG
+Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
+Keywords: template,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: COPYING.LESSER.md
+License-File: COPYING.md
+
 # YAECS (Yet Another Experiment Config System)
 
 [![Offial repo](https://img.shields.io/badge/official%20repo-YAECS-%23ff9626?logo=gitlab)](https://gitlab.com/reactivereality/public/yaecs)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
 [![License](https://img.shields.io/badge/license-LGPLV3%2B-%23c4c2c2)](https://www.gnu.org/licenses/)
 
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
+[![PyPI version](https://badge.fury.io/py/yaecs.svg)](https://badge.fury.io/py/yaecs)
+
+[![Documentation Status](https://readthedocs.org/projects/yaecs/badge/?version=latest)](https://yaecs.readthedocs.io/en/latest/?badge=latest)
+
 ---
 
+## Documentation: [here](https://yaecs.readthedocs.io/en/stable/)
+
 **DISCLAIMER: This repository is the public version of a repository that is the
 property of [Reactive Reality](https://www.reactivereality.com/). This
 repository IS NOT OFFICIAL and might not be maintained in the future. Some
 minor changes * are applied from the
 [official repository (GitLab)](https://gitlab.com/reactivereality/public/yaecs)
 (under lesser GNU license).**
 
 This package is a Config System which allows easy manipulation of config files
 for safe, clear and repeatable experiments. In a few words, it is:
 
 - built for Machine Learning with its constraints in mind, but also usable
 out-of-the-box for other kinds of projects;
 - built with scalability in mind and can adapt just as easily to large projects
-investigating hundreds of well-organized parameters across many experiments;
+investigating hundreds of well-organised parameters across many experiments;
 - designed to encourage good coding practices for research purposes, and if
 used rigorously will ensure a number of highly desirable properties such that
 **maintenance-less forward-compatibility** of old configs, **easy
 reproducibility** of any experiment, and **extreme clarity** of former
 experiments for your future self or collaborators.
 
 [LINK TO DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home)
 
 ## Installation
 
-The package can be installed from pipy: `pip install yaecs`
+The package can be installed from pipy:
+
+```bash
+pip install yaecs
+```
 
 ## Getting started
 
 This package is adapted to a *project* where you need to run a number of
 experiments. In this setup, it can be useful to gather all the parameters in
 the project to a common location, some "config files", so you can access and
 modify them easily. This package is based on YAML, therefore your config files
@@ -64,15 +88,15 @@
         return {}
 ```
 
 That's all there is to it! Now if we use
 `config = ProjectSpecific.load_config()`, we can then call `config.data_path`
 or `config.learning_rate` to get their values as defined in the default config.
 We don't need to specify where to get the default config because a project
-should only ever have one default config, which centralizes all the parameters
+should only ever have one default config, which centralises all the parameters
 in that project. Since the location of the default config is a project
 constant, it is defined in your project-specific subclass and there is no need
 to clutter your main code with it. Now, for example, your main.py could look
 like:
 
 ```python
 from project_config import ProjectSpecific
@@ -97,28 +121,28 @@
  - data_path : ./data
  - learning_rate : 0.001
 ```
 
 The Configuration hierarchy tells you about the creation history of the config,
 in this case only the default config was used. Then, all parameters are
 displayed. There are of course many other features in this package which you
-can use to organize your parameters, hierarchise your experiments etc. The
+can use to organise your parameters, hierarchise your experiments etc. The
 idea being that once the bare minimum presented above is set up, scaling up
 is just as simple.
 
 You can learn more about all these features in our
 [DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home).
 
 ## config_history
 
 The Config History is a side-feature of the main Config System. It can be
 configured for any project which uses the Config System and provides a
 flexible framework to easily build graphs representing past experiments. In
 these graphs, each node represents an experiment, and vertices are drawn
-between your experiments to visualize easily which parameters changed from one
+between your experiments to visualise easily which parameters changed from one
 node to another.
 
 The graph can be coloured to show your most successful experiments, or grouped
 by parameters to see how well they have been explored in your experiment
 history. This makes it very useful to review your past work, share it with
 colleagues or make unexpected correlations appear.
```

### Comparing `yaecs-3.2.5/docs/Makefile` & `yaecs-4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/docs/conf.py` & `yaecs-4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/docs/getting_started.md` & `yaecs-4.0.2/docs/getting_started.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return {}
 ```
 
 That's all there is to it! Now if we use
 `config = ProjectSpecific.load_config()`, we can then call `config.data_path`
 or `config.learning_rate` to get their values as defined in the default config.
 We don't need to specify where to get the default config because a project
-should only ever have one default config, which centralizes all the parameters
+should only ever have one default config, which centralises all the parameters
 in that project. Since the location of the default config is a project
 constant, it is defined in your project-specific subclass and there is no need
 to clutter your main code with it. Now, for example, your main.py could look
 like:
 
 ```python
 from project_config import ProjectSpecific
@@ -63,28 +63,28 @@
  - data_path : ./data
  - learning_rate : 0.001
 ```
 
 The Configuration hierarchy tells you about the creation history of the config,
 in this case only the default config was used. Then, all parameters are
 displayed. There are of course many other features in this package which you
-can use to organize your parameters, hierarchise your experiments etc. The
+can use to organise your parameters, hierarchise your experiments etc. The
 idea being that once the bare minimum presented above is set up, scaling up
 is just as simple.
 
 You can learn more about all these features in our
 [DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home).
 
 ## config_history
 
 The Config History is a side-feature of the main Config System. It can be
 configured for any project which uses the Config System and provides a
 flexible framework to easily build graphs representing past experiments. In
 these graphs, each node represents an experiment, and vertices are drawn
-between your experiments to visualize easily which parameters changed from one
+between your experiments to visualise easily which parameters changed from one
 node to another.
 
 The graph can be coloured to show your most successful experiments, or grouped
 by parameters to see how well they have been explored in your experiment
 history. This makes it very useful to review your past work, share it with
 colleagues or make unexpected correlations appear.
```

### Comparing `yaecs-3.2.5/docs/index.rst` & `yaecs-4.0.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 This package is a Config System which allows easy manipulation of config
 files for safe, clear and repeatable experiments. In a few words, it is:
 
 -  built for Machine Learning with its constraints in mind, but also
    usable out-of-the-box for other kinds of projects;
 -  built with scalability in mind and can adapt just as easily to large
-   projects investigating hundreds of well-organized parameters across
+   projects investigating hundreds of well-organised parameters across
    many experiments;
 -  designed to encourage good coding practices for research purposes,
    and if used rigorously will ensure a number of highly desirable
    properties such that **maintenance-less forward-compatibility** of
    old configs, **easy reproducibility** of any experiment, and
    **extreme clarity** of former experiments for your future self or
    collaborators.
```

### Comparing `yaecs-3.2.5/docs/license.md` & `yaecs-4.0.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/docs/make.bat` & `yaecs-4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/docs/yaecs.rst` & `yaecs-4.0.2/docs/yaecs.rst`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/docs/yaecs_config.rst` & `yaecs-4.0.2/docs/yaecs_config.rst`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/pyproject.toml` & `yaecs-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/resources/yaecs_constructor_overview.png` & `yaecs-4.0.2/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/setup.py` & `yaecs-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/short-readme.md` & `yaecs-4.0.2/short-readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return {}
 ```
 
 That's all there is to it! Now if we use
 `config = ProjectSpecific.load_config()`, we can then call `config.data_path`
 or `config.learning_rate` to get their values as defined in the default config.
 We don't need to specify where to get the default config because a project
-should only ever have one default config, which centralizes all the parameters
+should only ever have one default config, which centralises all the parameters
 in that project. Since the location of the default config is a project
 constant, it is defined in your project-specific subclass and there is no
 need to clutter your main code with it. Now, for example, your main.py could
 look like:
 
 ```python
 from project_config import ProjectSpecific
```

### Comparing `yaecs-3.2.5/unittests/config/conftest.py` & `yaecs-4.0.2/unittests/config/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 def yaml_default(tmpdir):
     index = len(os.listdir(tmpdir))
     content = (f"param1: 0.1\n--- !subconfig1\nparam2: 3.0\n---\n"
                f"def_second_path: '{tmpdir / f'default_second{index}.yaml'}'\n"
                "exp_second_path: null")
     with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
         fil.write(content)
-    content = ("--- !subconfig2\nparam3: 20.0\nsubconfig3: !subconfig3\n  "
+    content = ("--- !subconfig2\nparam3: 20.0\nsubconfig3:\n  "
                "param4: 'string'")
     with open(tmpdir / f'default_second{index}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'default{index}.yaml')
 
 
@@ -61,15 +61,15 @@
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'experiment{index}.yaml')
 
 
 @pytest.fixture
 def yaml_default_unlinked(tmpdir):
-    content = "param1:\n  param2: 1\n  param3: !param3\n    param4: 2"
+    content = "param1: !type:dict\n  param2: 1\n  param3:\n    param4: 2"
     with open(tmpdir / f'tmp{len(os.listdir(tmpdir))}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
@@ -79,15 +79,15 @@
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
 def yaml_default_sub_variations(tmpdir):
-    content = "param1: !param1\n  var: []"
+    content = "param1:\n  var: []"
     with open(tmpdir / f'tmp{len(os.listdir(tmpdir))}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
@@ -97,58 +97,58 @@
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
 def yaml_experiment_sub_star(tmpdir):
-    content = "subconfig2: !subconfig2\n  '*param*': 1.0"
+    content = "subconfig2:\n  '*param*': 1.0"
     with open(tmpdir / f'tmp{len(os.listdir(tmpdir))}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
 def yaml_experiment_sub_dot(tmpdir):
-    content = "subconfig2: !subconfig2\n  subconfig3.param4: 1.0"
+    content = "subconfig2:\n  subconfig3.param4: 1.0"
     with open(tmpdir / f'tmp{len(os.listdir(tmpdir))}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'tmp{len(os.listdir(tmpdir))-1}.yaml')
 
 
 @pytest.fixture
 def yaml_craziest_config(tmpdir):
     with open(tmpdir / 'd_first.yaml', "w", encoding='utf-8') as fil:
         fil.write("p1: 1\n"
                   "--- !c1\n"
-                  "c2: !c2\n"
+                  "c2:\n"
                   f"  f_path: {'d_second.yaml'}\n"
                   "---\n"
                   "c4.p3: 3\n"
                   "c4.p7: 7\n"
                   f"f_path: {tmpdir / 'd_second.yaml'}")
     with open(tmpdir / 'd_second.yaml', "w", encoding='utf-8') as fil:
         fil.write("--- !c3\n"
                   "p2: 2\n"
                   f"c5.s_path: {tmpdir / 'd_third.yaml'}\n"
                   "---\n"
                   "p6: 6")
     with open(tmpdir / 'd_third.yaml', "w", encoding='utf-8') as fil:
         fil.write("--- !c6\n"
-                  "p4: {a: 4}\n"
+                  "p4: !type:(dict,int) {a: 4}\n"
                   "---\n"
                   "p5: 5")
     with open(tmpdir / 'e_first.yaml', 'w', encoding='utf-8') as fil:
         fil.write("'*p6': 7\n"
                   "--- !c1\n"
                   f"c2.f_path: {tmpdir / 'e_second.yaml'}\n"
                   "---\n"
-                  "c4: !c4\n"
+                  "c4:\n"
                   "  p3: 'test'\n"
                   "c4.p7: 'test2'")
     with open(tmpdir / 'e_second.yaml', "w", encoding='utf-8') as fil:
         fil.write("--- !c3\n"
                   "'*.p*': 8\n"
                   "'*p4': {b: 5}")
     yield str(tmpdir / 'd_first.yaml'), str(tmpdir / 'e_first.yaml')
@@ -181,20 +181,20 @@
                           do_not_merge_command_line=True)
     yield config, config2
 
 
 @pytest.fixture
 def yaml_no_file_call_processing_while_loading_nested(tmpdir):
     with open(tmpdir / 'nd_first.yaml', "w", encoding='utf-8') as fil:
-        fil.write(f"c: !c\n  test_path: {tmpdir / 'nd_second.yaml'}\n  "
+        fil.write(f"c:\n  test_path: {tmpdir / 'nd_second.yaml'}\n  "
                   "exp_path: null")
     with open(tmpdir / 'nd_second.yaml', "w", encoding='utf-8') as fil:
         fil.write("param: 0.1")
     with open(tmpdir / 'ne_first.yaml', "w", encoding='utf-8') as fil:
-        fil.write(f"c: !c\n  exp_path: {tmpdir / 'ne_second.yaml'}")
+        fil.write(f"c:\n  exp_path: {tmpdir / 'ne_second.yaml'}")
     with open(tmpdir / 'ne_second.yaml', "w", encoding='utf-8') as fil:
         fil.write("param: 0.2")
     config = make_config(str(tmpdir / 'nd_first.yaml'),
                          str(tmpdir / 'ne_first.yaml'),
                          additional_configs_suffix="_path",
                          variations_suffix="var*", grids_suffix="grid",
                          do_not_merge_command_line=True)
@@ -210,15 +210,15 @@
                           do_not_merge_command_line=True)
     yield config, config2
 
 
 @pytest.fixture
 def yaml_type_check(tmpdir):
     index = len(os.listdir(tmpdir))
-    content = (f"root_path: '{tmpdir / f'default_second{index}.yaml'}'\nsubconfig: !subconfig\n  "
+    content = (f"root_path: '{tmpdir / f'default_second{index}.yaml'}'\nsubconfig:\n  "
                f"sub_path: '{tmpdir / f'default_second{index}.yaml'}'")
     with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
         fil.write(content)
     content = ("param_int: !type:int 1\nparam_float: !type:float 0.1\nparam_str: !type:str abc\n"
                "param_bool: !type:bool false\n"
                "param_none: !type:none null\nparam_list: !type:list [0]\nparam_dict: !type:dict\n  a: 0\n"
                "param_any: !type:Any null\nparam_tuple1: !type:(str,float) 0.4\nparam_tuple2: !type:(str,float) ab\n"
@@ -235,13 +235,42 @@
 def yaml_tag_assignment_check(tmpdir):
     index = len(os.listdir(tmpdir))
     content = (f"param1: !type:add_1 0.1\n--- !subconfig1\nparam2: 3.0\n---\n"
                f"def_second_path: '{tmpdir / f'default_second{index}.yaml'}'\n"
                "exp_second_path: null")
     with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
         fil.write(content)
-    content = ("--- !subconfig2\nparam3: 20.0\nsubconfig3: !subconfig3\n  "
+    content = ("--- !subconfig2\nparam3: 20.0\nsubconfig3:\n  "
                "param4: !type:copy 'param1'")
     with open(tmpdir / f'default_second{index}.yaml', "w",
               encoding='utf-8') as fil:
         fil.write(content)
     yield str(tmpdir / f'default{index}.yaml')
+
+
+@pytest.fixture
+def config_vs_dict_checks(tmpdir):
+    index = len(os.listdir(tmpdir))
+    content = ("config1:\n"
+               "  config2:\n"
+               "    param1: !type:dict\n"
+               "      key1: !type:dict\n"
+               "        key2: 0\n"
+               "      key3: ['!type:dict']\n"
+               "--- !config3.config4\n"
+               "config5:\n"
+               "  config6:\n"
+               "    param1: !type:dict\n"
+               "      key1: !type:dict\n"
+               "        key1: 0\n"
+               "      key2: ['!type:dict']\n"
+               "--- !config10.config11\n"
+               "config1.config7: !main_2\n"
+               "  config8:\n"
+               "    param1: !type:dict\n"
+               "      key1: !type:dict\n"
+               "        key1: 0\n"
+               "      key2: ['!type:dict']\n"
+               "  config9.param2: null")
+    with open(tmpdir / f'default{index}.yaml', "w", encoding='utf-8') as fil:
+        fil.write(content)
+    yield str(tmpdir / f'default{index}.yaml')
```

### Comparing `yaecs-3.2.5/unittests/config/test_config.py` & `yaecs-4.0.2/unittests/config/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os.path as osp
 from pathlib import Path
 from typing import Any
 
 import pytest
 
 from unittests.config.utils import load_config, template
-from yaecs import Configuration, Priority, assign_order, assign_yaml_tag
+from yaecs import Configuration, Experiment, Priority, assign_order, assign_yaml_tag
 from yaecs.user_utils import make_config
 from yaecs.yaecs_utils import compare_string_pattern
 
 
 def check_integrity(config, p_1: Any = 0.1, p_2: Any = 2.0, p_3: Any = 30.0,
                     p_4: Any = "string"):
     assert config["param1"] == p_1
@@ -357,15 +357,16 @@
             "var2": [{
                 "p2": 1.0
             }, {
                 "p2": 2.0
             }, {
                 "p2": 3.0
             }],
-            "grid": None
+            "grid": None,
+            "tracker_config": {"type": []}
         }, config_class=template(yaml_default), do_not_merge_command_line=True)
     captured = capsys.readouterr()
     assert "WARNING" not in captured.out
     assert config.p1 == 0.1 and config.p2 == 1.0
     variations = config.create_variations()
     assert len(variations) == 5
     assert variations[0] == variations[2] == config
@@ -378,14 +379,18 @@
     assert (variations[0] == config
             and variations[1].p1 == variations[2].p1 == 0.1
             and variations[3].p2 == 1.0)
     assert variations[3].p1 == variations[4].p1 == variations[5].p1 == 0.2
     assert (variations[1].p2 == variations[4].p2 == 2.0
             and variations[2].p2 == variations[5].p2 == 3.0)
 
+    def _main(config, tracker):
+        return
+    Experiment(config, _main, experiment_name="test", run_name="test").run(run_description="")
+
 
 def test_pre_processing(capsys, tmp_file_name,
                         yaml_no_file_call_processing_while_loading,
                         yaml_default,
                         yaml_no_file_call_processing_while_loading_nested,
                         yaml_default_preproc_default_dot_param,
                         yaml_experiment):
@@ -473,26 +478,27 @@
         def __eq__(self, other):
             return self.stored == other.stored
 
         def __repr__(self):
             return f"<Storage: {self.stored}>"
 
     postprocessing = {"*to_store": lambda x: Storage(**x)}
-    config = make_config({
+    default = {
         "a": 10,
         "b.to_store": {
             "i": 1,
             "j": 2
         }
-    }, post_processing_dict=postprocessing)
+    }
+    config = make_config(default, post_processing_dict=postprocessing)
     config.save(str(tmp_file_name))
-    assert config == make_config(str(tmp_file_name),
+    assert config == make_config(default, str(tmp_file_name),
                                  post_processing_dict=postprocessing)
-    assert make_config(str(tmp_file_name)).b.to_store == {"i": 1, "j": 2}
-    assert make_config(str(tmp_file_name)).a == 10
+    assert make_config(default, str(tmp_file_name)).b.to_store == {"i": 1, "j": 2}
+    assert make_config(default, str(tmp_file_name)).a == 10
     # Does post-processing interact correctly with get_command_line_arguments ?
     config = make_config({
         "a": 10,
         "b.to_store": {
             "i": 1,
             "j": 2
         }
@@ -671,14 +677,33 @@
         return value * 2
 
     postprocessing = {"param1": (add_1, double_value)}
     config = load_config(default_config=yaml_default, postprocessing=postprocessing)
     check_integrity(config, p_1=2.2, p_2=3.0, p_3=20.0)
 
 
+def test_config_vs_dict_checks(caplog, config_vs_dict_checks):
+
+    with caplog.at_level(logging.WARNING):
+        logging.getLogger("yaecs").propagate = True
+        config = load_config(default_config=config_vs_dict_checks)
+    assert caplog.text.count("WARNING") == 2
+    string = f"\nMAIN CONFIG :\nConfiguration hierarchy :\n> {config_vs_dict_checks}" \
+             "\n\n - config1 : \n	CONFIG1 CONFIG :\n	 - config2 : \n		CONFIG2 CONFIG :\n" \
+             "		 - param1 : {'key1': {'key2': 0}, 'key3': ['!type:dict']}\n\n\n - config3 : \n	CONFIG3 CONFIG :" \
+             "\n	 - config4 : \n		CONFIG4 CONFIG :\n		 - config5 : \n			CONFIG5 CONFIG :" \
+             "\n			 - config6 : \n				CONFIG6 CONFIG :\n				 - param1 : {'key1': {'key1':" \
+             " 0}, 'key2': ['!type:dict']}\n\n\n\n\n - config10 : \n	CONFIG10 CONFIG :\n	 - config11 : " \
+             "\n		CONFIG11 CONFIG :\n		 - config1 : \n			CONFIG1 CONFIG :\n			 - config7 : " \
+             "\n				CONFIG7 CONFIG :\n				 - config8 : \n					CONFIG8 CONFIG :" \
+             "\n					 - param1 : {'key1': {'key1': 0}, 'key2': ['!type:dict']}\n\n				 - co" \
+             "nfig9 : \n					CONFIG9 CONFIG :\n					 - param2 : None\n\n\n\n\n\n"
+    assert config.details() == string
+
+
 def test_warnings(caplog, tmp_file_name):
     # config = ConfigForTests(config_path_or_dictionary={
     #     "param": None, "lparam": [], "dparam": {"param2": 1}})
     # config.merge_from_command_line("--param=1 --lparam=[1] "
     #                                "--dparam={param2:2,param3:3}")
     # captured = capsys.readouterr()
     # assert captured.out.count("is None. It cannot be replaced from the") == 1
```

### Comparing `yaecs-3.2.5/unittests/config/utils.py` & `yaecs-4.0.2/unittests/config/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,9 +27,9 @@
                        additional_configs_suffix="_path",
                        variations_suffix="var*", grids_suffix="grid",
                        do_not_merge_command_line=True)
 
 
 def template(default_config=None):
     return get_template_class(default_config_path=default_config,
-                              additional_configs_suffix="_path",
+                              additional_configs_suffix="_path", tracker_config="tracker_config",
                               variations_suffix="var*", grids_suffix="grid")
```

### Comparing `yaecs-3.2.5/usage_example/configs/project_config.py` & `yaecs-4.0.2/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/usage_example/main.py` & `yaecs-4.0.2/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/usage_example/project_utils/utils.py` & `yaecs-4.0.2/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/yaecs/__init__.py` & `yaecs-4.0.2/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/yaecs/config/config.py` & `yaecs-4.0.2/yaecs/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
 import sys
 import time
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional
 
-from ..yaecs_utils import ConfigDeclarator, format_str
+from ..yaecs_utils import ConfigInput, ConfigDeclarator, format_str, get_config_from_argv
 from .config_base import _ConfigurationBase
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class Configuration(_ConfigurationBase):
     """
@@ -70,15 +70,15 @@
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param verbose: if set to false, message logging by this config will be deactivated
         :raises ValueError: if the overwriting regime is not valid
         :return: none
         """
 
-        # PROTECTED ATTRIBUTES
+        # Set protected attributes
         object.__setattr__(self, "_operating_creation_or_merging", True)
         self._state = [] if state is None else state
         self._main_config = self if main_config is None else main_config
         self._methods = [name for name in dir(self)
                          if name not in ["_operating_creation_or_merging", "_main_config", "_state"]]
         self._configuration_variations = []
         self._configuration_variations_names = []
@@ -87,43 +87,52 @@
         self._nesting_hierarchy = ([] if nesting_hierarchy is None else list(nesting_hierarchy))
         self._variation_name = (variation if main_config is None else main_config.get_variation_name())
         self._verbose = verbose
         kwargs = {"do_not_pre_process": do_not_pre_process, "do_not_post_process": do_not_post_process, **kwargs}
         super().__init__(**kwargs)
         self._protected_attributes = list(self.__dict__) + ["_protected_attributes"]
 
-        # SPECIAL ATTRIBUTES
+        # Set config metadata
         self.config_metadata = {
             "saving_time": time.time(),
             "config_hierarchy": [],
             "overwriting_regime": (overwriting_regime if main_config is None
                                    else main_config.config_metadata["overwriting_regime"]),
         }
         if self.config_metadata["overwriting_regime"] not in ["unsafe", "auto-save", "locked"]:
             raise ValueError("'overwriting_regime' needs to be either 'auto-save', "
                              "'locked' or 'unsafe'.")
 
-        # INITIALISATION
+        # Initialise config
         self._state.append(f"setup;{self._name}")
         config_path_or_dictionary = (self.get_default_config_path()
                                      if config_path_or_dictionary is None else config_path_or_dictionary)
         self.init_from_config(config_path_or_dictionary)
-        self.config_metadata["config_hierarchy"] = ([] if not self._nesting_hierarchy else list(
-            main_config.get('.'.join(self._nesting_hierarchy[:-1]), main_config).config_metadata['config_hierarchy']))
+
+        # Find config hierarchy from parents and set it
+        param = None
+        if self._nesting_hierarchy:
+            for index in range(len(self._nesting_hierarchy) - 1):
+                param = main_config.get('.'.join(self._nesting_hierarchy[:index + 1]), main_config)
+                if not isinstance(param, _ConfigurationBase):
+                    param = None  # encountered in temporary configs when merging a deep dict
+                    break
+        self.config_metadata["config_hierarchy"] = [] if param is None else param.config_metadata['config_hierarchy']
         self.config_metadata["config_hierarchy"] += [config_path_or_dictionary]
+
+        # Checkup and post-setup operations
         if not self._nesting_hierarchy:
             self._check_for_unlinked_sub_configs()
         if main_config is None:
             self.set_pre_processing(True)
         self._state.pop(-1)
         self._operating_creation_or_merging = False
 
     @classmethod
-    def load_config(cls, *configs: Union[List[ConfigDeclarator],
-                                         ConfigDeclarator], default_config_path: Optional[ConfigDeclarator] = None,
+    def load_config(cls, *configs: ConfigInput, default_config_path: Optional[ConfigDeclarator] = None,
                     overwriting_regime: str = "auto-save", do_not_merge_command_line: bool = False,
                     do_not_pre_process: bool = False, do_not_post_process: bool = False,
                     **kwargs) -> 'Configuration':
         """
         First creates a config using the default config, then merges config_path into it. If config_path is a list,
         successively merges all configs in the list instead from index 0 to the last.
 
@@ -156,18 +165,17 @@
                 config._merge(to_merge, do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process,
                               source="command line")
         config._post_process_modified_parameters()
         config.set_post_processing(True)
         return config
 
     @classmethod
-    def build_from_configs(cls, *configs: Union[List[ConfigDeclarator], ConfigDeclarator],
-                           overwriting_regime: str = "auto-save", do_not_merge_command_line: bool = False,
-                           do_not_pre_process: bool = False, do_not_post_process: bool = False,
-                           **kwargs) -> 'Configuration':
+    def build_from_configs(cls, *configs: ConfigInput, overwriting_regime: str = "auto-save",
+                           do_not_merge_command_line: bool = False, do_not_pre_process: bool = False,
+                           do_not_post_process: bool = False, **kwargs) -> 'Configuration':
         """
         First creates a config using the first config provided (or the first config in the provided list), then merges
         the subsequent configs into it from index 1 to the last.
 
         :param configs: config's path or dictionary, or list of default config's paths or dictionaries to merge
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
             config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
@@ -190,52 +198,47 @@
                             "please use build_from_configs([cfg1, cfg2, ...]) or "
                             "build_from_configs(cfg1, cfg2, ...)")
         return cls.load_config(list(configs[1:]), default_config_path=configs[0], overwriting_regime=overwriting_regime,
                                do_not_merge_command_line=do_not_merge_command_line,
                                do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process, **kwargs)
 
     @classmethod
-    def build_from_argv(cls, *configs: Union[List[ConfigDeclarator], ConfigDeclarator], fallback: Optional[str] = None,
+    def build_from_argv(cls, *configs: ConfigInput, fallback: Optional[ConfigInput] = None, pattern: str = "--config",
                         default_config_path: Optional[ConfigDeclarator] = None, overwriting_regime: str = "auto-save",
                         do_not_merge_command_line: bool = False, do_not_pre_process: bool = False,
                         do_not_post_process: bool = False, **kwargs) -> 'Configuration':
         """
         Assumes a pattern of the form '--config <path_to_config>' or '--config [<path1>,<path2>,...]' in sys.argv (the
         brackets are optional), and builds a config from the specified paths by merging them into the default config in
         the specified order.
 
         :param configs: config's path or dictionary, or list of config paths or dictionaries to merge. Those will be
             merged to the default config before the config from the command line.
         :param fallback: config path or dictionary, or list of config paths or dictionaries to fall back to if no config
             was detected in the argv
+        :param pattern: pattern to look for in sys.argv
         :param default_config_path: default config's path or dictionary
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
             config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
             using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility
             is not guaranteed).
         :param do_not_merge_command_line: if True, does not try to merge the command line parameters
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param kwargs: additional parameters to pass to Configuration
         :raises TypeError: if --config is not found and no fallback
         :return: instance of Configuration object containing the desired config
         """
-        if "--config" not in sys.argv and fallback is None:
-            raise TypeError("The pattern '--config' was not detected "
-                            "in sys.argv.")
-        if "--config" in sys.argv:
-            fallback = [cfg.strip(" ") for cfg in sys.argv[sys.argv.index("--config") + 1].strip("[]").split(",")]
-        if not isinstance(fallback, list):
-            fallback = [fallback]
+        configs_from_argv: List[ConfigDeclarator] = get_config_from_argv(pattern=pattern, fallback=fallback)
 
-        return cls.load_config(*configs, *fallback, default_config_path=default_config_path,
+        return cls.load_config(*configs, *configs_from_argv, default_config_path=default_config_path,
                                overwriting_regime=overwriting_regime,
                                do_not_merge_command_line=do_not_merge_command_line,
                                do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process,
-                               from_argv=True, **kwargs)
+                               from_argv=pattern if pattern in sys.argv else "", **kwargs)
 
     def create_variations(self) -> List['Configuration']:
         """
         Creates a list of configs that are derived from the current config using the internally tracked variations and
         grids registered via the corresponding functions (register_as_config_variations and register_as_grid).
 
         :raises TypeError: if grid dimension is empty or not registered
@@ -364,16 +367,17 @@
         Sets the variation index of the config. This function is not intended to be used by the user.
 
         :param name: index to set the variation index with
         :param deep: whether to also recursively set the variation name of all sub-configs
         """
         object.__setattr__(self, "_variation_name", name)
         if deep:
-            for subconfig in self._sub_configs_list:
-                subconfig.set_variation_name(name, deep=True)
+            for subconfig in self.get_all_sub_configs():
+                if ".".join(subconfig.get_nesting_hierarchy()).startswith(".".join(self.get_nesting_hierarchy())):
+                    object.__setattr__(subconfig, "_variation_name", name)
 
     @classmethod
     def _get_instance(cls, name: str = "main", overwriting_regime: str = "auto-save",
                       config_path_or_dictionary: Optional[ConfigDeclarator] = None,
                       nesting_hierarchy: Optional[List[str]] = None, state: Optional[List[str]] = None,
                       main_config: Optional['Configuration'] = None, variation: Optional[str] = None,
                       do_not_pre_process: bool = False, do_not_post_process: bool = False, verbose: bool = True,
```

### Comparing `yaecs-3.2.5/yaecs/config/config_base.py` & `yaecs-4.0.2/yaecs/config/config_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,44 +20,23 @@
 import logging
 import os
 import sys
 from collections.abc import Iterable
 from functools import partial
 from numbers import Real
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
+from typing import (TYPE_CHECKING,
+                    Any, Callable, Dict, List, Optional, Tuple, Type, Union)
 
 import yaml
 
-from ..yaecs_utils import (
-    YAML_EXPRESSIONS,
-    ConfigDeclarator,
-    TypeHint,
-    adapt_to_type,
-    are_same_sub_configs,
-    compare_string_pattern,
-    compose,
-    format_str,
-    get_order,
-    is_type_valid,
-    parse_type,
-    recursive_set_attribute,
-    set_function_attribute,
-    update_state,
-)
+from ..yaecs_utils import (YAML_EXPRESSIONS,
+                           ConfigDeclarator, TypeHint,
+                           adapt_to_type, compare_string_pattern, compose, format_str, get_order, is_type_valid,
+                           parse_type, recursive_set_attribute, set_function_attribute, update_state)
 from .config_convenience import ConfigConvenienceMixin
 from .config_getters import ConfigGettersMixin
 from .config_hooks import ConfigHooksMixin
 from .config_processing_functions import ConfigProcessingFunctionsMixin
 from .config_setters import ConfigSettersMixin
 
 if TYPE_CHECKING:
@@ -83,20 +62,20 @@
     _methods: List[str]
     _nesting_hierarchy: List[str]
     _operating_creation_or_merging: bool
     _protected_attributes: List[str]
     _state: List[str]
     _verbose: bool
 
-    def __init__(self, from_argv: bool = False, do_not_pre_process: bool = False, do_not_post_process: bool = False):
+    def __init__(self, from_argv: str = "", do_not_pre_process: bool = False, do_not_post_process: bool = False):
         """
         Should never be called directly by the user. Please use one of the constructors defined for the Configuration
         class instead, or the utils.make_config convenience function.
 
-        :param from_argv: whether the config was created with configs passed from the command line arguments
+        :param from_argv: pattern used to find the config in the command line arguments, or "" if not applicable
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :raises ValueError: if the overwriting regime is not valid
         :return: none
         """
 
         # PROTECTED ATTRIBUTES
@@ -244,15 +223,15 @@
 
         :param config_path_or_dict: path or dictionary for the config to merge
         """
         if config_path_or_dict is not None:
             if isinstance(config_path_or_dict, str):
                 with open(self._find_path(config_path_or_dict), encoding='utf-8') as yaml_file:
                     for dictionary_to_add in yaml.load_all(yaml_file, Loader=self._get_yaml_loader()):
-                        for item in dictionary_to_add.items():
+                        for item in self._superficial_dict_cleanup(dictionary_to_add).items():
                             self._process_item_to_merge_or_add(item)
             else:
                 for item in config_path_or_dict.items():
                     self._process_item_to_merge_or_add(item)
 
     def merge(self, config_path_or_dictionary: ConfigDeclarator, do_not_pre_process: bool = False,
               do_not_post_process: bool = False) -> None:
@@ -299,15 +278,15 @@
     def _check_for_unlinked_sub_configs(self) -> None:
         """ Used to raise an error when unlinked sub-configs are declared. """
         all_configs = self.get_all_sub_configs()
         linked_configs = self.get_all_linked_sub_configs()
         for i in all_configs:
             found_correspondence = False
             for j in linked_configs:
-                if are_same_sub_configs(i, j):
+                if self._are_same_sub_configs(i, j):
                     found_correspondence = True
                     break
             if not found_correspondence:
                 raise RuntimeError(f"Sub-config '{i.get_name()}' is unlinked. Unlinked "
                                    "sub-configs are not allowed.")
 
     def _find_path(self, path: str) -> str:
@@ -390,16 +369,19 @@
         raise FileNotFoundError(f"ERROR : path not found ({path}).")
 
     def _get_yaml_loader(self) -> Type[yaml.FullLoader]:
         """ Used to get a custom YAML loader capable of parsing config tags. """
 
         def generic_constructor(yaml_loader, tag, node):
 
-            if tag[1:].lower().startswith("type:"):
-                if not yaml_loader.constructed_objects:
+            is_param_tag = bool(yaml_loader.constructed_objects)
+
+            # If type tag, handle type-hinting or processing assignment.
+            if tag[1:].lower().startswith("type:") and tag[1:].lower() != "type:config":
+                if not is_param_tag:
                     raise RuntimeError(f"'{tag[1:]}' is not a valid sub-config name.")
                 if not any(state.startswith("setup") for state in self._state):
                     raise RuntimeError("Type-hinting is only allowed in the default config.")
                 name = yaml_loader.constructed_objects[list(yaml_loader.constructed_objects.keys())[-1]]
                 name = self._get_full_path(name)
                 type_hint = tag[6:]
                 if type_hint in self._assigned_as_yaml_tags:
@@ -421,47 +403,55 @@
                         if _can_be_str(parse_type(tag[6:])):
                             return yaml_loader.yaml_constructors["tag:yaml.org,2002:str"](yaml_loader, node)
                     for key, value in YAML_EXPRESSIONS.items():
                         if value.match(node.value):
                             return yaml_loader.yaml_constructors[f"tag:yaml.org,2002:{key}"](yaml_loader, node)
                     return yaml_loader.construct_scalar(node)
                 if isinstance(node, yaml.SequenceNode):
-                    return yaml_loader.construct_sequence(node)
+                    return yaml_loader.construct_sequence(node, deep=True)
                 if isinstance(node, yaml.MappingNode):
-                    return yaml_loader.construct_mapping(node)
-
-            sub_configs_name = tag[1:].split(".")
-            sub_config_name = sub_configs_name[0]
-            if len(sub_configs_name) > 1:
-                to_append = ".".join(sub_configs_name[1:])
-                for i in range(len(node.value)):  # pylint: disable=consider-using-enumerate
-                    node.value[i][0].value = to_append + "." + node.value[i][0].value
-            self._nesting_hierarchy.append(sub_config_name)
-            if yaml_loader.constructed_objects:
-                dict_to_return = self._get_instance(
-                    name=sub_config_name, config_path_or_dictionary=yaml_loader.construct_mapping(node, deep=True),
-                    nesting_hierarchy=self._nesting_hierarchy, state=self._state, main_config=self._main_config,
-                    verbose=self._verbose)
-                if all(not are_same_sub_configs(i, dict_to_return) for i in self._sub_configs_list):
-                    self._sub_configs_list.append(dict_to_return)
+                    return yaml_loader.construct_mapping(node, deep=True)
 
+            # Otherwise, assume sub-config tag
+            if is_param_tag:
+                # Case 1 : not root of the YAML file > infer name from parameter name
+                sub_configs_names = list(yaml_loader.constructed_objects.keys())[-1].value.split(".")
+                sub_config = sub_configs_names[0]
+                apply_to_node = ".".join(sub_configs_names[1:])
+                if tag[1:].lower() != "type:config":
+                    YAECS_LOGGER.warning(f"WARNING : Naming sub-configs is deprecated. Tag '{tag}' will be ignored and "
+                                         "should be removed. They might be used for a different purpose in a future "
+                                         "release."
+                                         "\nSince now YAML dicts are implicitly considered sub-configs, be sure to tag "
+                                         "with '!type:dict' if you want to use a dict.")
             else:
-                dict_to_return = {
-                    sub_config_name:
-                    self._get_instance(name=sub_config_name,
-                                       config_path_or_dictionary=yaml_loader.construct_mapping(node, deep=True),
-                                       nesting_hierarchy=self._nesting_hierarchy, state=self._state,
-                                       main_config=self._main_config, verbose=self._verbose)
-                }
-                if all(not are_same_sub_configs(i, dict_to_return[sub_config_name]) for i in self._sub_configs_list):
-                    self._sub_configs_list.append(dict_to_return[sub_config_name])
+                if tag[1:].lower() == "type:config":
+                    # Case 2 : name not provided and root of the YAML file > assume dict
+                    return yaml_loader.construct_mapping(node, deep=True)
+                # Case 3 : name provided and root of the YAML file > use first part as config name
+                sub_configs_names = tag[1:].split(".")
+                sub_config = sub_configs_names[0]
+                apply_to_node = ".".join(sub_configs_names[1:])
+
+            if apply_to_node:
+                # Add prefix to all sub-config parameters
+                for i in range(len(node.value)):  # pylint: disable=consider-using-enumerate
+                    node.value[i][0].value = apply_to_node + "." + node.value[i][0].value
+            self._nesting_hierarchy.append(sub_config)  # needs to be set temporarily (potential recursive call)
+            to_convert = yaml_loader.construct_mapping(node)
+            new_config = self._get_instance(name=sub_config,
+                                            config_path_or_dictionary=self._superficial_dict_cleanup(to_convert),
+                                            nesting_hierarchy=self._nesting_hierarchy, state=self._state,
+                                            main_config=self._main_config, verbose=self._verbose)
+            self.set_sub_config(new_config)
             self._nesting_hierarchy.pop(-1)
-            return dict_to_return
+            return new_config if is_param_tag else {sub_config: new_config}
 
         loader = yaml.FullLoader
+        loader.DEFAULT_MAPPING_TAG = "!type:config"
         yaml.add_multi_constructor("", generic_constructor, Loader=loader)
         return loader
 
     def _manual_merge(self, config_path_or_dictionary: ConfigDeclarator, do_not_pre_process: bool = False,
                       do_not_post_process: bool = False, source: str = 'config',
                       ) -> None:
         """ This method is called whenever a merge is done by the user, and not by the config creation process. It
@@ -490,15 +480,15 @@
             self.set_pre_processing(True)
             self._operating_creation_or_merging = False
         else:
             dicts_to_merge = []
             if isinstance(config_path_or_dictionary, str):
                 with open(self._find_path(config_path_or_dictionary), encoding='utf-8') as yaml_file:
                     for dictionary_to_add in yaml.load_all(yaml_file, Loader=self._get_yaml_loader()):
-                        dicts_to_merge.append(dictionary_to_add)
+                        dicts_to_merge.append(self._superficial_dict_cleanup(dictionary_to_add))
                     yaml_file.close()
             else:
                 dicts_to_merge.append(config_path_or_dictionary)
             for dictionary in dicts_to_merge:
                 self._main_config._merge(  # pylint: disable=protected-access
                     {self._get_full_path(a): b
                      for a, b in dictionary.items()}, do_not_pre_process=do_not_pre_process,
@@ -586,22 +576,28 @@
                 old_value = getattr(self, "___" + key if key in self._methods else key)
             except AttributeError as exception:
                 raise AttributeError(f"ERROR : parameter '{key}' cannot be merged : "
                                      f"it is not in the default '{self.get_name().upper()}' "
                                      f"config.\n{self._did_you_mean(key)}") from exception
             if isinstance(old_value, _ConfigurationBase):
                 if isinstance(value, _ConfigurationBase):
+                    self.unset_sub_config(value)
                     old_value.init_from_config(value.get_dict(deep=False))
                 elif isinstance(value, dict):
                     old_value.init_from_config(value)
                 else:
                     raise TypeError(f"Trying to set sub-config '{old_value.get_name()}'\n"
                                     f"with non-config element '{value}'.\n"
                                     "This replacement cannot be performed.")
             else:
+                if isinstance(value, _ConfigurationBase):
+                    self.unset_sub_config(value)
+                    for sub_config in value.get_all_linked_sub_configs():
+                        self.unset_sub_config(sub_config)
+                    value = value.get_dict(deep=True)
                 if self._verbose:
                     YAECS_LOGGER.debug(f"Setting '{key}' : \nold : '{old_value}' \n"
                                        f"new : '{value}'.")
                 object.__setattr__(self, "___" + key if key in self._methods else key,
                                    self._process_parameter(key, value, "pre"))
                 if key not in self._modified_buffer:
                     self._modified_buffer.append(key)
@@ -681,14 +677,15 @@
             self[name].add_type_hint(type_hint[len(prefix):], self._main_config.get_type_hint(type_hint))
             self._main_config.remove_type_hint(type_hint)
         if type_hints is not None:
             for key, value in type_hints.items():
                 self[name].add_type_hint(key, value)
         self[name].init_from_config(content)
         self[name].config_metadata["config_hierarchy"] += [content]
+        self.set_sub_config(self[name])
 
     def _gather_command_line_dict(self, string_to_merge: Optional[str] = None) -> Dict[str, Any]:
         """ Method called automatically at the end of each constructor to gather all parameters from the command line
         into a dictionary. This dictionary is then merged. """
         # If a string is passed as input, process it as sys.argv would
         if string_to_merge is not None:
             list_to_merge = [""]
@@ -714,19 +711,19 @@
 
         # Setting the config to operational mode in case this
         # is called manually
         object.__setattr__(self, "_operating_creation_or_merging", True)
 
         # Gather parameters, their values and their types
         to_merge = {}  # {param_name: [former_value, new_value, type_forcing], ...}
-        found_config_path = not self._from_argv
+        found_config_path = not bool(self._from_argv)
         in_param = []
         un_matched_params = []
         for element in list_to_merge:
-            if element.startswith("--") and (found_config_path or element[2:] != "config"):
+            if element.startswith("--") and (found_config_path or element != self._from_argv):
                 if "=" in element:
                     pattern, value = element[2:].split("=", 1)
                     value = value if value != "" else None
                 else:
                     pattern, value = element[2:], None
                 in_param = []
                 for parameter in self.get_parameter_names(deep=True):
@@ -852,7 +849,12 @@
                 main.save_value_before_postprocessing(self._get_full_path(name), old_value)
         elif processing_type == "pre":
             for processor in processors:
                 if processor.__name__.startswith("yaecs_config_hook__"):
                     for hook_name in processor.__name__.split("__")[1].split(","):
                         self.add_currently_processed_param_as_hook(hook_name)
         return parameter
+
+    @staticmethod
+    def _superficial_dict_cleanup(dictionary: dict) -> dict:
+        """ After a YAML loading operation, cleans up composed keys of Configuration items. """
+        return {(k.split(".")[0] if isinstance(v, _ConfigurationBase) else k): v for k, v in dictionary.items()}
```

### Comparing `yaecs-3.2.5/yaecs/config/config_convenience.py` & `yaecs-4.0.2/yaecs/config/config_convenience.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,16 @@
 
 import difflib
 import logging
 import os
 import time
 from copy import deepcopy
 from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    ItemsView,
-    KeysView,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    ValuesView,
-)
+from typing import (TYPE_CHECKING,
+                    Any, Callable, Dict, ItemsView, KeysView, List, Optional, Tuple, Type, Union, ValuesView)
 
 import yaml
 
 from ..yaecs_utils import compare_string_pattern, dict_apply, format_str
 
 if TYPE_CHECKING:
     from .config import Configuration
@@ -297,14 +285,30 @@
 
         :param deep: how to return sub-configs that would appear among the values. If False, do not convert them, else
             recursively convert them to dict
         :return: the values of the config as in dict.values()
         """
         return self.get_dict(deep).values()
 
+    @staticmethod
+    def _are_same_sub_configs(first: Any, second: Any) -> bool:
+        """
+        Checks if two sub-configs have identical nesting hierarchies.
+
+        :param first: first sub-config to check
+        :param second: second sub-config to check
+        :return: result of the check
+        """
+        if not isinstance(first, ConfigConvenienceMixin) or not isinstance(second, ConfigConvenienceMixin):
+            return False
+        if first.get_name() != second.get_name():
+            return False
+        nh1, nh2 = first.get_nesting_hierarchy(), second.get_nesting_hierarchy()
+        return len(nh1) == len(nh2) and all(nh1[i] == nh2[i] for i in range(len(nh1)))
+
     def _did_you_mean(self, name: str, filter_type: Optional[type] = None, suffix: str = "") -> str:
         """ Used to propose suggestions when the user tries to access a parameter which does not exist. """
         all_params = self.get_parameter_names(True)
         close_params = []
         for parameter in all_params:
             if filter_type is None or isinstance(self[parameter], filter_type):
                 if compare_string_pattern(parameter, f"*{name}*"):
@@ -330,15 +334,15 @@
 
     def _get_yaml_dumper(self) -> Type[yaml.Dumper]:
         """ Used to get a custom YAML dumper capable of writing config tags. """
 
         def config_representer(yaml_dumper, class_instance):
             # pylint: disable=bad-continuation
             return yaml_dumper.represent_mapping(
-                "!" + class_instance.get_name().split("_VARIATION_")[0], {
+                "tag:yaml.org,2002:map", {
                     a[3:] if a.startswith("___") else a: self._format_metadata() if a == "config_metadata" else
                     (b if (".".join(class_instance.get_nesting_hierarchy()
                                     + [a]) not in self.get_main_config().get_pre_post_processing_values()) else
                         (self.get_main_config().get_pre_post_processing_values(
                         )[".".join(class_instance.get_nesting_hierarchy() + [a])]))
                     for (a, b) in class_instance.__dict__.items()
                     if a not in self._protected_attributes
```

### Comparing `yaecs-3.2.5/yaecs/config/config_getters.py` & `yaecs-4.0.2/yaecs/config/config_getters.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,17 @@
 
     def get_all_sub_configs(self) -> List['Configuration']:
         """
         Returns the list of all sub-configs, including sub-configs of other sub-configs
 
         :return: list corresponding to the sub-configs
         """
-        all_configs = list(self._sub_configs_list)
-        for i in self._sub_configs_list:
-            all_configs = all_configs + i.get_all_sub_configs()
-        return all_configs
+        if self._are_same_sub_configs(self, self._main_config):
+            return list(self._sub_configs_list)
+        return self._main_config.get_all_sub_configs()
 
     def get_command_line_argument(self, deep: bool = True, do_return_string: bool = False,
                                   ignore_unknown_types: bool = False,
                                   ) -> Union[List[str], str]:
         """
         Returns a list of command line parameters that can be used in a bash shell to re-create this exact config
         from the default. Can alternatively return the string itself with do_return_string=True.
```

### Comparing `yaecs-3.2.5/yaecs/config/config_hooks.py` & `yaecs-4.0.2/yaecs/config/config_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,16 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
 import os
 from typing import Any, Callable, List, Optional, Tuple, Union
 
-from ..yaecs_utils import (
-    ConfigDeclarator,
-    Hooks,
-    Priority,
-    VariationDeclarator,
-    assign_order,
-    assign_yaml_tag,
-    hook,
-)
+from ..yaecs_utils import (ConfigDeclarator, Hooks, Priority, VariationDeclarator,
+                           assign_order, assign_yaml_tag, hook)
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigHooksMixin:
     """ Hooks Mixin class for YAECS configurations. Implements processing functions whose name start with `register_as_`
     and are decorated by the yaecs_utils.hook decorator. Users can use those processing either as pre- or
```

### Comparing `yaecs-3.2.5/yaecs/config/config_processing_functions.py` & `yaecs-4.0.2/yaecs/config/config_processing_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """ This file defines a library of convenient processing functions. """
 
 import logging
 import os
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, List, Optional
 
-from ..yaecs_utils import (
-    Priority,
-    assign_order,
-    assign_yaml_tag,
-    compare_string_pattern,
-    set_function_attribute,
-)
+from ..yaecs_utils import (Priority,
+                           assign_order, assign_yaml_tag, compare_string_pattern, set_function_attribute)
 
 if TYPE_CHECKING:
     from numbers import Number
 
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
@@ -95,17 +90,14 @@
         set_function_attribute(copy_fn, "__name__", "_copy")
         set_function_attribute(copy_fn, "order", Priority.OFTEN_LAST)
 
         current_processing = object.__getattribute__(main, "_added_post_processing")()
         if not any((compare_string_pattern(param_name, k) and v.__name__ == "_copy")
                    for k, v in current_processing.items()):
             main.add_processing_function_all(param_name, copy_fn, "post")
-        elif self.get_variation_name() is None:
-            YAECS_LOGGER.warning(f"WARNING : Parameter '{param_name}' was already declared as a copy of param "
-                                 f"'{path_to_copy}'. Processing function will not be added again.")
 
         return self.protected_param(path_to_copy)
 
     def check_number_in_range(self, minimum: 'Number' = -float('inf'), maximum: 'Number' = float('inf')) -> Callable:
         """
         Returns a pre-processing function that checks if a numerical param value is in a range. Returned function has
         order OFTEN_FIRST (-10).
```

### Comparing `yaecs-3.2.5/yaecs/config/config_setters.py` & `yaecs-4.0.2/yaecs/config/config_setters.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,29 +12,30 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Dict, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Union
 
 from ..yaecs_utils import TypeHint
 
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigSettersMixin:
     """ Setters Mixin class for YAECS configurations. """
 
     _main_config: 'Configuration'
     _pre_postprocessing_values: Dict[str, Any]
+    _sub_configs_list: List['Configuration']
     _type_hints: Dict[str, TypeHint]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def add_processing_function(self, param_name: str, function_to_add: Union[str, Callable], processing_type: str
                                 ) -> None:
@@ -65,39 +66,54 @@
             check_function = function_to_add
         if hasattr(check_function, "assigned_yaml_tag"):
             if check_function.assigned_yaml_tag[1] != processing_type:
                 name = "unknown_function" if not hasattr(check_function, "__name__") else check_function.__name__
                 YAECS_LOGGER.warning(f"WARNING : processing function {name} is recommended to use "
                                      f"as {check_function.assigned_yaml_tag[1]}-processing function, "
                                      f"but was declared as {processing_type}-processing function.")
-        # Add to main config
-        self._main_config.add_processing_function(param_name, function_to_add, processing_type)
-        # Add to current sub-configs
-        for subconfig in self._main_config.get_all_sub_configs():
-            subconfig.add_processing_function(param_name, function_to_add, processing_type)
-        # Add to future sub-configs
-        attribute = f"_{processing_type}_processing_functions"
-        current_processing = getattr(self, attribute)
-        attribute = f"_added_{processing_type}_processing"
-        current_added_processing = getattr(self, attribute)()
+        current_added_processing_name = f"_added_{processing_type}_processing"
+        current_added_processing = getattr(self, current_added_processing_name)()
+        current_processing_name = f"_{processing_type}_processing_functions"
+        current_processing = getattr(self, current_processing_name)
         set_name = param_name
         while set_name in current_processing or set_name in current_added_processing:
             set_name = set_name + " "
-        new_processing = {set_name: function_to_add, **current_added_processing}
-        setattr(self.__class__, attribute, lambda self: new_processing)
+        if not any(v == function_to_add if isinstance(function_to_add, str) else v.__name__ == function_to_add.__name__
+                   for k, v in current_added_processing.items()
+                   if set_name.strip(" ") == k.strip(" ")):
+            # Add to main config
+            self._main_config.add_processing_function(param_name, function_to_add, processing_type)
+            # Add to current sub-configs
+            for subconfig in self.get_all_sub_configs():
+                subconfig.add_processing_function(param_name, function_to_add, processing_type)
+            # Add to future sub-configs
+            new_processing = {set_name: function_to_add, **current_added_processing}
+            setattr(self.__class__, current_added_processing_name, lambda self: new_processing)
 
     def add_type_hint(self, name: str, type_hint: TypeHint) -> None:
         """
         Adds a type hint for a parameter to the list of type hints for automatic type checks.
 
         :param name: full path of the param in the main config
         :param type_hint: type of the param
         """
         self._type_hints[name] = type_hint
 
+    def set_sub_config(self, sub_config: 'Configuration') -> None:
+        """
+        Registers a new sub-config to the main config.
+
+        :param sub_config: sub-config to register
+        """
+        if self._are_same_sub_configs(self, self._main_config):
+            if all(not self._are_same_sub_configs(i, sub_config) for i in self.get_all_sub_configs()):
+                self._sub_configs_list.append(sub_config)
+        else:
+            self._main_config.set_sub_config(sub_config)
+
     def remove_value_before_postprocessing(self, name: str) -> None:
         """
         Function used for bookkeeping : it remove a parameter from the pre-post-processing archive.
 
         :param name: name of the parameter using the dot convention
         """
         if name in self._pre_postprocessing_values:
@@ -135,7 +151,21 @@
         """
         Sets the state of the master switch for pre-processing across the entire config object. Calling this for a
         sub-config will also affect the main config and all other sub-configs.
 
         :param value: value to set the pre-processing to
         """
         object.__setattr__(self._main_config, "_pre_process_master_switch", value)
+
+    def unset_sub_config(self, sub_config: 'Configuration') -> None:
+        """
+        Registers a new sub-config to the main config.
+
+        :param sub_config: sub-config to register
+        """
+        if self._are_same_sub_configs(self, self._main_config):
+            if not self._are_same_sub_configs(
+                    self._main_config.get(".".join(sub_config.get_nesting_hierarchy()), None), sub_config):
+                self._sub_configs_list = [c for c in self.get_all_sub_configs()
+                                          if not self._are_same_sub_configs(c, sub_config)]
+        else:
+            self._main_config.unset_sub_config(sub_config)
```

### Comparing `yaecs-3.2.5/yaecs/config_history.py` & `yaecs-4.0.2/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.5/yaecs/experiment.py` & `yaecs-4.0.2/yaecs/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
                 run_name = name_from_config.split(os.sep)[-2].split("_")[-1] + "_" + name_from_config.split(os.sep)[-1]
         else:
             run_name = self.run_name
         return exp_name, run_name
 
     def start_run(self, description: Optional[str] = None) -> None:
         """
-        Initializes the configured trackers, which most of the time means preparing their logger is self.loggers.
+        Initialises the configured trackers, which most of the time means preparing their logger is self.loggers.
         """
         experiment_name, run_name = self.extract_names()
         config = self.experiment.config
         params_to_log = {k: config[config.match_params("*" + k)[0]] for k in self.get_filtered_params(config)}
         for tracker_type in self.types:
             if tracker_type != "basic":
                 module = "tensorflow" if tracker_type == "tensorboard" else tracker_type
@@ -388,26 +388,32 @@
             will default to -1 for the basic tracker and will be logged as a "single value" for the clearml tracker
         :param sub_logger: if specified, logs to corresponding sub-logger. Can be interpreted as a sub-folder for the
             scalar name most of the time, but in the case of tensorboard will actually use a different summary writer
         :param description: only used for the tensorboard tracker, corresponds to a short description of the value
         :param main_process_only: do not try to log in pytorch-lightning sub-processes
         """
         if not main_process_only or not os.getenv('NODE_RANK'):  # do not track in a pytorch-lightning spawned process
-            value = float(value)
             if not self.types and self.basic_logger is None:
                 YAECS_LOGGER.warning("WARNING : no tracker configured, scalars will not be logged anywhere.")
                 if os.getenv('NODE_RANK'):
                     YAECS_LOGGER.warning("This is because trackers are deactivated in pytorch-lightning processes.\n"
                                          "To suppress this message, pass 'main_process_only=True'.")
             if self.basic_logger is not None:
                 extended_name = name
                 if sub_logger is not None:
                     extended_name = f"{sub_logger}/{extended_name}"
                 add_to_csv(os.path.join(self.basic_logger, "logged_scalars.csv"),
                            extended_name, value, -1 if step is None else step)
+            try:
+                value = float(value)
+            except ValueError:
+                types = [t for t in self.types if t != "basic"]
+                if types:
+                    YAECS_LOGGER.warning(f"WARNING : will not log non-float value {value} to {types} trackers.")
+                return
             if "sacred" in self.types:
                 extended_name = name
                 if sub_logger is not None:
                     extended_name = f"{sub_logger}/{extended_name}"
                 self.loggers["sacred"].log_scalar(name=extended_name, value=value, step=step)
                 if description is not None:
                     YAECS_LOGGER.warning("WARNING : in log_scalar : 'description' is not used in sacred.")
@@ -469,15 +475,15 @@
 
 
 class BasicTrackerContext:
     """ Class used to set up the context for YAECS' basic tracker """
 
     def __init__(self, logger_path: str, runs: Optional[int], current: Optional[int]):
         """
-        Initializes a context used to declare the loggers required by the basic tracker.
+        Initialises a context used to declare the loggers required by the basic tracker.
 
         :param logger_path: path used by the basic tracker to log
         :param runs: number of runs in the experiment
         :param current: index of current run from 0 to runs-1
         """
         self.runs, self.current = runs, current
         self.logging_handlers = [logging.FileHandler(os.path.join(logger_path, "stdout.log")),
@@ -557,15 +563,15 @@
 
 
 class CMLContext:
     """ Class used to set up the context for ClearML's tracker """
 
     def __init__(self, tracker: Tracker):
         """
-        Initializes a context used to close the ClearML runs when they are done.
+        Initialises a context used to close the ClearML runs when they are done.
 
         :param tracker: tracker object where to find the ClearML runs
         """
         self.tracker = tracker
 
     def __enter__(self):
         pass
```

### Comparing `yaecs-3.2.5/yaecs/pytorch_lightning_utils.py` & `yaecs-4.0.2/yaecs/pytorch_lightning_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,69 +65,69 @@
 class TrackerFriendlyBar(ProgressBar):
     """
     Progress bar class to use instead of TQDMProgressBar (formerly ProgressBar) in pytorch-lightning when yaecs is used
     as a tracker.
     Usage : https://pytorch-lightning.readthedocs.io/en/stable/common/progress_bar.html
     """
     def init_sanity_tqdm(self) -> Tqdm:
-        """Override this to customize the tqdm bar for the validation sanity run."""
+        """Override this to customise the tqdm bar for the validation sanity run."""
         tqdm_bar = Tqdm(
             desc=self.sanity_check_description if _NEW else "Validation sanity check",
             position=(2 * self.process_position),
             disable=self.is_disabled,
             leave=False,
             dynamic_ncols=True,
             file=tqdm_file(),
         )
         return tqdm_bar
 
     def init_train_tqdm(self) -> Tqdm:
-        """Override this to customize the tqdm bar for training."""
+        """Override this to customise the tqdm bar for training."""
         tqdm_bar = Tqdm(
             desc=self.train_description if _NEW else "Training",
             initial=self.train_batch_idx,
             position=(2 * self.process_position),
             disable=self.is_disabled,
             leave=True,
             dynamic_ncols=True,
             file=tqdm_file(),
             smoothing=0,
         )
         return tqdm_bar
 
     def init_predict_tqdm(self) -> Tqdm:
-        """Override this to customize the tqdm bar for predicting."""
+        """Override this to customise the tqdm bar for predicting."""
         tqdm_bar = Tqdm(
             desc=self.predict_description if _NEW else "Predicting",
             initial=self.train_batch_idx,
             position=(2 * self.process_position),
             disable=self.is_disabled,
             leave=True,
             dynamic_ncols=True,
             file=tqdm_file(),
             smoothing=0,
         )
         return tqdm_bar
 
     def init_validation_tqdm(self) -> Tqdm:
-        """Override this to customize the tqdm bar for validation."""
+        """Override this to customise the tqdm bar for validation."""
         # The main progress bar doesn't exist in `trainer.validate()`
         has_main_bar = self.trainer.state.fn != "validate" if _NEW else self.main_progress_bar is not None
         tqdm_bar = Tqdm(
             desc=self.validation_description if _NEW else "Validating",
             position=(2 * self.process_position + has_main_bar),
             disable=self.is_disabled,
             leave=(not has_main_bar) and _NEW,
             dynamic_ncols=True,
             file=tqdm_file(),
         )
         return tqdm_bar
 
     def init_test_tqdm(self) -> Tqdm:
-        """Override this to customize the tqdm bar for testing."""
+        """Override this to customise the tqdm bar for testing."""
         tqdm_bar = Tqdm(
             desc="Testing",
             position=(2 * self.process_position),
             disable=self.is_disabled,
             leave=True,
             dynamic_ncols=True,
             file=tqdm_file(),
```

### Comparing `yaecs-3.2.5/yaecs/user_utils.py` & `yaecs-4.0.2/yaecs/user_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import logging
+import sys
 from typing import Callable, Dict, List, Optional, Type, Union
 
 from .config.config import Configuration
-from .yaecs_utils import ConfigDeclarator, TqdmLogger
+from .yaecs_utils import ConfigInput, ConfigDeclarator, TqdmLogger, get_config_from_argv
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 def tqdm_file():
     """
     Utility function which returns a file to which users can log their TQDM bars to make them YAECS-friendly.
@@ -113,14 +114,15 @@
                 config_class: Optional[Type[Configuration]] = None,
                 pre_processing_dict: Optional[Dict[str, Callable]] = None,
                 post_processing_dict: Optional[Dict[str, Callable]] = None,
                 experiment_path: str = None, tracker_config: str = None,
                 additional_configs_suffix: Optional[str] = None, additional_configs_prefix: Optional[str] = None,
                 variations_suffix: Optional[str] = None, variations_prefix: Optional[str] = None,
                 grids_suffix: Optional[str] = None, grids_prefix: Optional[str] = None,
+                fallback: Optional[ConfigInput] = "{}", pattern: str = "--config",
                 **class_building_kwargs) -> Configuration:
     """
     One-liner wrapper to create a config from dicts/strings without the need for declaring a subclass. Useful for
     scripts or jupyter notebooks. Impractical/hacky for larger projects.
 
     :param configs: dicts and strings defining a config
     :param config_class: class to use to build the configuration. If not provided, use a template instead.
@@ -149,24 +151,37 @@
         Only used if config_class is not provided.
     :param grids_suffix: automatically adds relevant pre-processing rules to consider parameter names ending with
         'grids_suffix' as grids.
         Only used if config_class is not provided.
     :param grids_prefix: automatically adds relevant pre-processing rules to consider parameter names starting with
         'grids_prefix' as grids.
         Only used if config_class is not provided.
+    :param fallback: if provided, use this as a fallback when no config is provided in argv. The default value "{}"
+        stands for "by default do not merge anything if no merge pattern is found in argv"
+    :param pattern: pattern to use to find the config in argv.
     :param class_building_kwargs: same kwargs as those used in all Configuration constructors.
         Only used if config_class is not provided.
     :return: config object
     """
+
+    # Prepare class
     class_args = {
         "pre_processing_dict": pre_processing_dict, "post_processing_dict": post_processing_dict,
         "experiment_path": experiment_path, "tracker_config": tracker_config,
         "additional_configs_suffix": additional_configs_suffix, "additional_configs_prefix": additional_configs_prefix,
         "variations_suffix": variations_suffix, "variations_prefix": variations_prefix,
         "grids_suffix": grids_suffix, "grids_prefix": grids_prefix,
     }
     if config_class is None:
         config_class = get_template_class(**class_args)
     elif any(arg is not None for arg in class_args.values()):
         YAECS_LOGGER.warning("WARNING : The following arguments are not used if config_class is provided :\n"
                              f"{list(class_args.keys())}.")
-    return config_class.build_from_configs(*configs, **class_building_kwargs)
+
+    # Get configs from argv
+    configs_from_argv = get_config_from_argv(pattern=pattern, fallback={} if fallback == "{}" else fallback)
+    class_building_kwargs["from_argv"] = pattern if pattern in sys.argv else ""
+    if all(c == {} for c in configs_from_argv):
+        configs_from_argv = []
+        class_building_kwargs["from_argv"] = ""
+
+    return config_class.build_from_configs(*configs, *configs_from_argv, **class_building_kwargs)
```

### Comparing `yaecs-3.2.5/yaecs/yaecs_utils.py` & `yaecs-4.0.2/yaecs/yaecs_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 import re
 import sys
 from bisect import bisect
 from collections.abc import Mapping
 from enum import Enum
 from numbers import Real
 from types import ModuleType
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 YAECS_LOGGER = logging.getLogger(__name__)
 ConfigDeclarator = Union[str, dict]
+ConfigInput = Union[List[ConfigDeclarator], ConfigDeclarator]
 Hooks = Union[Dict[str, List[str]], List[str]]
 TypeHint = Union[type, tuple, list, dict, set, int]
 VariationDeclarator = Union[List[ConfigDeclarator], Dict[str, ConfigDeclarator]]
 
 
 def adapt_to_type(previous_value: Any, value_to_adapt: str, force: str, param: str) -> Any:
     """
@@ -239,28 +240,14 @@
     with open(csv_path, 'w', encoding='utf-8') as csv_file:
         csv_file.write(",".join(["steps"] + metrics) + "\n")
         for index, step_to_log in enumerate(steps):
             data = [str(step_to_log)] + [v[index] for v in values]
             csv_file.write(",".join(data) + "\n")
 
 
-def are_same_sub_configs(first, second) -> bool:
-    """
-    Checks if two sub-configs have identical nesting hierarchies.
-
-    :param first: first sub-config to check
-    :param second: second sub-config to check
-    :return: result of the check
-    """
-    if first.get_name() != second.get_name():
-        return False
-    nh1, nh2 = first.get_nesting_hierarchy(), second.get_nesting_hierarchy()
-    return len(nh1) == len(nh2) and all(nh1[i] == nh2[i] for i in range(len(nh1)))
-
-
 def assign_order(order: Union[Real, 'Priority'] = 0) -> Callable[[Callable], Callable]:
     """
     Decorator used to give an order to a processing function. If several processing functions would be called at a given
     step, they are called in increasing order.
 
     :param order: order to give the function
     :return: decorated function
@@ -378,14 +365,31 @@
     """
     to_return = str(config_path_or_dictionary)
     if YAECS_LOGGER.level >= logging.INFO:
         return to_return if len(to_return) < size else f"{to_return[:size//2 - 3]} [...] {to_return[-size//2 - 3:]}"
     return to_return
 
 
+def get_config_from_argv(pattern: str, fallback: Optional[ConfigInput] = None) -> List[str]:
+    """
+    Get a configuration from the command line arguments.
+
+    :param pattern: pattern to detect in sys.argv
+    :param fallback: fallback value if pattern is not detected in sys.argv
+    :return: the configuration
+    """
+    if pattern not in sys.argv and fallback is None:
+        raise TypeError(f"The pattern '{pattern}' was not detected in sys.argv.")
+    if pattern in sys.argv:
+        fallback = [cfg.strip(" ") for cfg in sys.argv[sys.argv.index(pattern) + 1].strip("[]").split(",")]
+    if not isinstance(fallback, list):
+        fallback = [fallback]
+    return fallback
+
+
 def get_order(func: Callable) -> Union[Real, 'Priority']:
     """
     If input function has an "order" attribute, returns it. Otherwise, returns Priority.INDIFFERENT.
 
     :param func: function to get the order of
     :return: the order value
     """
```

### Comparing `yaecs-3.2.5/yaecs.egg-info/PKG-INFO` & `yaecs-4.0.2/yaecs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.5
+Version: 4.0.2
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.LESSER.md
 License-File: COPYING.md
 
 # YAECS (Yet Another Experiment Config System)
 
 [![Offial repo](https://img.shields.io/badge/official%20repo-YAECS-%23ff9626?logo=gitlab)](https://gitlab.com/reactivereality/public/yaecs)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
 [![License](https://img.shields.io/badge/license-LGPLV3%2B-%23c4c2c2)](https://www.gnu.org/licenses/)
 
+![GitHub last commit (branch)](https://img.shields.io/github/last-commit/valentingol/yaecs/main)
+[![PyPI version](https://badge.fury.io/py/yaecs.svg)](https://badge.fury.io/py/yaecs)
+
+[![Documentation Status](https://readthedocs.org/projects/yaecs/badge/?version=latest)](https://yaecs.readthedocs.io/en/latest/?badge=latest)
+
 ---
 
+## Documentation: [here](https://yaecs.readthedocs.io/en/stable/)
+
 **DISCLAIMER: This repository is the public version of a repository that is the
 property of [Reactive Reality](https://www.reactivereality.com/). This
 repository IS NOT OFFICIAL and might not be maintained in the future. Some
 minor changes * are applied from the
 [official repository (GitLab)](https://gitlab.com/reactivereality/public/yaecs)
 (under lesser GNU license).**
 
 This package is a Config System which allows easy manipulation of config files
 for safe, clear and repeatable experiments. In a few words, it is:
 
 - built for Machine Learning with its constraints in mind, but also usable
 out-of-the-box for other kinds of projects;
 - built with scalability in mind and can adapt just as easily to large projects
-investigating hundreds of well-organized parameters across many experiments;
+investigating hundreds of well-organised parameters across many experiments;
 - designed to encourage good coding practices for research purposes, and if
 used rigorously will ensure a number of highly desirable properties such that
 **maintenance-less forward-compatibility** of old configs, **easy
 reproducibility** of any experiment, and **extreme clarity** of former
 experiments for your future self or collaborators.
 
 [LINK TO DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home)
 
 ## Installation
 
-The package can be installed from pipy: `pip install yaecs`
+The package can be installed from pipy:
+
+```bash
+pip install yaecs
+```
 
 ## Getting started
 
 This package is adapted to a *project* where you need to run a number of
 experiments. In this setup, it can be useful to gather all the parameters in
 the project to a common location, some "config files", so you can access and
 modify them easily. This package is based on YAML, therefore your config files
@@ -78,15 +88,15 @@
         return {}
 ```
 
 That's all there is to it! Now if we use
 `config = ProjectSpecific.load_config()`, we can then call `config.data_path`
 or `config.learning_rate` to get their values as defined in the default config.
 We don't need to specify where to get the default config because a project
-should only ever have one default config, which centralizes all the parameters
+should only ever have one default config, which centralises all the parameters
 in that project. Since the location of the default config is a project
 constant, it is defined in your project-specific subclass and there is no need
 to clutter your main code with it. Now, for example, your main.py could look
 like:
 
 ```python
 from project_config import ProjectSpecific
@@ -111,28 +121,28 @@
  - data_path : ./data
  - learning_rate : 0.001
 ```
 
 The Configuration hierarchy tells you about the creation history of the config,
 in this case only the default config was used. Then, all parameters are
 displayed. There are of course many other features in this package which you
-can use to organize your parameters, hierarchise your experiments etc. The
+can use to organise your parameters, hierarchise your experiments etc. The
 idea being that once the bare minimum presented above is set up, scaling up
 is just as simple.
 
 You can learn more about all these features in our
 [DOCUMENTATION](https://gitlab.com/reactivereality/public/yaecs/-/wikis/home).
 
 ## config_history
 
 The Config History is a side-feature of the main Config System. It can be
 configured for any project which uses the Config System and provides a
 flexible framework to easily build graphs representing past experiments. In
 these graphs, each node represents an experiment, and vertices are drawn
-between your experiments to visualize easily which parameters changed from one
+between your experiments to visualise easily which parameters changed from one
 node to another.
 
 The graph can be coloured to show your most successful experiments, or grouped
 by parameters to see how well they have been explored in your experiment
 history. This makes it very useful to review your past work, share it with
 colleagues or make unexpected correlations appear.
```

### Comparing `yaecs-3.2.5/yaecs.egg-info/SOURCES.txt` & `yaecs-4.0.2/yaecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

