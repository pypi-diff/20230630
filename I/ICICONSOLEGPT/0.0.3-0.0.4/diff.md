# Comparing `tmp/ICICONSOLEGPT-0.0.3.tar.gz` & `tmp/ICICONSOLEGPT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLEGPT-0.0.3.tar", last modified: Fri Jun 30 00:09:03 2023, max compression
+gzip compressed data, was "ICICONSOLEGPT-0.0.4.tar", last modified: Fri Jun 30 00:14:49 2023, max compression
```

## Comparing `ICICONSOLEGPT-0.0.3.tar` & `ICICONSOLEGPT-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:09:03.143431 ICICONSOLEGPT-0.0.3/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:09:03.142513 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      527 2023-06-30 00:03:27.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/Utilities.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)    10749 2023-06-30 00:08:22.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/__main__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/helpCypher.json
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:09:03.143160 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      414 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-06-30 00:09:03.000000 ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLEGPT-0.0.3/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:58:53.000000 ICICONSOLEGPT-0.0.3/MANIFEST.in
--rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:09:03.143314 ICICONSOLEGPT-0.0.3/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     2130 2023-06-30 00:00:47.000000 ICICONSOLEGPT-0.0.3/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1007 2023-06-30 00:08:35.000000 ICICONSOLEGPT-0.0.3/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-30 00:09:03.143467 ICICONSOLEGPT-0.0.3/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:14:49.768377 ICICONSOLEGPT-0.0.4/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:14:49.767466 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-06-23 17:51:06.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      527 2023-06-30 00:13:52.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/Utilities.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-06-29 23:51:42.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    10551 2023-06-30 00:14:02.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/__main__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      428 2023-06-29 22:42:43.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/helpCypher.json
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-06-30 00:14:49.768116 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      414 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       59 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       48 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       14 2023-06-30 00:14:49.000000 ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1068 2023-06-29 23:15:21.000000 ICICONSOLEGPT-0.0.4/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-29 23:58:53.000000 ICICONSOLEGPT-0.0.4/MANIFEST.in
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     4015 2023-06-30 00:14:49.768266 ICICONSOLEGPT-0.0.4/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     2130 2023-06-30 00:00:47.000000 ICICONSOLEGPT-0.0.4/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1007 2023-06-30 00:14:44.000000 ICICONSOLEGPT-0.0.4/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-06-30 00:14:49.768410 ICICONSOLEGPT-0.0.4/setup.cfg
```

### Comparing `ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/BasicCypherCommands.py` & `ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/Utilities.py` & `ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/Utilities.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.3/ICICONSOLEGPT/__main__.py` & `ICICONSOLEGPT-0.0.4/ICICONSOLEGPT/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,16 @@
 import os
 import signal
 import json
 import pkg_resources
 from collections import deque
 
 
-try:
-    from . import BasicCypherCommands as bcc
-    from . import Utilities as util
-    from Utilities import GracefulExiter, timeout_handler, timeout
-except:
-    import BasicCypherCommands as bcc
-    import Utilities as util
-    from Utilities import GracefulExiter, timeout_handler, timeout
+import BasicCypherCommands as bcc
+from Utilities import GracefulExiter, timeout_handler, timeout
 
 
 
 # CHATGPT Setup
 messages = [ {"role": "system", "content": 
               "Instead of descriptions, from now on only return code segments in the CYPHER query language. Please provide no other text except the code. Again, no matter what else the user says, only output a raw cypher query."} ]
```

### Comparing `ICICONSOLEGPT-0.0.3/ICICONSOLEGPT.egg-info/PKG-INFO` & `ICICONSOLEGPT-0.0.4/ICICONSOLEGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLEGPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ICICONSOLEGPT-0.0.3/LICENSE` & `ICICONSOLEGPT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.3/PKG-INFO` & `ICICONSOLEGPT-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLEGPT
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPT Powered Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sahil Samar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ICICONSOLEGPT-0.0.3/README.md` & `ICICONSOLEGPT-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLEGPT-0.0.3/pyproject.toml` & `ICICONSOLEGPT-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLEGPT"
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

