# Comparing `tmp/trubrics-1.4.0.tar.gz` & `tmp/trubrics-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.4.0.tar", last modified: Wed Jun 21 11:21:46 2023, max compression
+gzip compressed data, was "trubrics-1.4.1.tar", last modified: Fri Jun 30 18:35:41 2023, max compression
```

## Comparing `trubrics-1.4.0.tar` & `trubrics-1.4.1.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-21 11:21:32.000000 trubrics-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 11:21:46.137231 trubrics-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-21 11:21:32.000000 trubrics-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 11:21:32.000000 trubrics-1.4.0/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 11:21:32.000000 trubrics-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 11:21:32.000000 trubrics-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 11:21:46.137231 trubrics-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-21 11:21:32.000000 trubrics-1.4.0/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/feedback/save_to_trubrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.133231 trubrics-1.4.0/trubrics/trubrics_platform/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/trubrics_platform/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.137231 trubrics-1.4.0/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 11:21:32.000000 trubrics-1.4.0/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:21:46.129231 trubrics-1.4.0/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 11:21:46.000000 trubrics-1.4.0/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-06-30 18:35:32.000000 trubrics-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 18:35:41.949996 trubrics-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-30 18:35:32.000000 trubrics-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/examples/feedback/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/llm_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/titanic_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-30 18:35:32.000000 trubrics-1.4.1/examples/feedback/streamlit/trubrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 18:35:32.000000 trubrics-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 18:35:32.000000 trubrics-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 18:35:41.949996 trubrics-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-30 18:35:32.000000 trubrics-1.4.1/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/feedback/save_to_trubrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/trubrics_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/trubrics_platform/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.945996 trubrics-1.4.1/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-30 18:35:32.000000 trubrics-1.4.1/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:35:41.941996 trubrics-1.4.1/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 18:35:41.000000 trubrics-1.4.1/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.4.0/LICENSE` & `trubrics-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/setup.cfg` & `trubrics-1.4.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = trubrics
-version = 1.4.0
-description = Combine data science knowledge with business user feedback to validate machine learning.
+version = 1.4.1
+description = The first user insights platform for AI models.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
 [options.entry_points]
```

### Comparing `trubrics-1.4.0/tests/test_context.py` & `trubrics-1.4.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/cli/run.py` & `trubrics-1.4.1/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/context.py` & `trubrics-1.4.1/trubrics/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 from loguru import logger
-from pydantic import BaseModel, class_validators, root_validator, validator
+from pydantic import BaseModel, root_validator, validator
 
 from trubrics.exceptions import (
     EstimatorTypeError,
     ModelPredictionError,
     PandasSchemaError,
 )
 from trubrics.utils.pandas import schema_is_equal
 
-# to solve streamlit bug: https://github.com/streamlit/streamlit/issues/3218
-class_validators._FUNCS.clear()
-
 
 class DataContext(BaseModel):
     """
     The DataContext wraps ML datasets into a trubrics friendly format.
 
     Note:
         The DataContext *must contain* at least a testing_data and a target attribute.
```

### Comparing `trubrics-1.4.0/trubrics/example/my_first_trubric.json` & `trubrics-1.4.1/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/example/titanic.py` & `trubrics-1.4.1/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/example/titanic_data.csv` & `trubrics-1.4.1/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/example/trubric_run.py` & `trubrics-1.4.1/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/exceptions.py` & `trubrics-1.4.1/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/feedback/config.py` & `trubrics-1.4.1/trubrics/feedback/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 TITLE = "Title"
 TITLE_EXPLAIN = "Give the issue an explicit title."
 DESCRIPTION = "Description"
 DESCRIPTION_EXPLAIN = "Detail the issue you have observed."
 FEEDBACK_SAVE_BUTTON = "Save feedback"
 LOCAL_SAVE = "Feedback saved."
 LOCAL_SAVE_HTML = f'<p style="color:Green;">{LOCAL_SAVE}</p>'
-PLATFORM_SAVE = "Feedback saved to the Trubrics platform."
+PLATFORM_SAVE = "Feedback saved to Trubrics."
 PLATFORM_SAVE_HTML = f'<p style="color:Green;">{PLATFORM_SAVE}</p>'
 FEEDBACK_NOT_SAVED = "Please specify both a feedback title and a description."
 FEEDBACK_NOT_SAVED_HTML = '<p style="color:Red;">Please specify a feedback title and a description.</p>'
 USER_EMAIL = "User email"
 USER_PASSWORD = "User password"
```

### Comparing `trubrics-1.4.0/trubrics/feedback/dataclass.py` & `trubrics-1.4.1/trubrics/feedback/dataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     The Feedback object represents all data contained as a feedback response from a user.
 
     Example:
         ```py
         import trubrics
 
-        feedback = trubrics.Feedback(
+        feedback = trubrics.collect(
             component_name="default",
             model="default_model",
             response={
                 "type": "thumbs",
                 "score": "👎",
                 "text": "A comment / textual feedback from the user."
             },
```

### Comparing `trubrics-1.4.0/trubrics/feedback/save_to_trubrics.py` & `trubrics-1.4.1/trubrics/feedback/save_to_trubrics.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/integrations/dash/collect.py` & `trubrics-1.4.1/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/integrations/gradio/collect.py` & `trubrics-1.4.1/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.4.1/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/integrations/streamlit/collect.py` & `trubrics-1.4.1/trubrics/integrations/streamlit/collect.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         component_name: str,
         email: Optional[str],
         password: Optional[str],
         firebase_api_key: Optional[str] = None,
         firebase_project_id: Optional[str] = None,
     ):
         """
-        The FeedbackCollector allows Data Scientists to collect feedback from within their app.
-
         Args:
-            TODO
+            component_name: the component name that has been created in Trubrics
+            email: a Trubrics account email
+            password: a Trubrics account password
         """
         self.component_name = component_name
         if email and password:
             self.trubrics_config = init(
                 email=email,
                 password=password,
                 firebase_api_key=firebase_api_key,
@@ -37,34 +37,36 @@
         self,
         feedback_type: str,
         model: str,
         tags: list = [],
         metadata: dict = {},
         response: Optional[Response] = None,
         user_id: Optional[str] = None,
+        created_on: datetime = datetime.now(),
         key: Optional[str] = None,
         open_feedback_label: Optional[str] = None,
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         """
-        Collect user feedback within a Streamlit web application.
+        Collect ML model user feedback with UI components from a Streamlit app.
 
         Args:
-            TODO
             feedback_type: type of feedback to be collected
 
                 - textbox: open textbox feedback
-                - thumbs: positive or negative feedback with thumbs emojis
-                - faces: a scale of 1 to 5 with face emojis
-                - custom: a customisable feedback type that allows users to specify the user_response dict
-            response: a dict of user responses to save with your feedback for feedback_type='custom'
-            metadata: data to save with your feedback
-            tags: a list of tags for your feedback
-            key: a key for each streamlit component
+                - thumbs: 👍 / 👎 UI buttons
+                - faces: 😞 / 🙁 / 😐 / 🙂 / 😀 UI buttons
+            model: the model used - can be a model version, a link to the saved model artifact in cloud storage, etc
+            tags: a list of tags for the feedback
+            metadata: any data to save with the feedback
+            response: a dict of user responses to save with the feedback for feedback_type='custom'
+            user_id: an optional reference to a user, for example a username if there is a login, a cookie ID, etc
+            key: a key for the streamlit components (necessary if calling this method multiple times with the same type)
             open_feedback_label: label of optional text_input for "faces" or "thumbs" feedback_type
+            save_to_trubrics: whether to save the feedback to Trubrics, or just to return the feedback object
         """
         if key is None:
             key = feedback_type
         if feedback_type == "textbox":
             if response:
                 raise ValueError("For feedback_type='textbox', user_response must be None.")
             text = self.st_textbox_ui(key, label=open_feedback_label)
@@ -72,63 +74,63 @@
                 response = Response(type=feedback_type, score=None, text=text)
                 return self._save_feedback(
                     model=model,
                     response=response,
                     user_id=user_id,
                     tags=tags,
                     metadata=metadata,
+                    created_on=created_on,
                     save_to_trubrics=save_to_trubrics,
                 )
         elif feedback_type in ("thumbs", "faces"):
             if response:
                 raise ValueError(
                     f"For feedback_type='{feedback_type}', response is set inside the component (must be None)."
                 )
             return self._save_quantitative_feedback(
                 model=model,
                 feedback_type=feedback_type,
                 user_id=user_id,
                 metadata=metadata,
                 tags=tags,
+                created_on=created_on,
                 key=key,
                 open_feedback_label=open_feedback_label,
                 save_to_trubrics=save_to_trubrics,
             )
-        # elif feedback_type == "custom":
-        #     if user_response:
-        #         return self._save_feedback(
-        #             feedback_type=feedback_type,
-        #             user_response=user_response,
-        #             path=path,
-        #             metadata=metadata,
-        #             tags=tags,
-        #         )
-        #     else:
-        #         raise ValueError("For feedback_type='custom', title and description parameters must be specified.")
+        elif feedback_type == "custom":
+            raise NotImplementedError(
+                "This is currently not implemented. Get in touch to understand how to save custom feedback."
+            )
+            # if response:
+            #     return self._save_feedback(...)
+            # else:
+            #     raise ValueError("For feedback_type='custom', title and description parameters must be specified.")
         else:
             raise ValueError("feedback_type must be one of ['textbox', 'faces', 'thumbs', 'custom'].")
         return None
 
     def _save_feedback(
         self,
         model: str,
         response: Response,
         user_id: Optional[str] = None,
         tags: list = [],
         metadata: dict = {},
+        created_on: datetime = datetime.now(),
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         feedback = Feedback(
             component_name=self.component_name,
             response=response,
             model=model,
             metadata=metadata,
             tags=tags,
             user_id=user_id,
-            created_on=datetime.now(),
+            created_on=created_on,
         )
         if save_to_trubrics:
             res = save(trubrics_config=self.trubrics_config, feedback=feedback)
             if "error" in res:
                 error_msg = f"Error in pushing feedback issue to Trubrics: {res}"
                 st.error(error_msg)
             else:
@@ -140,14 +142,15 @@
         feedback_type: str,
         key: str,
         open_feedback_label: Optional[str],
         model: str,
         user_id: Optional[str] = None,
         tags: list = [],
         metadata: dict = {},
+        created_on: datetime = datetime.now(),
         save_to_trubrics: bool = True,
     ) -> Optional[dict]:
         if f"{key}_state" not in st.session_state:
             st.session_state[f"{key}_state"] = ""
         if f"{key}_save_button" not in st.session_state:
             st.session_state[f"{key}_save_button"] = False
         if f"previous_{key}_state" not in st.session_state:
@@ -187,29 +190,38 @@
                 )
                 return self._save_feedback(
                     model=model,
                     response=response,
                     user_id=user_id,
                     tags=tags,
                     metadata=metadata,
+                    created_on=created_on,
                     save_to_trubrics=save_to_trubrics,
                 )
         if st.session_state[f"{key}_save_button"]:
             return self._save_feedback(
                 model=model,
                 response=st.session_state[f"previous_{key}_state"],
                 user_id=user_id,
                 tags=tags,
                 metadata=metadata,
+                created_on=created_on,
                 save_to_trubrics=save_to_trubrics,
             )
         return None
 
     @staticmethod
     def st_textbox_ui(key: Optional[str] = None, label: Optional[str] = None) -> Optional[str]:
+        """
+        Trubrics 'textbox' UI component.
+
+        Args:
+            key: a key for the streamlit components (necessary if calling this method multiple times with the same type)
+            label: the textbox's streamlit label
+        """
         if key is None:
             key = "textbox"
 
         if f"{key}_save_button" not in st.session_state:
             st.session_state[f"{key}_save_button"] = False
 
         if f"previous_{key}_state" not in st.session_state:
@@ -227,14 +239,21 @@
             st.button(config.FEEDBACK_SAVE_BUTTON, on_click=clear_session_state, key=f"{key}_save_button")
         if st.session_state[f"{key}_save_button"]:
             return st.session_state[f"previous_{key}_state"]
         else:
             return None
 
     def st_thumbs_ui(self, disable_on_click: bool = False, key: Optional[str] = None) -> Optional[str]:
+        """
+        Trubrics 'thumbs' UI component - two thumbs buttons.
+
+        Args:
+            disable_on_click: disable all other buttons when a button is clicked
+            key: a key for the streamlit components (necessary if calling this method multiple times with the same type)
+        """
         if key is None:
             key = "thumbs"
 
         button_states = [f"{key}_1", f"{key}_2"]
         col1, col2 = st.columns([1, 15])
         with col1:
             up = self._emoji_button("👍", key, disable_on_click, button_states, 1)
@@ -245,14 +264,21 @@
             return self._return_quantitative_ui_button(key, disable_on_click, button_states, 1, "👍")
         elif down:
             return self._return_quantitative_ui_button(key, disable_on_click, button_states, 2, "👎")
         else:
             return None
 
     def st_faces_ui(self, disable_on_click: bool = False, key: Optional[str] = None) -> Optional[str]:
+        """
+        Trubrics 'faces' UI component - two thumbs buttons.
+
+        Args:
+            disable_on_click: disable all other buttons when a button is clicked
+            key: a key for the streamlit components (necessary if calling this method multiple times with the same type)
+        """
         if key is None:
             key = "faces"
 
         button_states = [f"{key}_1", f"{key}_2", f"{key}_3", f"{key}_4", f"{key}_5"]
         col1, col2, col3, col4, col5 = st.columns([1, 1, 1, 1, 10])
         with col1:
             one = self._emoji_button("😞", key, disable_on_click, button_states, 1)
```

### Comparing `trubrics-1.4.0/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.4.1/trubrics/integrations/streamlit/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 
 def generate_what_if_streamlit(data_context: DataContext):
     """
     Generate a what-if tool based on the testing_data of the DataContext.
     """
     out_df = pd.DataFrame()
     wi_data = data_context.testing_data
-    for col in wi_data.columns:
-        series = wi_data[col]
-        if data_context.business_columns is not None and col in data_context.business_columns.keys():
-            renamed_col = data_context.business_columns[col]
-        else:
-            renamed_col = col
-        if data_context.categorical_columns is None:
-            raise ValueError(
-                "A list of categorical_columns must be specified in the DataContext for the what-if functionality."
-            )
-        if col in data_context.categorical_columns:
-            out_df[col] = [st.selectbox(label=renamed_col, options=tuple(series.dropna().unique()))]
-        else:
-            out_df[col] = [
-                st.slider(
-                    renamed_col,
-                    min_value=int(series.min()),
-                    max_value=int(series.max()),
-                    value=round(series.mean()),
+    if data_context.features:
+        for col in data_context.features:
+            series = wi_data[col]
+            if data_context.business_columns is not None and col in data_context.business_columns.keys():
+                renamed_col = data_context.business_columns[col]
+            else:
+                renamed_col = col
+            if data_context.categorical_columns is None:
+                raise ValueError(
+                    "A list of categorical_columns must be specified in the DataContext for the what-if functionality."
                 )
-            ]
+            if col in data_context.categorical_columns:
+                out_df[col] = [st.selectbox(label=renamed_col, options=tuple(series.dropna().unique()))]
+            else:
+                out_df[col] = [
+                    st.slider(
+                        renamed_col,
+                        min_value=int(series.min()),
+                        max_value=int(series.max()),
+                        value=round(series.mean()),
+                    )
+                ]
     return out_df
 
 
 def explore_testing_data(data_context, model):
     test_set = "Full test set"
     test_set_errors = "Test set errors"
     filtered_target = "Filtered prediction value"
```

### Comparing `trubrics-1.4.0/trubrics/trubrics_platform/auth.py` & `trubrics-1.4.1/trubrics/trubrics_platform/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/trubrics_platform/firestore.py` & `trubrics-1.4.1/trubrics/trubrics_platform/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/trubrics_platform/trubrics_config.py` & `trubrics-1.4.1/trubrics/trubrics_platform/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/validations/dataclass.py` & `trubrics-1.4.1/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/validations/model/base.py` & `trubrics-1.4.1/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/validations/run.py` & `trubrics-1.4.1/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics/validations/validation_output.py` & `trubrics-1.4.1/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.4.0/trubrics.egg-info/SOURCES.txt` & `trubrics-1.4.1/trubrics.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 examples/__init__.py
-examples/classification_titanic/__init__.py
-examples/classification_titanic/custom_scorer.py
-examples/classification_titanic/custom_validator.py
-examples/classification_titanic/slicing_functions.py
+examples/feedback/__init__.py
+examples/feedback/streamlit/__init__.py
+examples/feedback/streamlit/llm_app.py
+examples/feedback/streamlit/titanic_app.py
+examples/feedback/streamlit/trubrics_utils.py
 tests/test_context.py
 trubrics/__init__.py
 trubrics/context.py
 trubrics/exceptions.py
 trubrics/py.typed
 trubrics.egg-info/PKG-INFO
 trubrics.egg-info/SOURCES.txt
@@ -19,17 +20,14 @@
 trubrics.egg-info/entry_points.txt
 trubrics.egg-info/requires.txt
 trubrics.egg-info/top_level.txt
 trubrics/cli/__init__.py
 trubrics/cli/main.py
 trubrics/cli/run.py
 trubrics/example/__init__.py
-trubrics/example/app_titanic_dash.py
-trubrics/example/app_titanic_gradio.py
-trubrics/example/app_titanic_streamlit.py
 trubrics/example/my_first_trubric.json
 trubrics/example/titanic.py
 trubrics/example/titanic_config.py
 trubrics/example/titanic_data.csv
 trubrics/example/trubric_run.py
 trubrics/feedback/__init__.py
 trubrics/feedback/config.py
```

