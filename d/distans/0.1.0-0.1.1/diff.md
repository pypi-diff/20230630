# Comparing `tmp/distans-0.1.0.tar.gz` & `tmp/distans-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distans-0.1.0.tar", max compression
+gzip compressed data, was "distans-0.1.1.tar", max compression
```

## Comparing `distans-0.1.0.tar` & `distans-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-30 14:34:23.009677 distans-0.1.0/LICENSE
--rw-r--r--   0        0        0      353 2023-06-30 17:07:26.079486 distans-0.1.0/README.md
--rw-r--r--   0        0        0       85 2023-06-30 17:02:03.099460 distans-0.1.0/distans/__init__.py
--rw-r--r--   0        0        0     1300 2023-06-30 17:06:57.109496 distans-0.1.0/distans/edit.py
--rw-r--r--   0        0        0      688 2023-06-30 17:06:57.120912 distans-0.1.0/distans/lp_space.py
--rw-r--r--   0        0        0        0 2023-06-30 17:16:03.035768 distans-0.1.0/distans/py.typed
--rw-r--r--   0        0        0      663 2023-06-30 17:14:57.886178 distans-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 distans-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 14:34:23.009677 distans-0.1.1/LICENSE
+-rw-r--r--   0        0        0      353 2023-06-30 17:07:26.079486 distans-0.1.1/README.md
+-rw-r--r--   0        0        0      116 2023-06-30 17:34:27.752684 distans-0.1.1/distans/__init__.py
+-rw-r--r--   0        0        0     1300 2023-06-30 17:06:57.109496 distans-0.1.1/distans/edit.py
+-rw-r--r--   0        0        0      688 2023-06-30 17:06:57.120912 distans-0.1.1/distans/lp_space.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:16:03.035768 distans-0.1.1/distans/py.typed
+-rw-r--r--   0        0        0      214 2023-06-30 17:34:35.226892 distans-0.1.1/distans/stuff.py
+-rw-r--r--   0        0        0      663 2023-06-30 17:21:01.258172 distans-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 distans-0.1.1/PKG-INFO
```

### Comparing `distans-0.1.0/LICENSE` & `distans-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `distans-0.1.0/distans/edit.py` & `distans-0.1.1/distans/edit.py`

 * *Files identical despite different names*

### Comparing `distans-0.1.0/distans/lp_space.py` & `distans-0.1.1/distans/lp_space.py`

 * *Files identical despite different names*

### Comparing `distans-0.1.0/pyproject.toml` & `distans-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "distans"
-version = "0.1.0"
+version = "0.1.1"
 repository = "https://github.com/cospectrum/distans"
 description = "Different distances for Python"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `distans-0.1.0/PKG-INFO` & `distans-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distans
-Version: 0.1.0
+Version: 0.1.1
 Summary: Different distances for Python
 Home-page: https://github.com/cospectrum/distans
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

