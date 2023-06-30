# Comparing `tmp/py_brainage-0.0.3.tar.gz` & `tmp/py_brainage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_brainage-0.0.3.tar", last modified: Fri Jun 30 16:45:52 2023, max compression
+gzip compressed data, was "py_brainage-0.0.4.tar", last modified: Fri Jun 30 16:57:01 2023, max compression
```

## Comparing `py_brainage-0.0.3.tar` & `py_brainage-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:45:52.437244 py_brainage-0.0.3/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.3/LICENSE
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 16:45:52.437244 py_brainage-0.0.3/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.3/README.md
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:45:52.437244 py_brainage-0.0.3/py_brainage.egg-info/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 16:45:52.000000 py_brainage-0.0.3/py_brainage.egg-info/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      215 2023-06-30 16:45:52.000000 py_brainage-0.0.3/py_brainage.egg-info/SOURCES.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:45:52.000000 py_brainage-0.0.3/py_brainage.egg-info/dependency_links.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 16:45:52.000000 py_brainage-0.0.3/py_brainage.egg-info/requires.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:45:52.000000 py_brainage-0.0.3/py_brainage.egg-info/top_level.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      649 2023-06-30 16:17:33.000000 py_brainage-0.0.3/pyproject.toml
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 16:45:52.437244 py_brainage-0.0.3/setup.cfg
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      287 2023-06-30 16:41:51.000000 py_brainage-0.0.3/setup.py
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:57:01.277144 py_brainage-0.0.4/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.4/LICENSE
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 16:57:01.277144 py_brainage-0.0.4/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.4/README.md
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:57:01.277144 py_brainage-0.0.4/py_brainage.egg-info/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      178 2023-06-30 16:57:01.000000 py_brainage-0.0.4/py_brainage.egg-info/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      215 2023-06-30 16:57:01.000000 py_brainage-0.0.4/py_brainage.egg-info/SOURCES.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:57:01.000000 py_brainage-0.0.4/py_brainage.egg-info/dependency_links.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 16:57:01.000000 py_brainage-0.0.4/py_brainage.egg-info/requires.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:57:01.000000 py_brainage-0.0.4/py_brainage.egg-info/top_level.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      649 2023-06-30 16:17:33.000000 py_brainage-0.0.4/pyproject.toml
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 16:57:01.277144 py_brainage-0.0.4/setup.cfg
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      286 2023-06-30 16:56:11.000000 py_brainage-0.0.4/setup.py
```

### Comparing `py_brainage-0.0.3/LICENSE` & `py_brainage-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_brainage-0.0.3/pyproject.toml` & `py_brainage-0.0.4/pyproject.toml`

 * *Files identical despite different names*

