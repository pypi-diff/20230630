# Comparing `tmp/ICICONSOLE-GPT-0.0.3.tar.gz` & `tmp/ICICONSOLE-GPT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-GPT-0.0.3.tar", last modified: Thu Jun 29 23:49:27 2023, max compression
+gzip compressed data, was "ICICONSOLE-GPT-0.0.4.tar", last modified: Thu Jun 29 23:52:30 2023, max compression
```

## Comparing `ICICONSOLE-GPT-0.0.3.tar` & `ICICONSOLE-GPT-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:49:27.699136 ICICONSOLE-GPT-0.0.3/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:49:27.698215 ICICONSOLE-GPT-0.0.3/ICICONSOLEGPT/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLEGPT/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    10661 2023-06-29 23:28:10.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLEGPT/__main__.py
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:49:27.698884 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4051 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      337 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-06-29 23:49:27.000000 ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLE-GPT-0.0.3/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       39 2023-06-29 23:46:48.000000 ICICONSOLE-GPT-0.0.3/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4051 2023-06-29 23:49:27.699024 ICICONSOLE-GPT-0.0.3/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     2165 2023-06-29 23:28:52.000000 ICICONSOLE-GPT-0.0.3/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1008 2023-06-29 23:49:21.000000 ICICONSOLE-GPT-0.0.3/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:49:27.699168 ICICONSOLE-GPT-0.0.3/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:52:30.207088 ICICONSOLE-GPT-0.0.4/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:52:30.206168 ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    10661 2023-06-29 23:28:10.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/__main__.py
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:52:30.206841 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4051 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      363 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-06-29 23:52:30.000000 ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLE-GPT-0.0.4/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       39 2023-06-29 23:46:48.000000 ICICONSOLE-GPT-0.0.4/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4051 2023-06-29 23:52:30.206978 ICICONSOLE-GPT-0.0.4/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     2165 2023-06-29 23:28:52.000000 ICICONSOLE-GPT-0.0.4/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1008 2023-06-29 23:52:23.000000 ICICONSOLE-GPT-0.0.4/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:52:30.207123 ICICONSOLE-GPT-0.0.4/setup.cfg
```

### Comparing `ICICONSOLE-GPT-0.0.3/ICICONSOLEGPT/BasicCypherCommands.py` & `ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-GPT-0.0.3/ICICONSOLEGPT/__main__.py` & `ICICONSOLE-GPT-0.0.4/ICICONSOLEGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-GPT-0.0.3/ICICONSOLE_GPT.egg-info/PKG-INFO` & `ICICONSOLE-GPT-0.0.4/ICICONSOLE_GPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE-GPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ICICONSOLE-GPT-0.0.3/LICENSE` & `ICICONSOLE-GPT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-GPT-0.0.3/PKG-INFO` & `ICICONSOLE-GPT-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE-GPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ICICONSOLE-GPT-0.0.3/README.md` & `ICICONSOLE-GPT-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-GPT-0.0.3/pyproject.toml` & `ICICONSOLE-GPT-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE-GPT"
-version = "0.0.3"
+version = "0.0.4"
 description = "GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

