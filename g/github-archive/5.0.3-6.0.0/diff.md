# Comparing `tmp/github-archive-5.0.3.tar.gz` & `tmp/github-archive-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-archive-5.0.3.tar", last modified: Mon May 15 15:49:47 2023, max compression
+gzip compressed data, was "github-archive-6.0.0.tar", last modified: Fri Jun 30 21:01:15 2023, max compression
```

## Comparing `github-archive-5.0.3.tar` & `github-archive-6.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 15:49:13.000000 github-archive-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-15 15:49:47.515304 github-archive-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-15 15:49:13.000000 github-archive-5.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/github_archive/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/gists.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-15 15:49:13.000000 github-archive-5.0.3/github_archive/repos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/github_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 15:49:47.000000 github-archive-5.0.3/github_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 15:49:13.000000 github-archive-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:49:47.515304 github-archive-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-15 15:49:13.000000 github-archive-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.511304 github-archive-5.0.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:47.515304 github-archive-5.0.3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_gists.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-15 15:49:13.000000 github-archive-5.0.3/test/unit/test_repos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:01:15.685424 github-archive-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 21:00:46.000000 github-archive-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-30 21:01:15.685424 github-archive-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-30 21:00:46.000000 github-archive-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:01:15.681424 github-archive-6.0.0/github_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/gists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-30 21:00:46.000000 github-archive-6.0.0/github_archive/repos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:01:15.681424 github-archive-6.0.0/github_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 21:01:15.000000 github-archive-6.0.0/github_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-30 21:00:46.000000 github-archive-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:01:15.685424 github-archive-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-30 21:00:46.000000 github-archive-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:01:15.677424 github-archive-6.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:01:15.685424 github-archive-6.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/test_gists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-30 21:00:46.000000 github-archive-6.0.0/test/unit/test_repos.py
```

### Comparing `github-archive-5.0.3/LICENSE` & `github-archive-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/PKG-INFO` & `github-archive-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: github-archive
-Version: 5.0.3
+Version: 6.0.0
 Summary: A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 Home-page: http://github.com/justintime50/github-archive
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # GitHub Archive
@@ -35,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install github-archive
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Usage:
     github-archive --users justintime50 --clone
@@ -92,12 +92,12 @@
 
 **Access**: GitHub Archive can only clone or pull git assets that the authenticated user has access to. This means that private repos from another user or org that you don't have access to will not be able to be cloned or pulled.
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python github_archive/cli.py --help
 ```
```

### Comparing `github-archive-5.0.3/README.md` & `github-archive-6.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install github-archive
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Usage:
     github-archive --users justintime50 --clone
@@ -77,12 +77,12 @@
 
 **Access**: GitHub Archive can only clone or pull git assets that the authenticated user has access to. This means that private repos from another user or org that you don't have access to will not be able to be cloned or pulled.
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python github_archive/cli.py --help
 ```
```

### Comparing `github-archive-5.0.3/github_archive/archive.py` & `github-archive-6.0.0/github_archive/archive.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/github_archive/cli.py` & `github-archive-6.0.0/github_archive/cli.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/github_archive/constants.py` & `github-archive-6.0.0/github_archive/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
-
-from typing_extensions import Literal
+from typing import Literal
 
 
 DEFAULT_BASE_URL = 'https://api.github.com'
 DEFAULT_LOCATION = os.path.expanduser(os.path.join('~', 'github-archive'))
 DEFAULT_NUM_THREADS = 10
 DEFAULT_TIMEOUT = 300
```

### Comparing `github-archive-5.0.3/github_archive/gists.py` & `github-archive-6.0.0/github_archive/gists.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/github_archive/logger.py` & `github-archive-6.0.0/github_archive/logger.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/github_archive/repos.py` & `github-archive-6.0.0/github_archive/repos.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/github_archive.egg-info/PKG-INFO` & `github-archive-6.0.0/github_archive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: github-archive
-Version: 5.0.3
+Version: 6.0.0
 Summary: A powerful tool to concurrently clone, pull, or fork user and org repos and gists to create a GitHub archive.
 Home-page: http://github.com/justintime50/github-archive
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # GitHub Archive
@@ -35,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install github-archive
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Usage:
     github-archive --users justintime50 --clone
@@ -92,12 +92,12 @@
 
 **Access**: GitHub Archive can only clone or pull git assets that the authenticated user has access to. This means that private repos from another user or org that you don't have access to will not be able to be cloned or pulled.
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python github_archive/cli.py --help
 ```
```

### Comparing `github-archive-5.0.3/github_archive.egg-info/SOURCES.txt` & `github-archive-6.0.0/github_archive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/test/unit/conftest.py` & `github-archive-6.0.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/test/unit/test_archive.py` & `github-archive-6.0.0/test/unit/test_archive.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/test/unit/test_gists.py` & `github-archive-6.0.0/test/unit/test_gists.py`

 * *Files identical despite different names*

### Comparing `github-archive-5.0.3/test/unit/test_repos.py` & `github-archive-6.0.0/test/unit/test_repos.py`

 * *Files identical despite different names*

