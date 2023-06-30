# Comparing `tmp/HandyLLM-0.0.2.tar.gz` & `tmp/HandyLLM-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.0.2.tar", last modified: Tue Jun 20 16:58:31 2023, max compression
+gzip compressed data, was "HandyLLM-0.1.0.tar", last modified: Fri Jun 30 05:37:57 2023, max compression
```

## Comparing `HandyLLM-0.0.2.tar` & `HandyLLM-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:58:31.589431 HandyLLM-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-20 16:58:31.589431 HandyLLM-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:58:31.589431 HandyLLM-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:58:31.585431 HandyLLM-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:58:31.589431 HandyLLM-0.0.2/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-20 16:58:31.000000 HandyLLM-0.0.2/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-20 16:58:31.000000 HandyLLM-0.0.2/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:58:31.000000 HandyLLM-0.0.2/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 16:58:31.000000 HandyLLM-0.0.2/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 16:58:31.000000 HandyLLM-0.0.2/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:58:31.589431 HandyLLM-0.0.2/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-20 16:58:22.000000 HandyLLM-0.0.2/src/handyllm/prompt_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.406128 HandyLLM-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/prompt_converter.py
```

### Comparing `HandyLLM-0.0.2/PKG-INFO` & `HandyLLM-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.0.2
+Version: 0.1.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.0.2/README.md` & `HandyLLM-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.0.2/pyproject.toml` & `HandyLLM-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.0.2/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.1.0/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.0.2
+Version: 0.1.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.0.2/src/handyllm/endpoint_manager.py` & `HandyLLM-0.1.0/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.0.2/src/handyllm/prompt_converter.py` & `HandyLLM-0.1.0/src/handyllm/prompt_converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,32 +13,48 @@
         self.substitute_map = {}
         blocks = re.split(r'(%\w+%)', content)
         for idx in range(1, len(blocks), 2):
             key = blocks[idx]
             value = blocks[idx+1]
             self.substitute_map[key] = value.strip()
 
-    def raw2chat(self, raw_prompt_path: str):
-        with open(raw_prompt_path, 'r', encoding='utf-8') as fin:
-            raw_prompt = fin.read()
-
+    def raw2chat(self, raw_prompt: str):
         # substitute pre-defined variables
         for key, value in self.substitute_map.items():
             raw_prompt = raw_prompt.replace(key, value)
 
         # convert plain text to chat format
         chat = []
         blocks = re.split(r'(\$\w+\$)', raw_prompt)
         for idx in range(1, len(blocks), 2):
             key = blocks[idx]
             value = blocks[idx+1]
             chat.append({"role": key[1:-1], "content": value.strip()})
         
         return chat
     
+    def rawfile2chat(self, raw_prompt_path: str):
+        with open(raw_prompt_path, 'r', encoding='utf-8') as fin:
+            raw_prompt = fin.read()
+        
+        return self.raw2chat(raw_prompt)
+    
+    def chat2raw(self, chat):
+        # convert chat format to plain text
+        messages = []
+        for message in chat:
+            messages.append(f"${message['role']}$\n{message['content']}")
+        raw_prompt = "\n\n".join(messages)
+        return raw_prompt
+    
+    def chat2rawfile(self, chat, raw_prompt_path: str):
+        raw_prompt = self.chat2raw(chat)
+        with open(raw_prompt_path, 'w', encoding='utf-8') as fout:
+            fout.write(raw_prompt)
+    
     def chat_replace_variables(self, chat, variable_map: dict, inplace=False):
         # replace every variable in chat content
         if inplace:
             for message in chat:
                 for var, value in variable_map.items():
                     if var in message['content']:
                         message['content'] = message['content'].replace(var, value)
```

