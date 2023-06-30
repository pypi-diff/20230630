# Comparing `tmp/bfgdealer-0.0.8.tar.gz` & `tmp/bfgdealer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.8.tar", last modified: Fri Jun 30 11:32:33 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.9.tar", last modified: Fri Jun 30 11:42:20 2023, max compression
```

## Comparing `bfgdealer-0.0.8.tar` & `bfgdealer-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.8/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1160 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.8/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.416379 bfgdealer-0.0.8/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.8/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/bfgdealer/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    22861 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1737 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     8556 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    28485 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16825 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14304 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/src/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/bfgdealer/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      289 2023-06-30 11:29:36.000000 bfgdealer-0.0.8/bfgdealer/tests/test_set_hands_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:32:33.416379 bfgdealer-0.0.8/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1160 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      471 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-30 11:32:33.000000 bfgdealer-0.0.8/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-30 11:32:33.419712 bfgdealer-0.0.8/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.8/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:42:20.764368 bfgdealer-0.0.9/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.9/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1220 2023-06-30 11:42:20.764368 bfgdealer-0.0.9/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.9/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:42:20.761034 bfgdealer-0.0.9/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.9/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:42:20.764368 bfgdealer-0.0.9/bfgdealer/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    22861 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1737 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     8556 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    28485 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16825 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14304 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/src/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:42:20.764368 bfgdealer-0.0.9/bfgdealer/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      289 2023-06-30 11:40:40.000000 bfgdealer-0.0.9/bfgdealer/tests/test_set_hands_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-30 11:42:20.764368 bfgdealer-0.0.9/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1220 2023-06-30 11:42:20.000000 bfgdealer-0.0.9/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      471 2023-06-30 11:42:20.000000 bfgdealer-0.0.9/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-30 11:42:20.000000 bfgdealer-0.0.9/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-30 11:42:20.000000 bfgdealer-0.0.9/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-30 11:42:20.767701 bfgdealer-0.0.9/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.9/setup.py
```

### Comparing `bfgdealer-0.0.8/LICENSE.txt` & `bfgdealer-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/PKG-INFO` & `bfgdealer-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.8
+Version: 0.0.9
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.9 30 Jun 2023
+
+1. Change source to src
+
+------
+
 Version 0.0.8 30 Jun 2023
 
 1. Linting and start tests
 
 ------
 
 Version 0.0.7 20 Jun 2023
```

### Comparing `bfgdealer-0.0.8/bfgdealer/__init__.py` & `bfgdealer-0.0.9/bfgdealer/__init__.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/board.py` & `bfgdealer-0.0.9/bfgdealer/src/board.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/constants.py` & `bfgdealer-0.0.9/bfgdealer/src/constants.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/dealer.py` & `bfgdealer-0.0.9/bfgdealer/src/dealer.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/dealer_duo.py` & `bfgdealer-0.0.9/bfgdealer/src/dealer_duo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/dealer_engine.py` & `bfgdealer-0.0.9/bfgdealer/src/dealer_engine.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer/src/dealer_solo.py` & `bfgdealer-0.0.9/bfgdealer/src/dealer_solo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.8/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.9/bfgdealer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.8
+Version: 0.0.9
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.9 30 Jun 2023
+
+1. Change source to src
+
+------
+
 Version 0.0.8 30 Jun 2023
 
 1. Linting and start tests
 
 ------
 
 Version 0.0.7 20 Jun 2023
```

### Comparing `bfgdealer-0.0.8/setup.py` & `bfgdealer-0.0.9/setup.py`

 * *Files identical despite different names*

