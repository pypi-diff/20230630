# Comparing `tmp/selis-1.0.0.tar.gz` & `tmp/selis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.0.0.tar", last modified: Sat Jun 24 12:33:17 2023, max compression
+gzip compressed data, was "selis-1.0.1.tar", last modified: Fri Jun 30 09:21:50 2023, max compression
```

## Comparing `selis-1.0.0.tar` & `selis-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 12:33:17.394398 selis-1.0.0/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 12:33:17.394282 selis-1.0.0/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 12:33:17.392878 selis-1.0.0/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-24 12:32:58.000000 selis-1.0.0/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3861 2023-06-24 12:32:55.000000 selis-1.0.0/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      786 2023-06-24 12:32:50.000000 selis-1.0.0/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1137 2023-06-24 12:33:14.000000 selis-1.0.0/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      410 2023-06-24 11:51:57.000000 selis-1.0.0/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 12:33:17.394068 selis-1.0.0/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-24 12:33:17.000000 selis-1.0.0/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-24 12:33:17.394441 selis-1.0.0/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      281 2023-06-24 12:32:39.000000 selis-1.0.0/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-30 09:21:50.472486 selis-1.0.1/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-30 09:21:50.472359 selis-1.0.1/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-30 09:21:50.471105 selis-1.0.1/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-24 12:32:58.000000 selis-1.0.1/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3861 2023-06-24 12:32:55.000000 selis-1.0.1/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      653 2023-06-30 09:21:18.000000 selis-1.0.1/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1137 2023-06-24 12:37:06.000000 selis-1.0.1/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      410 2023-06-24 11:51:57.000000 selis-1.0.1/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-30 09:21:50.472146 selis-1.0.1/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-30 09:21:50.000000 selis-1.0.1/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-30 09:21:50.472536 selis-1.0.1/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      281 2023-06-30 09:21:32.000000 selis-1.0.1/setup.py
```

### Comparing `selis-1.0.0/selis/client.py` & `selis-1.0.1/selis/client.py`

 * *Files identical despite different names*

### Comparing `selis-1.0.0/selis/selis.py` & `selis-1.0.1/selis/selis.py`

 * *Files identical despite different names*

