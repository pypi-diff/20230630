# Comparing `tmp/neon_gui-1.1.3a8.tar.gz` & `tmp/neon_gui-1.1.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_gui-1.1.3a8.tar", last modified: Tue Jun 27 21:41:13 2023, max compression
+gzip compressed data, was "neon_gui-1.1.3a9.tar", last modified: Thu Jun 29 22:17:32 2023, max compression
```

## Comparing `neon_gui-1.1.3a8.tar` & `neon_gui-1.1.3a9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/neon_gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/neon_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/neon_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 21:41:13.000000 neon_gui-1.1.3a8/neon_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:41:13.599428 neon_gui-1.1.3a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-27 21:41:03.000000 neon_gui-1.1.3a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/neon_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/neon_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/neon_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:17:32.000000 neon_gui-1.1.3a9/neon_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:17:32.507185 neon_gui-1.1.3a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-29 22:17:28.000000 neon_gui-1.1.3a9/setup.py
```

### Comparing `neon_gui-1.1.3a8/LICENSE.md` & `neon_gui-1.1.3a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/PKG-INFO` & `neon_gui-1.1.3a9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_gui
-Version: 1.1.3a8
+Version: 1.1.3a9
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a8/README.md` & `neon_gui-1.1.3a9/README.md`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui/__init__.py` & `neon_gui-1.1.3a9/neon_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui/__main__.py` & `neon_gui-1.1.3a9/neon_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui/cli.py` & `neon_gui-1.1.3a9/neon_gui/cli.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui/service.py` & `neon_gui-1.1.3a9/neon_gui/service.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui/utils.py` & `neon_gui-1.1.3a9/neon_gui/utils.py`

 * *Files identical despite different names*

### Comparing `neon_gui-1.1.3a8/neon_gui.egg-info/PKG-INFO` & `neon_gui-1.1.3a9/neon_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.3a8
+Version: 1.1.3a9
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_gui-1.1.3a8/setup.py` & `neon_gui-1.1.3a9/setup.py`

 * *Files identical despite different names*

