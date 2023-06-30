# Comparing `tmp/pyrdfsubset-0.0.4.tar.gz` & `tmp/pyrdfsubset-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdfsubset-0.0.4.tar", last modified: Thu Jun 29 12:34:09 2023, max compression
+gzip compressed data, was "pyrdfsubset-0.0.5.tar", last modified: Thu Jun 29 12:39:16 2023, max compression
```

## Comparing `pyrdfsubset-0.0.4.tar` & `pyrdfsubset-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/pyrdfsubset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/rdfsubset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:16.220703 pyrdfsubset-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:39:16.220703 pyrdfsubset-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:39:16.220703 pyrdfsubset-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:16.216703 pyrdfsubset-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:16.220703 pyrdfsubset-0.0.5/src/pyrdfsubset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/src/pyrdfsubset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/src/pyrdfsubset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-29 12:39:05.000000 pyrdfsubset-0.0.5/src/pyrdfsubset/rdfsubset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:39:16.220703 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 12:39:16.000000 pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/top_level.txt
```

### Comparing `pyrdfsubset-0.0.4/LICENSE` & `pyrdfsubset-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.0.4/PKG-INFO` & `pyrdfsubset-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyrdfsubset-0.0.4/pyproject.toml` & `pyrdfsubset-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrdfsubset"
-version = "0.0.4"
+version = "0.0.5"
 description = "Create RDF subsets based on ShEx constraints"
 readme = "README.md"
 authors = [{ name = "Andra Waagmeester", email = "andra@micelio.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/PKG-INFO` & `pyrdfsubset-0.0.5/src/pyrdfsubset.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

