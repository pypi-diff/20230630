# Comparing `tmp/spark-board-0.0.6.tar.gz` & `tmp/spark-board-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-a3bvgb9l/spark-board-0.0.6.tar", last modified: Mon Jun 26 03:20:09 2023, max compression
+gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-ez07i878/spark-board-0.0.7.tar", last modified: Thu Jun 29 23:33:21 2023, max compression
```

## Comparing `spark-board-0.0.6.tar` & `spark-board-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 03:19:54.000000 spark-board-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-26 03:20:09.000000 spark-board-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-26 03:19:54.000000 spark-board-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 03:19:54.000000 spark-board-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:20:09.000000 spark-board-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-26 03:19:54.000000 spark-board-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board/plan_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/dag_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/py4j_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/transformation_node_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-26 03:19:54.000000 spark-board-0.0.6/spark_board/plan_extractor/transformations_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/filter-baaad4cd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/group-daa83ef9.svg
--rw-r--r--   0 runner    (1001) docker     (123)   471474 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/index-946b5dbe.js
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/index-c952fe44.css
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/join-cbb2d651.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33550 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/logo-c54f7abe.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/project-5fbb0573.svg
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/sort-7864cb74.svg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/table-1441493a.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/assets/union-e6640cdd.png
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 03:20:03.000000 spark-board-0.0.6/spark_board/ui/assets/upload-4f5382f0.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 03:20:03.000000 spark-board-0.0.6/spark_board/ui/assets/upper-limit-2af54b76.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-26 03:20:02.000000 spark-board-0.0.6/spark_board/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 03:20:09.000000 spark-board-0.0.6/spark_board.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:20:09.000000 spark-board-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-26 03:19:54.000000 spark-board-0.0.6/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 23:33:03.000000 spark-board-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-29 23:33:21.000000 spark-board-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-29 23:33:12.000000 spark-board-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 23:33:03.000000 spark-board-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:33:21.000000 spark-board-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-29 23:33:03.000000 spark-board-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board/plan_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/dag_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/py4j_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/transformation_node_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-29 23:33:03.000000 spark-board-0.0.7/spark_board/plan_extractor/transformations_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-29 23:33:12.000000 spark-board-0.0.7/spark_board/ui/assets/filter-baaad4cd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/assets/group-daa83ef9.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   471474 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/assets/index-946b5dbe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/assets/index-c952fe44.css
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/assets/join-cbb2d651.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33550 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/logo-c54f7abe.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/assets/project-5fbb0573.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/sort-7864cb74.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/table-1441493a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/union-e6640cdd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/upload-4f5382f0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 23:33:14.000000 spark-board-0.0.7/spark_board/ui/assets/upper-limit-2af54b76.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-29 23:33:13.000000 spark-board-0.0.7/spark_board/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 23:33:21.000000 spark-board-0.0.7/spark_board.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:33:21.000000 spark-board-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-29 23:33:03.000000 spark-board-0.0.7/tests/test_integration.py
```

### Comparing `spark-board-0.0.6/LICENSE` & `spark-board-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/PKG-INFO` & `spark-board-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interactive visualization of Spark jobs
+Home-page: https://github.com/alijdens/spark-board
+Author: Axel Lijdens, Ezequiel Werner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `spark-board`: interactive PySpark dataframes visualization
 
 `spark-board` provides an interactive way to analize PySpark data frame execution plans as a static website displaying the transformations DAG.
 
-Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](./tests/examples/)).
+Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](https://github.com/alijdens/spark-board/tree/v0.0.7/tests/examples/)).
 
 ## Usage
 
 `spark-board` takes a PySpark data frame and inspects the operations to build the DAG. This usually is the final step of a PySpark script, right before writing it to disk.
 
 ### Install `spark-board`
 
@@ -43,8 +45,8 @@
 
 and that's it! `spark-board` will generate a static website in the defined `output_dir` folder. You can now serve the website using any web server and inspect the operations.
 
 You can check out the avaialble default settings [here](https://github.com/alijdens/spark-board/blob/main/spark_board/default_settings.py).
 
 ### Serving
 
-`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](./.github/workflows/deploy-examples.yml) in this repository).
+`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](https://github.com/alijdens/spark-board/tree/v0.0.7/.github/workflows/deploy-examples.yml) in this repository).
```

### Comparing `spark-board-0.0.6/README.md` & `spark-board-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # `spark-board`: interactive PySpark dataframes visualization
 
 `spark-board` provides an interactive way to analize PySpark data frame execution plans as a static website displaying the transformations DAG.
 
-Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](./tests/examples/)).
+Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](https://github.com/alijdens/spark-board/tree/v0.0.7/tests/examples/)).
 
 ## Usage
 
 `spark-board` takes a PySpark data frame and inspects the operations to build the DAG. This usually is the final step of a PySpark script, right before writing it to disk.
 
 ### Install `spark-board`
 
@@ -32,8 +32,8 @@
 
 and that's it! `spark-board` will generate a static website in the defined `output_dir` folder. You can now serve the website using any web server and inspect the operations.
 
 You can check out the avaialble default settings [here](https://github.com/alijdens/spark-board/blob/main/spark_board/default_settings.py).
 
 ### Serving
 
-`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](./.github/workflows/deploy-examples.yml) in this repository).
+`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](https://github.com/alijdens/spark-board/tree/v0.0.7/.github/workflows/deploy-examples.yml) in this repository).
```

### Comparing `spark-board-0.0.6/setup.py` & `spark-board-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 README = (this_directory / "README.md").read_text()
 
 
 setup(
     name="spark-board",
-    version="0.0.6",
-    authors=[
-        {"name": "Axel Lijdens", "email": "alijdens@fi.uba.ar"},
-        {"name": "Ezequiel Werner", "email": "ewerner@fi.uba.ar"},
-    ],
+    version="0.0.7",
+    author="Axel Lijdens, Ezequiel Werner",
+    url="https://github.com/alijdens/spark-board",
     description="Interactive visualization of Spark jobs",
     long_description_content_type="text/markdown",
     long_description=README,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `spark-board-0.0.6/spark_board/default_settings.py` & `spark-board-0.0.7/spark_board/default_settings.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/html.py` & `spark-board-0.0.7/spark_board/html.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/plan_extractor/dag.py` & `spark-board-0.0.7/spark_board/plan_extractor/dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/plan_extractor/dag_builder.py` & `spark-board-0.0.7/spark_board/plan_extractor/dag_builder.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/plan_extractor/transformation_node_builders.py` & `spark-board-0.0.7/spark_board/plan_extractor/transformation_node_builders.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/plan_extractor/transformations_dag.py` & `spark-board-0.0.7/spark_board/plan_extractor/transformations_dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/filter-baaad4cd.svg` & `spark-board-0.0.7/spark_board/ui/assets/filter-baaad4cd.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/group-daa83ef9.svg` & `spark-board-0.0.7/spark_board/ui/assets/group-daa83ef9.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/index-946b5dbe.js` & `spark-board-0.0.7/spark_board/ui/assets/index-946b5dbe.js`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/index-c952fe44.css` & `spark-board-0.0.7/spark_board/ui/assets/index-c952fe44.css`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/join-cbb2d651.svg` & `spark-board-0.0.7/spark_board/ui/assets/join-cbb2d651.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/logo-c54f7abe.png` & `spark-board-0.0.7/spark_board/ui/assets/logo-c54f7abe.png`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/project-5fbb0573.svg` & `spark-board-0.0.7/spark_board/ui/assets/project-5fbb0573.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/sort-7864cb74.svg` & `spark-board-0.0.7/spark_board/ui/assets/sort-7864cb74.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/table-1441493a.svg` & `spark-board-0.0.7/spark_board/ui/assets/table-1441493a.svg`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/assets/union-e6640cdd.png` & `spark-board-0.0.7/spark_board/ui/assets/union-e6640cdd.png`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board/ui/index.html` & `spark-board-0.0.7/spark_board/ui/index.html`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/spark_board.egg-info/PKG-INFO` & `spark-board-0.0.7/spark_board.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interactive visualization of Spark jobs
+Home-page: https://github.com/alijdens/spark-board
+Author: Axel Lijdens, Ezequiel Werner
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `spark-board`: interactive PySpark dataframes visualization
 
 `spark-board` provides an interactive way to analize PySpark data frame execution plans as a static website displaying the transformations DAG.
 
-Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](./tests/examples/)).
+Check out the [examples](https://alijdens.github.io/spark-board/) for a quick overview of the features (and the corresponding examples source code [here](https://github.com/alijdens/spark-board/tree/v0.0.7/tests/examples/)).
 
 ## Usage
 
 `spark-board` takes a PySpark data frame and inspects the operations to build the DAG. This usually is the final step of a PySpark script, right before writing it to disk.
 
 ### Install `spark-board`
 
@@ -43,8 +45,8 @@
 
 and that's it! `spark-board` will generate a static website in the defined `output_dir` folder. You can now serve the website using any web server and inspect the operations.
 
 You can check out the avaialble default settings [here](https://github.com/alijdens/spark-board/blob/main/spark_board/default_settings.py).
 
 ### Serving
 
-`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](./.github/workflows/deploy-examples.yml) in this repository).
+`spark-board` is intended to be a live documentation of PySpark scripts. Because of this, it's advisable to run it every time the source code is updated. For example, `spark-board` can be run as part of a CI pipeline and the generated website uploaded to a static website hosting service, like Github or Gitlab pages (we actually do this to [update and serve the examples](https://github.com/alijdens/spark-board/tree/v0.0.7/.github/workflows/deploy-examples.yml) in this repository).
```

### Comparing `spark-board-0.0.6/spark_board.egg-info/SOURCES.txt` & `spark-board-0.0.7/spark_board.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.6/tests/test_integration.py` & `spark-board-0.0.7/tests/test_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import pytest
 from pyspark.sql.session import SparkSession
 from spark_board.html import dump_dataframe, DefaultSettings
 from pathlib import Path
 
 
-def test_spark_board(spark: SparkSession) -> None:
+def test_spark_board(spark: SparkSession, tmp_path: Path) -> None:
     """This test intends to be a very simple smoke test for the normal spark-board
     usage."""
 
     # create a data frame
     df = spark.createDataFrame([], schema="struct<a:double, b:double, c:double>")
     df = df.withColumn("sum", (df.a + df.b) / df.c)
 
-    OUT_DIR = Path("spark_board_output")
+    OUT_DIR = tmp_path/"spark_board_output"
 
     # dump it expecting no errors
     dump_dataframe(
         df=df,
         output_dir=str(OUT_DIR),
         overwrite=True,  # overwrite output_dir if it already exists
         default_settings=DefaultSettings(),  # override default settings if desired
```

