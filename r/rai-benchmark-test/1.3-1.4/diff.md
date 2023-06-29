# Comparing `tmp/rai_benchmark_test-1.3.tar.gz` & `tmp/rai_benchmark_test-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-1.3.tar", last modified: Thu Jun 29 23:33:39 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-1.4.tar", last modified: Thu Jun 29 23:44:45 2023, max compression
```

## Comparing `rai_benchmark_test-1.3.tar` & `rai_benchmark_test-1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/
--rw-rw-rw-   0        0        0       63 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 23:33:38.974418 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 23:33:38.000000 rai_benchmark_test-1.3/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/setup.cfg
--rw-rw-rw-   0        0        0      410 2023-06-29 23:33:29.000000 rai_benchmark_test-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:33:39.015596 rai_benchmark_test-1.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.3/src/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-06-29 23:17:04.000000 rai_benchmark_test-1.3/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.3/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.3/src/assessment_flow.py
--rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.3/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.3/src/data_prep.py
--rw-rw-rw-   0        0        0     3818 2023-06-29 22:22:10.000000 rai_benchmark_test-1.3/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.3/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.3/src/job.py
--rw-rw-rw-   0        0        0     7863 2023-06-29 22:30:24.000000 rai_benchmark_test-1.3/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.3/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.3/src/prompt_data.py
--rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.3/src/request.py
--rw-rw-rw-   0        0        0     2229 2023-06-29 23:09:37.000000 rai_benchmark_test-1.3/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.3/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:44:45.758703 rai_benchmark_test-1.4/
+-rw-rw-rw-   0        0        0       63 2023-06-29 23:44:45.758703 rai_benchmark_test-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 23:44:45.522932 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 23:44:45.000000 rai_benchmark_test-1.4/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 23:44:45.758703 rai_benchmark_test-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      410 2023-06-29 23:44:36.000000 rai_benchmark_test-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:44:45.743081 rai_benchmark_test-1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.4/src/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-06-29 23:17:04.000000 rai_benchmark_test-1.4/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.4/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     3147 2023-06-29 23:43:56.000000 rai_benchmark_test-1.4/src/assessment_flow.py
+-rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.4/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.4/src/data_prep.py
+-rw-rw-rw-   0        0        0     3980 2023-06-29 23:43:26.000000 rai_benchmark_test-1.4/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.4/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.4/src/job.py
+-rw-rw-rw-   0        0        0     7863 2023-06-29 22:30:24.000000 rai_benchmark_test-1.4/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.4/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.4/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.4/src/request.py
+-rw-rw-rw-   0        0        0     2229 2023-06-29 23:09:37.000000 rai_benchmark_test-1.4/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.4/src/tokenizer.py
```

### Comparing `rai_benchmark_test-1.3/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-1.4/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/aml_auth.py` & `rai_benchmark_test-1.4/src/aml_auth.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/aml_fetch_data.py` & `rai_benchmark_test-1.4/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/assessment_flow.py` & `rai_benchmark_test-1.4/src/assessment_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 max_score=max_score,
                 **endpoint_args,
     )
 
     return annotations_df
 
 
-def test_benchmark(output_dir, sample_size, annotation_template, min_score, max_score, benchmark_df, eval_func, n_prompts_per_call, seed): # prompt_generate_func takes in min score and max score to generate a template
+def test_benchmark(output_dir, sample_size, annotation_template, min_score, max_score, benchmark_df, eval_func, n_prompts_per_call, token, seed): # prompt_generate_func takes in min score and max score to generate a template
     output_fp = f"{output_dir}/result.csv"
     confusion_matrix_fp = f"{output_dir}/confusion.csv"
     try:
         os.remove(output_fp)
         os.remove(confusion_matrix_fp)
     except:
         pass
@@ -77,17 +77,17 @@
     f = open(ENDPOINT_CONFIG_PATH)
     endpoint_config_from_file = json.load(f)
     f.close()
 
     try:
         endpoint_args = {"endpoint_url": endpoint_config_from_file["endpoint_url"],
                          "model": endpoint_config_from_file["model"],
-                         "token": endpoint_config_from_file["token"]}
+                         "token": token}
     except Exception:
-        raise Exception("endpoint config json should contain endpoint_url, model, and token")
+        raise Exception("endpoint config json should contain endpoint_url, model")
 
     annotated = assess_groundedness_template(
         annotation_template=annotation_template,
         target_df=benchmark_df,
         max_inputs=n_prompts_per_call,
         max_prompt_tokens=4000,
         num_samples=1,
```

### Comparing `rai_benchmark_test-1.3/src/data_prep.py` & `rai_benchmark_test-1.4/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/e2e_exp.py` & `rai_benchmark_test-1.4/src/e2e_exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from aml_auth import start_mlflow_experiment, end_mlflow_experiment, get_ml_client
 from assessment_flow import test_benchmark
 from aml_fetch_data import fetch_data
 from evaluation import eval_7class, eval_binary
 from constants import PROMPT_PATH
 
 
-def exp_benchmark(ml_client, dataset_name, min_score, max_score, sample_size, prompt_template, eval_func, n_prompts_per_call, seed=1234):
+def exp_benchmark(ml_client, dataset_name, min_score, max_score, sample_size, prompt_template, eval_func, n_prompts_per_call, token, seed=1234):
     df = fetch_data(ml_client, dataset_name)
-    acc = test_benchmark(f"./outputs/{dataset_name}", sample_size, prompt_template, min_score, max_score, df, eval_func, n_prompts_per_call, seed)
+    acc = test_benchmark(f"./outputs/{dataset_name}", sample_size, prompt_template, min_score, max_score, df, eval_func, n_prompts_per_call, token, seed)
     # log in mlflow
     mlflow.log_metric(f"{dataset_name}-acc", acc)
     return acc
 
 
-def exp_all_groundedness_benchmarks(ml_client, sample_size, prompt_template):
+def exp_all_groundedness_benchmarks(ml_client, sample_size, prompt_template, token):
     # save template in outputs for record, and log it in mlflow
     f = open("./outputs/prompt_template.txt", "a")
     f.write(prompt_template)
     f.close()
     mlflow.log_param("template", prompt_template[:500])
 
-    openai_acc = exp_benchmark(ml_client, "groundedness-openai", 1, 7, sample_size, prompt_template, eval_7class, 1)
-    fever_acc = exp_benchmark(ml_client, "groundedness-fever", 0, 1, sample_size, prompt_template, eval_binary, 5)
-    docnli_acc = exp_benchmark(ml_client, "groundedness-docnli", 0, 1, sample_size, prompt_template, eval_binary, 5)
-    mctest_acc = exp_benchmark(ml_client, "groundedness-mctest", 0, 1, sample_size, prompt_template, eval_binary, 5)
-    mnli_acc = exp_benchmark(ml_client, "groundedness-mnli", 0, 1, sample_size, prompt_template, eval_binary, 5)
+    openai_acc = exp_benchmark(ml_client, "groundedness-openai", 1, 7, sample_size, prompt_template, eval_7class, 1, token)
+    fever_acc = exp_benchmark(ml_client, "groundedness-fever", 0, 1, sample_size, prompt_template, eval_binary, 5, token)
+    docnli_acc = exp_benchmark(ml_client, "groundedness-docnli", 0, 1, sample_size, prompt_template, eval_binary, 5, token)
+    mctest_acc = exp_benchmark(ml_client, "groundedness-mctest", 0, 1, sample_size, prompt_template, eval_binary, 5, token)
+    mnli_acc = exp_benchmark(ml_client, "groundedness-mnli", 0, 1, sample_size, prompt_template, eval_binary, 5, token)
 
     # get average
     groundedness_avg_acc = (openai_acc+fever_acc+docnli_acc+mctest_acc+mnli_acc)/5
     mlflow.log_metric("groundedness-avg-acc", groundedness_avg_acc)
     return groundedness_avg_acc
 
 
@@ -57,24 +57,26 @@
 def main():
     # Instantiate the parser
     print("entered e2e exp")
     parser = argparse.ArgumentParser()
     parser.add_argument('--area', type=str, help='groundedness/contentharm/...')
     parser.add_argument('--samples_per_benchmark', type=int, help='number of samples per benchmark')
     parser.add_argument('--experiment_name', type=str, help='name of experiment')
+    parser.add_argument('--aoai_token', type=str, help='AOAI token')
     args = parser.parse_args()
 
     with open(PROMPT_PATH) as f:
         prompt = "\n".join(f.readlines())
 
     exp_name = args.experiment_name
     n_samples = args.samples_per_benchmark
+    token = args.aoai_token
 
     if args.area == "groundedness":
         start_mlflow_experiment(exp_name)
         ml_client = get_ml_client()
-        exp_all_groundedness_benchmarks(ml_client, n_samples, prompt)
+        exp_all_groundedness_benchmarks(ml_client, n_samples, prompt, token)
         end_mlflow_experiment()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `rai_benchmark_test-1.3/src/evaluation.py` & `rai_benchmark_test-1.4/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/job.py` & `rai_benchmark_test-1.4/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/job_manager.py` & `rai_benchmark_test-1.4/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/prompt_builder.py` & `rai_benchmark_test-1.4/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/request.py` & `rai_benchmark_test-1.4/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-1.3/src/run.py` & `rai_benchmark_test-1.4/src/run.py`

 * *Files identical despite different names*

