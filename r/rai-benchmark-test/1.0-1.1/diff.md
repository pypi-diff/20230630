# Comparing `tmp/rai_benchmark_test-1.0.tar.gz` & `tmp/rai_benchmark_test-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-1.0.tar", last modified: Thu Jun 29 22:15:31 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-1.1.tar", last modified: Thu Jun 29 22:22:35 2023, max compression
```

## Comparing `rai_benchmark_test-1.0.tar` & `rai_benchmark_test-1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.850823 rai_benchmark_test-1.0/
--rw-rw-rw-   0        0        0       63 2023-06-29 22:15:31.835680 rai_benchmark_test-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.630219 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 22:15:31.850823 rai_benchmark_test-1.0/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-29 22:14:50.000000 rai_benchmark_test-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.835680 rai_benchmark_test-1.0/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.0/src/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-1.0/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.0/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.0/src/assessment_flow.py
--rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.0/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.0/src/data_prep.py
--rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-1.0/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.0/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.0/src/job.py
--rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-1.0/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.0/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.0/src/prompt_data.py
--rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.0/src/request.py
--rw-rw-rw-   0        0        0     2030 2023-06-29 22:09:01.000000 rai_benchmark_test-1.0/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.0/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:35.444305 rai_benchmark_test-1.1/
+-rw-rw-rw-   0        0        0       63 2023-06-29 22:22:35.444305 rai_benchmark_test-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:35.413060 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 22:22:35.000000 rai_benchmark_test-1.1/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:22:35.444305 rai_benchmark_test-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-29 22:22:28.000000 rai_benchmark_test-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:35.428682 rai_benchmark_test-1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.1/src/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-1.1/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.1/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.1/src/assessment_flow.py
+-rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.1/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.1/src/data_prep.py
+-rw-rw-rw-   0        0        0     3818 2023-06-29 22:22:10.000000 rai_benchmark_test-1.1/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.1/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.1/src/job.py
+-rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-1.1/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.1/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.1/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.1/src/request.py
+-rw-rw-rw-   0        0        0     1943 2023-06-29 22:21:45.000000 rai_benchmark_test-1.1/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.1/src/tokenizer.py
```

### Comparing `rai_benchmark_test-1.0/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-1.1/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/aml_auth.py` & `rai_benchmark_test-1.1/src/aml_auth.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/aml_fetch_data.py` & `rai_benchmark_test-1.1/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/assessment_flow.py` & `rai_benchmark_test-1.1/src/assessment_flow.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/data_prep.py` & `rai_benchmark_test-1.1/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/e2e_exp.py` & `rai_benchmark_test-1.1/src/e2e_exp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import mlflow
 import argparse
 from aml_auth import start_mlflow_experiment, end_mlflow_experiment, get_ml_client
 from assessment_flow import test_benchmark
 from aml_fetch_data import fetch_data
 from evaluation import eval_7class, eval_binary
+from constants import PROMPT_PATH
 
 
-def exp_benchmark(ml_client, dataset_name, min_score, max_score, sample_size, model, prompt_template, eval_func, n_prompts_per_call, seed=1234):
+def exp_benchmark(ml_client, dataset_name, min_score, max_score, sample_size, prompt_template, eval_func, n_prompts_per_call, seed=1234):
     df = fetch_data(ml_client, dataset_name)
-    acc = test_benchmark(f"./outputs/{dataset_name}", sample_size, model, prompt_template, min_score, max_score, df, eval_func, n_prompts_per_call, seed)
+    acc = test_benchmark(f"./outputs/{dataset_name}", sample_size, prompt_template, min_score, max_score, df, eval_func, n_prompts_per_call, seed)
     # log in mlflow
     mlflow.log_metric(f"{dataset_name}-acc", acc)
     return acc
 
 
-def exp_all_groundedness_benchmarks(ml_client, sample_size, model, prompt_template):
+def exp_all_groundedness_benchmarks(ml_client, sample_size, prompt_template):
     # save template in outputs for record, and log it in mlflow
     f = open("./outputs/prompt_template.txt", "a")
     f.write(prompt_template)
     f.close()
     mlflow.log_param("template", prompt_template[:500])
 
-    openai_acc = exp_benchmark(ml_client, "groundedness-openai", 1, 7, sample_size, model, prompt_template, eval_7class, 1)
-    fever_acc = exp_benchmark(ml_client, "groundedness-fever", 0, 1, sample_size, model, prompt_template, eval_binary, 5)
-    docnli_acc = exp_benchmark(ml_client, "groundedness-docnli", 0, 1, sample_size, model, prompt_template, eval_binary, 5)
-    mctest_acc = exp_benchmark(ml_client, "groundedness-mctest", 0, 1, sample_size, model, prompt_template, eval_binary, 5)
-    mnli_acc = exp_benchmark(ml_client, "groundedness-mnli", 0, 1, sample_size, model, prompt_template, eval_binary, 5)
+    openai_acc = exp_benchmark(ml_client, "groundedness-openai", 1, 7, sample_size, prompt_template, eval_7class, 1)
+    fever_acc = exp_benchmark(ml_client, "groundedness-fever", 0, 1, sample_size, prompt_template, eval_binary, 5)
+    docnli_acc = exp_benchmark(ml_client, "groundedness-docnli", 0, 1, sample_size, prompt_template, eval_binary, 5)
+    mctest_acc = exp_benchmark(ml_client, "groundedness-mctest", 0, 1, sample_size, prompt_template, eval_binary, 5)
+    mnli_acc = exp_benchmark(ml_client, "groundedness-mnli", 0, 1, sample_size, prompt_template, eval_binary, 5)
 
     # get average
     groundedness_avg_acc = (openai_acc+fever_acc+docnli_acc+mctest_acc+mnli_acc)/5
     mlflow.log_metric("groundedness-avg-acc", groundedness_avg_acc)
     return groundedness_avg_acc
 
 
@@ -56,27 +57,24 @@
 def main():
     # Instantiate the parser
     print("entered e2e exp")
     parser = argparse.ArgumentParser()
     parser.add_argument('--area', type=str, help='groundedness/contentharm/...')
     parser.add_argument('--samples_per_benchmark', type=int, help='number of samples per benchmark')
     parser.add_argument('--experiment_name', type=str, help='name of experiment')
-    parser.add_argument('--prompt_file', type=str, help='file path of prompt')
-    parser.add_argument('--model_name', type=str, help='name of model, gpt-35-turbo for example')
     args = parser.parse_args()
 
-    with open(args.prompt_file) as f:
+    with open(PROMPT_PATH) as f:
         prompt = "\n".join(f.readlines())
 
     exp_name = args.experiment_name
     n_samples = args.samples_per_benchmark
-    model = args.model_name
 
     if args.area == "groundedness":
         start_mlflow_experiment(exp_name)
         ml_client = get_ml_client()
-        exp_all_groundedness_benchmarks(ml_client, n_samples, model, prompt)
+        exp_all_groundedness_benchmarks(ml_client, n_samples, prompt)
         end_mlflow_experiment()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `rai_benchmark_test-1.0/src/evaluation.py` & `rai_benchmark_test-1.1/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/job.py` & `rai_benchmark_test-1.1/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/job_manager.py` & `rai_benchmark_test-1.1/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/prompt_builder.py` & `rai_benchmark_test-1.1/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/request.py` & `rai_benchmark_test-1.1/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.0/src/run.py` & `rai_benchmark_test-1.1/src/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,24 @@
 
     script_params = [
       "--area",
       area,
       "--samples_per_benchmark",
       samples_per_benchmark,
       "--experiment_name",
-      experiment_name,
-      "--prompt_file",
-      prompt_new_path,
-      "--model_name",
-      model_name
+      experiment_name
     ]
 
 
     # copy non-package parameter files to the src directory so that they will be uploaded to aml
     # copy model config, including token
     shutil.copyfile(endpoint_config, path.join(path.dirname(__file__), ENDPOINT_CONFIG_PATH))
     # copy prompt
-    shutil.copyfile(prompt_file, path.join(path.dirname(__file__),PROMPT_PATH))
+    shutil.copyfile(prompt_file, path.join(path.dirname(__file__), PROMPT_PATH))
+
     src = ScriptRunConfig(source_directory=path.dirname(__file__),
                         script='e2e_exp.py',
                         compute_target='local',
                         environment=myenv,
                         arguments=script_params
                         )
```

