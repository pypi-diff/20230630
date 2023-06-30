# Comparing `tmp/bs_testing-0.2.1.tar.gz` & `tmp/bs_testing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_testing-0.2.1.tar", max compression
+gzip compressed data, was "bs_testing-0.3.0.tar", max compression
```

## Comparing `bs_testing-0.2.1.tar` & `bs_testing-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 bs_testing-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 bs_testing-0.2.1/blacksmith/__init__.py
--rw-r--r--   0        0        0     2452 2023-06-29 21:50:17.114047 bs_testing-0.2.1/blacksmith/agents.py
--rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 bs_testing-0.2.1/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
--rw-r--r--   0        0        0      718 2023-06-29 10:04:18.913031 bs_testing-0.2.1/blacksmith/defaults/prompts.py
--rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 bs_testing-0.2.1/blacksmith/llm.py
--rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 bs_testing-0.2.1/blacksmith/scripts/__init__.py
--rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 bs_testing-0.2.1/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4117 2023-06-30 08:23:28.853542 bs_testing-0.2.1/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     4352 2023-06-30 08:21:48.445763 bs_testing-0.2.1/blacksmith/scripts/__pycache__/images.cpython-311.pyc
--rw-r--r--   0        0        0     5865 2023-06-29 21:11:14.960357 bs_testing-0.2.1/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
--rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 bs_testing-0.2.1/blacksmith/scripts/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0     2235 2023-06-30 20:48:27.127415 bs_testing-0.2.1/blacksmith/scripts/cli.py
--rw-r--r--   0        0        0     3784 2023-06-30 08:21:39.811441 bs_testing-0.2.1/blacksmith/scripts/images.py
--rw-r--r--   0        0        0     5345 2023-06-30 20:49:29.575298 bs_testing-0.2.1/blacksmith/scripts/k8s.py
--rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 bs_testing-0.2.1/blacksmith/tools.py
--rw-r--r--   0        0        0      514 2023-06-30 20:56:50.111864 bs_testing-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 bs_testing-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 bs_testing-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 bs_testing-0.3.0/blacksmith/__init__.py
+-rw-r--r--   0        0        0     2452 2023-06-29 21:50:17.114047 bs_testing-0.3.0/blacksmith/agents.py
+-rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 bs_testing-0.3.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
+-rw-r--r--   0        0        0      718 2023-06-29 10:04:18.913031 bs_testing-0.3.0/blacksmith/defaults/prompts.py
+-rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 bs_testing-0.3.0/blacksmith/llm.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 bs_testing-0.3.0/blacksmith/scripts/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 bs_testing-0.3.0/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4117 2023-06-30 08:23:28.853542 bs_testing-0.3.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4352 2023-06-30 08:21:48.445763 bs_testing-0.3.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc
+-rw-r--r--   0        0        0     5865 2023-06-29 21:11:14.960357 bs_testing-0.3.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
+-rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 bs_testing-0.3.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0        0        0     2235 2023-06-30 20:48:27.127415 bs_testing-0.3.0/blacksmith/scripts/cli.py
+-rw-r--r--   0        0        0     3784 2023-06-30 08:21:39.811441 bs_testing-0.3.0/blacksmith/scripts/images.py
+-rw-r--r--   0        0        0     5351 2023-06-30 21:01:20.188340 bs_testing-0.3.0/blacksmith/scripts/k8s.py
+-rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 bs_testing-0.3.0/blacksmith/tools.py
+-rw-r--r--   0        0        0      514 2023-06-30 21:01:35.985452 bs_testing-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 bs_testing-0.3.0/PKG-INFO
```

### Comparing `bs_testing-0.2.1/blacksmith/agents.py` & `bs_testing-0.3.0/blacksmith/agents.py`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc` & `bs_testing-0.3.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/defaults/prompts.py` & `bs_testing-0.3.0/blacksmith/defaults/prompts.py`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/__pycache__/cli.cpython-311.pyc` & `bs_testing-0.3.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/__pycache__/images.cpython-311.pyc` & `bs_testing-0.3.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc` & `bs_testing-0.3.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/__pycache__/main.cpython-311.pyc` & `bs_testing-0.3.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/cli.py` & `bs_testing-0.3.0/blacksmith/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/images.py` & `bs_testing-0.3.0/blacksmith/scripts/images.py`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/blacksmith/scripts/k8s.py` & `bs_testing-0.3.0/blacksmith/scripts/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                                 }
                             ]
                         },
                     },
                 },
             }
             # Add the deployment to the manifest
-            with open(f"manifest.yaml", "a") as file:
+            with open(f"./k8s/manifest.yaml", "a") as file:
                 file.write(yaml.dump(deployment))
                 file.write("---\n")
 
             if spec["type"] == "AGENT":
                 # Build the NodePort service
                 node_port = {
                     "apiVersion": "v1",
```

### Comparing `bs_testing-0.2.1/blacksmith/tools.py` & `bs_testing-0.3.0/blacksmith/tools.py`

 * *Files identical despite different names*

### Comparing `bs_testing-0.2.1/pyproject.toml` & `bs_testing-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs-testing"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["alec <fkalec@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blacksmith"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bs_testing-0.2.1/PKG-INFO` & `bs_testing-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-testing
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: alec
 Author-email: fkalec@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.1.3,<7.0.0)
```

