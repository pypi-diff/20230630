# Comparing `tmp/ollama-0.0.6.tar.gz` & `tmp/ollama-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.6.tar", max compression
+gzip compressed data, was "ollama-0.0.7.tar", max compression
```

## Comparing `ollama-0.0.6.tar` & `ollama-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.6/LICENSE
--rw-r--r--   0        0        0     1595 2023-06-29 22:25:07.151800 ollama-0.0.6/README.md
--rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.6/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.6/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.6/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     3369 2023-06-29 22:25:07.147017 ollama-0.0.6/ollama/cmd/cli.py
--rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.6/ollama/cmd/server.py
--rw-r--r--   0        0        0     1780 2023-06-29 23:19:13.156536 ollama-0.0.6/ollama/engine.py
--rw-r--r--   0        0        0     3990 2023-06-29 22:25:07.147731 ollama-0.0.6/ollama/model.py
--rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.6/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.6/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.6/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.6/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.6/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.6/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.6/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.6/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.6/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.6/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      508 2023-06-29 23:21:48.781540 ollama-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 ollama-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1576 2023-06-30 16:39:01.392273 ollama-0.0.7/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.7/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.7/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.7/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     4503 2023-06-30 18:52:59.749836 ollama-0.0.7/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     1961 2023-06-30 18:52:59.750021 ollama-0.0.7/ollama/cmd/server.py
+-rw-r--r--   0        0        0     3309 2023-06-30 18:52:59.750201 ollama-0.0.7/ollama/engine.py
+-rw-r--r--   0        0        0     4007 2023-06-30 18:52:59.750360 ollama-0.0.7/ollama/model.py
+-rw-r--r--   0        0        0      620 2023-06-30 18:52:59.750710 ollama-0.0.7/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.7/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       95 2023-06-30 18:52:59.750969 ollama-0.0.7/ollama/templates/falcon.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.7/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.7/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0      216 2023-06-30 18:52:59.751064 ollama-0.0.7/ollama/templates/mpt.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.7/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.7/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.7/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.7/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0       30 2023-06-30 18:52:59.751171 ollama-0.0.7/ollama/templates/ultralm.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.7/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0      151 2023-06-30 18:52:59.751276 ollama-0.0.7/ollama/templates/wizardcoder.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.7/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      591 2023-06-30 18:54:09.101264 ollama-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 ollama-0.0.7/PKG-INFO
```

### Comparing `ollama-0.0.6/LICENSE` & `ollama-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.6/README.md` & `ollama-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 # Ollama
 
 Ollama is a tool for running any large language model on any machine. It's designed to be easy to use and fast, supporting the largest number of models possible by using the fastest loader available for your platform and model.
 
-> _Note: this project is a work in progress._
+> _Note: this project is a work in progress. Certain models that can be run with `ollama` are intended for research and/or non-commercial use only._
 
 ## Install
 
+Using `pip`:
+
 ```
 pip install ollama
 ```
 
+Using `docker`:
+
+```
+docker run ollama/ollama
+```
+
 ## Quickstart
 
 To run a model, use `ollama run`:
 
 ```
 ollama run orca-mini-3b
 ```
@@ -51,30 +59,14 @@
 
 List available local models
 
 ```python
 models = ollama.models()
 ```
 
-### `ollama.serve()`
-
-Serve the ollama http server
-
-```
-ollama.serve()
-```
-
-### `ollama.add(filepath)`
-
-Add a model by importing from a file
-
-```python
-ollama.add("./path/to/model")
-```
-
 ### `ollama.load(model)`
 
 Manually a model for generation
 
 ```python
 ollama.load("model")
 ```
```

### Comparing `ollama-0.0.6/ollama/model.py` & `ollama-0.0.7/ollama/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import requests
 import validators
+from pathlib import Path
 from os import path, walk
 from urllib.parse import urlsplit, urlunsplit
 from tqdm import tqdm
 
 
-models_endpoint_url = 'https://ollama.ai/api/models'
+MODELS_MANIFEST = 'https://ollama.ai/api/models'
+MODELS_CACHE_PATH = path.join(Path.home(), '.ollama', 'models')
 
 
-def models(models_home='.', *args, **kwargs):
-    for _, _, files in walk(models_home):
+def models(*args, **kwargs):
+    for _, _, files in walk(MODELS_CACHE_PATH):
         for file in files:
             base, ext = path.splitext(file)
             if ext == '.bin':
                 yield base
 
 
 # get the url of the model from our curated directory
 def get_url_from_directory(model):
-    response = requests.get(models_endpoint_url)
+    response = requests.get(MODELS_MANIFEST)
     response.raise_for_status()
     directory = response.json()
     for model_info in directory:
         if model_info.get('name') == model:
             return model_info.get('url')
     return model
 
 
-def download_from_repo(url, file_name, models_home='.'):
+def download_from_repo(url, file_name):
     parts = urlsplit(url)
     path_parts = parts.path.split('/tree/')
 
     if len(path_parts) == 1:
         location = path_parts[0]
         branch = 'main'
     else:
         location, branch = path_parts
 
     location = location.strip('/')
     if file_name == '':
-        file_name = path.basename(location)
+        file_name = path.basename(location).lower()
 
     download_url = urlunsplit(
         (
             'https',
             parts.netloc,
             f'/api/models/{location}/tree/{branch}',
             parts.query,
@@ -51,15 +53,15 @@
         )
     )
     response = requests.get(download_url)
     response.raise_for_status()
     json_response = response.json()
 
     download_url, file_size = find_bin_file(json_response, location, branch)
-    return download_file(download_url, models_home, file_name, file_size)
+    return download_file(download_url, file_name, file_size)
 
 
 def find_bin_file(json_response, location, branch):
     download_url = None
     file_size = 0
     for file_info in json_response:
         if file_info.get('type') == 'file' and file_info.get('path').endswith('.bin'):
@@ -71,16 +73,16 @@
 
     if download_url is None:
         raise Exception('No model found')
 
     return download_url, file_size
 
 
-def download_file(download_url, models_home, file_name, file_size):
-    local_filename = path.join(models_home, file_name) + '.bin'
+def download_file(download_url, file_name, file_size):
+    local_filename = path.join(MODELS_CACHE_PATH, file_name) + '.bin'
 
     first_byte = path.getsize(local_filename) if path.exists(local_filename) else 0
 
     if first_byte >= file_size:
         return local_filename
 
     print(f'Pulling {file_name}...')
@@ -104,30 +106,30 @@
         for data in response.iter_content(chunk_size=1024):
             size = file.write(data)
             bar.update(size)
 
     return local_filename
 
 
-def pull(model, models_home='.', *args, **kwargs):
+def pull(model, *args, **kwargs):
     if path.exists(model):
         # a file on the filesystem is being specified
         return model
     # check the remote model location and see if it needs to be downloaded
     url = model
     file_name = ""
     if not validators.url(url) and not url.startswith('huggingface.co'):
         url = get_url_from_directory(model)
         file_name = model
 
     if not (url.startswith('http://') or url.startswith('https://')):
         url = f'https://{url}'
 
     if not validators.url(url):
-        if model in models(models_home):
+        if model in models(MODELS_CACHE_PATH):
             # the model is already downloaded, and specified by name
             return model
         raise Exception(f'Unknown model {model}')
 
-    local_filename = download_from_repo(url, file_name, models_home)
+    local_filename = download_from_repo(url, file_name)
 
     return local_filename
```

### Comparing `ollama-0.0.6/ollama/prompt.py` & `ollama-0.0.7/ollama/prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import os
+from os import path
 from difflib import SequenceMatcher
 from jinja2 import Environment, PackageLoader
 
 
-def template(model, prompt):
+def template(name, prompt):
     best_ratio = 0
     best_template = ''
 
     environment = Environment(loader=PackageLoader(__name__, 'templates'))
     for template in environment.list_templates():
-        base, _ = os.path.splitext(template)
-        ratio = SequenceMatcher(None, os.path.basename(model.lower()), base).ratio()
+        base, _ = path.splitext(template)
+        ratio = SequenceMatcher(None, path.basename(name).lower(), base).ratio()
         if ratio > best_ratio:
             best_ratio = ratio
             best_template = template
 
     template = environment.get_template(best_template)
     return template.render(prompt=prompt)
```

### Comparing `ollama-0.0.6/PKG-INFO` & `ollama-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.0.6
+Version: 0.0.7
 Summary: Run ai models locally
 Author: ollama team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiohttp-cors (>=0.7.0,<0.8.0)
+Requires-Dist: ctransformers (>=0.2.10,<0.3.0)
+Requires-Dist: fuzzywuzzy[speedup] (>=0.18.0,<0.19.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: llama-cpp-python (>=0.1.66,<0.2.0)
+Requires-Dist: llama-cpp-python (>=0.1.67,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Ollama
 
 Ollama is a tool for running any large language model on any machine. It's designed to be easy to use and fast, supporting the largest number of models possible by using the fastest loader available for your platform and model.
 
-> _Note: this project is a work in progress._
+> _Note: this project is a work in progress. Certain models that can be run with `ollama` are intended for research and/or non-commercial use only._
 
 ## Install
 
+Using `pip`:
+
 ```
 pip install ollama
 ```
 
+Using `docker`:
+
+```
+docker run ollama/ollama
+```
+
 ## Quickstart
 
 To run a model, use `ollama run`:
 
 ```
 ollama run orca-mini-3b
 ```
@@ -72,30 +82,14 @@
 
 List available local models
 
 ```python
 models = ollama.models()
 ```
 
-### `ollama.serve()`
-
-Serve the ollama http server
-
-```
-ollama.serve()
-```
-
-### `ollama.add(filepath)`
-
-Add a model by importing from a file
-
-```python
-ollama.add("./path/to/model")
-```
-
 ### `ollama.load(model)`
 
 Manually a model for generation
 
 ```python
 ollama.load("model")
 ```
```

