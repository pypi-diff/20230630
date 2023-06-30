# Comparing `tmp/kaggle-1.6.0a0.tar.gz` & `tmp/kaggle-1.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaggle-1.6.0a0.tar", last modified: Wed Jun  7 17:10:58 2023, max compression
+gzip compressed data, was "kaggle-1.6.0a2.tar", last modified: Tue Jun 13 00:13:46 2023, max compression
```

## Comparing `kaggle-1.6.0a0.tar` & `kaggle-1.6.0a2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    11541 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/LICENSE
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       19 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/MANIFEST.in
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/PKG-INFO
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    34704 2023-06-07 17:10:55.000000 kaggle-1.6.0a0/README.md
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.985743 kaggle-1.6.0a0/kaggle/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      799 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/__init__.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.989743 kaggle-1.6.0a0/kaggle/api/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      742 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)   191004 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/kaggle_api.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)   152973 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    25458 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/api_client.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    73219 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/cli.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     8858 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/configuration.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/kaggle/models/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1849 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4851 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/collaborator.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     7424 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_column.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    12281 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_new_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9991 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    10114 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4342 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/error.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     6915 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    19316 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/kernel_push_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     4077 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/license.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     5051 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/model_instance_new_version_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9699 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_instance_update_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    12103 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_new_instance_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    10055 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/model_new_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     9096 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/model_update_request.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     2895 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/models/result.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     5439 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/models/upload_file.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)    13927 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle/rest.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/kaggle/tests/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      596 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/tests/__init__.py
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1782 2023-06-07 17:10:56.000000 kaggle-1.6.0a0/kaggle/tests/test_authenticate.py
-drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-07 17:10:57.989743 kaggle-1.6.0a0/kaggle.egg-info/
--rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/PKG-INFO
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1077 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/SOURCES.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)        1 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/dependency_links.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       43 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/entry_points.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       78 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/requires.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)        7 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/kaggle.egg-info/top_level.txt
--rw-r--r--   0 philmod  (394664) primarygroup (89939)       79 2023-06-07 17:10:57.997743 kaggle-1.6.0a0/setup.cfg
--rw-r--r--   0 philmod  (394664) primarygroup (89939)     1680 2023-06-07 17:10:57.000000 kaggle-1.6.0a0/setup.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    11541 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/LICENSE
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       19 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/MANIFEST.in
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/PKG-INFO
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    35072 2023-06-13 00:13:37.000000 kaggle-1.6.0a2/README.md
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.872311 kaggle-1.6.0a2/kaggle/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      799 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/__init__.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.876311 kaggle-1.6.0a2/kaggle/api/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      742 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)   196727 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/kaggle_api.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)   153689 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    25458 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/api_client.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    74254 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/cli.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     8858 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/configuration.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/kaggle/models/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1849 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4851 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/collaborator.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     7424 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/dataset_column.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    12281 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9991 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    10114 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4342 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/error.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     6915 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    19316 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     4077 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/license.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     5051 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/model_instance_new_version_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9699 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_instance_update_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    12103 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_new_instance_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    10055 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/model_new_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     9096 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/models/model_update_request.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     2895 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/result.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     5439 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/models/upload_file.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)    13927 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/kaggle/rest.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/kaggle/tests/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      596 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/tests/__init__.py
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1782 2023-06-13 00:13:38.000000 kaggle-1.6.0a2/kaggle/tests/test_authenticate.py
+drwxr-xr-x   0 philmod  (394664) primarygroup (89939)        0 2023-06-13 00:13:46.872311 kaggle-1.6.0a2/kaggle.egg-info/
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)      609 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/PKG-INFO
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1077 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/SOURCES.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)        1 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/dependency_links.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       43 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/entry_points.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       78 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/requires.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)        7 2023-06-13 00:13:46.000000 kaggle-1.6.0a2/kaggle.egg-info/top_level.txt
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)       79 2023-06-13 00:13:46.884311 kaggle-1.6.0a2/setup.cfg
+-rw-r--r--   0 philmod  (394664) primarygroup (89939)     1680 2023-06-13 00:13:39.000000 kaggle-1.6.0a2/setup.py
```

### Comparing `kaggle-1.6.0a0/LICENSE` & `kaggle-1.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/PKG-INFO` & `kaggle-1.6.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a0
+Version: 1.6.0a2
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a0/README.md` & `kaggle-1.6.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,17 @@
 The command line tool supports the following commands:
 
 ``` 
 kaggle competitions {list, files, download, submit, submissions, leaderboard}
 kaggle datasets {list, files, download, create, version, init}
 kaggle kernels {list, init, push, pull, output, status}
 kaggle models {get, list, init, create, delete, update}
-kaggle models instances {init, create, delete, update}
+kaggle models instances {get, init, create, delete, update}
 kaggle models instances versions {init, create, download, delete}
+kaggle models instances {get, init, create, delete, update}
 kaggle config {view, set, unset}
 ```
 
 See more details below for using each of these commands.
 
 ### Competitions
 
@@ -640,15 +641,15 @@
 
 Example:
 
 `kaggle models delete tensorflow/toxicity`
 
 ##### Update a model
 
-If you want to update a new model, you need a metadata file at first. You can fetch the data by running `kaggle models get owner/slug -p folder`.
+If you want to update a model, you need a metadata file at first. You can fetch the data by running `kaggle models get owner/slug -p folder`.
 
 ```
 usage: kaggle models update [-h] [-p FOLDER]
 
 optional arguments:
   -h, --help            show this help message and exit
   -p FOLDER, --path FOLDER
@@ -667,20 +668,39 @@
 usage: kaggle models instances [-h]
                              {init, create, delete, update} ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 commands:
-  {init, create}
+  {get, init, create, delete}
+    get                 Get a model instance
     init                Initialize metadata file for model instance creation
     create              Create a new model instance
     delete              Delete a model instance
+    update              Update a model instance
 ```
 
+##### Get model instance
+
+```
+usage: kaggle models instances get [-h] [-p FOLDER] [modelInstance]
+
+required arguments:
+  modelInstance         Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  Folder where the special model-instance-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata) will be downloaded (if specified).
+```
+
+Example:
+
+`kaggle models instances get tensorflow/toxicity/tfjs/default`
+
 ##### Initialize metadata file for a model instance
 
 ```
 usage: kaggle models instances init [-h] [-p FOLDER]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -724,14 +744,16 @@
 
 Example:
 
 `kaggle models instances delete tensorflow/toxicity/tfjs/default`
 
 ##### Update a model instance
 
+If you want to update a model instance, you need a metadata file at first. You can fetch the data by running `kaggle models instances get owner-slug/model-slug/framework/instance-slug -p folder`.
+
 ```
 usage: kaggle models instances update [-h] [-p FOLDER]
 
 optional arguments:
   -h, --help            show this help message and exit
   -p FOLDER, --path FOLDER
                         Folder containing the special model-instance-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
@@ -749,54 +771,40 @@
 usage: kaggle models instances versions [-h]
                              {init, create, download, delete} ...
 
 optional arguments:
   -h, --help            show this help message and exit
 
 commands:
-  {init, create}
-    init                Initialize metadata file for model instance version creation
+  {create, download, delete}
     create              Create a new model instance version
+    download            Download a model instance version
     delete              Delete a model instance version
 ```
 
-##### Initialize metadata file for a model instance version
-
-```
-usage: kaggle models instances versions init [-h] [-p FOLDER]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -p FOLDER, --path FOLDER
-                        Folder to create the model-instance-version-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
-```
-
-Example:
-
-`kaggle models instances versions init -p /path/to/modelinstanceversion`
-
 ##### Create a new model instance version
 
-If you want to create a new model instance version, you need to initiate metadata file at first. You could fulfill this by running `kaggle models instances versions init` as describe above.
-
 ```
-usage: kaggle models instances versions create [-h] [-p FOLDER]
+usage: kaggle models instances versions create [-h] [modelInstance] [-p FOLDER] [-n NOTES]
 
 optional arguments:
   -h, --help            show this help message and exit
+  modelInstance         Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>
   -p FOLDER, --path FOLDER
-                        Folder containing the special model-instance-version-metadata.json file (https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). Defaults to current working directory
+                        Folder containing the model files to upload
+  -n, --version-notes NOTES
+                        Version notes to record for this new version
   -q, --quiet           Suppress printing information about the upload progress
   -r {skip,zip,tar}, --dir-mode {skip,zip,tar}
                         What to do with directories: "skip" - ignore; "zip" - compressed upload; "tar" - uncompressed upload
 ```
 
 Example:
 
-`kaggle models instances versions create -p /path/to/modelinstanceversion`
+`kaggle models instances versions create tensorflow/toxicity/tfjs/default -p /path/to/files -n "updated weights"`
 
 ##### Download a model instance version
 
 ```
 usage: kaggle models instances versions download [-h] [-p PATH] [--untar] [-f] [-q] [modelInstanceVersion]
 
 optional arguments:
```

### Comparing `kaggle-1.6.0a0/kaggle/__init__.py` & `kaggle-1.6.0a2/kaggle/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/api/__init__.py` & `kaggle-1.6.0a2/kaggle/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/api/kaggle_api.py` & `kaggle-1.6.0a2/kaggle/api/kaggle_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2553,36 +2553,157 @@
         if ('model_slug' not in params or
                 params['model_slug'] is None):
             raise ValueError("Missing the required parameter `model_slug` when calling `get_model`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'owner_slug' in params:
+            path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
+        if 'model_slug' in params:
+            path_params['modelSlug'] = params['model_slug']  # noqa: E501
 
         query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/models/{ownerSlug}/{modelSlug}/get', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Result',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_model_instance(self, owner_slug, model_slug, framework, instance_slug, **kwargs):  # noqa: E501
+        """Get a model instance  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_model_instance(owner_slug, model_slug, framework, instance_slug, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner_slug: Model owner (required)
+        :param str model_slug: Model name (required)
+        :param str framework: Model instance framework (required)
+        :param str instance_slug: Model instance slug (required)
+        :return: Result
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, **kwargs)  # noqa: E501
+            return data
+
+    def get_model_instance_with_http_info(self, owner_slug, model_slug, framework, instance_slug, **kwargs):  # noqa: E501
+        """Get a model instance  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_model_instance_with_http_info(owner_slug, model_slug, framework, instance_slug, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner_slug: Model owner (required)
+        :param str model_slug: Model name (required)
+        :param str framework: Model instance framework (required)
+        :param str instance_slug: Model instance slug (required)
+        :return: Result
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner_slug', 'model_slug', 'framework', 'instance_slug']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_model_instance" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner_slug' is set
+        if ('owner_slug' not in params or
+                params['owner_slug'] is None):
+            raise ValueError("Missing the required parameter `owner_slug` when calling `get_model_instance`")  # noqa: E501
+        # verify the required parameter 'model_slug' is set
+        if ('model_slug' not in params or
+                params['model_slug'] is None):
+            raise ValueError("Missing the required parameter `model_slug` when calling `get_model_instance`")  # noqa: E501
+        # verify the required parameter 'framework' is set
+        if ('framework' not in params or
+                params['framework'] is None):
+            raise ValueError("Missing the required parameter `framework` when calling `get_model_instance`")  # noqa: E501
+        # verify the required parameter 'instance_slug' is set
+        if ('instance_slug' not in params or
+                params['instance_slug'] is None):
+            raise ValueError("Missing the required parameter `instance_slug` when calling `get_model_instance`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
         if 'owner_slug' in params:
-            query_params.append(('ownerSlug', params['owner_slug']))  # noqa: E501
+            path_params['ownerSlug'] = params['owner_slug']  # noqa: E501
         if 'model_slug' in params:
-            query_params.append(('modelSlug', params['model_slug']))  # noqa: E501
+            path_params['modelSlug'] = params['model_slug']  # noqa: E501
+        if 'framework' in params:
+            path_params['framework'] = params['framework']  # noqa: E501
+        if 'instance_slug' in params:
+            path_params['instanceSlug'] = params['instance_slug']  # noqa: E501
+
+        query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['basicAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/models/get', 'GET',
+            '/models/{ownerSlug}/{modelSlug}/{framework}/{instanceSlug}/get', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Result',  # noqa: E501
```

### Comparing `kaggle-1.6.0a0/kaggle/api/kaggle_api_extended.py` & `kaggle-1.6.0a2/kaggle/api/kaggle_api_extended.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,29 @@
 try:
     unicode  # Python 2
 except NameError:
     unicode = str  # Python 3
 
 
 class KaggleApi(KaggleApi):
-    __version__ = '1.6.0a0'
+    __version__ = '1.6.0a2'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
 
     HEADER_API_VERSION = 'X-Kaggle-ApiVersion'
     DATASET_METADATA_FILE = 'dataset-metadata.json'
     OLD_DATASET_METADATA_FILE = 'datapackage.json'
     KERNEL_METADATA_FILE = 'kernel-metadata.json'
     MODEL_METADATA_FILE = 'model-metadata.json'
     MODEL_INSTANCE_METADATA_FILE = 'model-instance-metadata.json'
-    MODEL_INSTANCE_VERSION_METADATA_FILE = 'model-instance-version-metadata.json'
 
     config_dir = os.environ.get('KAGGLE_CONFIG_DIR') or os.path.join(
         expanduser('~'), '.kaggle')
     if not os.path.exists(config_dir):
         os.makedirs(config_dir)
 
     config_file = 'kaggle.json'
@@ -2244,22 +2243,15 @@
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
         """
         if model is None:
             raise ValueError('A model must be specified')
-        if '/' in model:
-            self.validate_model_string(model)
-            model_urls = model.split('/')
-            owner_slug = model_urls[0]
-            model_slug = model_urls[1]
-        else:
-            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
-            model_slug = model
+        owner_slug, model_slug = self.split_model_string(model)
 
         model_get_result = self.process_response(
             self.get_model_with_http_info(owner_slug, model_slug))
         return model_get_result
 
     def model_get_cli(self, model, folder=None, model_opt=None):
         """ wrapper for client for model_get, with additional
@@ -2466,22 +2458,15 @@
              Parameters
             ==========
             model: the string identified of the model
                      should be in format [owner]/[model-name]
         """
         if model is None:
             raise ValueError('A model must be specified')
-        if '/' in model:
-            self.validate_model_string(model)
-            model_urls = model.split('/')
-            owner_slug = model_urls[0]
-            model_slug = model_urls[1]
-        else:
-            owner_slug = self.get_config_value(self.CONFIG_NAME_USER)
-            model_slug = model
+        owner_slug, model_slug = self.split_model_string(model)
 
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_with_http_info(owner_slug, model_slug)))
         return res
 
     def model_delete_cli(self, model, model_opt=None):
@@ -2576,14 +2561,70 @@
 
         if result.hasId:
             print('Your model was updated. Id={}. Url={}'.format(
                 result.id, result.url))
         else:
             print('Model update error: ' + result.error)
 
+    def model_instance_get(self, model_instance):
+        """ call to get a model instance from the API
+             Parameters
+            ==========
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
+        """
+        if model_instance is None:
+            raise ValueError('A model instance must be specified')
+        owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
+            model_instance)
+
+        mi = self.process_response(
+            self.get_model_instance_with_http_info(owner_slug, model_slug,
+                                                   framework, instance_slug))
+        return mi
+
+    def model_instance_get_cli(self,
+                               model_instance,
+                               folder=None,
+                               model_instance_opt=None):
+        """ wrapper for client for model_instance_get, with additional
+            model_instance_opt to get a model instance from the API
+             Parameters
+            ==========
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
+            folder: the folder to download the model metadata file
+            model_instance_opt: an alternative to model_instance
+        """
+        m = model_instance or model_instance_opt
+        mi = self.model_instance_get(m)
+        if folder is None:
+            self.print_obj(mi)
+        else:
+            meta_file = os.path.join(folder, self.MODEL_INSTANCE_METADATA_FILE)
+
+            owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
+                model_instance)
+
+            data = {}
+            data['id'] = mi['id']
+            data['ownerSlug'] = owner_slug
+            data['modelSlug'] = model_slug
+            data['instanceSlug'] = mi['slug']
+            data['framework'] = mi['framework']
+            data['overview'] = mi['overview']
+            data['usage'] = mi['usage']
+            data['licenseName'] = mi['licenseName']
+            data['fineTunable'] = mi['fineTunable']
+            data['trainingData'] = mi['trainingData']
+
+            with open(meta_file, 'w') as f:
+                json.dump(data, f, indent=2)
+            print('Metadata file written to {}'.format(meta_file))
+
     def model_instance_initialize(self, folder):
         """ initialize a folder with a model instance configuration (metadata) file
              Parameters
             ==========
             folder: the folder to initialize the metadata file in
         """
         if not os.path.isdir(folder):
@@ -2680,16 +2721,15 @@
                                           framework=framework,
                                           overview=overview,
                                           usage=usage,
                                           license_name=license_name,
                                           fine_tunable=fine_tunable,
                                           training_data=training_data,
                                           files=[])
-        resources = meta_data.get('resources')
-        self.upload_files(request, resources, folder, 'model', quiet, dir_mode)
+        self.upload_files(request, None, folder, 'model', quiet, dir_mode)
         result = ModelNewResponse(
             self.process_response(
                 self.models_create_instance_with_http_info(
                     owner_slug, model_slug, request)))
 
         return result
 
@@ -2715,21 +2755,16 @@
              Parameters
             ==========
             model_instance: the string identified of the model instance
                      should be in format [owner]/[model-name]/[framework]/[instance-slug]
         """
         if model_instance is None:
             raise ValueError('A model instance must be specified')
-
-        self.validate_model_instance_string(model_instance)
-        urls = model_instance.split('/')
-        owner_slug = urls[0]
-        model_slug = urls[1]
-        framework = urls[2]
-        instance_slug = urls[3]
+        owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
+            model_instance)
 
         res = ModelDeleteResponse(
             self.process_response(
                 self.delete_model_instance_with_http_info(
                     owner_slug, model_slug, framework, instance_slug)))
         return res
 
@@ -2838,110 +2873,65 @@
 
         if result.hasId:
             print('Your model instance was updated. Id={}. Url={}'.format(
                 result.id, result.url))
         else:
             print('Model update error: ' + result.error)
 
-    def model_instance_version_initialize(self, folder):
-        """ initialize a folder with a a model instance version configuration (metadata) file
-            Parameters
-            ==========
-            folder: the folder to initialize the metadata file in
-        """
-        if not os.path.isdir(folder):
-            raise ValueError('Invalid folder: ' + folder)
-
-        meta_data = {
-            'ownerSlug': 'INSERT_OWNER_SLUG_HERE',
-            'modelSlug': 'INSERT_EXISTING_MODEL_SLUG_HERE',
-            'instanceSlug': 'INSERT_EXISTING_INSTANCE_SLUG_HERE',
-            'framework': 'INSERT_EXISTING_FRAMEWORK_SLUG_HERE',
-            'versionNotes': '',
-        }
-        meta_file = os.path.join(folder,
-                                 self.MODEL_INSTANCE_VERSION_METADATA_FILE)
-        with open(meta_file, 'w') as f:
-            json.dump(meta_data, f, indent=2)
-
-        print('Model Instance Version template written to: ' + meta_file)
-        return meta_file
-
-    def model_instance_version_initialize_cli(self, folder):
-        folder = folder or os.getcwd()
-        self.model_instance_version_initialize(folder)
-
     def model_instance_version_create(self,
+                                      model_instance,
                                       folder,
+                                      version_notes='',
                                       quiet=False,
                                       dir_mode='skip'):
         """ create a new model instance version.
              Parameters
             ==========
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
             folder: the folder to get the metadata file from
+            version_notes: the version notes to record for this new version
             quiet: suppress verbose output (default is False)
             dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
         """
-        if not os.path.isdir(folder):
-            raise ValueError('Invalid folder: ' + folder)
-
-        meta_file = self.get_model_instance_version_metadata_file(folder)
-
-        # read json
-        with open(meta_file) as f:
-            meta_data = json.load(f)
-        owner_slug = self.get_or_fail(meta_data, 'ownerSlug')
-        model_slug = self.get_or_fail(meta_data, 'modelSlug')
-        instance_slug = self.get_or_fail(meta_data, 'instanceSlug')
-        framework = self.get_or_fail(meta_data, 'framework')
-        version_notes = self.get_or_fail(meta_data, 'versionNotes')
-
-        # validations
-        if owner_slug == 'INSERT_OWNER_SLUG_HERE':
-            raise ValueError(
-                'Default ownerSlug detected, please change values before uploading'
-            )
-        if model_slug == 'INSERT_EXISTING_MODEL_SLUG_HERE':
-            raise ValueError(
-                'Default modelSlug detected, please change values before uploading'
-            )
-        if instance_slug == 'INSERT_EXISTING_INSTANCE_SLUG_HERE':
-            raise ValueError(
-                'Default instanceSlug detected, please change values before uploading'
-            )
-        if framework == 'INSERT_EXISTING_FRAMEWORK_SLUG_HERE':
-            raise ValueError(
-                'Default framework detected, please change values before uploading'
-            )
+        if model_instance is None:
+            raise ValueError('A model instance must be specified')
+        owner_slug, model_slug, framework, instance_slug = self.split_model_instance_string(
+            model_instance)
 
         request = ModelInstanceNewVersionRequest(version_notes=version_notes,
                                                  files=[])
-        resources = meta_data.get('resources')
-        self.upload_files(request, resources, folder, 'model', quiet, dir_mode)
+        self.upload_files(request, None, folder, 'model', quiet, dir_mode)
         result = ModelNewResponse(
             self.process_response(
                 self.models_create_instance_version_with_http_info(
                     owner_slug, model_slug, framework, instance_slug,
                     request)))
 
         return result
 
     def model_instance_version_create_cli(self,
+                                          model_instance,
                                           folder,
+                                          version_notes='',
                                           quiet=False,
                                           dir_mode='skip'):
         """ client wrapper for creating a new model instance version
              Parameters
             ==========
+            model_instance: the string identified of the model instance
+                     should be in format [owner]/[model-name]/[framework]/[instance-slug]
             folder: the folder to get the metadata file from
+            version_notes: the version notes to record for this new version
             quiet: suppress verbose output (default is False)
             dir_mode: what to do with directories: "skip" - ignore; "zip" - compress and upload
         """
-        folder = folder or os.getcwd()
-        result = self.model_instance_version_create(folder, quiet, dir_mode)
+        result = self.model_instance_version_create(model_instance, folder,
+                                                    version_notes, quiet,
+                                                    dir_mode)
 
         if result.hasId:
             print('Your model instance version was created. Url={}'.format(
                 result.url))
         else:
             print('Model instance version creation error: ' + result.error)
 
@@ -3186,22 +3176,14 @@
     def get_model_instance_metadata_file(self, folder):
         meta_file = os.path.join(folder, self.MODEL_INSTANCE_METADATA_FILE)
         if not os.path.isfile(meta_file):
             raise ValueError('Metadata file not found: ' +
                              self.MODEL_INSTANCE_METADATA_FILE)
         return meta_file
 
-    def get_model_instance_version_metadata_file(self, folder):
-        meta_file = os.path.join(folder,
-                                 self.MODEL_INSTANCE_VERSION_METADATA_FILE)
-        if not os.path.isfile(meta_file):
-            raise ValueError('Metadata file not found: ' +
-                             self.MODEL_INSTANCE_VERSION_METADATA_FILE)
-        return meta_file
-
     def process_response(self, result):
         """ process a response from the API. We check the API version against
             the client's to see if it's old, and give them a warning (once)
 
             Parameters
             ==========
             result: the result from the API
@@ -3268,16 +3250,15 @@
             entity: dataset or model
             quiet: suppress verbose output (default is False)
         """
         for file_name in os.listdir(folder):
             if (file_name in [
                     self.DATASET_METADATA_FILE, self.OLD_DATASET_METADATA_FILE,
                     self.KERNEL_METADATA_FILE, self.MODEL_METADATA_FILE,
-                    self.MODEL_INSTANCE_METADATA_FILE,
-                    self.MODEL_INSTANCE_VERSION_METADATA_FILE
+                    self.MODEL_INSTANCE_METADATA_FILE
             ]):
                 continue
             full_path = os.path.join(folder, file_name)
 
             if os.path.isfile(full_path):
                 exitcode = self._upload_file(file_name, full_path, quiet,
                                              request, resources, entity)
@@ -3290,15 +3271,16 @@
                         _, dir_name = os.path.split(full_path)
                         archive_path = shutil.make_archive(
                             os.path.join(temp_dir, dir_name), dir_mode,
                             full_path)
                         _, archive_name = os.path.split(archive_path)
                         exitcode = self._upload_file(archive_name,
                                                      archive_path, quiet,
-                                                     request, resources)
+                                                     request, resources,
+                                                     entity)
                     finally:
                         shutil.rmtree(temp_dir)
                     if exitcode:
                         return
                 elif not quiet:
                     print("Skipping folder: " + file_name +
                           "; use '--dir-mode' to upload folders")
@@ -3444,14 +3426,27 @@
                 raise ValueError('Model must be specified in the form of '
                                  '\'{owner}/{model-slug}\'')
 
             split = model.split('/')
             if not split[0] or not split[1]:
                 raise ValueError('Invalid model specification ' + model)
 
+    def split_model_string(self, model):
+        """ split a model string into owner_slug, model_slug
+             Parameters
+            ==========
+            model: the model name to split
+        """
+        if '/' in model:
+            self.validate_model_string(model)
+            model_urls = model.split('/')
+            return model_urls[0], model_urls[1]
+        else:
+            return self.get_config_value(self.CONFIG_NAME_USER), model
+
     def validate_model_instance_string(self, model_instance):
         """ determine if a model instance string is valid, meaning it is in the format
             of {owner}/{model-slug}/{framework}/{instance-slug}.
              Parameters
             ==========
             model_instance: the model instance name to validate
         """
@@ -3462,14 +3457,25 @@
                     '\'{owner}/{model-slug}/{framework}/{instance-slug}\'')
 
             split = model_instance.split('/')
             if not split[0] or not split[1] or not split[2] or not split[3]:
                 raise ValueError('Invalid model instance specification ' +
                                  model_instance)
 
+    def split_model_instance_string(self, model_instance):
+        """ split a model instance string into owner_slug, model_slug, 
+            framework, instance_slug
+             Parameters
+            ==========
+            model_instance: the model instance name to validate
+        """
+        self.validate_model_instance_string(model_instance)
+        urls = model_instance.split('/')
+        return urls[0], urls[1], urls[2], urls[3]
+
     def validate_model_instance_version_string(self, model_instance_version):
         """ determine if a model instance version string is valid, meaning it is in the format
             of {owner}/{model-slug}/{framework}/{instance-slug}/{version-number}.
              Parameters
             ==========
             model_instance_version: the model instance version name to validate
         """
```

### Comparing `kaggle-1.6.0a0/kaggle/api_client.py` & `kaggle-1.6.0a2/kaggle/api_client.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/cli.py` & `kaggle-1.6.0a2/kaggle/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -988,14 +988,41 @@
         title='commands', dest='command')
     subparsers_model_intances.required = True
     subparsers_model_intances.choices = Help.model_instances_choices
 
     # Models Instances Versions.
     parse_model_instance_versions(subparsers_model_intances)
 
+    # Models Instances get
+    parser_model_instance_get = subparsers_model_intances.add_parser(
+        'get',
+        formatter_class=argparse.RawTextHelpFormatter,
+        help=Help.command_model_instances_get)
+    parser_model_instance_get_optional = parser_model_instance_get._action_groups.pop(
+    )
+    parser_model_instance_get_optional.add_argument(
+        'model_instance',
+        nargs='?',
+        default=None,
+        help=Help.param_model_instance)
+    parser_model_instance_get_optional.add_argument('-m',
+                                                    '--modelInstance',
+                                                    dest='model_instance',
+                                                    required=False,
+                                                    help=argparse.SUPPRESS)
+    parser_model_instance_get_optional.add_argument(
+        '-p',
+        '--path',
+        dest='folder',
+        required=False,
+        help=Help.param_model_instance_downfile)
+    parser_model_instance_get._action_groups.append(
+        parser_model_instance_get_optional)
+    parser_model_instance_get.set_defaults(func=api.model_instance_get_cli)
+
     # Model Instances init
     parser_model_instances_init = subparsers_model_intances.add_parser(
         'init',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instances_init)
     parser_model_instances_init_optional = parser_model_instances_init._action_groups.pop(
     )
@@ -1089,46 +1116,39 @@
         aliases=['miv'])
 
     subparsers_model_intance_versions = parser_model_instance_versions.add_subparsers(
         title='commands', dest='command')
     subparsers_model_intance_versions.required = True
     subparsers_model_intance_versions.choices = Help.model_instance_versions_choices
 
-    # Model Instance Versions init
-    parser_model_instance_versions_init = subparsers_model_intance_versions.add_parser(
-        'init',
-        formatter_class=argparse.RawTextHelpFormatter,
-        help=Help.command_model_instances_init)
-    parser_model_instance_versions_init_optional = parser_model_instance_versions_init._action_groups.pop(
-    )
-    parser_model_instance_versions_init_optional.add_argument(
-        '-p',
-        '--path',
-        dest='folder',
-        required=False,
-        help=Help.param_model_instance_version_upfile)
-    parser_model_instance_versions_init._action_groups.append(
-        parser_model_instance_versions_init_optional)
-    parser_model_instance_versions_init.set_defaults(
-        func=api.model_instance_version_initialize_cli)
-
     # Model Instance Versions create
     parser_model_instance_versions_create = subparsers_model_intance_versions.add_parser(
         'create',
         formatter_class=argparse.RawTextHelpFormatter,
         help=Help.command_model_instance_versions_new)
     parser_model_instance_versions_create_optional = parser_model_instance_versions_create._action_groups.pop(
     )
     parser_model_instance_versions_create_optional.add_argument(
+        'model_instance',
+        nargs='?',
+        default=None,
+        help=Help.param_model_instance)
+    parser_model_instance_versions_create_optional.add_argument(
         '-p',
         '--path',
         dest='folder',
         required=False,
         help=Help.param_model_instance_version_upfile)
     parser_model_instance_versions_create_optional.add_argument(
+        '-n',
+        '--version-notes',
+        dest='version_notes',
+        required=False,
+        help=Help.param_model_instance_version_upfile)
+    parser_model_instance_versions_create_optional.add_argument(
         '-q',
         '--quiet',
         dest='quiet',
         action='store_true',
         help=Help.param_quiet)
     parser_model_instance_versions_create_optional.add_argument(
         '-r',
@@ -1271,15 +1291,15 @@
         'status'
     ]
     kernels_choices = ['list', 'init', 'push', 'pull', 'output', 'status']
     models_choices = [
         'instances', 'get', 'list', 'init', 'create', 'delete', 'update'
     ]
     model_instances_choices = [
-        'versions', 'init', 'create', 'delete', 'update'
+        'versions', 'get', 'init', 'create', 'delete', 'update'
     ]
     model_instance_versions_choices = ['init', 'create', 'download', 'delete']
     config_choices = ['view', 'set', 'unset']
 
     kaggle = 'Use one of:\ncompetitions {' + ', '.join(
         competitions_choices) + '}\ndatasets {' + ', '.join(
             datasets_choices) + '}\nmodels {' + ', '.join(
@@ -1495,39 +1515,43 @@
         '(https://github.com/Kaggle/kaggle-api/wiki/Model-Metadata). '
         'Defaults to current working directory')
 
     # Model Instances params
     param_model_instance = (
         'Model Instance URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>'
     )
+    command_model_instances_get = 'Get a model instance'
     command_model_instances_init = 'Initialize metadata file for model instance creation'
     command_model_instances_new = 'Create a new model instance'
+    param_model_instance_downfile = (
+        'Folder for downloading the special model-instance-metadata.json file '
+        '(https://github.com/Kaggle/kaggle-api/wiki/ModelInstance-Metadata). ')
     param_model_instance_upfile = (
         'Folder for upload, containing data files and a '
         'special model-instance-metadata.json file '
         '(https://github.com/Kaggle/kaggle-api/wiki/ModelInstance-Metadata). '
         'Defaults to current working directory')
     command_model_instances_delete = 'Delete a model instance'
     command_model_instances_update = 'Update a model instance'
 
     # Model Instance Versions params
     param_model_instance_version = (
         'Model Instance Version URL suffix in format <owner>/<model-name>/<framework>/<instance-slug>/<version-number>'
     )
 
     # Model Instance Versions params
-    command_model_instance_versions_init = 'Initialize metadata file for model instance version creation'
     command_model_instance_versions_new = 'Create a new model instance version'
     param_model_instance_version_upfile = (
         'Folder for upload, containing data files and a '
         'special model-instance_version-metadata.json file '
         '(https://github.com/Kaggle/kaggle-api/wiki/ModelInstanceVersion-Metadata). '
         'Defaults to current working directory')
     command_model_instance_versions_delete = 'Delete a model instance version'
     command_model_instance_versions_download = 'Download model instance version files'
+    param_model_instance_version_notes = 'Version notes to record for the new model instance version'
 
     # Config params
     param_config_name = ('Name of the configuration parameter\n(one of '
                          'competition, path, proxy)')
     param_config_value = (
         ('Value of the configuration parameter, valid values '
          'depending on name\n- competition: ') + param_competition_nonempty +
```

### Comparing `kaggle-1.6.0a0/kaggle/configuration.py` & `kaggle-1.6.0a2/kaggle/configuration.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/__init__.py` & `kaggle-1.6.0a2/kaggle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/collaborator.py` & `kaggle-1.6.0a2/kaggle/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/dataset_column.py` & `kaggle-1.6.0a2/kaggle/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/dataset_new_request.py` & `kaggle-1.6.0a2/kaggle/models/dataset_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/dataset_new_version_request.py` & `kaggle-1.6.0a2/kaggle/models/dataset_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/dataset_update_settings_request.py` & `kaggle-1.6.0a2/kaggle/models/dataset_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/error.py` & `kaggle-1.6.0a2/kaggle/models/error.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/kaggle_models_extended.py` & `kaggle-1.6.0a2/kaggle/models/kaggle_models_extended.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/kernel_push_request.py` & `kaggle-1.6.0a2/kaggle/models/kernel_push_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/license.py` & `kaggle-1.6.0a2/kaggle/models/license.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/model_instance_new_version_request.py` & `kaggle-1.6.0a2/kaggle/models/model_instance_new_version_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/model_instance_update_request.py` & `kaggle-1.6.0a2/kaggle/models/model_instance_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/model_new_instance_request.py` & `kaggle-1.6.0a2/kaggle/models/model_new_instance_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/model_new_request.py` & `kaggle-1.6.0a2/kaggle/models/model_new_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/model_update_request.py` & `kaggle-1.6.0a2/kaggle/models/model_update_request.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/result.py` & `kaggle-1.6.0a2/kaggle/models/result.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/models/upload_file.py` & `kaggle-1.6.0a2/kaggle/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/rest.py` & `kaggle-1.6.0a2/kaggle/rest.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/tests/__init__.py` & `kaggle-1.6.0a2/kaggle/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle/tests/test_authenticate.py` & `kaggle-1.6.0a2/kaggle/tests/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/kaggle.egg-info/PKG-INFO` & `kaggle-1.6.0a2/kaggle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaggle
-Version: 1.6.0a0
+Version: 1.6.0a2
 Summary: Kaggle API
 Home-page: https://github.com/Kaggle/kaggle-api
 Author: Kaggle
 Author-email: support@kaggle.com
 License: Apache 2.0
 Project-URL: Documentation, https://www.kaggle.com/docs/api
 Project-URL: GitHub, https://github.com/Kaggle/kaggle-api
```

### Comparing `kaggle-1.6.0a0/kaggle.egg-info/SOURCES.txt` & `kaggle-1.6.0a2/kaggle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaggle-1.6.0a0/setup.py` & `kaggle-1.6.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='kaggle',
-    version='1.6.0a0',
+    version='1.6.0a2',
     description='Kaggle API',
     long_description=
     ('Official API for https://www.kaggle.com, accessible using a command line '
      'tool implemented in Python. Beta release - Kaggle reserves the right to '
      'modify the API functionality currently offered.'),
     author='Kaggle',
     author_email='support@kaggle.com',
```

