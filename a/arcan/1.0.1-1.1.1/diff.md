# Comparing `tmp/arcan-1.0.1.tar.gz` & `tmp/arcan-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.0.1.tar", max compression
+gzip compressed data, was "arcan-1.1.1.tar", max compression
```

## Comparing `arcan-1.0.1.tar` & `arcan-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1566 2023-06-28 16:20:57.850099 arcan-1.0.1/LICENSE
--rw-r--r--   0        0        0     1167 2023-06-28 16:20:57.854099 arcan-1.0.1/README.md
--rw-r--r--   0        0        0       44 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/engines/__init__.py
--rw-r--r--   0        0        0       23 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-06-28 16:20:57.854099 arcan-1.0.1/arcan/session/__init__.py
--rw-r--r--   0        0        0      561 2023-06-28 16:20:57.854099 arcan-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 arcan-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1566 2023-06-30 05:14:18.086413 arcan-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3924 2023-06-30 05:14:18.086413 arcan-1.1.1/README.md
+-rw-r--r--   0        0        0       44 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-30 05:14:18.086413 arcan-1.1.1/api/arcan/session/__init__.py
+-rw-r--r--   0        0        0      614 2023-06-30 05:14:18.090413 arcan-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 arcan-1.1.1/PKG-INFO
```

### Comparing `arcan-1.0.1/LICENSE` & `arcan-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.0.1/pyproject.toml` & `arcan-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "arcan"
-version = "1.0.1"
+version = "1.1.1"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+packages = [{include = "api/arcan"}]
+
 
 [tool.poetry.dependencies]
 python = "^3.10"
-databricks-session = "^0.2.1"
+fastapi = "^0.98.0"
+uvicorn = "^0.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-arcan = 'main:main'
+arcan = 'api.arcan:main'
```

