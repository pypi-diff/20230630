# Comparing `tmp/prolog_primitives-0.2.0.tar.gz` & `tmp/prolog_primitives-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-0.2.0.tar", last modified: Thu Jun 29 21:18:20 2023, max compression
+gzip compressed data, was "prolog_primitives-0.3.0.tar", last modified: Fri Jun 30 09:03:28 2023, max compression
```

## Comparing `prolog_primitives-0.2.0.tar` & `prolog_primitives-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:18:20.799777 prolog_primitives-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 21:18:20.799777 prolog_primitives-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:18:20.799777 prolog_primitives-0.2.0/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 21:18:13.000000 prolog_primitives-0.2.0/prolog_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/prolog_primitives/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:18:20.799777 prolog_primitives-0.2.0/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 21:18:20.000000 prolog_primitives-0.2.0/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 21:18:20.799777 prolog_primitives-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-29 21:16:45.000000 prolog_primitives-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/ntPrimitive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.198164 prolog_primitives-0.3.0/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.198164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/Collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:03:27.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/setup.py
```

### Comparing `prolog_primitives-0.2.0/LICENSE` & `prolog_primitives-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.2.0/PKG-INFO` & `prolog_primitives-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 0.2.0
+Version: 0.3.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.2.0/prolog_primitives/__main__.py` & `prolog_primitives-0.3.0/prolog_primitives/__main__.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.2.0/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-0.3.0/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 0.2.0
+Version: 0.3.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.2.0/setup.py` & `prolog_primitives-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         with version_file.open('w') as f:
             f.write(version)
         return version
     except subprocess.CalledProcessError:
         if version_file.exists():
             return version_file.read_text().strip()
         else:
-            return '0.2.0'
+            return '0.3.0'
 
 
 version = get_version_from_git()
 
 
 print(f"Detected version {version} from git describe")
```

