# Comparing `tmp/rai_benchmark_test-1.2.tar.gz` & `tmp/rai_benchmark_test-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-1.2.tar", last modified: Thu Jun 29 22:30:58 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-1.3.tar", last modified: Thu Jun 29 23:33:39 2023, max compression
```

## Comparing `rai_benchmark_test-1.2.tar` & `rai_benchmark_test-1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:30:58.360837 rai_benchmark_test-1.2/
--rw-rw-rw-   0        0        0       63 2023-06-29 22:30:58.360837 rai_benchmark_test-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 22:30:58.203758 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 22:30:57.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 22:30:58.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:30:57.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 22:30:57.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 22:30:57.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 22:30:57.000000 rai_benchmark_test-1.2/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 22:30:58.360837 rai_benchmark_test-1.2/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-29 22:30:30.000000 rai_benchmark_test-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:30:58.360837 rai_benchmark_test-1.2/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.2/src/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-1.2/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.2/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.2/src/assessment_flow.py
--rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.2/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.2/src/data_prep.py
--rw-rw-rw-   0        0        0     3818 2023-06-29 22:22:10.000000 rai_benchmark_test-1.2/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.2/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.2/src/job.py
--rw-rw-rw-   0        0        0     7863 2023-06-29 22:30:24.000000 rai_benchmark_test-1.2/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.2/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.2/src/prompt_data.py
--rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.2/src/request.py
--rw-rw-rw-   0        0        0     1943 2023-06-29 22:21:45.000000 rai_benchmark_test-1.2/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.2/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/
+-rw-rw-rw-   0        0        0       63 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 23:33:38.974418 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      410 2023-06-29 23:33:29.000000 rai_benchmark_test-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.3/src/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-06-29 23:17:04.000000 rai_benchmark_test-1.3/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.3/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.3/src/assessment_flow.py
+-rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.3/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.3/src/data_prep.py
+-rw-rw-rw-   0        0        0     3818 2023-06-29 22:22:10.000000 rai_benchmark_test-1.3/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.3/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.3/src/job.py
+-rw-rw-rw-   0        0        0     7863 2023-06-29 22:30:24.000000 rai_benchmark_test-1.3/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.3/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.3/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.3/src/request.py
+-rw-rw-rw-   0        0        0     2229 2023-06-29 23:09:37.000000 rai_benchmark_test-1.3/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.3/src/tokenizer.py
```

### Comparing `rai_benchmark_test-1.2/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-1.3/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/aml_fetch_data.py` & `rai_benchmark_test-1.3/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/assessment_flow.py` & `rai_benchmark_test-1.3/src/assessment_flow.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/data_prep.py` & `rai_benchmark_test-1.3/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/e2e_exp.py` & `rai_benchmark_test-1.3/src/e2e_exp.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/evaluation.py` & `rai_benchmark_test-1.3/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/job.py` & `rai_benchmark_test-1.3/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/job_manager.py` & `rai_benchmark_test-1.3/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/prompt_builder.py` & `rai_benchmark_test-1.3/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/request.py` & `rai_benchmark_test-1.3/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.2/src/run.py` & `rai_benchmark_test-1.3/src/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import sys
 from azureml.core import ScriptRunConfig
 from azureml.core import Experiment
 from azureml.core import Environment
 import click
-from src.aml_auth import get_aml_workspace
+from src.aml_auth import get_aml_workspace, get_secret
 from src.constants import ENDPOINT_CONFIG_PATH, PROMPT_PATH
 from os import path
 import shutil
-
+import json
 
 @click.command()
 @click.option('--area', type=str, help='groundedness/contentharm/...')
 @click.option('--samples_per_benchmark', type=str, help='number of samples per benchmark')
 @click.option('--experiment_name', type=str, help='name of experiment')
 @click.option('--prompt_file', type=str, help='file path of prompt')
 @click.option('--endpoint_config', type=str, help='file path of endpoint config including model name, url, token')
 def submit_run(area, samples_per_benchmark, experiment_name, prompt_file, endpoint_config):
-    print("entered main")
 
     myenv = Environment("user-managed-env")
     myenv.python.user_managed_dependencies = True
 
-    
+    # retrievei AOAI token from any keyvault you persoanlly have access to
+    f = open(endpoint_config)
+    endpoint_config_json = json.load(f)
+    f.close()
+    token = get_secret(endpoint_config_json["keyvault_url"], endpoint_config_json["token_name"])
 
     script_params = [
       "--area",
       area,
       "--samples_per_benchmark",
       samples_per_benchmark,
       "--experiment_name",
-      experiment_name
+      experiment_name,
+      "--aoai_token",
+      token
     ]
 
-
     # copy non-package parameter files to the src directory so that they will be uploaded to aml
     # copy model config, including token
     shutil.copyfile(endpoint_config, path.join(path.dirname(__file__), ENDPOINT_CONFIG_PATH))
     # copy prompt
     shutil.copyfile(prompt_file, path.join(path.dirname(__file__), PROMPT_PATH))
 
     src = ScriptRunConfig(source_directory=path.dirname(__file__),
```

