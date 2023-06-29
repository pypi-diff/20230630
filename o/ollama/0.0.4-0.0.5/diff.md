# Comparing `tmp/ollama-0.0.4.tar.gz` & `tmp/ollama-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.4.tar", max compression
+gzip compressed data, was "ollama-0.0.5.tar", max compression
```

## Comparing `ollama-0.0.4.tar` & `ollama-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2023-06-26 21:19:19.222162 ollama-0.0.4/LICENSE
--rw-r--r--   0        0        0     1870 2023-06-29 14:42:40.514873 ollama-0.0.4/README.md
--rw-r--r--   0        0        0      152 2023-06-28 21:06:55.414148 ollama-0.0.4/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 14:49:14.157072 ollama-0.0.4/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 20:49:24.964439 ollama-0.0.4/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     3269 2023-06-29 20:42:43.077175 ollama-0.0.4/ollama/cmd/cli.py
--rw-r--r--   0        0        0     2123 2023-06-29 14:42:40.516389 ollama-0.0.4/ollama/cmd/server.py
--rw-r--r--   0        0        0     1682 2023-06-29 20:22:30.476717 ollama-0.0.4/ollama/engine.py
--rw-r--r--   0        0        0     3905 2023-06-29 19:09:36.124508 ollama-0.0.4/ollama/model.py
--rw-r--r--   0        0        0      618 2023-06-29 19:36:57.583354 ollama-0.0.4/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 19:41:40.782502 ollama-0.0.4/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782730 ollama-0.0.4/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782903 ollama-0.0.4/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0       13 2023-06-28 19:41:40.783102 ollama-0.0.4/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 19:41:40.783315 ollama-0.0.4/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 19:41:40.783509 ollama-0.0.4/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 19:41:40.783707 ollama-0.0.4/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0      186 2023-06-28 19:41:40.783935 ollama-0.0.4/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0       27 2023-06-28 19:41:40.784222 ollama-0.0.4/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      508 2023-06-29 20:53:13.348101 ollama-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 ollama-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1595 2023-06-29 22:25:07.151800 ollama-0.0.5/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.5/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.5/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.5/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     3369 2023-06-29 22:25:07.147017 ollama-0.0.5/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.5/ollama/cmd/server.py
+-rw-r--r--   0        0        0     1778 2023-06-29 22:25:07.147570 ollama-0.0.5/ollama/engine.py
+-rw-r--r--   0        0        0     3990 2023-06-29 22:25:07.147731 ollama-0.0.5/ollama/model.py
+-rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.5/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.5/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.5/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.5/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.5/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.5/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.5/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.5/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.5/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.5/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      508 2023-06-29 22:26:31.061352 ollama-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 ollama-0.0.5/PKG-INFO
```

### Comparing `ollama-0.0.4/LICENSE` & `ollama-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.4/README.md` & `ollama-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,58 @@
-# Ollama
-
-Run ai models locally.
+Metadata-Version: 2.1
+Name: ollama
+Version: 0.0.5
+Summary: Run ai models locally
+Author: ollama team
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: aiohttp-cors (>=0.7.0,<0.8.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: llama-cpp-python (>=0.1.66,<0.2.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: yaspin (>=2.3.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-> _Note: this project is a work in progress. The features below are still in development_
+# Ollama
 
-**Features**
+Ollama is a tool for running any large language model on any machine. It's designed to be easy to use and fast, supporting the largest number of models possible by using the fastest loader available for your platform and model.
 
-- Run models locally on macOS (Windows, Linux and other platforms coming soon)
-- Ollama uses the fastest loader available for your platform and model (e.g. llama.cpp, Core ML and other loaders coming soon)
-- Import models from local files
-- Find and download models on Hugging Face and other sources (coming soon)
-- Support for running and switching between multiple models at a time (coming soon)
-- Native desktop experience (coming soon)
-- Built-in memory (coming soon)
+> _Note: this project is a work in progress._
 
 ## Install
 
 ```
 pip install ollama
 ```
 
 ## Quickstart
 
+To run a model, use `ollama run`:
+
+```
+ollama run orca-mini-3b
 ```
-% ollama run huggingface.co/TheBloke/orca_mini_3B-GGML
-Pulling huggingface.co/TheBloke/orca_mini_3B-GGML...
-Downloading [================           ] 66.67% 11.8MiB/s
 
-...
-...
-...
+You can also run models from hugging face:
 
-> Hello
+```
+ollama run huggingface.co/TheBloke/orca_mini_3B-GGML
+```
+
+Or directly via downloaded model files:
 
-Hello, how may I help you?
+```
+ollama run ~/Downloads/orca-mini-13b.ggmlv3.q4_0.bin
 ```
 
 ## Python SDK
 
 ### Example
 
 ```python
@@ -110,7 +125,8 @@
 ```python
 ollama.search("llama-7b")
 ```
 
 ## Documentation
 
 - [Development](docs/development.md)
+
```

### Comparing `ollama-0.0.4/ollama/cmd/cli.py` & `ollama-0.0.5/ollama/cmd/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,22 +75,26 @@
 
 def generate_oneshot(*args, **kwargs):
     print(flush=True)
 
     spinner = yaspin()
     spinner.start()
     spinner_running = True
-    for output in engine.generate(*args, **kwargs):
-        choices = output.get("choices", [])
-        if len(choices) > 0:
-            if spinner_running:
-                spinner.stop()
-                spinner_running = False
-                print("\r", end="")  # move cursor back to beginning of line again
-            print(choices[0].get("text", ""), end="", flush=True)
+    try:
+        for output in engine.generate(*args, **kwargs):
+            choices = output.get("choices", [])
+            if len(choices) > 0:
+                if spinner_running:
+                    spinner.stop()
+                    spinner_running = False
+                    print("\r", end="")  # move cursor back to beginning of line again
+                print(choices[0].get("text", ""), end="", flush=True)
+    except Exception:
+        spinner.stop()
+        raise
 
     # end with a new line
     print(flush=True)
     print(flush=True)
 
 
 def generate_interactive(*args, **kwargs):
```

### Comparing `ollama-0.0.4/ollama/cmd/server.py` & `ollama-0.0.5/ollama/cmd/server.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.4/ollama/engine.py` & `ollama-0.0.5/ollama/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-import os
-import json
+from os import path, dup, dup2, devnull
 import sys
 from contextlib import contextmanager
 from llama_cpp import Llama as LLM
 
 import ollama.model
 import ollama.prompt
 
 
 @contextmanager
 def suppress_stderr():
-    stderr = os.dup(sys.stderr.fileno())
-    with open(os.devnull, "w") as devnull:
-        os.dup2(devnull.fileno(), sys.stderr.fileno())
+    stderr = dup(sys.stderr.fileno())
+    with open(devnull, "w") as devnull:
+        dup2(devnull.fileno(), sys.stderr.fileno())
         yield
 
-    os.dup2(stderr, sys.stderr.fileno())
+    dup2(stderr, sys.stderr.fileno())
 
 
 def generate(model, prompt, models_home=".", llms={}, *args, **kwargs):
     llm = load(model, models_home=models_home, llms=llms)
 
     prompt = ollama.prompt.template(model, prompt)
     if "max_tokens" not in kwargs:
@@ -34,20 +33,23 @@
     for output in llm(prompt, *args, **kwargs):
         yield output
 
 
 def load(model, models_home=".", llms={}):
     llm = llms.get(model, None)
     if not llm:
-        stored_model_path = os.path.join(models_home, model, ".bin")
-        if os.path.exists(stored_model_path):
+        stored_model_path = path.join(models_home, model) + ".bin"
+        if path.exists(stored_model_path):
             model_path = stored_model_path
         else:
             # try loading this as a path to a model, rather than a model name
-            model_path = os.path.abspath(model)
+            model_path = path.abspath(model)
+
+        if not path.exists(model_path):
+            raise Exception(f"Model not found: {model}")
 
         try:
             # suppress LLM's output
             with suppress_stderr():
                 llm = LLM(model_path, verbose=False)
                 llms.update({model: llm})
         except Exception as e:
```

### Comparing `ollama-0.0.4/ollama/model.py` & `ollama-0.0.5/ollama/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import os
 import requests
 import validators
+from os import path, walk
 from urllib.parse import urlsplit, urlunsplit
 from tqdm import tqdm
 
 
 models_endpoint_url = 'https://ollama.ai/api/models'
 
 
 def models(models_home='.', *args, **kwargs):
-    for _, _, files in os.walk(models_home):
+    for _, _, files in walk(models_home):
         for file in files:
-            base, ext = os.path.splitext(file)
+            base, ext = path.splitext(file)
             if ext == '.bin':
                 yield base
 
 
 # get the url of the model from our curated directory
 def get_url_from_directory(model):
     response = requests.get(models_endpoint_url)
@@ -23,25 +23,27 @@
     directory = response.json()
     for model_info in directory:
         if model_info.get('name') == model:
             return model_info.get('url')
     return model
 
 
-def download_from_repo(url, models_home='.'):
+def download_from_repo(url, file_name, models_home='.'):
     parts = urlsplit(url)
     path_parts = parts.path.split('/tree/')
 
     if len(path_parts) == 1:
         location = path_parts[0]
         branch = 'main'
     else:
         location, branch = path_parts
 
     location = location.strip('/')
+    if file_name == '':
+        file_name = path.basename(location)
 
     download_url = urlunsplit(
         (
             'https',
             parts.netloc,
             f'/api/models/{location}/tree/{branch}',
             parts.query,
@@ -49,15 +51,15 @@
         )
     )
     response = requests.get(download_url)
     response.raise_for_status()
     json_response = response.json()
 
     download_url, file_size = find_bin_file(json_response, location, branch)
-    return download_file(download_url, models_home, location, file_size)
+    return download_file(download_url, models_home, file_name, file_size)
 
 
 def find_bin_file(json_response, location, branch):
     download_url = None
     file_size = 0
     for file_info in json_response:
         if file_info.get('type') == 'file' and file_info.get('path').endswith('.bin'):
@@ -69,25 +71,23 @@
 
     if download_url is None:
         raise Exception('No model found')
 
     return download_url, file_size
 
 
-def download_file(download_url, models_home, location, file_size):
-    local_filename = os.path.join(models_home, os.path.basename(location)) + '.bin'
+def download_file(download_url, models_home, file_name, file_size):
+    local_filename = path.join(models_home, file_name) + '.bin'
 
-    first_byte = (
-        os.path.getsize(local_filename) if os.path.exists(local_filename) else 0
-    )
+    first_byte = path.getsize(local_filename) if path.exists(local_filename) else 0
 
     if first_byte >= file_size:
         return local_filename
 
-    print(f'Pulling {os.path.basename(location)}...')
+    print(f'Pulling {file_name}...')
 
     header = {'Range': f'bytes={first_byte}-'} if first_byte != 0 else {}
 
     response = requests.get(download_url, headers=header, stream=True)
     response.raise_for_status()
 
     total_size = int(response.headers.get('content-length', 0)) + first_byte
@@ -105,27 +105,29 @@
             size = file.write(data)
             bar.update(size)
 
     return local_filename
 
 
 def pull(model, models_home='.', *args, **kwargs):
-    if os.path.exists(model):
+    if path.exists(model):
         # a file on the filesystem is being specified
         return model
     # check the remote model location and see if it needs to be downloaded
     url = model
+    file_name = ""
     if not validators.url(url) and not url.startswith('huggingface.co'):
         url = get_url_from_directory(model)
+        file_name = model
 
     if not (url.startswith('http://') or url.startswith('https://')):
         url = f'https://{url}'
 
     if not validators.url(url):
         if model in models(models_home):
             # the model is already downloaded, and specified by name
             return model
         raise Exception(f'Unknown model {model}')
 
-    local_filename = download_from_repo(url, models_home)
+    local_filename = download_from_repo(url, file_name, models_home)
 
     return local_filename
```

### Comparing `ollama-0.0.4/ollama/prompt.py` & `ollama-0.0.5/ollama/prompt.py`

 * *Files identical despite different names*

