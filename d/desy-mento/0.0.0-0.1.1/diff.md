# Comparing `tmp/desy-mento-0.0.0.tar.gz` & `tmp/desy-mento-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desy-mento-0.0.0.tar", last modified: Wed Jun 28 15:05:27 2023, max compression
+gzip compressed data, was "desy-mento-0.1.1.tar", last modified: Fri Jun 30 15:02:48 2023, max compression
```

## Comparing `desy-mento-0.0.0.tar` & `desy-mento-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-28 15:05:27.921466 desy-mento-0.0.0/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-06-28 15:05:27.921466 desy-mento-0.0.0/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     6886 2023-06-28 15:02:33.000000 desy-mento-0.0.0/README.rst
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      168 2023-06-28 15:05:27.921466 desy-mento-0.0.0/setup.cfg
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     1070 2023-06-28 15:05:22.000000 desy-mento-0.0.0/setup.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-28 15:05:27.920466 desy-mento-0.0.0/src/
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-28 15:05:27.920466 desy-mento-0.0.0/src/desy_mento.egg-info/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-06-28 15:05:27.000000 desy-mento-0.0.0/src/desy_mento.egg-info/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      367 2023-06-28 15:05:27.000000 desy-mento-0.0.0/src/desy_mento.egg-info/SOURCES.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        1 2023-06-28 15:05:27.000000 desy-mento-0.0.0/src/desy_mento.egg-info/dependency_links.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)       34 2023-06-28 15:05:27.000000 desy-mento-0.0.0/src/desy_mento.egg-info/requires.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        6 2023-06-28 15:05:27.000000 desy-mento-0.0.0/src/desy_mento.egg-info/top_level.txt
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-28 15:05:27.920466 desy-mento-0.0.0/src/mento/
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      420 2022-06-27 12:44:38.000000 desy-mento-0.0.0/src/mento/__init__.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11594 2023-06-28 12:35:53.000000 desy-mento-0.0.0/src/mento/metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11937 2023-06-28 12:35:53.000000 desy-mento-0.0.0/src/mento/trigger.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     9696 2023-06-28 12:35:53.000000 desy-mento-0.0.0/src/mento/utils.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-28 15:05:27.920466 desy-mento-0.0.0/tests/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     8285 2023-06-28 12:35:53.000000 desy-mento-0.0.0/tests/test_metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     5242 2023-06-28 12:35:53.000000 desy-mento-0.0.0/tests/test_trigger.py
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     3684 2022-06-27 12:44:38.000000 desy-mento-0.0.0/tests/test_utils.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     7747 2023-06-30 15:02:48.536481 desy-mento-0.1.1/PKG-INFO
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     6809 2023-06-28 15:09:51.000000 desy-mento-0.1.1/README.rst
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     1190 2023-06-30 15:00:43.000000 desy-mento-0.1.1/pyproject.toml
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)       38 2023-06-30 15:02:48.536481 desy-mento-0.1.1/setup.cfg
+-rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      238 2023-06-30 14:45:08.000000 desy-mento-0.1.1/setup.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.535481 desy-mento-0.1.1/src/
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.535481 desy-mento-0.1.1/src/desy_mento.egg-info/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     7747 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/PKG-INFO
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)      372 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/SOURCES.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)        1 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/dependency_links.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)       47 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/requires.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)        6 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/top_level.txt
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/src/mento/
+-rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      420 2022-06-27 12:44:38.000000 desy-mento-0.1.1/src/mento/__init__.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11594 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/metadata.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11937 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/trigger.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     9696 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/utils.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/tests/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     8285 2023-06-28 12:35:53.000000 desy-mento-0.1.1/tests/test_metadata.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     5242 2023-06-28 12:35:53.000000 desy-mento-0.1.1/tests/test_trigger.py
+-rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     3684 2022-06-27 12:44:38.000000 desy-mento-0.1.1/tests/test_utils.py
```

### Comparing `desy-mento-0.0.0/README.rst` & `desy-mento-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 Installation
 ============
 
 At PETRA III beamlines, the easiest way to install the |oa| package would be to use ``pip``.
 The package can be downloaded as an artifact from the Gitlab repository page, or used directly
 in your ``pip`` command as follows::
 
-    python3 -m pip install desy-mento --index-url https://gitlab.desy.de/api/v4/projects/1078/packages/pypi/simple
+    python3 -m pip install desy-mento
 
 
 
 API documentation
 =================
 API documentation can be found in docs_.
```

### Comparing `desy-mento-0.0.0/src/mento/metadata.py` & `desy-mento-0.1.1/src/mento/metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.0.0/src/mento/trigger.py` & `desy-mento-0.1.1/src/mento/trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.0.0/src/mento/utils.py` & `desy-mento-0.1.1/src/mento/utils.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.0.0/tests/test_metadata.py` & `desy-mento-0.1.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.0.0/tests/test_trigger.py` & `desy-mento-0.1.1/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.0.0/tests/test_utils.py` & `desy-mento-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

