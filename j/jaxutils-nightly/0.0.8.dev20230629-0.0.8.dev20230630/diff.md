# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230629.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230629.tar", last modified: Thu Jun 29 00:06:33 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230630.tar", last modified: Fri Jun 30 00:06:33 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230629.tar` & `jaxutils-nightly-0.0.8.dev20230630.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-06-29 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-06-29 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-29 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-06-29 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-06-29 00:06:33.145440 jaxutils-nightly-0.0.8.dev20230629/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-06-29 00:06:27.000000 jaxutils-nightly-0.0.8.dev20230629/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-06-30 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-06-30 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-30 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-30 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-06-30 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-06-30 00:06:33.884175 jaxutils-nightly-0.0.8.dev20230630/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-06-30 00:06:28.000000 jaxutils-nightly-0.0.8.dev20230630/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230629/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230630/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230629
+Version: 0.0.8.dev20230630
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230629/README.md` & `jaxutils-nightly-0.0.8.dev20230630/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230630/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230629
+Version: 0.0.8.dev20230630
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230629/setup.py` & `jaxutils-nightly-0.0.8.dev20230630/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230629/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230630/versioneer.py`

 * *Files identical despite different names*

