# Comparing `tmp/matchmsextras-0.4.1.tar.gz` & `tmp/matchmsextras-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmsextras-0.4.1.tar", last modified: Mon Feb  6 09:49:16 2023, max compression
+gzip compressed data, was "matchmsextras-0.4.2.tar", last modified: Fri Jun 30 13:57:17 2023, max compression
```

## Comparing `matchmsextras-0.4.1.tar` & `matchmsextras-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:49:16.216460 matchmsextras-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-06 09:49:16.216460 matchmsextras-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:49:16.216460 matchmsextras-0.4.1/matchmsextras/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/library_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    40160 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/plotting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/matchmsextras/pubchem_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 09:49:16.216460 matchmsextras-0.4.1/matchmsextras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-06 09:49:15.000000 matchmsextras-0.4.1/matchmsextras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-06 09:49:16.000000 matchmsextras-0.4.1/matchmsextras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 09:49:15.000000 matchmsextras-0.4.1/matchmsextras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 09:49:15.000000 matchmsextras-0.4.1/matchmsextras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-06 09:49:15.000000 matchmsextras-0.4.1/matchmsextras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-06 09:49:15.000000 matchmsextras-0.4.1/matchmsextras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 09:49:16.216460 matchmsextras-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-06 09:49:05.000000 matchmsextras-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:57:17.886443 matchmsextras-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-30 13:57:17.886443 matchmsextras-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:57:17.886443 matchmsextras-0.4.2/matchmsextras/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/library_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40160 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/plotting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/matchmsextras/pubchem_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:57:17.886443 matchmsextras-0.4.2/matchmsextras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 13:57:17.000000 matchmsextras-0.4.2/matchmsextras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:57:17.886443 matchmsextras-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-30 13:57:05.000000 matchmsextras-0.4.2/setup.py
```

### Comparing `matchmsextras-0.4.1/LICENSE` & `matchmsextras-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmsextras-0.4.1/PKG-INFO` & `matchmsextras-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmsextras
-Version: 0.4.1
+Version: 0.4.2
 Summary: Additional functionalities to be used with matchms
 Home-page: https://github.com/matchms/matchmsextras
 Author: Netherlands eScience Center
 Author-email: f.huber@esciencecenter.nl
 License: Apache Software License 2.0
 Description: <img src="https://github.com/matchms/matchmsextras/blob/main/images/matchmsextras_logo.png" width="600">
```

### Comparing `matchmsextras-0.4.1/README.md` & `matchmsextras-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `matchmsextras-0.4.1/matchmsextras/library_search.py` & `matchmsextras-0.4.2/matchmsextras/library_search.py`

 * *Files identical despite different names*

### Comparing `matchmsextras-0.4.1/matchmsextras/networking.py` & `matchmsextras-0.4.2/matchmsextras/networking.py`

 * *Files identical despite different names*

### Comparing `matchmsextras-0.4.1/matchmsextras/plotting_functions.py` & `matchmsextras-0.4.2/matchmsextras/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `matchmsextras-0.4.1/matchmsextras.egg-info/PKG-INFO` & `matchmsextras-0.4.2/matchmsextras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmsextras
-Version: 0.4.1
+Version: 0.4.2
 Summary: Additional functionalities to be used with matchms
 Home-page: https://github.com/matchms/matchmsextras
 Author: Netherlands eScience Center
 Author-email: f.huber@esciencecenter.nl
 License: Apache Software License 2.0
 Description: <img src="https://github.com/matchms/matchmsextras/blob/main/images/matchmsextras_logo.png" width="600">
```

### Comparing `matchmsextras-0.4.1/setup.py` & `matchmsextras-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     test_suite="tests",
     python_requires='>=3.7',
     install_requires=[
         "matchms>=0.11.0",
         "spec2vec",
         "python-louvain",
         "networkx",
-        "pandas",
+        "pandas<2.0.0",
+        "pubchempy"
     ],
     extras_require={"dev": ["bump2version",
                             "isort>=4.2.5,<5",
                             "prospector[with_pyroma]",
                             "pytest",
                             "pytest-cov",
                             "sphinx>=3.0.0,!=3.2.0,!=3.5.0,<4.0.0",
```

