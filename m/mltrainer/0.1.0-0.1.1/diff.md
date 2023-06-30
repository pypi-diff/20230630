# Comparing `tmp/mltrainer-0.1.0.tar.gz` & `tmp/mltrainer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltrainer-0.1.0.tar", last modified: Thu Jun 29 21:33:49 2023, max compression
+gzip compressed data, was "mltrainer-0.1.1.tar", last modified: Fri Jun 30 09:52:24 2023, max compression
```

## Comparing `mltrainer-0.1.0.tar` & `mltrainer-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       50 2023-06-29 21:33:02.956591 mltrainer-0.1.0/README.md
--rw-r--r--   0        0        0      181 2023-06-29 21:26:09.334571 mltrainer-0.1.0/mltrainer/__init__.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.0/mltrainer/imagemodels.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.0/mltrainer/metrics.py
--rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.0/mltrainer/rnn_models.py
--rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.0/mltrainer/settings.py
--rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.0/mltrainer/tokenizer.py
--rw-r--r--   0        0        0     8808 2023-06-29 21:24:17.208433 mltrainer-0.1.0/mltrainer/trainer.py
--rw-r--r--   0        0        0     2489 2023-06-29 21:20:14.997117 mltrainer-0.1.0/mltrainer/vae.py
--rw-r--r--   0        0        0     1412 2023-06-29 21:33:49.829347 mltrainer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 mltrainer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.1/README.md
+-rw-r--r--   0        0        0      177 2023-06-30 09:46:36.899325 mltrainer-0.1.1/mltrainer/__init__.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.1/mltrainer/imagemodels.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.1/mltrainer/metrics.py
+-rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.1/mltrainer/rnn_models.py
+-rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.1/mltrainer/settings.py
+-rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.1/mltrainer/tokenizer.py
+-rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.1/mltrainer/trainer.py
+-rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.1/mltrainer/vae.py
+-rw-r--r--   0        0        0     1665 2023-06-30 09:52:24.201118 mltrainer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 mltrainer-0.1.1/PKG-INFO
```

### Comparing `mltrainer-0.1.0/mltrainer/imagemodels.py` & `mltrainer-0.1.1/mltrainer/imagemodels.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/mltrainer/metrics.py` & `mltrainer-0.1.1/mltrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/mltrainer/rnn_models.py` & `mltrainer-0.1.1/mltrainer/rnn_models.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/mltrainer/settings.py` & `mltrainer-0.1.1/mltrainer/settings.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/mltrainer/tokenizer.py` & `mltrainer-0.1.1/mltrainer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/mltrainer/trainer.py` & `mltrainer-0.1.1/mltrainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # needed to make summarywriter load without error
 import torch
 from loguru import logger
 from ray import tune
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 
-from deeptoolkit.settings import ReportTypes, TrainerSettings
+from mltrainer import ReportTypes, TrainerSettings
 
 
 def write_gin(dir: Path, txt: str) -> None:
     path = dir / "saved_config.gin"
     with open(path, "w") as file:
         file.write(txt)
```

### Comparing `mltrainer-0.1.0/mltrainer/vae.py` & `mltrainer-0.1.1/mltrainer/vae.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.0/pyproject.toml` & `mltrainer-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 [project]
 name = "mltrainer"
-version = "0.1.0"
+version = "0.1.1"
 description = "toolkit for training pytorch models"
 authors = [
     { name = "R.Grouls", email = "Raoul.Grouls@han.nl" },
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
-]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
@@ -36,14 +24,35 @@
 tuning = [
     "mlflow>=2.4.1",
     "bayesian-optimization>=1.4.3",
     "hpbandster>=0.7.4",
     "configspace>=0.7.1",
 ]
 
+[tools.urls]
+GitHub = "https://github.com/raoulg/mltrainer"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Programming Language :: Python :: 3.10",
+    "Typing :: Typed",
+]
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
+]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.flake8]
```

### Comparing `mltrainer-0.1.0/PKG-INFO` & `mltrainer-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 Metadata-Version: 2.1
 Name: mltrainer
-Version: 0.1.0
+Version: 0.1.1
 Summary: toolkit for training pytorch models
 Author-Email: R.Grouls <Raoul.Grouls@han.nl>
 License: MIT
 Requires-Python: >=3.10
-Requires-Dist: gin-config>=0.5.0
-Requires-Dist: numpy>=1.25.0
-Requires-Dist: torch>=2.0.1
-Requires-Dist: loguru>=0.7.0
-Requires-Dist: ray[tune]>=2.5.1
-Requires-Dist: tqdm>=4.65.0
-Requires-Dist: pydantic>=1.10.9
-Requires-Dist: torchvision>=0.15.2
-Requires-Dist: torchtext>=0.15.2
-Requires-Dist: torch-tb-profiler>=0.4.1
+Provides-Extra: lint
+Provides-Extra: tuning
 Requires-Dist: Flake8-pyproject>=1.2.3; extra == "lint"
 Requires-Dist: pep8-naming>=0.13.3; extra == "lint"
 Requires-Dist: flake8-annotations>=3.0.1; extra == "lint"
 Requires-Dist: black>=23.3.0; extra == "lint"
 Requires-Dist: flake8>=6.0.0; extra == "lint"
 Requires-Dist: isort>=5.12.0; extra == "lint"
 Requires-Dist: mypy>=1.4.1; extra == "lint"
 Requires-Dist: mlflow>=2.4.1; extra == "tuning"
 Requires-Dist: bayesian-optimization>=1.4.3; extra == "tuning"
 Requires-Dist: hpbandster>=0.7.4; extra == "tuning"
 Requires-Dist: configspace>=0.7.1; extra == "tuning"
-Provides-Extra: lint
-Provides-Extra: tuning
 Description-Content-Type: text/markdown
 
 # ml-trainer
 
 toolkit for training pytorch models
```

