# Comparing `tmp/pyrorouter-0.1.0.tar.gz` & `tmp/pyrorouter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrorouter-0.1.0.tar", last modified: Mon Aug 15 12:12:39 2022, max compression
+gzip compressed data, was "pyrorouter-0.1.1.tar", max compression
```

## Comparing `pyrorouter-0.1.0.tar` & `pyrorouter-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-15 12:12:39.171625 pyrorouter-0.1.0/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2022-08-15 11:56:17.000000 pyrorouter-0.1.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    41144 2022-08-15 12:12:39.171625 pyrorouter-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)       42 2022-08-15 11:56:17.000000 pyrorouter-0.1.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)      678 2022-08-15 12:08:25.000000 pyrorouter-0.1.0/pyproject.toml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-15 12:12:39.167625 pyrorouter-0.1.0/pyrorouter/
--rw-r--r--   0 user      (1000) user      (1000)      140 2022-08-15 11:53:50.000000 pyrorouter-0.1.0/pyrorouter/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      527 2022-08-15 10:25:38.000000 pyrorouter-0.1.0/pyrorouter/client.py
--rw-r--r--   0 user      (1000) user      (1000)     3971 2022-08-15 11:43:05.000000 pyrorouter-0.1.0/pyrorouter/router.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-15 12:12:39.167625 pyrorouter-0.1.0/pyrorouter.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    41144 2022-08-15 12:12:39.000000 pyrorouter-0.1.0/pyrorouter.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      275 2022-08-15 12:12:39.000000 pyrorouter-0.1.0/pyrorouter.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-08-15 12:12:39.000000 pyrorouter-0.1.0/pyrorouter.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       27 2022-08-15 12:12:39.000000 pyrorouter-0.1.0/pyrorouter.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2022-08-15 12:12:39.000000 pyrorouter-0.1.0/pyrorouter.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-08-15 12:12:39.171625 pyrorouter-0.1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1583 2022-08-15 12:12:23.000000 pyrorouter-0.1.0/setup.py
+-rw-r--r--   0        0        0    35149 2023-06-30 15:27:15.820952 pyrorouter-0.1.1/LICENSE
+-rw-r--r--   0        0        0       42 2023-06-30 15:27:15.820952 pyrorouter-0.1.1/README.md
+-rw-r--r--   0        0        0      369 2023-06-30 15:27:15.824952 pyrorouter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-06-30 15:27:15.824952 pyrorouter-0.1.1/pyrorouter/__init__.py
+-rw-r--r--   0        0        0      527 2023-06-30 15:27:15.824952 pyrorouter-0.1.1/pyrorouter/client.py
+-rw-r--r--   0        0        0     3971 2023-06-30 15:27:15.824952 pyrorouter-0.1.1/pyrorouter/router.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 pyrorouter-0.1.1/PKG-INFO
```

### Comparing `pyrorouter-0.1.0/LICENSE` & `pyrorouter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrorouter-0.1.0/pyrorouter/client.py` & `pyrorouter-0.1.1/pyrorouter/client.py`

 * *Files identical despite different names*

### Comparing `pyrorouter-0.1.0/pyrorouter/router.py` & `pyrorouter-0.1.1/pyrorouter/router.py`

 * *Files identical despite different names*

