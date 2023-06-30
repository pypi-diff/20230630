# Comparing `tmp/pyarcade-0.0.1.tar.gz` & `tmp/pyarcade-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcade-0.0.1.tar", last modified: Fri Jun 30 19:35:40 2023, max compression
+gzip compressed data, was "pyarcade-0.0.3.tar", last modified: Fri Jun 30 20:29:52 2023, max compression
```

## Comparing `pyarcade-0.0.1.tar` & `pyarcade-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.459065 pyarcade-0.0.1/
--rw-r--r--   0 adamsrosales   (501) staff       (20)    11357 2023-06-30 16:19:19.000000 pyarcade-0.0.1/LICENSE
--rw-r--r--   0 adamsrosales   (501) staff       (20)      377 2023-06-30 19:35:40.458964 pyarcade-0.0.1/PKG-INFO
--rw-r--r--   0 adamsrosales   (501) staff       (20)       78 2023-06-30 19:32:59.000000 pyarcade-0.0.1/README.md
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.456065 pyarcade-0.0.1/pyarcade/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 18:20:11.000000 pyarcade-0.0.1/pyarcade/__init__.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.457155 pyarcade-0.0.1/pyarcade/api/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/api/__init__.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)     2078 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/api/client.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)      614 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/api/config.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)     1129 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/api/sync.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.457371 pyarcade-0.0.1/pyarcade/dao/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/dao/__init__.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)     1653 2023-06-30 19:27:38.000000 pyarcade-0.0.1/pyarcade/dao/database.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.457930 pyarcade-0.0.1/pyarcade/model/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:06:09.000000 pyarcade-0.0.1/pyarcade/model/__init__.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)       94 2023-06-30 19:13:28.000000 pyarcade-0.0.1/pyarcade/model/database.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)      379 2023-06-30 19:20:27.000000 pyarcade-0.0.1/pyarcade/model/request.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.456569 pyarcade-0.0.1/pyarcade.egg-info/
--rw-r--r--   0 adamsrosales   (501) staff       (20)      377 2023-06-30 19:35:40.000000 pyarcade-0.0.1/pyarcade.egg-info/PKG-INFO
--rw-r--r--   0 adamsrosales   (501) staff       (20)      570 2023-06-30 19:35:40.000000 pyarcade-0.0.1/pyarcade.egg-info/SOURCES.txt
--rw-r--r--   0 adamsrosales   (501) staff       (20)        1 2023-06-30 19:35:40.000000 pyarcade-0.0.1/pyarcade.egg-info/dependency_links.txt
--rw-r--r--   0 adamsrosales   (501) staff       (20)       56 2023-06-30 19:35:40.000000 pyarcade-0.0.1/pyarcade.egg-info/requires.txt
--rw-r--r--   0 adamsrosales   (501) staff       (20)       15 2023-06-30 19:35:40.000000 pyarcade-0.0.1/pyarcade.egg-info/top_level.txt
--rw-r--r--   0 adamsrosales   (501) staff       (20)       38 2023-06-30 19:35:40.459094 pyarcade-0.0.1/setup.cfg
--rw-r--r--   0 adamsrosales   (501) staff       (20)      645 2023-06-30 19:06:09.000000 pyarcade-0.0.1/setup.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.458163 pyarcade-0.0.1/tests/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:06:09.000000 pyarcade-0.0.1/tests/__init__.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.458479 pyarcade-0.0.1/tests/api/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:06:09.000000 pyarcade-0.0.1/tests/api/__init__.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)     1170 2023-06-30 19:06:09.000000 pyarcade-0.0.1/tests/api/test_client.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)      437 2023-06-30 19:06:09.000000 pyarcade-0.0.1/tests/api/test_config.py
-drwxr-xr-x   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:35:40.458741 pyarcade-0.0.1/tests/model/
--rw-r--r--   0 adamsrosales   (501) staff       (20)        0 2023-06-30 19:08:51.000000 pyarcade-0.0.1/tests/model/__init__.py
--rw-r--r--   0 adamsrosales   (501) staff       (20)      580 2023-06-30 19:10:23.000000 pyarcade-0.0.1/tests/model/test_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.301172 pyarcade-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 20:29:47.000000 pyarcade-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-30 20:29:52.301172 pyarcade-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-30 20:29:47.000000 pyarcade-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/pyarcade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/pyarcade/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/api/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/pyarcade/dao/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/dao/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/pyarcade/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-30 20:29:47.000000 pyarcade-0.0.3/pyarcade/model/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/pyarcade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-30 20:29:52.000000 pyarcade-0.0.3/pyarcade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-30 20:29:52.000000 pyarcade-0.0.3/pyarcade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:29:52.000000 pyarcade-0.0.3/pyarcade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 20:29:52.000000 pyarcade-0.0.3/pyarcade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 20:29:52.000000 pyarcade-0.0.3/pyarcade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 20:29:52.301172 pyarcade-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 20:29:47.000000 pyarcade-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.297172 pyarcade-0.0.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/api/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:52.301172 pyarcade-0.0.3/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 20:29:47.000000 pyarcade-0.0.3/tests/model/test_request.py
```

### Comparing `pyarcade-0.0.1/LICENSE` & `pyarcade-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/pyarcade/api/client.py` & `pyarcade-0.0.3/pyarcade/api/client.py`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/pyarcade/api/config.py` & `pyarcade-0.0.3/pyarcade/api/config.py`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/pyarcade/api/sync.py` & `pyarcade-0.0.3/pyarcade/api/sync.py`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/pyarcade/dao/database.py` & `pyarcade-0.0.3/pyarcade/dao/database.py`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/pyarcade.egg-info/SOURCES.txt` & `pyarcade-0.0.3/pyarcade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/setup.py` & `pyarcade-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="pyarcade",
-    version="0.0.1",
+    version="0.0.3",
     author="Adams Rosales",
     author_email="adams.rosales.92@gmail.com",
     description="A Python driver for ArcadeDB",
     extras_require={
         "test": [
             "pytest",
             "pytest-cov",
```

### Comparing `pyarcade-0.0.1/tests/api/test_client.py` & `pyarcade-0.0.3/tests/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pyarcade-0.0.1/tests/model/test_request.py` & `pyarcade-0.0.3/tests/model/test_request.py`

 * *Files identical despite different names*

