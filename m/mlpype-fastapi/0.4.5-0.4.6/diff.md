# Comparing `tmp/mlpype-fastapi-0.4.5.tar.gz` & `tmp/mlpype-fastapi-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.4.5.tar", last modified: Mon Jun 26 20:42:43 2023, max compression
+gzip compressed data, was "mlpype-fastapi-0.4.6.tar", last modified: Fri Jun 30 14:22:06 2023, max compression
```

## Comparing `mlpype-fastapi-0.4.5.tar` & `mlpype-fastapi-0.4.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:43.089187 mlpype-fastapi-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:42:43.089187 mlpype-fastapi-0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:42:43.089187 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 20:42:43.000000 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 20:42:43.000000 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:42:43.000000 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 20:42:43.000000 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:42:43.000000 mlpype-fastapi-0.4.5/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:42:43.089187 mlpype-fastapi-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-26 20:39:45.000000 mlpype-fastapi-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:06.583292 mlpype-fastapi-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 14:22:06.583292 mlpype-fastapi-0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:06.583292 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 14:22:06.000000 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-30 14:22:06.000000 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:06.000000 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-30 14:22:06.000000 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:06.000000 mlpype-fastapi-0.4.6/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:06.583292 mlpype-fastapi-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-30 14:18:44.000000 mlpype-fastapi-0.4.6/setup.py
```

### Comparing `mlpype-fastapi-0.4.5/setup.py` & `mlpype-fastapi-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.5"
+    version = "0.4.6"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

