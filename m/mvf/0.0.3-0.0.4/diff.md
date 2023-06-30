# Comparing `tmp/mvf-0.0.3.tar.gz` & `tmp/mvf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.3.tar", last modified: Tue Jun 27 14:42:50 2023, max compression
+gzip compressed data, was "mvf-0.0.4.tar", last modified: Fri Jun 30 16:22:11 2023, max compression
```

## Comparing `mvf-0.0.3.tar` & `mvf-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.808687 mvf-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-27 14:42:47.000000 mvf-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3135 2023-06-27 14:42:50.808687 mvf-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-27 14:42:47.000000 mvf-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.801687 mvf-0.0.3/mvf/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.803687 mvf-0.0.3/mvf/cli/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.803687 mvf-0.0.3/mvf/dag/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/dag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7144 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/dag/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/process/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/process/validate_model_r.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/test/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.804687 mvf-0.0.3/mvf/test/integration/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.806687 mvf-0.0.3/mvf/test/integration/config/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/mvf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/config/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.807687 mvf-0.0.3/mvf/test/integration/process/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-27 14:42:47.000000 mvf-0.0.3/mvf/test/integration/process/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.802687 mvf-0.0.3/mvf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3135 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1199 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-27 14:42:50.000000 mvf-0.0.3/mvf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 14:42:50.808687 mvf-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-06-27 14:42:47.000000 mvf-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 14:42:50.808687 mvf-0.0.3/test/
--rw-rw-rw-   0 root         (0) root         (0)     5868 2023-06-27 14:42:47.000000 mvf-0.0.3/test/test_build_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-27 14:42:47.000000 mvf-0.0.3/test/test_python_testing_framework.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-30 16:22:07.000000 mvf-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-06-30 16:22:11.451746 mvf-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-30 16:22:07.000000 mvf-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.444746 mvf-0.0.4/mvf/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.446746 mvf-0.0.4/mvf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.446746 mvf-0.0.4/mvf/dag/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/dag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11252 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/dag/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.447746 mvf-0.0.4/mvf/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.448746 mvf-0.0.4/mvf/integration/config/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/config/validate_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/mvf_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.449746 mvf-0.0.4/mvf/integration/process/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/integration/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/mvf/process/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3619 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-30 16:22:07.000000 mvf-0.0.4/mvf/process/validate_model_r.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.445746 mvf-0.0.4/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-30 16:22:11.000000 mvf-0.0.4/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 16:22:11.451746 mvf-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-30 16:22:07.000000 mvf-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 16:22:11.451746 mvf-0.0.4/test/
+-rw-rw-rw-   0 root         (0) root         (0)     6632 2023-06-30 16:22:07.000000 mvf-0.0.4/test/test_build_dag.py
```

### Comparing `mvf-0.0.3/LICENSE` & `mvf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mvf-0.0.3/PKG-INFO` & `mvf-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,29 @@
-Metadata-Version: 2.1
-Name: mvf
-Version: 0.0.3
-Summary: A package implementing a supervised learning model validation framework.
-Home-page: UNKNOWN
-Author: Tom Kim
-Author-email: tom.kim@certus-tech.com
-License: UNKNOWN
-Keywords: python,R,machine learning,validation,framework
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: License :: Free For Educational Use
-Classifier: Operating System :: Unix
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
+Test change on dev branch
+
+Test change on dev-tk branch
+
 ## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Main features
 
-
+* Automates the supervised ML workflow with simple configuration.
+* R and Python models can be plugged in easily.
 
 ## For developers
 
 ### Dependencies
 
-R dependencies are managed using `renv`. Spin up a Python Virtual Environment
+You need Python>=3.9 and R>=4.0. 
 
-Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
+Additionally, you must have a working installation of the `R6`, [`IRkernel`](https://github.com/IRkernel/IRkernel) and `arrow` R packages to leverage the R/Python interoperability.
 
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
@@ -73,9 +59,7 @@
 
 The version stored in the `version` file must be incremented for a deployment of the package to be successful.
 
 ### Documentation
 
 This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory.
 
-
-
```

### Comparing `mvf-0.0.3/README.md` & `mvf-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,48 @@
+Metadata-Version: 2.1
+Name: mvf
+Version: 0.0.4
+Summary: A package implementing a supervised learning model validation framework.
+Home-page: UNKNOWN
+Author: Tom Kim
+Author-email: tom.kim@certus-tech.com
+License: UNKNOWN
+Keywords: python,R,machine learning,validation,framework
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Framework :: Jupyter
+Classifier: License :: Free For Educational Use
+Classifier: Operating System :: Unix
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
+Test change on dev branch
+
+Test change on dev-tk branch
+
 ## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Main features
 
-
+* Automates the supervised ML workflow with simple configuration.
+* R and Python models can be plugged in easily.
 
 ## For developers
 
 ### Dependencies
 
-R dependencies are managed using `renv`. Spin up a Python Virtual Environment
+You need Python>=3.9 and R>=4.0. 
 
-Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
+Additionally, you must have a working installation of the `R6`, [`IRkernel`](https://github.com/IRkernel/IRkernel) and `arrow` R packages to leverage the R/Python interoperability.
 
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
@@ -54,7 +78,9 @@
 
 The version stored in the `version` file must be incremented for a deployment of the package to be successful.
 
 ### Documentation
 
 This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory.
 
+
+
```

### Comparing `mvf-0.0.3/mvf/cli/cli.py` & `mvf-0.0.4/mvf/cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import click
 import os
-import yaml
 import sys
 from mvf.cli import cli
-from mvf.dag.builder import build_dag
-from mvf.test.integration.config import mvf as mvf_config
+from mvf.cli import utils
+from mvf.dag.builder import DagBuilder
 
 
 def cmd_router():
     '''
     CLI entry point.
     '''
     # parse the command
@@ -29,36 +28,25 @@
 
 
 ### CLI COMMANDS ###
 
 
 def run():
     # load project config
-    config = load_config(os.path.join(os.getcwd(), 'mvf_conf.yaml'))
-    dag = build_dag(config)
+    config = utils.load_config(os.path.join(os.getcwd(), 'mvf_conf.yaml'))
+    # build dag from config
+    dag_builder = DagBuilder(config, output_dir='output')
+    dag_builder.build()
     click.echo('Running MVF project...')
-    dag.build()
+    # access the built dag and execute it
+    dag_builder.dag.build()
 
 
 def plot():
     # load project config
-    config = load_config(os.path.join(os.getcwd(), 'mvf_conf.yaml'))
-    dag = build_dag(config)
+    config = utils.load_config(os.path.join(os.getcwd(), 'mvf_conf.yaml'))
+    # build dag from config
+    dag_builder = DagBuilder(config, output_dir='output')
+    dag_builder.build()
     click.echo('Plotting workflow...')
-    dag.plot(os.path.join('output', 'pipeline.html'))
-
-
-### UTILITY FUNCTIONS
-
-
-def load_config(path):
-    # open the mvf config file
-    try:
-        with open(path, 'r') as f:
-            config = yaml.safe_load(f)
-    except FileNotFoundError:
-        raise Exception('No `mvf_conf.yaml` found in the working directory.')
-    else:
-        # validate the config against the schema
-        click.echo('Validating config...')
-        mvf_config.check_config(config)
-        return config
+    # access the built dag and plot it
+    dag_builder.dag.plot(os.path.join('output', 'pipeline.html'))
```

### Comparing `mvf-0.0.3/mvf/process/split_data.py` & `mvf-0.0.4/mvf/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.3/mvf/test/integration/config/fit_model.py` & `mvf-0.0.4/mvf/integration/config/fit_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import rpy2.robjects as robjects
 from rpy2.robjects import pandas2ri
 import rpy2_r6.r6b as r6b
 
 
 def fit_model_params(product: dict, params: dict) -> None:
     # check params for fit_model tasks
-    assert 'model' in product, 'The \'model\' product must be defined.'
     assert 'model_name' in params, 'The \'model_name\' parameter must be defined.'
     assert 'split_type' in params, 'The \'split_type\' parameter must be defined.'
+    if params['split_type'] == 'train_test':
+        assert 'model' in product, 'The \'model\' product must be defined.'
+    elif params['split_type'] == 'k_fold':
+        assert 'n_folds' in params, 'For a K fold split, the n_folds must be defined.'
+        n_folds = params['n_folds']
+        for i in range(1, n_folds+1):
+            assert f'model_{i}' in product, f'The {i}-th model product must be defined.'
 
 
 def fit_model_r(product: dict, params: dict) -> None:
     # check params
     fit_model_params(product, params)
     # check that the correct model class is available
     r = robjects.r
@@ -46,11 +52,11 @@
 if __name__ == '__main__':
     product = {
         'nb': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2.ipynb'),
         'nb_html': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2.html'),
         'model': File('/home/tom/projects/model-validation-framework/examples/project1/output/fit_model_2')
     }
     params = {
-      'model_name': 'BayesReg',
+      'model_name': 'r_pois_reg',
       'split_type': 'train_test'
     }
     fit_model_r(product, params)
```

### Comparing `mvf-0.0.3/mvf/test/integration/config/mvf.py` & `mvf-0.0.4/mvf/integration/mvf_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from schema import Schema, Or, Optional, And
 
 
 def check_config(config):
     # schema for mvf_conf.yaml
     mvf_conf = Schema(
         {
-            'project_name': str,
             'data': {
                 'source': str,
                 'split': Or('train_test', 'k_fold'),
                 Optional('test_size'): lambda x: 0 <= x <= 1,
                 Optional('n_folds'): And(int, lambda x: x > 0),
             },
             'models': [
```

### Comparing `mvf-0.0.3/mvf/test/integration/config/split_data.py` & `mvf-0.0.4/mvf/integration/config/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.3/mvf/test/integration/process/fit_model.py` & `mvf-0.0.4/mvf/integration/process/fit_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,57 @@
-import pickle
 import rpy2.robjects as robjects
 from rpy2.robjects import pandas2ri
 import rpy2_r6.r6b as r6b
 
 def fit_model_py(product: dict, params: dict) -> None:
-    # load model(s)
-    with open(product['model'], 'rb') as f:
-        model = pickle.load(f)
+    import models
+    # get model class
+    model_class = getattr(models, params['model_name'])
     # different tests by split type
     if params['split_type'] == 'train_test':
+        # load model
+        model = model_class()
+        model.load(product['model'])
         # check the model has a predict method
         assert hasattr(model, 'predict'), f'The model saved at {product["model"]} must have a predict() method.'
+        assert callable(getattr(model, 'predict')), f'The model saved at {product["model"]} must have a predict() method. The class\' predict attribute is not currently callable.'
     elif params['split_type'] == 'k_fold':
-        raise NotImplementedError(f"The {params['split_type']} implementation is not tested. This is unacceptable.")
+        for i in range(1, params['n_folds'] + 1):
+            model = model_class()
+            model.load(product[f'model_{i}'])
+            # check the model has a predict method
+            assert hasattr(model, 'predict'), f'The model saved at {product["model"]} must have a predict() method.'
+            assert callable(getattr(model, 'predict')), f'The model saved at {product["model"]} must have a predict() method. The class\' predict attribute is not currently callable.'
     else:
         raise NotImplementedError(f"The {params['split_type']} implementation is not tested. This is unacceptable.")
 
 def fit_model_r(product: dict, params: dict) -> None:
     # load model
     r = robjects.r
     r.source('models.R')
     model_class = r6b.R6DynamicClassGenerator(r[params['model_name']])
-    model = model_class.new()
-    assert hasattr(model, 'predict'), f'The class {params["model_name"]} must have a predict() method. The class does not currently have a predict attribute.'
-    assert callable(getattr(model, 'predict')), f'The class {params["model_name"]} must have a predict() method. The class\' predict attribute is not currently callable.'
-
 
+    # different tests by split type
+    if params['split_type'] == 'train_test':
+        # load model
+        model = model_class.new()
+        model.load(str(product['model']))
+        # check the model has a predict method
+        assert hasattr(model, 'predict'), f'The model saved at {product["model"]} must have a predict() method.'
+        assert callable(getattr(model, 'predict')), f'The model saved at {product["model"]} must have a predict() method. The class\' predict attribute is not currently callable.'
+    elif params['split_type'] == 'k_fold':
+        for i in range(1, params['n_folds'] + 1):
+            model = model_class.new()
+            model.load(str(product[f'model_{i}']))
+            # check the model has a predict method
+            assert hasattr(model, 'predict'), f'The model saved at {product["model"]} must have a predict() method.'
+            assert callable(getattr(model, 'predict')), f'The model saved at {product["model"]} must have a predict() method. The class\' predict attribute is not currently callable.'
+    else:
+        raise NotImplementedError(f"The {params['split_type']} implementation is not tested. This is unacceptable.")
+    
 
 
 
 #### example code for debugging a test
 # ensure correct data is in locations specified
 # run test using
 #
```

### Comparing `mvf-0.0.3/mvf/test/integration/process/split_data.py` & `mvf-0.0.4/mvf/integration/process/split_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,30 +9,35 @@
         y_test = feather.read_dataframe(product['test_y_data'])
 
         assert X_train.shape[0] == y_train.shape[0], f'X and y train data should have the same number of instances. Currently {X_train.shape[0]} and {y_train.shape[0]}'
         assert X_test.shape[0] == y_test.shape[0], f'X and y test data should have the same number of instances. Currently {X_test.shape[0]} and {y_test.shape[0]}'
         assert X_train.shape[1] == X_test.shape[1], f'X train and test data should have the same number of features. Currently {X_train.shape[1]} and {X_test.shape[1]}'
         assert y_train.shape[1] == y_test.shape[1], f'y train and test data should have the same number of features. Currently {y_train.shape[1]} and {y_test.shape[1]}'
         assert (X_test.shape[0] / (X_test.shape[0] + X_train.shape[0])) - params['test_size'] < 1e-4, 'The actual test size differs too much from the test_size parameter. If you have a very small dataset, choose an appropriate test size for the number of data points.'
-
-        # check that no instances are shared across test and train?
+        assert (X_train.index == y_train.index).all(), 'The indices for X and y training data do not match up.'
+        assert (X_test.index == y_test.index).all(), 'The indices for X and y testing data do not match up.'
+        assert len(set(X_train.index).intersection(set(X_test.index))) == 0, 'The train and test indices are not distinct.'
     elif params['split_type'] == 'k_fold':
         X_data = []
         y_data = []
         n_instances = set()
+        indices = []
         for i in range(1, params['n_folds'] + 1):
             fold_i_X_data = feather.read_dataframe(product[f'fold_{i}_X_data'])
             fold_i_y_data = feather.read_dataframe(product[f'fold_{i}_y_data'])
 
             assert fold_i_X_data.shape[0] == fold_i_y_data.shape[0], f'X and y data from a particular fold should have the same number of instances. Currently {fold_i_X_data.shape[0]} and {fold_i_y_data.shape[0]} for the {i}th fold.'
-
+            assert (fold_i_X_data.index == fold_i_y_data.index).all(), f'The indices for X and y from the {i}th fold do not match up.'
+            
             X_data.append(fold_i_X_data)
             y_data.append(fold_i_y_data)
             n_instances.add(fold_i_X_data.shape[0])
+            indices.append(set(fold_i_X_data.index))
 
         assert len(n_instances) <= 2 and -1 <= list(n_instances)[0] - list(n_instances)[-1] <= 1, f'The number of instances in each fold must be as equal as possible. The number of instances in folds are currently {n_instances}.'
-        
+        assert len(set.intersection(*indices)) == 0, 'The fold indices are not distinct.'
+
         for i in range(params['n_folds'] - 1):
             assert X_data[i].shape[1] == X_data[i+1].shape[1], f'X data should have the same number of features across all folds. {i}th fold has {X_data[i].shape[1]} features but {i+1}th fold has {X_data[i+1].shape[1]} features.'
             assert y_data[i].shape[1] == y_data[i+1].shape[1], f'y data should have the same number of features across all folds. {i}th fold has {y_data[i].shape[1]} features but {i+1}th fold has {y_data[i+1].shape[1]} features.'
     else:
         raise NotImplementedError(f"The {params['split_type']} implementation is not tested. This is unacceptable.")
```

### Comparing `mvf-0.0.3/mvf.egg-info/PKG-INFO` & `mvf-0.0.4/mvf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
@@ -15,29 +15,34 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 MVF stands for model validation framework. MVF is a pluggable ML/statistical modelling framework that allows for the easy comparison of models implemented in Python and R. Write simple wrapper classes for your models and compare their performance on a particular dataset.
 
+Test change on dev branch
+
+Test change on dev-tk branch
+
 ## Getting started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Main features
 
-
+* Automates the supervised ML workflow with simple configuration.
+* R and Python models can be plugged in easily.
 
 ## For developers
 
 ### Dependencies
 
-R dependencies are managed using `renv`. Spin up a Python Virtual Environment
+You need Python>=3.9 and R>=4.0. 
 
-Python dependencies are specified by `requirements.txt`. This file is generated from `requirements.in` by running `python3 -m piptools compile`.
+Additionally, you must have a working installation of the `R6`, [`IRkernel`](https://github.com/IRkernel/IRkernel) and `arrow` R packages to leverage the R/Python interoperability.
 
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
```

### Comparing `mvf-0.0.3/mvf.egg-info/SOURCES.txt` & `mvf-0.0.4/mvf.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 mvf.egg-info/SOURCES.txt
 mvf.egg-info/dependency_links.txt
 mvf.egg-info/entry_points.txt
 mvf.egg-info/requires.txt
 mvf.egg-info/top_level.txt
 mvf/cli/__init__.py
 mvf/cli/cli.py
+mvf/cli/utils.py
 mvf/dag/__init__.py
 mvf/dag/builder.py
+mvf/integration/__init__.py
+mvf/integration/mvf_config.py
+mvf/integration/config/__init__.py
+mvf/integration/config/fit_model.py
+mvf/integration/config/predict_model.py
+mvf/integration/config/preprocess_data.py
+mvf/integration/config/split_data.py
+mvf/integration/config/validate.py
+mvf/integration/config/validate_model.py
+mvf/integration/process/__init__.py
+mvf/integration/process/fit_model.py
+mvf/integration/process/predict_model.py
+mvf/integration/process/preprocess_data.py
+mvf/integration/process/split_data.py
+mvf/integration/process/validate.py
+mvf/integration/process/validate_model.py
 mvf/process/__init__.py
 mvf/process/fit_model.py
 mvf/process/predict_model.py
 mvf/process/split_data.py
 mvf/process/validate.py
 mvf/process/validate_model_r.py
-mvf/test/__init__.py
-mvf/test/integration/__init__.py
-mvf/test/integration/config/__init__.py
-mvf/test/integration/config/fit_model.py
-mvf/test/integration/config/mvf.py
-mvf/test/integration/config/predict_model.py
-mvf/test/integration/config/preprocess_data.py
-mvf/test/integration/config/split_data.py
-mvf/test/integration/config/validate.py
-mvf/test/integration/config/validate_model.py
-mvf/test/integration/process/__init__.py
-mvf/test/integration/process/fit_model.py
-mvf/test/integration/process/predict_model.py
-mvf/test/integration/process/preprocess_data.py
-mvf/test/integration/process/split_data.py
-mvf/test/integration/process/validate.py
-mvf/test/integration/process/validate_model.py
-test/test_build_dag.py
-test/test_python_testing_framework.py
+test/test_build_dag.py
```

### Comparing `mvf-0.0.3/setup.py` & `mvf-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,14 @@
     packages=find_packages(
         exclude=[
             'test*',
             'documentation*',
             'examples*',
         ],
     ),
-    # package_dir={
-    #     '': 'mvf'
-    # },
     install_requires=[
         'click',
         'feather-format',
         'pandas',
         'ploomber',
         'rpy2',
         'rpy2-r6',
```

### Comparing `mvf-0.0.3/test/test_build_dag.py` & `mvf-0.0.4/test/test_build_dag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-from mvf.dag.builder import build_dag
-from mvf.cli.cli import load_config
+from mvf.dag.builder import DagBuilder
+from mvf.cli.utils import load_config
 from ploomber.spec import DAGSpec
 import os
+import pytest
 
-# def test_build_dag_smoke():
-#     testing_dir = os.getcwd()
-#     os.chdir('test/test_resources/test_project_1')
-
-#     try:
-#         # load config
-#         config = load_config('mvf_conf.yaml')
-#         # build dag from config
-#         dag = build_dag(config)
-#         dag.build()
-    
-#     finally:
-#         os.chdir(testing_dir)
-
-def test_build_dag():
+@pytest.mark.parametrize(
+    ('test_project_path'),
+    [
+        ('test/test_resources/test_project_1'),
+        ('test/test_resources/test_project_2')
+    ]
+)
+
+
+def test_build_dag(test_project_path):
+    '''
+    Tests
+
+        * Python `preprocess_data` template
+        * `train_test` parameter on the `split_data` process
+    '''
     testing_dir = os.getcwd()
-    os.chdir('test/test_resources/test_project_1')
+    os.chdir(test_project_path)
 
     try:
         # load in output dag
         spec = DAGSpec('pipeline.yaml')
         expected_dag = spec.to_dag()
 
         # load config
         config = load_config('mvf_conf.yaml')
         # build dag from config
-        dag = build_dag(config)
+        dag_builder = DagBuilder(config)
+        dag_builder.build()
+        dag = dag_builder.dag
 
         ###
         ### TESTING ###
         ###
         assert dag.name == expected_dag.name
 
         ### preprocess task ###
@@ -55,18 +59,24 @@
         ### split task ###
         split = dag.get('split_data')
         expected = expected_dag.get('split_data')
 
         # source
         assert split.source.loc == expected.source.loc
         # product
-        assert split.product['train_X_data'] == expected.product['train_X_data']
-        assert split.product['test_X_data'] == expected.product['test_X_data']
-        assert split.product['train_y_data'] == expected.product['train_y_data']
-        assert split.product['test_y_data'] == expected.product['test_y_data']
+        if config['data']['split'] == 'train_test':
+            assert split.product['train_X_data'] == expected.product['train_X_data']
+            assert split.product['test_X_data'] == expected.product['test_X_data']
+            assert split.product['train_y_data'] == expected.product['train_y_data']
+            assert split.product['test_y_data'] == expected.product['test_y_data']
+        elif config['data']['split'] == 'k_fold':
+            n_folds = config['data']['n_folds']
+            for i in range(1, n_folds + 1):
+                assert split.product[f'fold_{i}_X_data'] == expected.product[f'fold_{i}_X_data']
+                assert split.product[f'fold_{i}_y_data'] == expected.product[f'fold_{i}_y_data']
         # params
         assert split.params == expected.params
         # upstream
         assert split.upstream.keys() == expected.upstream.keys()
         # name
         assert split.name == expected.name
         # hooks
@@ -80,15 +90,20 @@
             ### fit task ###
             fit = dag.get(model_name + '_fit')
             expected = expected_dag.get(model_name + '_fit')
 
             # source
             assert fit.source.loc == expected.source.loc
             # product
-            assert fit.product['model'] == expected.product['model']
+            if config['data']['split'] == 'train_test':
+                assert fit.product['model'] == expected.product['model']
+            elif config['data']['split'] == 'k_fold':
+                n_folds = config['data']['n_folds']
+                for i in range(1, n_folds + 1):
+                    assert fit.product[f'model_{i}'] == expected.product[f'model_{i}']
             # params
             assert fit.params == expected.params
             # upstream
             assert fit.upstream.keys() == expected.upstream.keys()
             # name
             assert fit.name == expected.name
             # hooks
@@ -125,30 +140,31 @@
             # upstream
             assert predict.upstream.keys() == expected.upstream.keys()
             # name
             assert predict.name == expected.name
             # hooks
             assert predict.on_render.__name__ == expected.on_render.callable.__name__
             assert predict.on_finish.__name__ == expected.on_finish.callable.__name__
-            if model['lang'] == 'R':
-                # params
-                assert predict.params == expected.params
+            # params
+            assert predict.params == expected.params
         
         ### validate task ###
         validate = dag.get('validate')
         expected = expected_dag.get('validate')
 
         # source
         assert validate.source.loc.resolve() == expected.source.loc.resolve()
         # product
         assert validate.product['nb'] == expected.product['nb']
         # upstream
         assert validate.upstream.keys() == expected.upstream.keys(), f'Upstream tasks are {validate.upstream.keys()}. Should be {expected.upstream.keys()}.'
+        # params
+        assert validate.params == expected.params
         # name
         assert validate.name == expected.name
         # hooks
         assert validate.on_render.__name__ == expected.on_render.callable.__name__
         assert validate.on_finish.__name__ == expected.on_finish.callable.__name__
 
     finally:
         os.chdir(testing_dir)
-    
+
```

