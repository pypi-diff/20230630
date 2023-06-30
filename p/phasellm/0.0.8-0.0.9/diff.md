# Comparing `tmp/phasellm-0.0.8.tar.gz` & `tmp/phasellm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.8.tar", last modified: Mon Jun  5 00:28:05 2023, max compression
+gzip compressed data, was "phasellm-0.0.9.tar", last modified: Mon Jun  5 01:08:32 2023, max compression
```

## Comparing `phasellm-0.0.8.tar` & `phasellm-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-06-02 18:12:47.000000 phasellm-0.0.8/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 00:28:05.722988 phasellm-0.0.8/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4999 2023-06-02 18:12:47.000000 phasellm-0.0.8/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/phasellm/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/agents.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4802 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/eval.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4372 2023-06-02 18:12:47.000000 phasellm-0.0.8/phasellm/exceptions.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3044 2023-06-02 23:00:21.000000 phasellm-0.0.8/phasellm/html.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    17831 2023-06-02 18:38:12.000000 phasellm-0.0.8/phasellm/llms.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 00:28:05.722988 phasellm-0.0.8/phasellm.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      299 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-06-05 00:28:05.000000 phasellm-0.0.8/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-06-05 00:28:05.722988 phasellm-0.0.8/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-06-02 18:18:06.000000 phasellm-0.0.8/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 01:08:32.699783 phasellm-0.0.9/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-06-02 18:12:47.000000 phasellm-0.0.9/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 01:08:32.699783 phasellm-0.0.9/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4999 2023-06-02 18:12:47.000000 phasellm-0.0.9/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 01:08:32.699783 phasellm-0.0.9/phasellm/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-06-02 18:12:47.000000 phasellm-0.0.9/phasellm/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-06-02 18:12:47.000000 phasellm-0.0.9/phasellm/agents.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4802 2023-06-02 18:12:47.000000 phasellm-0.0.9/phasellm/eval.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4372 2023-06-02 18:12:47.000000 phasellm-0.0.9/phasellm/exceptions.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3044 2023-06-05 01:07:10.000000 phasellm-0.0.9/phasellm/html.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    18063 2023-06-05 01:07:10.000000 phasellm-0.0.9/phasellm/llms.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-06-05 01:08:32.699783 phasellm-0.0.9/phasellm.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-06-05 01:08:32.000000 phasellm-0.0.9/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      299 2023-06-05 01:08:32.000000 phasellm-0.0.9/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-06-05 01:08:32.000000 phasellm-0.0.9/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-06-05 01:08:32.000000 phasellm-0.0.9/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-06-05 01:08:32.000000 phasellm-0.0.9/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-06-05 01:08:32.699783 phasellm-0.0.9/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-06-05 01:07:10.000000 phasellm-0.0.9/setup.py
```

### Comparing `phasellm-0.0.8/LICENSE` & `phasellm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/PKG-INFO` & `phasellm-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.8/README.md` & `phasellm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/__init__.py` & `phasellm-0.0.9/phasellm/__init__.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/agents.py` & `phasellm-0.0.9/phasellm/agents.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/eval.py` & `phasellm-0.0.9/phasellm/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/exceptions.py` & `phasellm-0.0.9/phasellm/exceptions.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/html.py` & `phasellm-0.0.9/phasellm/html.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.8/phasellm/llms.py` & `phasellm-0.0.9/phasellm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,11 +509,17 @@
 
     def chat(self, message):
         """
         Chats with the chatbot.
         """
         self._append_message('user', message)
         start_time = time.time()
-        response = self.llm.complete_chat(self.messages, "assistant")
+
+        clean_messages = [] # We remove fields that the ChatBot class specifically tracks.
+        for m in self.messages:
+            m_copy = {"role":m["role"], "content":m["content"]}
+            clean_messages.append(m_copy)
+
+        response = self.llm.complete_chat(clean_messages, "assistant")
         self._append_message('assistant', response, log_time_seconds = time.time() - start_time)
         return response
```

### Comparing `phasellm-0.0.8/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.9/phasellm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.8/setup.py` & `phasellm-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

