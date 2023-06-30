# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230627-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230628-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 2404459 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Jun-28 05:01 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6832592 b- defN 23-Jun-28 05:03 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Jun-28 05:01 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Jun-28 05:01 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Jun-28 05:01 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-28 05:03 tflite_runtime_nightly-2.14.0.dev20230627.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Jun-28 05:03 tflite_runtime_nightly-2.14.0.dev20230627.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-28 05:03 tflite_runtime_nightly-2.14.0.dev20230627.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jun-28 05:03 tflite_runtime_nightly-2.14.0.dev20230627.dist-info/RECORD
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jun-29 05:15 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6832592 b- defN 23-Jun-29 05:17 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Jun-29 05:15 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Jun-29 05:15 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Jun-29 05:15 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-29 05:17 tflite_runtime_nightly-2.14.0.dev20230628.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Jun-29 05:17 tflite_runtime_nightly-2.14.0.dev20230628.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-29 05:17 tflite_runtime_nightly-2.14.0.dev20230628.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jun-29 05:17 tflite_runtime_nightly-2.14.0.dev20230628.dist-info/RECORD
 9 files, 6877482 bytes uncompressed, 2402913 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230627.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230628.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230627.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230628.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230627.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230628.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230627.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230628.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230627'
-__git_version__ = '0.6.0-149856-gf0b8b9a1457'
+__version__ = '2.14.0dev20230628'
+__git_version__ = '0.6.0-149943-g7ceb9602172'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230627.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230628.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230627
+Version: 2.14.0.dev20230628
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230627.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230628.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=MrUj0MrbSgcVI_e7wLKKgAIlmQ8KpxHXe6A-UFae1kE,80
+tflite_runtime/__init__.py,sha256=s-lseXxCd2pWqIfqQXRj9paifWfgVSB3aQ9peXf3nGs,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=nkCqLMjFsYt3wCaNbrdho1PCQC-VT6kgm5F0yL22b2I,6832592
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230627.dist-info/METADATA,sha256=7OCLWNMa2CgOCHRJvpKmDuukKf-RWwDs-KTl_UOczIg,1441
-tflite_runtime_nightly-2.14.0.dev20230627.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.14.0.dev20230627.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230627.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230628.dist-info/METADATA,sha256=6ASGPoqZ42XRX6P9aDg7ynKMXkzDfiKT4v7mg_OBHFI,1441
+tflite_runtime_nightly-2.14.0.dev20230628.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.14.0.dev20230628.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230628.dist-info/RECORD,,
```

