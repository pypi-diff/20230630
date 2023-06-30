# Comparing `tmp/dysweep-0.1.0.tar.gz` & `tmp/dysweep-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.1.0.tar", last modified: Fri Jun 30 16:54:48 2023, max compression
+gzip compressed data, was "dysweep-0.1.1.tar", last modified: Fri Jun 30 19:42:32 2023, max compression
```

## Comparing `dysweep-0.1.0.tar` & `dysweep-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 16:52:28.000000 dysweep-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-30 16:54:48.136932 dysweep-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 16:52:28.000000 dysweep-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:54:48.136932 dysweep-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-30 16:52:28.000000 dysweep-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 19:40:04.000000 dysweep-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 19:42:32.927796 dysweep-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-30 19:40:04.000000 dysweep-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 19:40:04.000000 dysweep-0.1.1/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:42:32.927796 dysweep-0.1.1/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 19:42:32.000000 dysweep-0.1.1/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:42:32.927796 dysweep-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-30 19:40:04.000000 dysweep-0.1.1/setup.py
```

### Comparing `dysweep-0.1.0/PKG-INFO` & `dysweep-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
-License: Apache License 2.0
+License: MIT
 Description: # Dysweep
         
         Dysweep is a Python library enhancing the functionalities of the [Weights and Biases sweep library](https://docs.wandb.ai/guides/sweeps). It allows entire experiments to be executed using a configuration dictionary (YAML/JSON).
         
         ## Features
         
         - **Checkpointing for the Sweep Server**: Dysweep introduces checkpointing that allows resuming certain runs, useful when only a small fraction of runs fail, eliminating the need to re-run the entire sweep.
```

### Comparing `dysweep-0.1.0/README.md` & `dysweep-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-# *Dysweep* 
 
-![PyPI](https://img.shields.io/badge/PyPI-Compatible-green?style=for-the-badge&logo=PyPI)
+<div align="center">
+
+<h1>
+<big><b><i>Dysweep</i></b></big><br/>
+</h1>
+<h4>
+<i>Generic hierarchical configurations and resumable runs on Weights & Biases for Research</i>
+</h4>
+
+
+
+
+[![PyPI version](https://badge.fury.io/py/dysweep.svg)](https://pypi.org/project/dysweep/)
+[![Slack](https://img.shields.io/badge/chat-on%20slack-red.svg)](https://join.slack.com/t/dysweep/shared_invite/zt-1ynkfdpdc-wiYHkiLzjrZ8yGqYkM9brQ)
+
+</div>
 
 ![Bird's Eye View](./images/main-figure.svg)
+Use the extended capabilities of *Dysweep* library on top of Weights & Biases for fast and comprehensive experimentation in your research projects.
 
 ## Table of Contents
 
 - [Features](#features)
 - [Applications](#applications)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Visualizing the Sweep](#visualizing-the-sweep)
 - [Tutorial and Use-Cases](#tutorial-and-use-cases)
 - [License](#license)
 
 
 
-#### Use Weights & Biases Sweeps for Everything!
 Dysweep is an innovative Python library designed to extend and enhance the functionalities of the [Weights and Biases (WandB) sweep library](https://docs.wandb.ai/guides/sweeps). Dysweep is built with the belief that an entire experiment should be executable through a configuration dictionary, whether it's formatted as a YAML or JSON file.
 
 ## Features
 
 Dysweep introduces two major enhancements:
 
 ### Checkpointing for the Sweep Server
@@ -113,10 +127,10 @@
 pip install -r requirements.txt
 # The requirements for running the examples
 pip install -r requirements-testing.txt
 ```
 
 ## License
 
-Dysweep is licensed under the [Apache License 2.0](./LICENSE).
+Dysweep is released under [MIT License](./LICENSE).
```

### Comparing `dysweep-0.1.0/dysweep/console.py` & `dysweep-0.1.1/dysweep/console.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.0/dysweep/parallel.py` & `dysweep-0.1.1/dysweep/parallel.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.0/dysweep/utils.py` & `dysweep-0.1.1/dysweep/utils.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.0/dysweep/wandbX.py` & `dysweep-0.1.1/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.1.0/dysweep.egg-info/PKG-INFO` & `dysweep-0.1.1/dysweep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
-License: Apache License 2.0
+License: MIT
 Description: # Dysweep
         
         Dysweep is a Python library enhancing the functionalities of the [Weights and Biases sweep library](https://docs.wandb.ai/guides/sweeps). It allows entire experiments to be executed using a configuration dictionary (YAML/JSON).
         
         ## Features
         
         - **Checkpointing for the Sweep Server**: Dysweep introduces checkpointing that allows resuming certain runs, useful when only a small fraction of runs fail, eliminating the need to re-run the entire sweep.
```

### Comparing `dysweep-0.1.0/setup.py` & `dysweep-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("readme_pypi.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dysweep",
     packages=find_packages(include=["dysweep", "dysweep.*"]),
     version=__version__,
-    license="Apache License 2.0",
+    license='MIT',
     description="Use Weights and Biases Sweeps for Dynamic Configuration generation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hamid Kamkari",
     author_email="hamidrezakamkari@gmail.com",
     url="https://github.com/HamidrezaKmK/dysweep",
     entry_points={
```

