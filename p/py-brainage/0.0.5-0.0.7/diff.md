# Comparing `tmp/py_brainage-0.0.5.tar.gz` & `tmp/py_brainage-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_brainage-0.0.5.tar", last modified: Fri Jun 30 17:02:27 2023, max compression
+gzip compressed data, was "py_brainage-0.0.7.tar", last modified: Fri Jun 30 17:28:55 2023, max compression
```

## Comparing `py_brainage-0.0.5.tar` & `py_brainage-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 17:02:27.887094 py_brainage-0.0.5/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.5/LICENSE
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 17:02:27.887094 py_brainage-0.0.5/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.5/README.md
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 17:02:27.887094 py_brainage-0.0.5/py_brainage.egg-info/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 17:02:27.000000 py_brainage-0.0.5/py_brainage.egg-info/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      215 2023-06-30 17:02:27.000000 py_brainage-0.0.5/py_brainage.egg-info/SOURCES.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 17:02:27.000000 py_brainage-0.0.5/py_brainage.egg-info/dependency_links.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 17:02:27.000000 py_brainage-0.0.5/py_brainage.egg-info/requires.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 17:02:27.000000 py_brainage-0.0.5/py_brainage.egg-info/top_level.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      649 2023-06-30 16:17:33.000000 py_brainage-0.0.5/pyproject.toml
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 17:02:27.887094 py_brainage-0.0.5/setup.cfg
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      286 2023-06-30 17:02:15.000000 py_brainage-0.0.5/setup.py
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 17:28:55.986854 py_brainage-0.0.7/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.7/LICENSE
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 17:28:55.986854 py_brainage-0.0.7/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.7/README.md
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 17:28:55.986854 py_brainage-0.0.7/py_brainage/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 12:41:05.000000 py_brainage-0.0.7/py_brainage/__init__.py
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     2943 2023-06-30 15:37:15.000000 py_brainage-0.0.7/py_brainage/trees.py
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 17:28:55.986854 py_brainage-0.0.7/py_brainage.egg-info/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 17:28:55.000000 py_brainage-0.0.7/py_brainage.egg-info/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      260 2023-06-30 17:28:55.000000 py_brainage-0.0.7/py_brainage.egg-info/SOURCES.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 17:28:55.000000 py_brainage-0.0.7/py_brainage.egg-info/dependency_links.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 17:28:55.000000 py_brainage-0.0.7/py_brainage.egg-info/requires.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       12 2023-06-30 17:28:55.000000 py_brainage-0.0.7/py_brainage.egg-info/top_level.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      649 2023-06-30 16:17:33.000000 py_brainage-0.0.7/pyproject.toml
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 17:28:55.986854 py_brainage-0.0.7/setup.cfg
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      287 2023-06-30 17:28:08.000000 py_brainage-0.0.7/setup.py
```

### Comparing `py_brainage-0.0.5/LICENSE` & `py_brainage-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_brainage-0.0.5/pyproject.toml` & `py_brainage-0.0.7/pyproject.toml`

 * *Files identical despite different names*

