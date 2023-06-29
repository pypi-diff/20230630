# Comparing `tmp/rai_benchmark_test-0.9.tar.gz` & `tmp/rai_benchmark_test-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-0.9.tar", last modified: Thu Jun 29 20:45:14 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-1.0.tar", last modified: Thu Jun 29 22:15:31 2023, max compression
```

## Comparing `rai_benchmark_test-0.9.tar` & `rai_benchmark_test-1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.586038 rai_benchmark_test-0.9/
--rw-rw-rw-   0        0        0       63 2023-06-29 20:45:14.586038 rai_benchmark_test-0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.471437 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:45:14.587037 rai_benchmark_test-0.9/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-29 20:44:51.000000 rai_benchmark_test-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.583902 rai_benchmark_test-0.9/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.9/src/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-0.9/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.9/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.9/src/assessment_flow.py
--rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.9/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.9/src/data_prep.py
--rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.9/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.9/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.9/src/job.py
--rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.9/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.9/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.9/src/prompt_data.py
--rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.9/src/request.py
--rw-rw-rw-   0        0        0     1588 2023-06-29 20:44:33.000000 rai_benchmark_test-0.9/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.9/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.850823 rai_benchmark_test-1.0/
+-rw-rw-rw-   0        0        0       63 2023-06-29 22:15:31.835680 rai_benchmark_test-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.630219 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 22:15:31.000000 rai_benchmark_test-1.0/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:15:31.850823 rai_benchmark_test-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-29 22:14:50.000000 rai_benchmark_test-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:15:31.835680 rai_benchmark_test-1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-1.0/src/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-1.0/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-1.0/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     3180 2023-06-29 22:05:31.000000 rai_benchmark_test-1.0/src/assessment_flow.py
+-rw-rw-rw-   0        0        0      172 2023-06-29 22:08:38.000000 rai_benchmark_test-1.0/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-1.0/src/data_prep.py
+-rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-1.0/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-1.0/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-1.0/src/job.py
+-rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-1.0/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-1.0/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-1.0/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4752 2023-06-29 21:53:44.000000 rai_benchmark_test-1.0/src/request.py
+-rw-rw-rw-   0        0        0     2030 2023-06-29 22:09:01.000000 rai_benchmark_test-1.0/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-29 22:01:26.000000 rai_benchmark_test-1.0/src/tokenizer.py
```

### Comparing `rai_benchmark_test-0.9/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-1.0/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/aml_auth.py` & `rai_benchmark_test-1.0/src/aml_auth.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/aml_fetch_data.py` & `rai_benchmark_test-1.0/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/assessment_flow.py` & `rai_benchmark_test-1.0/src/assessment_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from prompt_builder import _PromptBuilder
 from job_manager import _JobManager
-from constants import ANSWER, CONTEXT
-
+from constants import ANSWER, CONTEXT, ENDPOINT_CONFIG_PATH
+import json
 
 def assess_groundedness_template(
     *,
     annotation_template,
     target_df,
     max_inputs,
     max_prompt_tokens,
@@ -50,35 +50,44 @@
                 max_score=max_score,
                 **endpoint_args,
     )
 
     return annotations_df
 
 
-def test_benchmark(output_dir, sample_size, model, annotation_template, min_score, max_score, benchmark_df, eval_func, n_prompts_per_call, seed): # prompt_generate_func takes in min score and max score to generate a template
+def test_benchmark(output_dir, sample_size, annotation_template, min_score, max_score, benchmark_df, eval_func, n_prompts_per_call, seed): # prompt_generate_func takes in min score and max score to generate a template
     output_fp = f"{output_dir}/result.csv"
     confusion_matrix_fp = f"{output_dir}/confusion.csv"
     try:
         os.remove(output_fp)
         os.remove(confusion_matrix_fp)
     except:
         pass
 
     request_args = {
-            "model": model,
+            #"model": model,
             "temperature": 0,
             "top_p": 1,
             "num_samples": 1,
             "max_tokens": 1000,
             "frequency_penalty": 0,
             "presence_penalty": 0
     }
 
-    endpoint_args = {"model": model,
-                     "token": "x"}
+    # read config args
+    f = open(ENDPOINT_CONFIG_PATH)
+    endpoint_config_from_file = json.load(f)
+    f.close()
+
+    try:
+        endpoint_args = {"endpoint_url": endpoint_config_from_file["endpoint_url"],
+                         "model": endpoint_config_from_file["model"],
+                         "token": endpoint_config_from_file["token"]}
+    except Exception:
+        raise Exception("endpoint config json should contain endpoint_url, model, and token")
 
     annotated = assess_groundedness_template(
         annotation_template=annotation_template,
         target_df=benchmark_df,
         max_inputs=n_prompts_per_call,
         max_prompt_tokens=4000,
         num_samples=1,
```

### Comparing `rai_benchmark_test-0.9/src/data_prep.py` & `rai_benchmark_test-1.0/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/e2e_exp.py` & `rai_benchmark_test-1.0/src/e2e_exp.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/evaluation.py` & `rai_benchmark_test-1.0/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/job.py` & `rai_benchmark_test-1.0/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/job_manager.py` & `rai_benchmark_test-1.0/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/prompt_builder.py` & `rai_benchmark_test-1.0/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.9/src/request.py` & `rai_benchmark_test-1.0/src/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     request_count = 0
     outputs = []
     for job in jobs:
         request_count += 1
 
         # Copy request_data to avoid modifying the original dict.
         request_data = {
-            "model": job.request_params["model"],
+            #"model": job.request_params["model"],
             "temperature": job.request_params["temperature"],
             "top_p": job.request_params["top_p"],
             "n": job.request_params["num_samples"],
             "max_tokens": job.request_params["max_tokens"],
             "frequency_penalty": job.request_params["frequency_penalty"],
             "presence_penalty": job.request_params["presence_penalty"],
             "messages": [{"role": "user", "content": job.prompt_data.prompt}],
@@ -121,26 +121,22 @@
         time.sleep(api_call_delay_sec)
     return outputs
 
 
 def _request_prompt_batch(
     jobs: List[_Job],
     token: str,
-    model: str,
+    endpoint_url: str,
     request_error_rate_threshold: float = 0.5,
     api_call_delay_sec: float = 0.5,
     api_call_retry_backoff_factor: int = 3,
     api_call_retry_max_count: int = 3,
     api_call_max_parallel_count: int = 1
 ) -> List[_Job]:
 
-    endpoint_url = f"https://aoai-raidev.openai.azure.com/openai/deployments/{model}/chat/completions?api-version=2023-03-15-preview"
-
-    #print(f"Determined endpoint URL {endpoint_url}")
-
     httpClient = _HTTPClientWithRetry(
         n_retry=api_call_retry_max_count,
         backoff_factor=api_call_retry_backoff_factor,
     )
 
     with httpClient.client as session:
         if len(jobs) == 0:
```

