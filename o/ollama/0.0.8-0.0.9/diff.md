# Comparing `tmp/ollama-0.0.8.tar.gz` & `tmp/ollama-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.8.tar", max compression
+gzip compressed data, was "ollama-0.0.9.tar", max compression
```

## Comparing `ollama-0.0.8.tar` & `ollama-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.8/LICENSE
--rw-r--r--   0        0        0     1576 2023-06-30 16:39:01.392273 ollama-0.0.8/README.md
--rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.8/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.8/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.8/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     4535 2023-06-30 20:04:31.797685 ollama-0.0.8/ollama/cmd/cli.py
--rw-r--r--   0        0        0     1961 2023-06-30 18:52:59.750021 ollama-0.0.8/ollama/cmd/server.py
--rw-r--r--   0        0        0     3299 2023-06-30 20:04:31.797829 ollama-0.0.8/ollama/engine.py
--rw-r--r--   0        0        0     4033 2023-06-30 20:04:31.797966 ollama-0.0.8/ollama/model.py
--rw-r--r--   0        0        0      383 2023-06-30 18:54:29.839790 ollama-0.0.8/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.8/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       95 2023-06-30 18:52:59.750969 ollama-0.0.8/ollama/templates/falcon.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.8/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.8/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0      216 2023-06-30 18:52:59.751064 ollama-0.0.8/ollama/templates/mpt.prompt
--rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.8/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.8/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.8/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.8/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0       30 2023-06-30 18:52:59.751171 ollama-0.0.8/ollama/templates/ultralm.prompt
--rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.8/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0      151 2023-06-30 18:52:59.751276 ollama-0.0.8/ollama/templates/wizardcoder.prompt
--rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.8/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      591 2023-06-30 20:04:40.503997 ollama-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 ollama-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 21:19:19.222162 ollama-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1560 2023-06-30 20:25:37.776051 ollama-0.0.9/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 21:06:55.414148 ollama-0.0.9/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:49:14.157072 ollama-0.0.9/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:49:24.964439 ollama-0.0.9/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     5495 2023-06-30 20:25:37.776371 ollama-0.0.9/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     1961 2023-06-30 18:55:36.494770 ollama-0.0.9/ollama/cmd/server.py
+-rw-r--r--   0        0        0     3233 2023-06-30 20:25:37.776696 ollama-0.0.9/ollama/engine.py
+-rw-r--r--   0        0        0     4665 2023-06-30 20:26:46.472404 ollama-0.0.9/ollama/model.py
+-rw-r--r--   0        0        0      432 2023-06-30 20:25:37.777243 ollama-0.0.9/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 19:41:40.782502 ollama-0.0.9/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       95 2023-06-30 18:55:36.498118 ollama-0.0.9/ollama/templates/falcon.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782730 ollama-0.0.9/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782903 ollama-0.0.9/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0      216 2023-06-30 18:55:36.498327 ollama-0.0.9/ollama/templates/mpt.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 19:41:40.783102 ollama-0.0.9/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 19:41:40.783315 ollama-0.0.9/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 19:41:40.783509 ollama-0.0.9/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 19:41:40.783707 ollama-0.0.9/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0       30 2023-06-30 18:55:36.498465 ollama-0.0.9/ollama/templates/ultralm.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 19:41:40.783935 ollama-0.0.9/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0      151 2023-06-30 18:55:36.498594 ollama-0.0.9/ollama/templates/wizardcoder.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 19:41:40.784222 ollama-0.0.9/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      591 2023-06-30 20:28:10.315669 ollama-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 ollama-0.0.9/PKG-INFO
```

### Comparing `ollama-0.0.8/LICENSE` & `ollama-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.8/README.md` & `ollama-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,14 @@
 
 Download a model
 
 ```python
 ollama.pull("huggingface.co/thebloke/llama-7b-ggml")
 ```
 
-## Coming Soon
-
 ### `ollama.search("query")`
 
 Search for compatible models that Ollama can run
 
 ```python
 ollama.search("llama-7b")
 ```
```

### Comparing `ollama-0.0.8/ollama/cmd/cli.py` & `ollama-0.0.9/ollama/cmd/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,29 +33,33 @@
     # create models home if it doesn't exist
     os.makedirs(model.MODELS_CACHE_PATH, exist_ok=True)
 
     subparsers = parser.add_subparsers(
         title='commands',
     )
 
-    server.set_parser(
-        subparsers.add_parser(
-            "serve",
-            description="Start a persistent server to interact with models via the API.",
-            help="Start a persistent server to interact with models via the API.",
-        )
-    )
-
     list_parser = subparsers.add_parser(
         "models",
         description="List all available models stored locally.",
         help="List all available models stored locally.",
     )
     list_parser.set_defaults(fn=list_models)
 
+    search_parser = subparsers.add_parser(
+        "search",
+        description="Search for compatible models that Ollama can run.",
+        help="Search for compatible models that Ollama can run. Usage: search [model]",
+    )
+    search_parser.add_argument(
+        "query",
+        nargs="?",
+        help="Optional name of the model to search for.",
+    )
+    search_parser.set_defaults(fn=search)
+
     pull_parser = subparsers.add_parser(
         "pull",
         description="Download a specified model from a remote source.",
         help="Download a specified model from a remote source. Usage: pull [model]",
     )
     pull_parser.add_argument("model", help="Name of the model to download.")
     pull_parser.set_defaults(fn=pull)
@@ -69,14 +73,22 @@
     run_parser.add_argument(
         "prompt",
         nargs="?",
         help="Optional prompt for the model, interactive mode enabled when not specified.",
     )
     run_parser.set_defaults(fn=run)
 
+    server.set_parser(
+        subparsers.add_parser(
+            "serve",
+            description="Start a persistent server to interact with models via the API.",
+            help="Start a persistent server to interact with models via the API.",
+        )
+    )
+
     args = parser.parse_args()
     args = vars(args)
 
     try:
         fn = args.pop("fn")
         fn(**args)
     except KeyboardInterrupt:
@@ -142,14 +154,30 @@
 def generate_batch(*args, **kwargs):
     for line in sys.stdin:
         print(">>> ", line, end="", flush=True)
         kwargs.update({"prompt": line})
         generate_oneshot(*args, **kwargs)
 
 
+def search(*args, **kwargs):
+    try:
+        model_names = model.search_directory(*args, **kwargs)
+        if len(model_names) == 0:
+            print("No models found.")
+            return
+        elif len(model_names) == 1:
+            print(f"Found {len(model_names)} available model:")
+        else:
+            print(f"Found {len(model_names)} available models:")
+        for model_name in model_names:
+            print(model_name.lower())
+    except Exception as e:
+        print("Failed to fetch available models, check your network connection")
+
+
 def pull(*args, **kwargs):
     model.pull(model_name=kwargs.pop('model'), *args, **kwargs)
 
 
 def run(*args, **kwargs):
     name = model.pull(model_name=kwargs.pop('model'), *args, **kwargs)
     kwargs.update({"model": name})
```

### Comparing `ollama-0.0.8/ollama/cmd/server.py` & `ollama-0.0.9/ollama/cmd/server.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.8/ollama/engine.py` & `ollama-0.0.9/ollama/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 from os import path
+from pathlib import Path
 from contextlib import contextmanager
 from fuzzywuzzy import process
 from llama_cpp import Llama
 from ctransformers import AutoModelForCausalLM
 
 import ollama.prompt
 from ollama.model import MODELS_CACHE_PATH
@@ -26,15 +27,15 @@
     return model.generate(inputs, *args, **kwargs)
 
 
 def load(model_name, models={}):
     if not models.get(model_name, None):
         model_path = path.expanduser(model_name)
         if not path.exists(model_path):
-            model_path = MODELS_CACHE_PATH / model_name + ".bin"
+            model_path = str(MODELS_CACHE_PATH / (model_name + ".bin"))
 
         runners = {
             model_type: cls
             for cls in [LlamaCppRunner, CtransformerRunner]
             for model_type in cls.model_types()
         }
 
@@ -48,22 +49,18 @@
 
 def unload(model_name, models={}):
     if model_name in models:
         models.pop(model_name)
 
 
 class LlamaCppRunner:
-
     def __init__(self, model_path, model_type):
         try:
             with suppress(sys.stderr), suppress(sys.stdout):
-                self.model = Llama(model_path,
-                                   verbose=False,
-                                   n_gpu_layers=1,
-                                   seed=-1)
+                self.model = Llama(model_path, verbose=False, n_gpu_layers=1, seed=-1)
         except Exception:
             raise Exception("Failed to load model", model_path, model_type)
 
     @staticmethod
     def model_types():
         return [
             'llama',
@@ -84,18 +81,18 @@
 
         with suppress(sys.stderr):
             for output in self.model(prompt, *args, **kwargs):
                 yield output
 
 
 class CtransformerRunner:
-
     def __init__(self, model_path, model_type):
         self.model = AutoModelForCausalLM.from_pretrained(
-            model_path, model_type=model_type, local_files_only=True)
+            model_path, model_type=model_type, local_files_only=True
+        )
 
     @staticmethod
     def model_types():
         return [
             'falcon',
             'mpt',
             'starcoder',
```

### Comparing `ollama-0.0.8/ollama/model.py` & `ollama-0.0.9/ollama/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,21 +14,34 @@
     for _, _, files in walk(MODELS_CACHE_PATH):
         for file in files:
             base, ext = path.splitext(file)
             if ext == '.bin':
                 yield base
 
 
+# search the directory and return all models which contain the search term as a substring,
+# or all models if no search term is provided
+def search_directory(query):
+    response = requests.get(MODELS_MANIFEST)
+    response.raise_for_status()
+    directory = response.json()
+    model_names = []
+    for model_info in directory:
+        if not query or query.lower() in model_info.get('name', '').lower():
+            model_names.append(model_info.get('name'))
+    return model_names
+
+
 # get the url of the model from our curated directory
 def get_url_from_directory(model):
     response = requests.get(MODELS_MANIFEST)
     response.raise_for_status()
     directory = response.json()
     for model_info in directory:
-        if model_info.get('name') == model:
+        if model_info.get('name').lower() == model.lower():
             return model_info.get('url')
     return model
 
 
 def download_from_repo(url, file_name):
     parts = urlsplit(url)
     path_parts = parts.path.split('/tree/')
@@ -38,15 +51,14 @@
         branch = 'main'
     else:
         location, branch = path_parts
 
     location = location.strip('/')
     if file_name == '':
         file_name = path.basename(location).lower()
-
     download_url = urlunsplit(
         (
             'https',
             parts.netloc,
             f'/api/models/{location}/tree/{branch}',
             parts.query,
             parts.fragment,
@@ -74,15 +86,15 @@
     if download_url is None:
         raise Exception('No model found')
 
     return download_url, file_size
 
 
 def download_file(download_url, file_name, file_size):
-    local_filename = MODELS_CACHE_PATH / file_name + '.bin'
+    local_filename = MODELS_CACHE_PATH / str(file_name + '.bin')
 
     first_byte = path.getsize(local_filename) if path.exists(local_filename) else 0
 
     if first_byte >= file_size:
         return local_filename
 
     print(f'Pulling {file_name}...')
@@ -107,24 +119,24 @@
             size = file.write(data)
             bar.update(size)
 
     return local_filename
 
 
 def pull(model_name, *args, **kwargs):
-    if path.exists(model_name):
+    maybe_existing_model_location = MODELS_CACHE_PATH / str(model_name + '.bin')
+    if path.exists(model_name) or path.exists(maybe_existing_model_location):
         # a file on the filesystem is being specified
         return model_name
     # check the remote model location and see if it needs to be downloaded
     url = model_name
     file_name = ""
     if not validators.url(url) and not url.startswith('huggingface.co'):
         url = get_url_from_directory(model_name)
         file_name = model_name
-
     if not (url.startswith('http://') or url.startswith('https://')):
         url = f'https://{url}'
 
     if not validators.url(url):
         if model_name in models(MODELS_CACHE_PATH):
             # the model is already downloaded, and specified by name
             return model_name
```

### Comparing `ollama-0.0.8/pyproject.toml` & `ollama-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ollama"
-version = "0.0.8"
+version = "0.0.9"
 description = "Run ai models locally"
 authors = ["ollama team"]
 readme = "README.md"
 packages = [{include = "ollama"}]
 scripts = {ollama = "ollama.cmd.cli:main"}
 
 [tool.poetry.dependencies]
```

### Comparing `ollama-0.0.8/PKG-INFO` & `ollama-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run ai models locally
 Author: ollama team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -106,16 +106,14 @@
 
 Download a model
 
 ```python
 ollama.pull("huggingface.co/thebloke/llama-7b-ggml")
 ```
 
-## Coming Soon
-
 ### `ollama.search("query")`
 
 Search for compatible models that Ollama can run
 
 ```python
 ollama.search("llama-7b")
 ```
```

