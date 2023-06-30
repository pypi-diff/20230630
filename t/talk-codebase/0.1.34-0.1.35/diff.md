# Comparing `tmp/talk_codebase-0.1.34.tar.gz` & `tmp/talk_codebase-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.34.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.35.tar", max compression
```

## Comparing `talk_codebase-0.1.34.tar` & `talk_codebase-0.1.35.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2874 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/README.md
--rw-r--r--   0        0        0      896 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2898 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/cli.py
--rw-r--r--   0        0        0     1615 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/consts.py
--rw-r--r--   0        0        0     4777 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/llm.py
--rw-r--r--   0        0        0     2278 2023-06-29 07:25:30.692569 talk_codebase-0.1.34/talk_codebase/utils.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0     2874 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/README.md
+-rw-r--r--   0        0        0      957 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1702 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/talk_codebase/consts.py
+-rw-r--r--   0        0        0     4777 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-06-30 14:34:53.763597 talk_codebase-0.1.35/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.35/PKG-INFO
```

### Comparing `talk_codebase-0.1.34/README.md` & `talk_codebase-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.34/pyproject.toml` & `talk_codebase-0.1.35/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.34"
+version = "0.1.35"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
@@ -19,14 +19,17 @@
 gitpython = "^3.1.31"
 questionary = "^1.10.0"
 gpt4all = "^0.2.3"
 sentence-transformers = "^2.2.2"
 unstructured = "^0.6.10"
 
 
+[tool.poetry.group.dev.dependencies]
+setuptools = "^68.0.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
 "Source" = "https://github.com/rsaryev/talk-codebase"
 "Bug Tracker" = "https://github.com/rsaryev/talk-codebase/issues"
```

### Comparing `talk_codebase-0.1.34/talk_codebase/cli.py` & `talk_codebase-0.1.35/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.34/talk_codebase/consts.py` & `talk_codebase-0.1.35/talk_codebase/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,13 +42,16 @@
     ".md": {
         "loader": UnstructuredMarkdownLoader,
         "args": {}
     },
     ".pdf": {
         "loader": PDFMinerLoader,
         "args": {}
-    },
-    ".txt": {
-        "loader": TextLoader,
-        "args": {}
-    },
+    }
 }
+
+for ext in ALLOW_FILES:
+    if ext not in LOADER_MAPPING:
+        LOADER_MAPPING[ext] = {
+            "loader": TextLoader,
+            "args": {}
+        }
```

### Comparing `talk_codebase-0.1.34/talk_codebase/llm.py` & `talk_codebase-0.1.35/talk_codebase/llm.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.34/talk_codebase/utils.py` & `talk_codebase-0.1.35/talk_codebase/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import glob
 import multiprocessing
 import os
 import sys
 
 import tiktoken
 from git import Repo
-from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 from talk_codebase.consts import LOADER_MAPPING, EXCLUDE_FILES
 
 
 def get_repo(root_dir):
```

### Comparing `talk_codebase-0.1.34/PKG-INFO` & `talk_codebase-0.1.35/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.34
+Version: 0.1.35
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

