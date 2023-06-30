# Comparing `tmp/mlpype-spark-0.4.5.tar.gz` & `tmp/mlpype-spark-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.4.5.tar", last modified: Mon Jun 26 20:43:11 2023, max compression
+gzip compressed data, was "mlpype-spark-0.4.6.tar", last modified: Fri Jun 30 14:22:39 2023, max compression
```

## Comparing `mlpype-spark-0.4.5.tar` & `mlpype-spark-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:11.521528 mlpype-spark-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 20:43:11.521528 mlpype-spark-0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:43:11.517528 mlpype-spark-0.4.5/mlpype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 20:43:11.000000 mlpype-spark-0.4.5/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-26 20:43:11.000000 mlpype-spark-0.4.5/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:11.000000 mlpype-spark-0.4.5/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 20:43:11.000000 mlpype-spark-0.4.5/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:43:11.000000 mlpype-spark-0.4.5/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:43:11.521528 mlpype-spark-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 20:39:45.000000 mlpype-spark-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:39.967440 mlpype-spark-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 14:22:39.963440 mlpype-spark-0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:39.963440 mlpype-spark-0.4.6/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 14:22:39.000000 mlpype-spark-0.4.6/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 14:22:39.000000 mlpype-spark-0.4.6/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:39.000000 mlpype-spark-0.4.6/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-30 14:22:39.000000 mlpype-spark-0.4.6/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:39.000000 mlpype-spark-0.4.6/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:39.967440 mlpype-spark-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 14:18:44.000000 mlpype-spark-0.4.6/setup.py
```

### Comparing `mlpype-spark-0.4.5/setup.py` & `mlpype-spark-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.5"
+    version = "0.4.6"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

