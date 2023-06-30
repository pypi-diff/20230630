# Comparing `tmp/raga-testing-platform-1.0.8.tar.gz` & `tmp/raga-testing-platform-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.0.8.tar", last modified: Wed Jun 21 13:14:37 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.0.9.tar", last modified: Thu Jun 22 14:00:53 2023, max compression
```

## Comparing `raga-testing-platform-1.0.8.tar` & `raga-testing-platform-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.957271 raga-testing-platform-1.0.8/
--rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-20 07:04:12.000000 raga-testing-platform-1.0.8/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)     3097 2023-06-21 06:26:56.000000 raga-testing-platform-1.0.8/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.8/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-21 13:14:37.957051 raga-testing-platform-1.0.8/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)     2408 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.8/README.md
--rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-21 13:14:19.000000 raga-testing-platform-1.0.8/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.947783 raga-testing-platform-1.0.8/raga/
--rw-r--r--   0 manabroy   (501) staff       (20)     1061 2023-06-20 07:45:29.000000 raga-testing-platform-1.0.8/raga/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)    10213 2023-06-21 12:16:32.000000 raga-testing-platform-1.0.8/raga/dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)      486 2023-06-16 07:12:34.000000 raga-testing-platform-1.0.8/raga/dataset_creds.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.948405 raga-testing-platform-1.0.8/raga/docs/
--rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.8/raga/docs/conf.py
--rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.8/raga/docs/index.rst
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.951336 raga-testing-platform-1.0.8/raga/examples/
--rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-14 12:00:51.000000 raga-testing-platform-1.0.8/raga/examples/.DS_Store
--rw-r--r--   0 manabroy   (501) staff       (20)   242124 2023-06-20 13:18:25.000000 raga-testing-platform-1.0.8/raga/examples/MA.json
--rw-r--r--   0 manabroy   (501) staff       (20)   255328 2023-06-20 13:18:25.000000 raga-testing-platform-1.0.8/raga/examples/MB.json
--rw-r--r--   0 manabroy   (501) staff       (20)     2797 2023-06-21 12:08:55.000000 raga-testing-platform-1.0.8/raga/examples/example.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2338 2023-06-21 12:56:24.000000 raga-testing-platform-1.0.8/raga/examples/example2.py
--rw-r--r--   0 manabroy   (501) staff       (20)     3401 2023-06-21 12:35:55.000000 raga-testing-platform-1.0.8/raga/raga_schema.py
--rw-r--r--   0 manabroy   (501) staff       (20)     4770 2023-06-20 10:46:46.000000 raga-testing-platform-1.0.8/raga/test_session.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.952930 raga-testing-platform-1.0.8/raga/tests/
--rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.8/raga/tests/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)    11627 2023-06-16 18:34:16.000000 raga-testing-platform-1.0.8/raga/tests/test_dataset.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1358 2023-06-16 18:24:34.000000 raga-testing-platform-1.0.8/raga/tests/test_dataset_util.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5143 2023-06-16 14:00:15.000000 raga-testing-platform-1.0.8/raga/tests/test_http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)    12830 2023-06-16 16:57:58.000000 raga-testing-platform-1.0.8/raga/tests/test_test_session.py
--rw-r--r--   0 manabroy   (501) staff       (20)       59 2023-06-12 07:51:37.000000 raga-testing-platform-1.0.8/raga/tests.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.954609 raga-testing-platform-1.0.8/raga/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)      108 2023-06-16 07:16:41.000000 raga-testing-platform-1.0.8/raga/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)     3830 2023-06-21 12:55:56.000000 raga-testing-platform-1.0.8/raga/utils/dataset_util.py
--rw-r--r--   0 manabroy   (501) staff       (20)      789 2023-06-16 07:10:30.000000 raga-testing-platform-1.0.8/raga/utils/file.py
--rw-r--r--   0 manabroy   (501) staff       (20)     4579 2023-06-20 13:47:33.000000 raga-testing-platform-1.0.8/raga/utils/http_client.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2055 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.8/raga/utils/raga_config_reader.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.955575 raga-testing-platform-1.0.8/raga/validators/
--rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.8/raga/validators/dataset_creds_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1064 2023-06-15 13:06:56.000000 raga-testing-platform-1.0.8/raga/validators/dataset_validations.py
--rw-r--r--   0 manabroy   (501) staff       (20)      760 2023-06-15 13:09:40.000000 raga-testing-platform-1.0.8/raga/validators/test_session_validation.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-21 13:14:37.956731 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-21 13:14:37.000000 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      944 2023-06-21 13:14:37.000000 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-21 13:14:37.000000 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-21 13:14:37.000000 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-21 13:14:37.000000 raga-testing-platform-1.0.8/raga_testing_platform.egg-info/top_level.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-21 13:14:37.957331 raga-testing-platform-1.0.8/setup.cfg
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.512846 raga-testing-platform-1.0.9/
+-rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-20 07:04:12.000000 raga-testing-platform-1.0.9/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)     3115 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)     1073 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.9/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-22 14:00:53.512548 raga-testing-platform-1.0.9/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)     2408 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.9/README.md
+-rw-r--r--   0 manabroy   (501) staff       (20)     1005 2023-06-22 14:00:37.000000 raga-testing-platform-1.0.9/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.497300 raga-testing-platform-1.0.9/raga/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1083 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     4391 2023-06-22 13:50:17.000000 raga-testing-platform-1.0.9/raga/_tests.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9838 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      486 2023-06-16 07:12:34.000000 raga-testing-platform-1.0.9/raga/dataset_creds.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.497956 raga-testing-platform-1.0.9/raga/docs/
+-rw-r--r--   0 manabroy   (501) staff       (20)       82 2023-06-12 07:15:42.000000 raga-testing-platform-1.0.9/raga/docs/conf.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      160 2023-06-12 09:52:28.000000 raga-testing-platform-1.0.9/raga/docs/index.rst
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.506523 raga-testing-platform-1.0.9/raga/examples/
+-rw-r--r--   0 manabroy   (501) staff       (20)     6148 2023-06-22 14:00:31.000000 raga-testing-platform-1.0.9/raga/examples/.DS_Store
+-rw-r--r--   0 manabroy   (501) staff       (20)   242124 2023-06-20 13:18:25.000000 raga-testing-platform-1.0.9/raga/examples/MA.json
+-rw-r--r--   0 manabroy   (501) staff       (20)   255328 2023-06-20 13:18:25.000000 raga-testing-platform-1.0.9/raga/examples/MB.json
+-rw-r--r--   0 manabroy   (501) staff       (20)     3451 2023-06-22 10:56:39.000000 raga-testing-platform-1.0.9/raga/examples/code_testing.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     3447 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/examples/example.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     4420 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/raga_schema.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     4743 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/test_session.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.508487 raga-testing-platform-1.0.9/raga/tests/
+-rw-r--r--   0 manabroy   (501) staff       (20)       51 2023-06-12 07:15:00.000000 raga-testing-platform-1.0.9/raga/tests/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9417 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/tests/test_dataset.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1358 2023-06-16 18:24:34.000000 raga-testing-platform-1.0.9/raga/tests/test_dataset_util.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5143 2023-06-16 14:00:15.000000 raga-testing-platform-1.0.9/raga/tests/test_http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    13074 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/tests/test_test_session.py
+-rw-r--r--   0 manabroy   (501) staff       (20)    11320 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/tests/test_tests.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.510060 raga-testing-platform-1.0.9/raga/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)      108 2023-06-16 07:16:41.000000 raga-testing-platform-1.0.9/raga/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     4194 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/utils/dataset_util.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      789 2023-06-16 07:10:30.000000 raga-testing-platform-1.0.9/raga/utils/file.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     4581 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/utils/http_client.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2055 2023-06-15 13:02:22.000000 raga-testing-platform-1.0.9/raga/utils/raga_config_reader.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.510985 raga-testing-platform-1.0.9/raga/validators/
+-rw-r--r--   0 manabroy   (501) staff       (20)      860 2023-06-12 10:10:59.000000 raga-testing-platform-1.0.9/raga/validators/dataset_creds_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1383 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/validators/dataset_validations.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1177 2023-06-22 13:43:51.000000 raga-testing-platform-1.0.9/raga/validators/test_session_validation.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-06-22 14:00:53.512187 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3110 2023-06-22 14:00:53.000000 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      974 2023-06-22 14:00:53.000000 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-06-22 14:00:53.000000 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       61 2023-06-22 14:00:53.000000 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        5 2023-06-22 14:00:53.000000 raga-testing-platform-1.0.9/raga_testing_platform.egg-info/top_level.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-06-22 14:00:53.512923 raga-testing-platform-1.0.9/setup.cfg
```

### Comparing `raga-testing-platform-1.0.8/.DS_Store` & `raga-testing-platform-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/.gitignore` & `raga-testing-platform-1.0.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,11 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-*.log
+*.log
+
+
+code_testing.py
```

### Comparing `raga-testing-platform-1.0.8/LICENSE` & `raga-testing-platform-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/PKG-INFO` & `raga-testing-platform-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.8
+Version: 1.0.9
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.0.8/README.md` & `raga-testing-platform-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/pyproject.toml` & `raga-testing-platform-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-testing-platform"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Raga AI", email="support@ragaai.com" },
 ]
 maintainers = [{ name = "Raga AI", email = "support@ragaai.com" }]
 dependencies = [
     "pandas==2.0.2",
     "urllib3==1.26.7",
```

### Comparing `raga-testing-platform-1.0.8/raga/__init__.py` & `raga-testing-platform-1.0.9/raga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,7 +28,8 @@
     logger = logging.getLogger(__name__)
     logger.addHandler(file_handler)
 
 from .test_session import *
 from .dataset_creds import *
 from .dataset import *
 from .raga_schema import *
+from ._tests import *
```

### Comparing `raga-testing-platform-1.0.8/raga/dataset.py` & `raga-testing-platform-1.0.9/raga/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,136 @@
 import json
 import os
+import sys
+import time
+import requests
 from typing import Optional
 import pandas as pd
 from raga.validators.dataset_validations import DatasetValidator
 from raga.dataset_creds import DatasetCreds
 from raga import TestSession
 import logging
 import zipfile
-from raga.utils import get_file_name, delete_files, upload_file, create_csv_and_zip_from_data_frame, data_frame_extractor, make_arg
+from raga.utils import get_file_name, delete_files, upload_file, create_csv_and_zip_from_data_frame, data_frame_extractor, make_arg, on_upload_success, on_upload_failed
 
 logger = logging.getLogger(__name__)
-class Dataset:
+class Dataset():
+    MAX_RETRIES = 3
+    RETRY_DELAY = 1
+
     def __init__(
         self,
         test_session:TestSession,
         name: str,
         creds: Optional[DatasetCreds] = None,
+        u_test = False
     ):
         self.test_session = test_session
         self.name = DatasetValidator.validate_name(name)
         self.creds = DatasetValidator.validate_creds(creds)
         self.csv_file = f"experiment_{test_session.experiment_id}.csv"
         self.zip_file = f"experiment_{test_session.experiment_id}.zip"
-        self.dataset_id = self.create_dataset()
-    
-    def load(
+        self.dataset_id = None
+        if not u_test:
+            self.dataset_id = self.create_dataset()
+        self.dataset_file_id = None
+        self.data_set_top_five_rows = {}
+
+
+    def initialize(
         self,
         data = None, 
         schema = None, 
         format= None,
         model_name = None,
         inference_col_name= None,
-        embedding_col_name= None
-    ):
+        embedding_col_name= None):
         from raga import RagaSchema
         # Validate and process the data argument
         if data is not None:
             if isinstance(data, str):
                 # Assume it's a file path
                 self.load_labels_from_file(
                 data,
                 format,
                 model_name,
                 inference_col_name,
                 embedding_col_name
             )
             elif isinstance(data, pd.DataFrame):
-                # Validate and process the schema argument
-                if schema is not None:
-                    if isinstance(schema, RagaSchema):
-                        # Use the provided schema object
-                        dataset_column = schema.columns
-                        # Use the provided DataFrame
-                        self.load_data_frame(data_frame_extractor(data), dataset_column)
-                        # print(json.dumps(dataset_column))
 
-                    else:
-                        raise ValueError("Invalid schema argument. Expected an instance of RagaSchema.")
+                if not data.empty:
+                    # Validate and process the schema argument
+                    if schema is not None:
+                        if isinstance(schema, RagaSchema):
+                            # Use the provided schema object
+                            dataset_column = schema.columns
+                            # Use the provided DataFrame
+                            self.load_data_frame(data_frame_extractor(data), dataset_column)
+                            # print(json.dumps(dataset_column))
+
+                        else:
+                            raise ValueError("Invalid schema argument. Expected an instance of RagaSchema.")
+                else:
+                    raise ValueError("Empty DataFrame data argument.")
             else:
                 raise ValueError("Invalid data argument. Expected a DataFrame or a file path.")
+    
+    def load(
+        self,
+        data = None, 
+        schema = None, 
+        format= None,
+        model_name = None,
+        inference_col_name= None,
+        embedding_col_name= None
+    ):
+        retries = 0
+        while retries < self.MAX_RETRIES:
+            try:
+                self.initialize(data, schema, format, model_name, inference_col_name, embedding_col_name)
+                print("Data loaded successful!")
+                break  # Exit the loop if initialization succeeds
+            except requests.exceptions.RequestException as e:
+                print(f"Network error occurred: {str(e)}")
+                retries += 1
+                if retries < self.MAX_RETRIES:
+                    print(f"Retrying in {self.RETRY_DELAY} second(s)...")
+                    time.sleep(self.RETRY_DELAY)
+            except KeyError as e:
+                print(f"Key error occurred: {str(e)}")
+                sys.exit()# No need to retry if a KeyError occurs 
+            except ValueError as e:
+                print(f"Value error occurred: {str(e)}")
+                sys.exit() # No need to retry if a ValueError occurs
+            except Exception as e:
+                print(f"An unexpected error occurred: {str(e)}")
+                sys.exit() # No need to retry if an unexpected error occurs
 
 
     def load_data_frame(self, data_frame:pd.DataFrame, dataset_column):
         """
         Loads the data frame, creates a CSV file, zips it, and uploads it to the server.
         """
         logger.debug("Loading Data Frames")
         create_csv_and_zip_from_data_frame(data_frame, self.csv_file, self.zip_file)
         signedUploadPath, filePath = self.get_pre_signed_s3_url(self.zip_file)
         upload_file(
             signedUploadPath,
             self.zip_file,
-            success_callback=self.on_upload_success,
-            failure_callback=self.on_upload_failed,
+            success_callback=on_upload_success,
+            failure_callback=on_upload_failed,
         )
         delete_files(self.csv_file, self.zip_file)
 
-        self.create_dataset_load_definition(self.dataset_id, filePath, "csv", dataset_column)
+        self.dataset_file_id = self.create_dataset_load_definition(filePath, "csv", dataset_column)
         self.notify_server()
 
+        self.put_head(self.name, data_frame)
+
     def load_labels_from_file(
         self,
         path_to_file,
         format,
         model_name,
         inference_col_name,
         embedding_col_name
@@ -129,17 +177,32 @@
             os.remove(zip_file_name)
             logger.debug("Zip file deleted")
         else:
             logger.debug("Zip file not found")
 
         arguments = make_arg(model_name, inference_col_name, embedding_col_name)
 
-        self.create_dataset_load_definition(self.dataset_id, filePath, format, arguments)
+        self.dataset_file_id = self.create_dataset_load_definition(filePath, format, arguments)
         self.notify_server()
 
+
+    def head(self):
+        print(f'Dataset Name: {self.data_set_top_five_rows.get("Dataset Name:")}')
+        print(self.data_set_top_five_rows.get("Rows"))
+
+
+    def put_head(self, dataset, data_f: pd.DataFrame):
+        if len(data_f) >= 5:
+            top_5 = data_f.head(5)
+        else:
+            top_5 = data_f
+        self.data_set_top_five_rows["Dataset Name:"] = dataset
+        self.data_set_top_five_rows["Rows"] = top_5
+
+
     def get_pre_signed_s3_url(self, file_name: str):
         """
         Generates a pre-signed URL for uploading the file to an S3 bucket.
 
         Args:
             file_name (str): The name of the file.
 
@@ -160,122 +223,48 @@
 
 
     def notify_server(self):
         """
         Notifies the server to load the dataset with the provided experiment ID and data definition.
         """
         res_data = self.test_session.http_client.post(
-            "api/experiment/pushtoes",
-            {"experimentId": self.test_session.experiment_id, "dataDefinition": ""},
+            "api/experiment/load-data",
+            {"experimentId": self.test_session.experiment_id, "datasetFileId": self.dataset_file_id},
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
-        print("Notified ES server")
+        print(json.dumps(res_data.get('data', {})))
         return res_data
 
     def create_dataset(self):
-        if not self.name:
-            raise ValueError("Dataset name is required.")
         if not self.test_session.project_id:
             raise ValueError("Project ID is required.")
         if not self.test_session.token:
             raise ValueError("Token is required.")
 
         res_data = self.test_session.http_client.post(
             "api/dataset",
-            {"name": self.name, "projectId": self.test_session.project_id},
+            {"name": self.name, "projectId": self.test_session.project_id, "experimentId":self.test_session.experiment_id},
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
 
         if not res_data or 'data' not in res_data or 'id' not in res_data['data']:
             raise ValueError("Failed to create dataset.")
 
         return res_data['data']['id']
 
-    def create_dataset_asset_credentials(self, credentials):
-        # res_data = self.test_session.http_client.post(
-        #     "api/dataset/credential",
-        #     {"datasetId": self.dataset_id, "credentials": credentials},
-        #     {"Authorization": f'Bearer {self.test_session.token}'},
-        # )
-        # return res_data["data"]
-        return 1
-
-    def create_dataset_file(self, filePath):
-        res_data = self.test_session.http_client.post(
-            "api/dataset/file",
-            {"datasetId": self.dataset_id, "filePath": filePath},
-            {"Authorization": f'Bearer {self.test_session.token}'},
-        )
-        return res_data["data"]["id"]
-
-    def create_dataset_file(self, filePath):
-        if not self.dataset_id:
-            raise ValueError("Dataset ID is required.")
-        if not filePath:
-            raise ValueError("File path is required.")
-        if not self.test_session.token:
-            raise ValueError("Token is required.")
-
-        res_data = self.test_session.http_client.post(
-            "api/dataset/file",
-            {"datasetId": self.dataset_id, "filePath": filePath},
-            {"Authorization": f'Bearer {self.test_session.token}'},
-        )
-
-        if not res_data or 'data' not in res_data or 'id' not in res_data['data']:
-            raise ValueError("Failed to create dataset file.")
-
-        return res_data['data']['id']
-
-
-    def create_dataset_columns(self, columns):
-        if not self.dataset_id:
-            raise ValueError("Dataset ID is required.")
-        if not columns:
-            raise ValueError("Columns data is required.")
-        if not self.test_session.token:
-            raise ValueError("Token is required.")
-
-        payload = {
-            "datasetId": self.dataset_id,
-            "columns": columns
-        }
-
-        res_data = self.test_session.http_client.post(
-            "api/dataset/columns", payload,
-            {"Authorization": f'Bearer {self.test_session.token}'},
-        )
-
-        if not res_data or 'data' not in res_data:
-            raise ValueError("Failed to create dataset columns.")
-
-        return res_data["data"]
     
-    def create_dataset_load_definition(self, dataset_file_id: str, filePath: str, type: str, arguments: dict):
+    def create_dataset_load_definition(self, filePath: str, type: str, arguments: dict):
         payload = {
             "datasetId": self.dataset_id,
-            "dataset_file_id": dataset_file_id,
             "filePath": filePath,
             "type": type,
             "arguments": arguments
         }
 
         res_data = self.test_session.http_client.post(
             "api/dataset/definition", payload,
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
-        return res_data["data"]
+        return res_data.get('data',{}).get('id')
 
 
-    def on_upload_success(self):
-        """
-        Callback function to be called on successful file upload.
-        """
-        logger.debug("File uploaded successfully")
-        print("File uploaded successfully")
 
-    def on_upload_failed(self, error):
-        """
-        Callback function to be called on file upload failure.
-        """
-        logger.debug(f"ERROR: {error}")
-        print("File upload failed")
```

### Comparing `raga-testing-platform-1.0.8/raga/examples/MA.json` & `raga-testing-platform-1.0.9/raga/examples/MA.json`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/examples/MB.json` & `raga-testing-platform-1.0.9/raga/examples/MB.json`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/examples/example2.py` & `raga-testing-platform-1.0.9/raga/examples/code_testing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from raga import *
 import pandas as pd
 import json
+import ast
 
-ds_json_file = "MA.json"
+ds_json_file = "MB.json"
 
 test_df = []
 with open(ds_json_file, 'r') as json_file:
     # Load JSON data
     json_data = json.load(json_file)
     
     # Process the JSON data
     transformed_data = []
     for item in json_data:
         AnnotationsV1 = ImageDetectionObject()
         ROIVectorsM1 = ROIEmbedding()
         ImageVectorsM1 = ImageEmbedding()
         for detection in item["outputs"][0]["detections"]:
-            AnnotationsV1.add(ObjectDetection(Id=item["inputs"][0], ClassName=detection['class'], Confidence=detection['confidence'], Format="xywh_normalized"))
+            AnnotationsV1.add(ObjectDetection(Id=0, ClassId=0, ClassName=detection['class'], Confidence=detection['confidence'], BBox= detection['bbox'], Format="xywh_normalized"))
             for roi_emb in detection['roi_embedding']:
                 ROIVectorsM1.add(Embedding(roi_emb))
         
         attributes_dict = {}
         attributes = item.get("attributes", {})
         for key, value in attributes.items():
             attributes_dict[key] = StringElement(value)
@@ -28,37 +29,58 @@
         image_embeddings = item.get("image_embedding", {})
         for value in image_embeddings:
             ImageVectorsM1.add(Embedding(value))
 
         data_point = {
             'ImageId': StringElement(item["inputs"][0]),
             'TimeOfCapture': TimeStampElement(item["capture_time"]),
-            'SourceLink': StringElement(item["source"]),
+            'SourceLink': StringElement(item["inputs"][0]),
             'AnnotationsV1': AnnotationsV1,
             'ROIVectorsM1': ROIVectorsM1,
             'ImageVectorsM1': ImageVectorsM1,
         }
 
         merged_dict = {**data_point, **attributes_dict}
 
         test_df.append(merged_dict)
         
 
 pd_ds = pd.DataFrame(test_df)
 
-# print(data_frame_extractor(pd_ds).to_csv("MA_new.csv"))
+
+# data_frame_extractor(pd_ds).to_csv("MB_new.csv", index=False)
+
 schema = RagaSchema()
 schema.add("ImageId", PredictionSchemaElement())
 schema.add("TimeOfCapture", TimeOfCaptureSchemaElement())
 schema.add("SourceLink", FeatureSchemaElement())
 schema.add("Resolution", AttributeSchemaElement())
 schema.add("Scene", AttributeSchemaElement())
-schema.add("AnnotationsV1", InferenceSchemaElement(model="57_baseline"))
-schema.add("ImageVectorsM1", ImageEmbeddingSchemaElement(model="57_baseline", ref_col_name=""))
-schema.add("ROIVectorsM1", RoiEmbeddingSchemaElement(model="57_baseline", ref_col_name=""))
-
-test_session = TestSession("testingProject", "test_exp_serve_5")
+schema.add("AnnotationsV1", InferenceSchemaElement(model="57_improved"))
+schema.add("ImageVectorsM1", ImageEmbeddingSchemaElement(model="57_improved", ref_col_name=""))
+schema.add("ROIVectorsM1", RoiEmbeddingSchemaElement(model="57_improved", ref_col_name=""))
+
+test_session = TestSession("testingProject", "test_exp_serve_test_31")
+
+# Create an instance of the Dataset class
+test_ds = Dataset(test_session, "ServeDataset_6")
+
+# test_ds.load(pd_ds, schema)
+# test_ds.head()
+
+
+modelA = StringElement("modelA")
+modelB = StringElement("modelB")
+gt = StringElement("GT")
+labelled_type = ModelABTestTypeElement("labelled")
+unlabelled_type = ModelABTestTypeElement("unlabelled")
+aggregation_level = AggregationLevelElement()
+aggregation_level.add(StringElement("weather"))
+aggregation_level.add(StringElement("scene"))
+aggregation_level.add(StringElement("time_of_day"))
+rules = ModelABTestRules()
+rules.add(metric = StringElement("precision_diff"), IoU = FloatElement(0.5), _class = StringElement("all"), threshold = FloatElement(0.05))
+rules.add(metric = StringElement("‘difference_count’"), IoU = FloatElement(0.5), _class = StringElement("‘vehicle’"), threshold = FloatElement(0.05))
 
-# # # Create an instance of the Dataset class
-test_ds = Dataset(test_session, "ServeDataset_5")
+model_comparison_check = model_ab_test(test_ds, modelA = modelA , modelB = modelB , gt = gt,  type = labelled_type, aggregation_level = aggregation_level, rules = rules)
 
-test_ds.load(pd_ds, schema)
+model_comparison_check = model_ab_test(test_ds, modelA = modelA , modelB = modelB , type = unlabelled_type, aggregation_level = aggregation_level, rules = rules)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `raga-testing-platform-1.0.8/raga/raga_schema.py` & `raga-testing-platform-1.0.9/raga/raga_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self.type: str
         self.model: Optional[str]
         self.ref_col_name: Optional[str]
 
 class PredictionSchemaElement(RagaSchemaElement):
     def __init__(self):
         super().__init__()
-        self.type = "prediction"
+        self.type = "imageName"
         self.model = ""
         self.ref_col_name = ""
 
 class TimeOfCaptureSchemaElement(RagaSchemaElement):
     def __init__(self):
         super().__init__()
         self.type = "timestamp"
@@ -67,21 +67,58 @@
 
 class StringElement():
     def __init__(self, value:str):
         self.value = value
 
     def get(self):
         return self.value
+    
+class FloatElement():
+    def __init__(self, value:float):
+        self.value = value
+
+    def get(self):
+        return self.value
+    
 class TimeStampElement():
     def __init__(self, date_time:datetime):
         self.date_time = date_time
 
     def get(self):
         return self.date_time
+    
+class AggregationLevelElement():
+    def __init__(self):
+        self.levels = []
+
+    def add(self, level:StringElement):
+        self.levels.append(level.get())
+
+    def get(self):
+        return self.levels
+    
+class ModelABTestTypeElement():
+    def __init__(self, type:str):
+        self.type = type
+        if self.type not in ["labelled", "unlabelled"]:
+            raise ValueError("Invalid value for 'type'. Must be one of: ['labelled', 'unlabelled'].")
+
+    def get(self):
+        return self.type    
 
+       
+class ModelABTestRules():
+    def __init__(self):
+        self.rules = []
+
+    def add(self, metric:StringElement, IoU:FloatElement, _class:StringElement, threshold:FloatElement):
+        self.rules.append({ "metric" : metric.get(), "iou": IoU.get(),  "class": _class.get(), "threshold":threshold.get() })
+
+    def get(self):
+        return self.rules
 class ObjectDetection:
     def __init__(self, Id:Optional[str], Format:Optional[str], Confidence:Optional[float], ClassId:Optional[str] = None, ClassName:Optional[str]=None, BBox=None):
         self.Id = Id
         self.ClassId = ClassId
         self.ClassName = ClassName
         self.BBox = BBox
         self.Format = Format
```

### Comparing `raga-testing-platform-1.0.8/raga/test_session.py` & `raga-testing-platform-1.0.9/raga/test_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from raga.utils import HTTPClient
 from raga.utils import read_raga_config, get_config_value
 
 class TestSession():
     MAX_RETRIES = 3
     RETRY_DELAY = 1
 
-    def __init__(self, project_name: str, run_name: str):
+    def __init__(self, project_name: str, run_name: str, u_test=False):
         config_data = read_raga_config()
         self.project_name = TestSessionValidator.validate_project_name(project_name)
         self.run_name = TestSessionValidator.validate_run_name(run_name)
         self.api_host = get_config_value(config_data, 'default', 'api_host')
         self.raga_access_key_id = get_config_value(config_data, 'default', 'raga_access_key_id')
         self.raga_secret_access_key = get_config_value(config_data, 'default', 'raga_secret_access_key')
         self.http_client = HTTPClient(self.api_host)
 
         self.token = None
         self.project_id = None
         self.experiment_id = None
-        self.initialize()
+        if not u_test:
+            self.initialize()
     
     def initialize(self):
         retries = 0
         while retries < self.MAX_RETRIES:
             try:
                 self.token = self.create_token()
                 self.project_id = self.get_project_id()
@@ -36,24 +37,21 @@
                 print(f"Network error occurred: {str(e)}")
                 retries += 1
                 if retries < self.MAX_RETRIES:
                     print(f"Retrying in {self.RETRY_DELAY} second(s)...")
                     time.sleep(self.RETRY_DELAY)
             except KeyError as e:
                 print(f"Key error occurred: {str(e)}")
-                sys.exit()
-                break  # No need to retry if a KeyError occurs
+                sys.exit() # No need to retry if a KeyError occurs
             except ValueError as e:
                 print(f"Value error occurred: {str(e)}")
-                sys.exit()
-                break  # No need to retry if a ValueError occurs
+                sys.exit() # No need to retry if a ValueError occurs
             except Exception as e:
                 print(f"An unexpected error occurred: {str(e)}")
-                sys.exit()
-                break  # No need to retry if an unexpected error occurs
+                sys.exit()  # No need to retry if an unexpected error occurs
 
     def create_token(self):
         """
         Creates an authentication token by sending a request to the Raga API.
 
         Returns:
             str: The authentication token.
```

### Comparing `raga-testing-platform-1.0.8/raga/tests/test_dataset.py` & `raga-testing-platform-1.0.9/raga/tests/test_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,46 +39,14 @@
         self.assertEqual(file_id, expected_file_id)
         mock_create_dataset_file.assert_called_once_with(
             "api/dataset/file",
             {"datasetId": self.dataset.dataset_id, "filePath": "path/to/file.csv"},
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
 
-    def test_create_dataset_columns(self):
-        expected_columns = [
-            {
-                "name": "image_id",
-                "model": "",
-                "type": "prediction",
-                "description": "",
-            },
-            {
-                "name": "label_name",
-                "model": "label_name",
-                "type": "inferences",
-                "description": "",
-            },
-            {
-                "name": "col_name",
-                "model": "label_name",
-                "type": "roi",
-                "description": "",
-            }
-        ]
-        mock_create_dataset_columns = MagicMock(return_value={"data": expected_columns})
-        self.test_session.http_client.post = mock_create_dataset_columns
-
-        columns = self.dataset.create_dataset_columns(expected_columns)
-
-        self.assertEqual(columns, expected_columns)
-        mock_create_dataset_columns.assert_called_once_with(
-            "api/dataset/columns",
-            {"datasetId": self.dataset.dataset_id, "columns": expected_columns},
-            {"Authorization": f'Bearer {self.test_session.token}'},
-        )
 
     def test_get_pre_signed_s3_url(self):
         expected_signed_upload_path = "https://s3.amazonaws.com/my-bucket/upload"
         expected_file_path = "my-bucket/folder/file.zip"
         mock_get_pre_signed_url = MagicMock(return_value={"data": {"signedUploadPath": expected_signed_upload_path, "filePath": expected_file_path}})
         self.test_session.http_client.get = mock_get_pre_signed_url
 
@@ -117,48 +85,14 @@
         mock_post.assert_called_once_with(
             "api/dataset/file",
             {"datasetId": "dataset_id", "filePath": "file_path"},
             {"Authorization": "Bearer token"},
         )
         self.assertEqual(file_id, "file_id")
 
-    def test_create_dataset_columns(self):
-        self.dataset.dataset_id = "dataset_id"
-        columns = [
-            {
-                "name": "image_id",
-                "model": "",
-                "type": "prediction",
-                "description": "",
-            },
-            {
-                "name": "label_name",
-                "model": "label_name",
-                "type": "inferences",
-                "description": "",
-            },
-            {
-                "name": "col_name",
-                "model": "label_name",
-                "type": "roi",
-                "description": "",
-            },
-        ]
-        mock_post = MagicMock(return_value={"data": "columns_data"})
-        self.test_session.http_client.post = mock_post
-
-        result = self.dataset.create_dataset_columns(columns)
-
-        mock_post.assert_called_once_with(
-            "api/dataset/columns",
-            {"datasetId": "dataset_id", "columns": columns},
-            {"Authorization": "Bearer token"},
-        )
-        self.assertEqual(result, "columns_data")
-
     def test_create_dataset_load_definition(self):
         self.dataset.dataset_id = "dataset_id"
         dataset_file_id = "file_id"
         file_path = "file_path"
         data_type = "pandas"
         arguments = {"arg1": "value1", "arg2": "value2"}
         mock_post = MagicMock(return_value={"data": "load_definition_data"})
```

### Comparing `raga-testing-platform-1.0.8/raga/tests/test_dataset_util.py` & `raga-testing-platform-1.0.9/raga/tests/test_dataset_util.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/tests/test_http_client.py` & `raga-testing-platform-1.0.9/raga/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/tests/test_test_session.py` & `raga-testing-platform-1.0.9/raga/tests/test_test_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import unittest
+from unittest import mock
 from unittest.mock import MagicMock, patch, Mock, call
 from requests import Response
 import requests
 from raga import TestSession
 
 class TestTestSession(unittest.TestCase):
 
     def setUp(self):
         self.project_name = "project_name"
         self.run_name = "run_name"
         self.mock_http_client = MagicMock()
-        self.test_session = TestSession(self.project_name, self.run_name)
+        self.test_session = TestSession(self.project_name, self.run_name, u_test=True)
         self.test_session.http_client = self.mock_http_client
 
     def test_create_token(self):
         expected_token = "token"
         mock_response_data = {"data": {"token": expected_token}}
         self.mock_http_client.post.return_value = mock_response_data
 
@@ -69,15 +70,15 @@
         # Call the method and assert it raises a KeyError
         with self.assertRaises(KeyError):
             self.test_session.create_experiment()
 
     @patch("raga.test_session.HTTPClient")
     def test_get_project_id(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
 
         # Mock the HTTPClient instance and its get method
         mock_get = Mock(return_value={"data": {"id": "project_id"}})
         mock_http_client.return_value.get = mock_get
 
         # Call the get_project_id method
         project_id = test_session.get_project_id()
@@ -92,15 +93,15 @@
 
         # Verify the returned project_id
         self.assertEqual(project_id, "project_id")
 
     @patch("raga.test_session.HTTPClient")
     def test_get_project_id_no_data(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
         # Mock the HTTPClient instance and its get method
         mock_get = Mock(return_value={})
         mock_http_client.return_value.get = mock_get
 
         with self.assertRaises(KeyError):
             test_session.get_project_id()
 
@@ -110,15 +111,15 @@
             params={"name": "project_name"},
             headers={"Authorization": f'Bearer {self.test_session.token}'},
         )
 
     @patch("raga.test_session.HTTPClient")
     def test_get_project_id_invalid_response(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
         # Mock the HTTPClient instance and its get method
         mock_get = Mock(return_value="invalid_response")
         mock_http_client.return_value.get = mock_get
 
         with self.assertRaises(ValueError):
             test_session.get_project_id()
 
@@ -128,15 +129,15 @@
             params={"name": "project_name"},
             headers={"Authorization": f'Bearer {self.test_session.token}'},
         )
 
     @patch("raga.test_session.HTTPClient")
     def test_create_experiment(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
         # Mock the HTTPClient instance and its post method
         mock_post = Mock(return_value={"data": {"id": "experiment_id"}})
         mock_http_client.return_value.post = mock_post
 
         experiment_id = test_session.create_experiment()
 
         mock_http_client.assert_called_once()
@@ -146,15 +147,15 @@
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
         self.assertEqual(experiment_id, "experiment_id")
 
     @patch("raga.test_session.HTTPClient")
     def test_create_experiment_no_data(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
         # Mock the HTTPClient instance and its post method
         mock_post = Mock(return_value={})
         mock_http_client.return_value.post = mock_post
 
         with self.assertRaises(KeyError):
             test_session.create_experiment()
 
@@ -164,15 +165,15 @@
             {"name": "run_name", "projectId": self.test_session.project_id},
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
 
     @patch("raga.test_session.HTTPClient")
     def test_create_experiment_invalid_response(self, mock_http_client):
         # Create a TestSession instance
-        test_session = TestSession("project_name", "run_name")
+        test_session = TestSession("project_name", "run_name", u_test=True)
         # Mock the HTTPClient instance and its post method
         mock_post = Mock(return_value="invalid_response")
         mock_http_client.return_value.post = mock_post
 
         with self.assertRaises(ValueError):
             test_session.create_experiment()
 
@@ -228,16 +229,16 @@
             ]
             mock_print.assert_has_calls(expected_calls)
             self.assertEqual(mock_print.call_count, len(expected_calls))
             self.assertEqual(mock_create_token.call_count, self.test_session.MAX_RETRIES)
             self.assertEqual(mock_get_project_id.call_count, 0)
             self.assertEqual(mock_create_experiment.call_count, 0)
 
-
-    def test_initialize_key_error(self):
+    @mock.patch('sys.exit')
+    def test_initialize_key_error(self, mock_exit):
         mock_create_token = MagicMock(return_value="token")
         mock_get_project_id = MagicMock(side_effect=KeyError("Invalid response data"))
         mock_create_experiment = MagicMock()
 
         self.test_session.create_token = mock_create_token
         self.test_session.get_project_id = mock_get_project_id
         self.test_session.create_experiment = mock_create_experiment
@@ -251,16 +252,17 @@
                 call("Key error occurred: 'Invalid response data'")
             ]
             mock_print.assert_has_calls(expected_calls, any_order=False)
             self.assertEqual(mock_print.call_count, 1)
             self.assertEqual(mock_create_token.call_count, 1)
             self.assertEqual(mock_get_project_id.call_count, 1)
             self.assertEqual(mock_create_experiment.call_count, 0)
-
-    def test_initialize_value_error(self):
+            
+    @mock.patch('sys.exit')
+    def test_initialize_value_error(self, mock_exit):
         mock_create_token = MagicMock(return_value="token")
         mock_get_project_id = MagicMock(side_effect=ValueError("Invalid response data. Expected a dictionary."))
         mock_create_experiment = MagicMock()
 
         self.test_session.create_token = mock_create_token
         self.test_session.get_project_id = mock_get_project_id
         self.test_session.create_experiment = mock_create_experiment
@@ -275,16 +277,16 @@
             ]
             mock_print.assert_has_calls(expected_calls, any_order=False)
             self.assertEqual(mock_print.call_count, 1)
             self.assertEqual(mock_create_token.call_count, 1)
             self.assertEqual(mock_get_project_id.call_count, 1)
             self.assertEqual(mock_create_experiment.call_count, 0)
 
-
-    def test_initialize_unexpected_error(self):
+    @mock.patch('sys.exit')
+    def test_initialize_unexpected_error(self, mock_exit):
         mock_create_token = MagicMock(return_value="token")
         mock_get_project_id = MagicMock(return_value="project_id")
         mock_create_experiment = MagicMock(side_effect=Exception("An unexpected error occurred"))
 
         self.test_session.create_token = mock_create_token
         self.test_session.get_project_id = mock_get_project_id
         self.test_session.create_experiment = mock_create_experiment
```

### Comparing `raga-testing-platform-1.0.8/raga/utils/dataset_util.py` & `raga-testing-platform-1.0.9/raga/utils/dataset_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -101,8 +101,22 @@
         logger.debug("CSV file not found")
 
     if os.path.exists(zip_file):
         os.remove(zip_file)
         logger.debug("Zip file deleted")
     else:
         logger.debug("Zip file not found")
-        
+        
+
+def on_upload_success():
+    """
+    Callback function to be called on successful file upload.
+    """
+    logger.debug("File uploaded successfully")
+    print("File uploaded successfully")
+
+def on_upload_failed(error):
+    """
+    Callback function to be called on file upload failure.
+    """
+    logger.debug(f"ERROR: {error}")
+    print("File upload failed")
```

### Comparing `raga-testing-platform-1.0.8/raga/utils/file.py` & `raga-testing-platform-1.0.9/raga/utils/file.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/utils/http_client.py` & `raga-testing-platform-1.0.9/raga/utils/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,7 +114,9 @@
             return json_data
         else:
             error_message = json_data.get("message")
             if error_message:
                 raise ValueError(f"Request failed with status code {status_code}: {error_message}")
             else:
                 raise ValueError(f"Request failed with status code {status_code}")
+
+
```

### Comparing `raga-testing-platform-1.0.8/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.0.9/raga/utils/raga_config_reader.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.0.9/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.0.8/raga/validators/dataset_validations.py` & `raga-testing-platform-1.0.9/raga/validators/dataset_validations.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,20 @@
         # Additional validation logic specific to test_df, e.g., checking required columns or shape
         return test_df
 
     @staticmethod
     def validate_name(name: str) -> str:
         if not name:
             raise ValueError("Name is required.")
+        
+        # Check if name contains any special characters except "_"
+        allowed_chars = set("._abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789 ")
+
+        if not set(name).issubset(allowed_chars):
+            raise ValueError("Name should only contain alphanumeric characters and '_', '.'.")
         # Additional validation logic specific to name, e.g., checking length or format
         return name
 
     @staticmethod
     def validate_creds(creds: Optional[DatasetCreds] = None) -> Optional[DatasetCreds]:
         if creds is not None and not isinstance(creds, DatasetCreds):
             raise TypeError("DatasetCreds must be an instance of the DatasetCreds class.")
```

### Comparing `raga-testing-platform-1.0.8/raga_testing_platform.egg-info/PKG-INFO` & `raga-testing-platform-1.0.9/raga_testing_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.0.8
+Version: 1.0.9
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.0.8/raga_testing_platform.egg-info/SOURCES.txt` & `raga-testing-platform-1.0.9/raga_testing_platform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 .DS_Store
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 raga/__init__.py
+raga/_tests.py
 raga/dataset.py
 raga/dataset_creds.py
 raga/raga_schema.py
 raga/test_session.py
-raga/tests.py
 raga/docs/conf.py
 raga/docs/index.rst
 raga/examples/.DS_Store
 raga/examples/MA.json
 raga/examples/MB.json
+raga/examples/code_testing.py
 raga/examples/example.py
-raga/examples/example2.py
 raga/tests/__init__.py
 raga/tests/test_dataset.py
 raga/tests/test_dataset_util.py
 raga/tests/test_http_client.py
 raga/tests/test_test_session.py
+raga/tests/test_tests.py
 raga/utils/__init__.py
 raga/utils/dataset_util.py
 raga/utils/file.py
 raga/utils/http_client.py
 raga/utils/raga_config_reader.py
 raga/validators/dataset_creds_validations.py
 raga/validators/dataset_validations.py
```

