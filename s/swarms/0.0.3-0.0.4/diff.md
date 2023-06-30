# Comparing `tmp/swarms-0.0.3.tar.gz` & `tmp/swarms-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.3.tar", last modified: Fri Jun 30 13:27:30 2023, max compression
+gzip compressed data, was "swarms-0.0.4.tar", last modified: Fri Jun 30 18:08:11 2023, max compression
```

## Comparing `swarms-0.0.3.tar` & `swarms-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 13:27:17.000000 swarms-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 13:27:30.460657 swarms-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-30 13:27:17.000000 swarms-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:27:30.460657 swarms-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-30 13:27:17.000000 swarms-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/swarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 18:08:00.000000 swarms-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 18:08:11.927374 swarms-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-30 18:08:00.000000 swarms-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:08:11.927374 swarms-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 18:08:00.000000 swarms-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/swarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 18:08:00.000000 swarms-0.0.4/swarms/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:08:11.927374 swarms-0.0.4/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 18:08:11.000000 swarms-0.0.4/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.3/LICENSE` & `swarms-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.3/PKG-INFO` & `swarms-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.3
+Version: 0.0.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.3/README.md` & `swarms-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.0.3/swarms/agents/swarms.py` & `swarms-0.0.4/swarms/agents/swarms.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,14 @@
 
 
 llm = ChatOpenAI(model_name="gpt-4", temperature=1.0, openai_api_key="")
 
 
 
 ####################################################################### => Worker Node
-####################################################################### => Worker Node
-####################################################################### => Worker Node
-
 
 class WorkerNode:
     def __init__(self, llm, tools, vectorstore):
         self.llm = llm
         self.tools = tools
         self.vectorstore = vectorstore
```

### Comparing `swarms-0.0.3/swarms/agents/utils.py` & `swarms-0.0.4/swarms/agents/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.0.3/swarms.egg-info/PKG-INFO` & `swarms-0.0.4/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.3
+Version: 0.0.4
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

