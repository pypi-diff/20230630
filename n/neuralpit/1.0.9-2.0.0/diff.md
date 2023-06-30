# Comparing `tmp/neuralpit-1.0.9.tar.gz` & `tmp/neuralpit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.9.tar", last modified: Wed May 31 17:40:20 2023, max compression
+gzip compressed data, was "neuralpit-2.0.0.tar", last modified: Fri Jun 30 06:01:48 2023, max compression
```

## Comparing `neuralpit-1.0.9.tar` & `neuralpit-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.378085 neuralpit-1.0.9/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:39:38.000000 neuralpit-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 17:40:20.378085 neuralpit-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 17:39:38.000000 neuralpit-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 17:39:38.000000 neuralpit-1.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:40:20.378085 neuralpit-1.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/api.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/converter.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/services/converterFactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/tools/chat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit/utils/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-31 17:39:38.000000 neuralpit-1.0.9/src/neuralpit/utils/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 17:40:20.000000 neuralpit-1.0.9/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:40:20.374086 neuralpit-1.0.9/test/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testDocChat.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testGetServiceProfile.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 17:39:38.000000 neuralpit-1.0.9/test/testGetUserProfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.111025 neuralpit-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 06:01:19.000000 neuralpit-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-30 06:01:48.111025 neuralpit-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-30 06:01:19.000000 neuralpit-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-06-30 06:01:19.000000 neuralpit-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 06:01:48.111025 neuralpit-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.107025 neuralpit-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.107025 neuralpit-2.0.0/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-06-30 06:01:19.000000 neuralpit-2.0.0/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.111025 neuralpit-2.0.0/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 06:01:19.000000 neuralpit-2.0.0/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-30 06:01:19.000000 neuralpit-2.0.0/src/neuralpit/services/conversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.111025 neuralpit-2.0.0/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-30 06:01:48.000000 neuralpit-2.0.0/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-30 06:01:48.000000 neuralpit-2.0.0/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 06:01:48.000000 neuralpit-2.0.0/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-30 06:01:48.000000 neuralpit-2.0.0/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-30 06:01:48.000000 neuralpit-2.0.0/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:01:48.111025 neuralpit-2.0.0/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 06:01:19.000000 neuralpit-2.0.0/test/testCreateConversation.py
```

### Comparing `neuralpit-1.0.9/PKG-INFO` & `neuralpit-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.9
+Version: 2.0.0
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -15,7 +15,10 @@
 python -m pip install pip-tools
 pip install bumpver
 pip-compile --extra dev pyproject.toml
 bumpver update --minor
 
 # Install package locally
 python -m pip install -e .
+
+# Using SDK
+RUn NeuralPitSDK.init(api_endpoint, api_key)
```

### Comparing `neuralpit-1.0.9/pyproject.toml` & `neuralpit-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.9"
+version = "2.0.0"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["api", "neural", "neuralpit"]
 dependencies = [
-    "requests",
-    "lxml",
-    "toml",
-    "langchain",
-    "openai",
-    "bs4"
+    "requests"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
```

### Comparing `neuralpit-1.0.9/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.0.0/src/neuralpit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.9
+Version: 2.0.0
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -15,7 +15,10 @@
 python -m pip install pip-tools
 pip install bumpver
 pip-compile --extra dev pyproject.toml
 bumpver update --minor
 
 # Install package locally
 python -m pip install -e .
+
+# Using SDK
+RUn NeuralPitSDK.init(api_endpoint, api_key)
```

