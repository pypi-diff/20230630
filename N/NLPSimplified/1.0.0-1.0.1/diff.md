# Comparing `tmp/NLPSimplified-1.0.0.tar.gz` & `tmp/NLPSimplified-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NLPSimplified-1.0.0.tar", last modified: Fri Jun 30 01:41:16 2023, max compression
+gzip compressed data, was "NLPSimplified-1.0.1.tar", last modified: Fri Jun 30 01:45:06 2023, max compression
```

## Comparing `NLPSimplified-1.0.0.tar` & `NLPSimplified-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:41:16.434848 NLPSimplified-1.0.0/
--rw-rw-rw-   0        0        0     1034 2023-06-30 01:39:25.000000 NLPSimplified-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-30 01:41:16.428329 NLPSimplified-1.0.0/NLPSimplified/
--rw-rw-rw-   0        0        0       82 2023-06-29 03:46:10.000000 NLPSimplified-1.0.0/NLPSimplified/__init__.py
--rw-rw-rw-   0        0        0      861 2023-06-29 03:46:09.000000 NLPSimplified-1.0.0/NLPSimplified/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:41:16.432845 NLPSimplified-1.0.0/NLPSimplified.egg-info/
--rw-rw-rw-   0        0        0      257 2023-06-30 01:41:16.000000 NLPSimplified-1.0.0/NLPSimplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-30 01:41:16.000000 NLPSimplified-1.0.0/NLPSimplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:41:16.000000 NLPSimplified-1.0.0/NLPSimplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-30 01:41:16.000000 NLPSimplified-1.0.0/NLPSimplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 01:41:16.000000 NLPSimplified-1.0.0/NLPSimplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      257 2023-06-30 01:41:16.434848 NLPSimplified-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2471 2023-06-30 01:39:27.000000 NLPSimplified-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 01:41:16.434848 NLPSimplified-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-06-30 01:41:11.000000 NLPSimplified-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:45:06.518657 NLPSimplified-1.0.1/
+-rw-rw-rw-   0        0        0     1034 2023-06-30 01:39:25.000000 NLPSimplified-1.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-30 01:45:06.511653 NLPSimplified-1.0.1/NLPSimplified/
+-rw-rw-rw-   0        0        0       82 2023-06-30 01:44:50.000000 NLPSimplified-1.0.1/NLPSimplified/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-06-30 01:44:52.000000 NLPSimplified-1.0.1/NLPSimplified/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:45:06.516656 NLPSimplified-1.0.1/NLPSimplified.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-06-30 01:45:06.000000 NLPSimplified-1.0.1/NLPSimplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-30 01:45:06.000000 NLPSimplified-1.0.1/NLPSimplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:45:06.000000 NLPSimplified-1.0.1/NLPSimplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-30 01:45:06.000000 NLPSimplified-1.0.1/NLPSimplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 01:45:06.000000 NLPSimplified-1.0.1/NLPSimplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      257 2023-06-30 01:45:06.517656 NLPSimplified-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2471 2023-06-30 01:44:40.000000 NLPSimplified-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:45:06.518657 NLPSimplified-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      315 2023-06-30 01:44:39.000000 NLPSimplified-1.0.1/setup.py
```

### Comparing `NLPSimplified-1.0.0/LICENSE` & `NLPSimplified-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NLPSimplified-1.0.0/NLPSimplified/pipeline.py` & `NLPSimplified-1.0.1/NLPSimplified/pipeline.py`

 * *Files identical despite different names*

### Comparing `NLPSimplified-1.0.0/README.md` & `NLPSimplified-1.0.1/README.md`

 * *Files identical despite different names*

