# Comparing `tmp/hyperx-0.0.3.tar.gz` & `tmp/hyperx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.0.3.tar", last modified: Wed Mar 22 16:10:26 2023, max compression
+gzip compressed data, was "hyperx-0.1.0.tar", last modified: Fri Jun 30 15:47:45 2023, max compression
```

## Comparing `hyperx-0.0.3.tar` & `hyperx-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.766935 hyperx-0.0.3/
--rw-rw-rw-   0        0        0      480 2023-03-22 16:10:26.766935 hyperx-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-21 18:16:23.000000 hyperx-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.719807 hyperx-0.0.3/hyperx/
--rw-rw-rw-   0        0        0      811 2023-03-22 15:40:41.000000 hyperx-0.0.3/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.752868 hyperx-0.0.3/hyperx/api/
--rw-rw-rw-   0        0        0       81 2023-03-21 19:10:07.000000 hyperx-0.0.3/hyperx/api/Db.py
--rw-rw-rw-   0        0        0       18 2023-03-21 22:33:02.000000 hyperx-0.0.3/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.759934 hyperx-0.0.3/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-22 15:40:30.000000 hyperx-0.0.3/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-21 22:52:18.000000 hyperx-0.0.3/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-21 20:33:51.000000 hyperx-0.0.3/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.763935 hyperx-0.0.3/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-21 22:47:36.000000 hyperx-0.0.3/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2014 2023-03-21 22:53:30.000000 hyperx-0.0.3/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 16:10:26.747261 hyperx-0.0.3/hyperx.egg-info/
--rw-rw-rw-   0        0        0      480 2023-03-22 16:10:26.000000 hyperx-0.0.3/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-03-22 16:10:26.000000 hyperx-0.0.3/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 16:10:26.000000 hyperx-0.0.3/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-22 16:10:26.000000 hyperx-0.0.3/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-22 16:10:26.000000 hyperx-0.0.3/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      584 2023-03-22 16:09:51.000000 hyperx-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 16:10:26.767992 hyperx-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.221887 hyperx-0.1.0/
+-rw-rw-rw-   0        0        0      535 2023-06-30 15:47:45.221887 hyperx-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.186131 hyperx-0.1.0/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.0/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.206360 hyperx-0.1.0/hyperx/api/
+-rw-rw-rw-   0        0        0   145913 2023-06-30 15:38:21.000000 hyperx-0.1.0/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.209350 hyperx-0.1.0/hyperx/api/types/
+-rw-rw-rw-   0        0        0    24178 2023-06-29 20:33:40.000000 hyperx-0.1.0/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.215329 hyperx-0.1.0/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.219894 hyperx-0.1.0/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.0/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.204370 hyperx-0.1.0/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-06-30 15:47:20.000000 hyperx-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 15:47:45.222885 hyperx-0.1.0/setup.cfg
```

### Comparing `hyperx-0.0.3/hyperx/library/find.py` & `hyperx-0.1.0/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.0.3/hyperx/library/library.py` & `hyperx-0.1.0/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.0.3/hyperx/utils/utils.py` & `hyperx-0.1.0/hyperx/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 """
 
 import os
 import subprocess
 import csv
 from pathlib import Path
 from typing import Any
+import errno
 
-from ..api import Db
+from ..api import Application
+from ..library import _api
 
-
-def Open(hdbPath: os.PathLike) -> Db:
+def Open(hdbPath: os.PathLike) -> Application:
     '''Opens a HyperX database for script access.'''
-    pass
+    if not os.path.isabs(hdbPath):
+        hdbPath = os.path.abspath(hdbPath)
+    
+    if not os.path.exists(hdbPath):
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), hdbPath)
+
+    _api.Environment.Initialize()
+    database = _api.Application()
+    database.OpenDatabase(hdbPath)
+    return Application(database)
 
 
 def OpenWithDefault(filepath: str):
     '''Opens a file in the default application for its file extension.'''
     cmd = f'explorer.exe "{Path(filepath)}"'
     CallExternalProcess(cmd)
```

