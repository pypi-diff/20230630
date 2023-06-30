# Comparing `tmp/pypandora-1.4.0.tar.gz` & `tmp/pypandora-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypandora-1.4.0.tar", max compression
+gzip compressed data, was "pypandora-1.5.0.tar", max compression
```

## Comparing `pypandora-1.4.0.tar` & `pypandora-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1706 2022-01-22 01:01:50.539848 pypandora-1.4.0/LICENSE
--rw-r--r--   0        0        0     1176 2022-10-24 15:12:26.293308 pypandora-1.4.0/README.md
--rw-r--r--   0        0        0     1819 2022-05-06 12:40:32.243438 pypandora-1.4.0/pypandora/__init__.py
--rw-r--r--   0        0        0     9697 2023-02-20 13:01:38.696822 pypandora-1.4.0/pypandora/api.py
--rw-r--r--   0        0        0        0 2021-12-30 14:56:01.442918 pypandora-1.4.0/pypandora/py.typed
--rw-r--r--   0        0        0     1371 2023-03-31 10:38:02.951806 pypandora-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 pypandora-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1706 2022-01-22 01:01:50.539848 pypandora-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1176 2022-10-24 15:12:26.293308 pypandora-1.5.0/README.md
+-rw-r--r--   0        0        0     1819 2022-05-06 12:40:32.243438 pypandora-1.5.0/pypandora/__init__.py
+-rw-r--r--   0        0        0     9697 2023-02-20 13:01:38.696822 pypandora-1.5.0/pypandora/api.py
+-rw-r--r--   0        0        0        0 2021-12-30 14:56:01.442918 pypandora-1.5.0/pypandora/py.typed
+-rw-r--r--   0        0        0     1457 2023-06-30 14:03:28.310680 pypandora-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pypandora-1.5.0/PKG-INFO
```

### Comparing `pypandora-1.4.0/LICENSE` & `pypandora-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypandora-1.4.0/README.md` & `pypandora-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pypandora-1.4.0/pypandora/__init__.py` & `pypandora-1.5.0/pypandora/__init__.py`

 * *Files identical despite different names*

### Comparing `pypandora-1.4.0/pypandora/api.py` & `pypandora-1.5.0/pypandora/api.py`

 * *Files identical despite different names*

### Comparing `pypandora-1.4.0/pyproject.toml` & `pypandora-1.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypandora"
-version = "1.4.0"
+version = "1.5.0"
 description = "Python CLI and module for pandora"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/pandora-analysis/pypandora"
 documentation = "https://pypandora.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -29,22 +29,25 @@
 include = ['README.md']
 
 [tool.poetry.scripts]
 pandora = 'pypandora:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.2"
-Sphinx = { version = "^6.1.3", optional = true }
+requests = "^2.31.0"
+Sphinx = { version = "^7.0.1", optional = true }
 
-[tool.poetry.dev-dependencies]
-mypy = "^1.1.1"
-types-requests = "^2.28.11.17"
-ipython = "^8.12.0"
-pytest = "^7.2.2"
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.4.1"
+types-requests = "^2.31.0.1"
+ipython = [
+    {version = "<8.13.0", python = "<3.9"},
+    {version = "^8.13.0", python = ">=3.9"}
+]
+pytest = "^7.4.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

