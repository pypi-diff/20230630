# Comparing `tmp/ice_simplex_assimilate-0.1.0.tar.gz` & `tmp/ice_simplex_assimilate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ice_simplex_assimilate-0.1.0.tar", max compression
+gzip compressed data, was "ice_simplex_assimilate-0.1.1.tar", max compression
```

## Comparing `ice_simplex_assimilate-0.1.0.tar` & `ice_simplex_assimilate-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-14 19:27:28.966885 ice_simplex_assimilate-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 14:57:09.141690 ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/__init__.py
--rw-r--r--   0        0        0     3430 2023-06-14 18:46:53.104387 ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/deltize.py
--rw-r--r--   0        0        0      298 2023-06-14 18:30:25.741811 ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/io.py
--rw-r--r--   0        0        0     7655 2023-06-10 12:08:05.805803 ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/visualize.py
--rw-r--r--   0        0        0      533 2023-06-14 19:28:24.252519 ice_simplex_assimilate-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 ice_simplex_assimilate-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-14 19:27:28.966885 ice_simplex_assimilate-0.1.1/README.md
+-rw-r--r--   0        0        0       46 2023-06-14 19:41:47.179033 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/__init__.py
+-rw-r--r--   0        0        0     3430 2023-06-14 18:46:53.104387 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/deltize.py
+-rw-r--r--   0        0        0      298 2023-06-14 18:30:25.741811 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/io.py
+-rw-r--r--   0        0        0     7655 2023-06-10 12:08:05.805803 ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/visualize.py
+-rw-r--r--   0        0        0      550 2023-06-30 07:53:09.305475 ice_simplex_assimilate-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 ice_simplex_assimilate-0.1.1/PKG-INFO
```

### Comparing `ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/deltize.py` & `ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/deltize.py`

 * *Files identical despite different names*

### Comparing `ice_simplex_assimilate-0.1.0/ice_simplex_assimilate/visualize.py` & `ice_simplex_assimilate-0.1.1/ice_simplex_assimilate/visualize.py`

 * *Files identical despite different names*

### Comparing `ice_simplex_assimilate-0.1.0/pyproject.toml` & `ice_simplex_assimilate-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "ice-simplex-assimilate"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Oscar Laird <olaird25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ice_simplex_assimilate"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pytest = "^7.3.2"
 simplex-assimilate = "^0.1.0"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 simplex-assimilate = {path = "/home/oscar/grooms/simplex_assimilate"}
 pytest-cov = "^4.1.0"
 jupyter = "^1.0.0"
 
 [build-system]
```

