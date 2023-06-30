# Comparing `tmp/prolog_primitives-0.3.0.tar.gz` & `tmp/prolog_primitives-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-0.3.0.tar", last modified: Fri Jun 30 09:03:28 2023, max compression
+gzip compressed data, was "prolog_primitives-0.4.0.tar", last modified: Fri Jun 30 13:52:24 2023, max compression
```

## Comparing `prolog_primitives-0.3.0.tar` & `prolog_primitives-0.4.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/basic/ntPrimitive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.198164 prolog_primitives-0.3.0/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 09:03:19.000000 prolog_primitives-0.3.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.198164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/Collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.202164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:03:28.194164 prolog_primitives-0.3.0/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:03:27.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 09:03:28.000000 prolog_primitives-0.3.0/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:03:28.206164 prolog_primitives-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 09:01:35.000000 prolog_primitives-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.336921 prolog_primitives-0.4.0/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/basic/ntPrimitive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 13:52:15.000000 prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.340921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/Collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.344921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:52:24.336921 prolog_primitives-0.4.0/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 13:52:24.000000 prolog_primitives-0.4.0/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:52:24.348921 prolog_primitives-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 13:50:34.000000 prolog_primitives-0.4.0/setup.py
```

### Comparing `prolog_primitives-0.3.0/LICENSE` & `prolog_primitives-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/PKG-INFO` & `prolog_primitives-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 0.3.0
+Version: 0.4.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.3.0/prolog_primitives/__main__.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from .ml_lib.schema.schema import schemaPrimitive
-from .ml_lib.schema.theoryToSchema import theoryToSchemaPrimitive
-from .ml_lib.dataset.theoryToDataset import theoryToDatasetPrimitive
-from .ml_lib.dataset.randomSplit import randomSplitPrimitive
-from .ml_lib.dataset.column import columnPrimitive
-from .ml_lib.dataset.row import rowPrimitive
-from .ml_lib.dataset.cell import cellPrimitive
-from .ml_lib.dataset.fold import foldPrimitive
-from .ml_lib.dataset.theory_from_Dataset import theoryFromDatasetPrimitive
-from .ml_lib.trasformations.schema_trasformation import schemaTrasformation
-from .ml_lib.trasformations.normalization import normalizePrimitive
-from .ml_lib.trasformations.one_hot_encode import one_hot_encodePrimitive
-from .ml_lib.trasformations.drop import dropPrimitive
-from .ml_lib.trasformations.fit import fitPrimitive
-from .ml_lib.trasformations.transform import transformPrimitive
-from .ml_lib.neuralNetwork.inputLayer import inputLayerPrimitive
-from .ml_lib.neuralNetwork.denseLayer import denseLayerPrimitive
-from .ml_lib.neuralNetwork.outputLayer import outputLayerPrimitive
-from .ml_lib.neuralNetwork.neuralNetwork import neuralNetworkPrimitive
-from .ml_lib.predictors.train import trainPrimitive
-from .ml_lib.predictors.predict import predictPrimitive
-from .ml_lib.predictors.classify import classifyPrimitive
-from .ml_lib.predictors.score import msePrimitive
-from .basic import PrimitiveWrapper, DistributedElements
+from .schema.schema import schemaPrimitive
+from .schema.theoryToSchema import theoryToSchemaPrimitive
+from .dataset.theoryToDataset import theoryToDatasetPrimitive
+from .dataset.randomSplit import randomSplitPrimitive
+from .dataset.column import columnPrimitive
+from .dataset.row import rowPrimitive
+from .dataset.cell import cellPrimitive
+from .dataset.fold import foldPrimitive
+from .dataset.theory_from_Dataset import theoryFromDatasetPrimitive
+from .transformations.schema_trasformation import schemaTrasformation
+from .transformations.normalization import normalizePrimitive
+from .transformations.one_hot_encode import one_hot_encodePrimitive
+from .transformations.drop import dropPrimitive
+from .transformations.fit import fitPrimitive
+from .transformations.transform import transformPrimitive
+from .neuralNetwork.inputLayer import inputLayerPrimitive
+from .neuralNetwork.denseLayer import denseLayerPrimitive
+from .neuralNetwork.outputLayer import outputLayerPrimitive
+from .neuralNetwork.neuralNetwork import neuralNetworkPrimitive
+from .predictors.train import trainPrimitive
+from .predictors.predict import predictPrimitive
+from .predictors.classify import classifyPrimitive
+from .predictors.score import msePrimitive
+from ..basic import PrimitiveWrapper, DistributedElements
 from concurrent.futures import ThreadPoolExecutor
 
 servers = []
 libraryName = "customLibrary"
 
 def launchPrimitive(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int):
     server = PrimitiveWrapper.serve(primitive, port, libraryName)
@@ -48,15 +48,14 @@
     future = executor.submit(launchPrimitive, primitive, port)
     port += 1
 
 try:
     for server in servers:
         server.wait_for_termination()
 except (Exception, KeyboardInterrupt, SystemExit) as inst:
-    from .basic import DBManager
     executor.shutdown(wait=False, cancel_futures=True)
     for server in servers:
         server.stop(0)
 
-for primitive in primitives:
-    DBManager.deletePrimitive(primitive.functor, primitive.arity, libraryName)
+#for primitive in primitives:
+#    DBManager.deletePrimitive(primitive.functor, primitive.arity, libraryName)
 print("Done!")
```

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/DBManager.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,22 +44,23 @@
         
         context.add_callback(lambda: queue.put(None))
         while context.is_active():
             msg: primitivesMsg.GeneratorMsg = queue.get()
             if(msg != None):
                 yield msg              
 
-def serve(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int = 8080, libraryName: str = ""):
+def serve(primitive: DistributedElements.DistributedPrimitiveWrapper, port: int = 8080, libraryName: str = "", withDB: bool = False):
     executor = futures.ThreadPoolExecutor(64)
     service = GenericPrimitive(primitive.primitive, primitive.functor, primitive.arity, executor)
     server = grpc.server(executor)
     Server.add_GenericPrimitiveServiceServicer_to_server(service, server)
     server.add_insecure_port('[::]:' + str(port))
     server.start()
-    DBManager.addPrimitive(service.functor, service.arity, libraryName, "localhost", port)
+    if(withDB):
+        DBManager.addPrimitive(service.functor, service.arity, libraryName, "localhost", port)
     print("Server started, listening on " + str(port))
     return server
```

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/Session.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/Utils.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/basic/ntPrimitive.py` & `prolog_primitives-0.4.0/prolog_primitives/basic/ntPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-0.4.0/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-0.4.0/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-0.4.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-0.4.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/Collections.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/Collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/predictors/train.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/drop.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/fit.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/normalization.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/one_hot_encode.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/schema_trasformation.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transform.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives/ml_lib/trasformations/transformationClass.py` & `prolog_primitives-0.4.0/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.3.0/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-0.4.0/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 0.3.0
+Version: 0.4.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.3.0/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-0.4.0/prolog_primitives.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 prolog_primitives/__init__.py
-prolog_primitives/__main__.py
 prolog_primitives.egg-info/PKG-INFO
 prolog_primitives.egg-info/SOURCES.txt
 prolog_primitives.egg-info/dependency_links.txt
 prolog_primitives.egg-info/not-zip-safe
 prolog_primitives.egg-info/requires.txt
 prolog_primitives.egg-info/top_level.txt
 prolog_primitives/basic/DBManager.py
@@ -28,14 +27,15 @@
 prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
 prolog_primitives/generatedProto/primitiveService_pb2.py
 prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
 prolog_primitives/ml_lib/Collections.py
 prolog_primitives/ml_lib/__init__.py
+prolog_primitives/ml_lib/__main__.py
 prolog_primitives/ml_lib/dataset/__init__.py
 prolog_primitives/ml_lib/dataset/cell.py
 prolog_primitives/ml_lib/dataset/column.py
 prolog_primitives/ml_lib/dataset/fold.py
 prolog_primitives/ml_lib/dataset/randomSplit.py
 prolog_primitives/ml_lib/dataset/row.py
 prolog_primitives/ml_lib/dataset/theoryToDataset.py
@@ -50,15 +50,15 @@
 prolog_primitives/ml_lib/predictors/predict.py
 prolog_primitives/ml_lib/predictors/score.py
 prolog_primitives/ml_lib/predictors/train.py
 prolog_primitives/ml_lib/schema/__init__.py
 prolog_primitives/ml_lib/schema/schema.py
 prolog_primitives/ml_lib/schema/schemaClass.py
 prolog_primitives/ml_lib/schema/theoryToSchema.py
-prolog_primitives/ml_lib/trasformations/__init__.py
-prolog_primitives/ml_lib/trasformations/drop.py
-prolog_primitives/ml_lib/trasformations/fit.py
-prolog_primitives/ml_lib/trasformations/normalization.py
-prolog_primitives/ml_lib/trasformations/one_hot_encode.py
-prolog_primitives/ml_lib/trasformations/schema_trasformation.py
-prolog_primitives/ml_lib/trasformations/transform.py
-prolog_primitives/ml_lib/trasformations/transformationClass.py
+prolog_primitives/ml_lib/transformations/__init__.py
+prolog_primitives/ml_lib/transformations/drop.py
+prolog_primitives/ml_lib/transformations/fit.py
+prolog_primitives/ml_lib/transformations/normalization.py
+prolog_primitives/ml_lib/transformations/one_hot_encode.py
+prolog_primitives/ml_lib/transformations/schema_trasformation.py
+prolog_primitives/ml_lib/transformations/transform.py
+prolog_primitives/ml_lib/transformations/transformationClass.py
```

### Comparing `prolog_primitives-0.3.0/setup.py` & `prolog_primitives-0.4.0/setup.py`

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
-            return '0.3.0'
+            return '0.4.0'
 
 
 version = get_version_from_git()
 
 
 print(f"Detected version {version} from git describe")
```

