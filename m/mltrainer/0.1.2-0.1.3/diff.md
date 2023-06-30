# Comparing `tmp/mltrainer-0.1.2.tar.gz` & `tmp/mltrainer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltrainer-0.1.2.tar", last modified: Fri Jun 30 09:58:21 2023, max compression
+gzip compressed data, was "mltrainer-0.1.3.tar", last modified: Fri Jun 30 10:16:39 2023, max compression
```

## Comparing `mltrainer-0.1.2.tar` & `mltrainer-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.2/README.md
--rw-r--r--   0        0        0      177 2023-06-30 09:58:12.815609 mltrainer-0.1.2/mltrainer/__init__.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.2/mltrainer/imagemodels.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.2/mltrainer/metrics.py
--rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.2/mltrainer/rnn_models.py
--rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.2/mltrainer/settings.py
--rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.2/mltrainer/tokenizer.py
--rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.2/mltrainer/trainer.py
--rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.2/mltrainer/vae.py
--rw-r--r--   0        0        0     1651 2023-06-30 09:58:21.490172 mltrainer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 mltrainer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.3/README.md
+-rw-r--r--   0        0        0      177 2023-06-30 10:15:32.147818 mltrainer-0.1.3/mltrainer/__init__.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.3/mltrainer/imagemodels.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.3/mltrainer/metrics.py
+-rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.3/mltrainer/rnn_models.py
+-rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.3/mltrainer/settings.py
+-rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.3/mltrainer/tokenizer.py
+-rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.3/mltrainer/trainer.py
+-rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.3/mltrainer/vae.py
+-rw-r--r--   0        0        0     1643 2023-06-30 10:16:39.356120 mltrainer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 mltrainer-0.1.3/PKG-INFO
```

### Comparing `mltrainer-0.1.2/mltrainer/imagemodels.py` & `mltrainer-0.1.3/mltrainer/imagemodels.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/metrics.py` & `mltrainer-0.1.3/mltrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/rnn_models.py` & `mltrainer-0.1.3/mltrainer/rnn_models.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/settings.py` & `mltrainer-0.1.3/mltrainer/settings.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/tokenizer.py` & `mltrainer-0.1.3/mltrainer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/trainer.py` & `mltrainer-0.1.3/mltrainer/trainer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/mltrainer/vae.py` & `mltrainer-0.1.3/mltrainer/vae.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.2/pyproject.toml` & `mltrainer-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 [project]
 name = "mltrainer"
-version = "0.1.2"
+version = "0.1.3"
 description = "toolkit for training pytorch models"
 authors = [
     { name = "R.Grouls", email = "Raoul.Grouls@han.nl" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+dependencies = [
+    "gin-config>=0.5.0",
+    "numpy>=1.25.0",
+    "torch>=2.0.1",
+    "loguru>=0.7.0",
+    "ray[tune]>=2.5.1",
+    "tqdm>=4.65.0",
+    "pydantic>=1.10.9",
+    "torchvision>=0.15.2",
+    "torchtext>=0.15.2",
+    "torch-tb-profiler>=0.4.1",
+    "mlflow>=2.4.1",
+    "hpbandster>=0.7.4",
+    "configspace>=0.7.1",
+    "bayesian-optimization>=1.4.3",
+]
 
 [project.license]
 text = "MIT"
 
 [project.pdm.dev-dependencies]
 lint = [
     "Flake8-pyproject>=1.2.3",
@@ -23,33 +39,17 @@
 ]
 
 [tools.urls]
 GitHub = "https://github.com/raoulg/mltrainer"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python",
     "Typing :: Typed",
 ]
-dependencies = [
-    "gin-config>=0.5.0",
-    "numpy>=1.25.0",
-    "torch>=2.0.1",
-    "loguru>=0.7.0",
-    "ray[tune]>=2.5.1",
-    "tqdm>=4.65.0",
-    "pydantic>=1.10.9",
-    "torchvision>=0.15.2",
-    "torchtext>=0.15.2",
-    "torch-tb-profiler>=0.4.1",
-    "mlflow>=2.4.1",
-    "bayesian-optimization>=1.4.3",
-    "hpbandster>=0.7.4",
-    "configspace>=0.7.1",
-]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

