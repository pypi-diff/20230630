# Comparing `tmp/xoa-core-2.0.0.tar.gz` & `tmp/xoa-core-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-core-2.0.0.tar", last modified: Fri Jun  2 07:25:54 2023, max compression
+gzip compressed data, was "xoa-core-2.0.1.tar", last modified: Fri Jun 30 11:47:39 2023, max compression
```

## Comparing `xoa-core-2.0.0.tar` & `xoa-core-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-02 07:25:44.000000 xoa-core-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-02 07:25:54.068522 xoa-core-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-02 07:25:44.000000 xoa-core-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 07:25:44.000000 xoa-core-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:25:54.068522 xoa-core-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 07:25:44.000000 xoa-core-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/executor_state_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/executors/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/generic_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/messenger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/messenger/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/plugin_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core/core/resources/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/resources/resource/models/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/__decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/resource/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/test_suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/test_suites/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.068522 xoa-core-2.0.0/xoa_core/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/core/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 07:25:44.000000 xoa-core-2.0.0/xoa_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:25:54.064522 xoa-core-2.0.0/xoa_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 07:25:54.000000 xoa-core-2.0.0/xoa_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-30 11:47:29.000000 xoa-core-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-30 11:47:39.321982 xoa-core-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-30 11:47:29.000000 xoa-core-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 11:47:29.000000 xoa-core-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 11:47:39.321982 xoa-core-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-30 11:47:29.000000 xoa-core-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_state_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/generic_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/plugin_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/resources/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/resources/resource/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/__decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/test_suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/top_level.txt
```

### Comparing `xoa-core-2.0.0/LICENSE` & `xoa-core-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/PKG-INFO` & `xoa-core-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
 Author: Artem Constantinov, Leonard Yu
 Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-core-2.0.0/README.md` & `xoa-core-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/setup.py` & `xoa-core-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/controller.py` & `xoa-core-2.0.1/xoa_core/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/exceptions.py` & `xoa-core-2.0.1/xoa_core/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/executors/executor.py` & `xoa-core-2.0.1/xoa_core/core/executors/executor.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/executors/executor_state.py` & `xoa-core-2.0.1/xoa_core/core/executors/executor_state.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/executors/executor_state_conditions.py` & `xoa-core-2.0.1/xoa_core/core/executors/executor_state_conditions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/executors/manager.py` & `xoa-core-2.0.1/xoa_core/core/executors/manager.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/generic_types.py` & `xoa-core-2.0.1/xoa_core/core/generic_types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/messenger/handler.py` & `xoa-core-2.0.1/xoa_core/core/messenger/handler.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/messenger/misc.py` & `xoa-core-2.0.1/xoa_core/core/messenger/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     state: Optional[str]
     old_state: Optional[str]
 
 
 class Progress(BaseModel):
     current: int
     total: int
+    loop: int
 
 
 class TransmitFunc(Protocol):
     def __call__(self, msg: Any, *, msg_type: EMsgType, **meta: Any) -> None:
         ...
 
 
@@ -62,18 +63,19 @@
     def __init__(self, transmit: "TransmitFunc", suite_name: str) -> None:
         self.__transmit = transmit
         self.__suite_name = suite_name
 
     def send_statistics(self, data: dict[str, Any] | "BaseModel") -> None:
         self.__transmit(data, msg_type=EMsgType.STATISTICS, suite_name=self.__suite_name)
 
-    def send_progress(self, current: int, total: int = 100) -> None:
+    def send_progress(self, current: int, total: int = 100, loop: int = 0) -> None:
         progress = Progress(
             current=current,
-            total=total
+            total=total,
+            loop=loop,
         )
         self.__transmit(progress, msg_type=EMsgType.PROGRESS, suite_name=self.__suite_name)
 
     def send_warning(self, warning: Exception) -> None:
         self.__transmit(str(warning), msg_type=EMsgType.WARNING, suite_name=self.__suite_name)
 
     def send_error(self, error: Exception) -> None:
```

### Comparing `xoa-core-2.0.0/xoa_core/core/messenger/pipe.py` & `xoa-core-2.0.1/xoa_core/core/messenger/pipe.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/plugin_abstract.py` & `xoa-core-2.0.1/xoa_core/core/plugin_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class PPipeFacade(typing.Protocol):
     def __init__(self, transmit: "TransmitFunc", suite_name: str) -> None: ...  # noqa: E704
 
     def send_statistics(self, data: typing.Union[typing.Dict, "BaseModel"]) -> None:
         """Method used for push statistics data into the messages pipe for future distribution"""
 
-    def send_progress(self, current: int, total: int) -> None:
+    def send_progress(self, current: int, total: int = 100, loop: int = 0) -> None:
         """Method used for push current progress value into the messages pipe for future distribution"""
 
     def send_warning(self, warning: Exception) -> None:
         """Method used for push warning exceptions into the messages pipe for future distribution"""
 
     def send_error(self, error: Exception) -> None:
         """Method used for push error exceptions into the messages pipe for future distribution"""
```

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/controller.py` & `xoa-core-2.0.1/xoa_core/core/resources/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/pool.py` & `xoa-core-2.0.1/xoa_core/core/resources/pool.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/exceptions.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/facade.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/facade.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/misc.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/models/module.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/models/module.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/models/port.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/models/port.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/models/tester.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/models/tester.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/resource/models/types.py` & `xoa-core-2.0.1/xoa_core/core/resources/resource/models/types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/resources/storage.py` & `xoa-core-2.0.1/xoa_core/core/resources/storage.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/test_suites/_loader.py` & `xoa-core-2.0.1/xoa_core/core/test_suites/_loader.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/test_suites/controller.py` & `xoa-core-2.0.1/xoa_core/core/test_suites/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/test_suites/datasets.py` & `xoa-core-2.0.1/xoa_core/core/test_suites/datasets.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/utils/observer.py` & `xoa-core-2.0.1/xoa_core/core/utils/observer.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/core/utils/validators.py` & `xoa-core-2.0.1/xoa_core/core/utils/validators.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/exceptions.py` & `xoa-core-2.0.1/xoa_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core/types.py` & `xoa-core-2.0.1/xoa_core/types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.0/xoa_core.egg-info/PKG-INFO` & `xoa-core-2.0.1/xoa_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
 Author: Artem Constantinov, Leonard Yu
 Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-core-2.0.0/xoa_core.egg-info/SOURCES.txt` & `xoa-core-2.0.1/xoa_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

