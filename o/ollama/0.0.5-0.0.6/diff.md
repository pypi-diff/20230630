# Comparing `tmp/ollama-0.0.5.tar.gz` & `tmp/ollama-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.5.tar", max compression
+gzip compressed data, was "ollama-0.0.6.tar", max compression
```

## Comparing `ollama-0.0.5.tar` & `ollama-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.5/LICENSE
--rw-r--r--   0        0        0     1595 2023-06-29 22:25:07.151800 ollama-0.0.5/README.md
--rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.5/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.5/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.5/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     3369 2023-06-29 22:25:07.147017 ollama-0.0.5/ollama/cmd/cli.py
--rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.5/ollama/cmd/server.py
--rw-r--r--   0        0        0     1778 2023-06-29 22:25:07.147570 ollama-0.0.5/ollama/engine.py
--rw-r--r--   0        0        0     3990 2023-06-29 22:25:07.147731 ollama-0.0.5/ollama/model.py
--rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.5/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.5/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.5/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.5/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.5/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.5/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.5/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.5/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.5/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.5/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      508 2023-06-29 22:26:31.061352 ollama-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 ollama-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1595 2023-06-29 22:25:07.151800 ollama-0.0.6/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.6/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.6/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.6/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     3369 2023-06-29 22:25:07.147017 ollama-0.0.6/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.6/ollama/cmd/server.py
+-rw-r--r--   0        0        0     1780 2023-06-29 23:19:13.156536 ollama-0.0.6/ollama/engine.py
+-rw-r--r--   0        0        0     3990 2023-06-29 22:25:07.147731 ollama-0.0.6/ollama/model.py
+-rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.6/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.6/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.6/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.6/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.6/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.6/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.6/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.6/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.6/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.6/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      508 2023-06-29 23:21:48.781540 ollama-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 ollama-0.0.6/PKG-INFO
```

### Comparing `ollama-0.0.5/LICENSE` & `ollama-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/README.md` & `ollama-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/ollama/cmd/cli.py` & `ollama-0.0.6/ollama/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/ollama/cmd/server.py` & `ollama-0.0.6/ollama/cmd/server.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/ollama/engine.py` & `ollama-0.0.6/ollama/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from os import path, dup, dup2, devnull
+import os
 import sys
+from os import path
 from contextlib import contextmanager
 from llama_cpp import Llama as LLM
 
 import ollama.model
 import ollama.prompt
 
 
 @contextmanager
 def suppress_stderr():
-    stderr = dup(sys.stderr.fileno())
-    with open(devnull, "w") as devnull:
-        dup2(devnull.fileno(), sys.stderr.fileno())
+    stderr = os.dup(sys.stderr.fileno())
+    with open(os.devnull, "w") as devnull:
+        os.dup2(devnull.fileno(), sys.stderr.fileno())
         yield
 
-    dup2(stderr, sys.stderr.fileno())
+    os.dup2(stderr, sys.stderr.fileno())
 
 
 def generate(model, prompt, models_home=".", llms={}, *args, **kwargs):
     llm = load(model, models_home=models_home, llms=llms)
 
     prompt = ollama.prompt.template(model, prompt)
     if "max_tokens" not in kwargs:
```

### Comparing `ollama-0.0.5/ollama/model.py` & `ollama-0.0.6/ollama/model.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/ollama/prompt.py` & `ollama-0.0.6/ollama/prompt.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.5/PKG-INFO` & `ollama-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.0.5
+Version: 0.0.6
 Summary: Run ai models locally
 Author: ollama team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

