# Comparing `tmp/tf_nightly_cpu-2.14.0.dev20230629-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly_cpu-2.14.0.dev20230630-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 2098 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     2626 b- defN 23-Jun-29 07:50 tf_nightly_cpu-2.14.0.dev20230629.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 23-Jun-29 07:50 tf_nightly_cpu-2.14.0.dev20230629.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-29 07:50 tf_nightly_cpu-2.14.0.dev20230629.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      377 b- defN 23-Jun-29 07:50 tf_nightly_cpu-2.14.0.dev20230629.dist-info/RECORD
+-rw-rw-r--  2.0 unx     2626 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      377 b- defN 23-Jun-30 07:51 tf_nightly_cpu-2.14.0.dev20230630.dist-info/RECORD
 4 files, 3103 bytes uncompressed, 1356 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly_cpu-2.14.0.dev20230629.dist-info/METADATA
+Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230629.dist-info/WHEEL
+Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230629.dist-info/top_level.txt
+Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly_cpu-2.14.0.dev20230629.dist-info/RECORD
+Filename: tf_nightly_cpu-2.14.0.dev20230630.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly_cpu-2.14.0.dev20230629.dist-info/METADATA` & `tf_nightly_cpu-2.14.0.dev20230630.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly-cpu
-Version: 2.14.0.dev20230629
+Version: 2.14.0.dev20230630
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -25,17 +25,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-macos (==2.14.0-dev20230629) ; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230629) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tf-nightly-intel (==2.14.0-dev20230629) ; platform_system == "Windows"
+Requires-Dist: tf-nightly-macos (==2.14.0-dev20230630) ; platform_system == "Darwin" and platform_machine == "arm64"
+Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230630) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
+Requires-Dist: tf-nightly-intel (==2.14.0-dev20230630) ; platform_system == "Windows"
 
 [![Python](https://img.shields.io/pypi/pyversions/tensorflow.svg?style=plastic)](https://badge.fury.io/py/tensorflow)
 [![PyPI](https://badge.fury.io/py/tensorflow.svg)](https://badge.fury.io/py/tensorflow)
 
 TensorFlow is an open source software library for high performance numerical
 computation. Its flexible architecture allows easy deployment of computation
 across a variety of platforms (CPUs, GPUs, TPUs), and from desktops to clusters
```

