# Comparing `tmp/grai_graph-0.2.4a0.tar.gz` & `tmp/grai_graph-0.2.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_graph-0.2.4a0.tar", max compression
+gzip compressed data, was "grai_graph-0.2.4a2.tar", max compression
```

## Comparing `grai_graph-0.2.4a0.tar` & `grai_graph-0.2.4a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      211 2023-05-19 11:07:12.919359 grai_graph-0.2.4a0/README.md
--rw-r--r--   0        0        0      997 2023-06-30 04:44:12.057351 grai_graph-0.2.4a0/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-15 00:41:57.145583 grai_graph-0.2.4a0/src/grai_graph/__init__.py
--rw-r--r--   0        0        0     9328 2023-06-14 21:02:53.363823 grai_graph-0.2.4a0/src/grai_graph/analysis.py
--rw-r--r--   0        0        0      369 2023-06-14 21:02:53.293703 grai_graph-0.2.4a0/src/grai_graph/client_monkeypatch.py
--rw-r--r--   0        0        0     5595 2023-06-30 03:54:33.886359 grai_graph-0.2.4a0/src/grai_graph/graph.py
--rw-r--r--   0        0        0     3494 2023-06-30 04:33:56.941788 grai_graph-0.2.4a0/src/grai_graph/utils.py
--rw-r--r--   0        0        0     2697 2023-06-01 16:01:43.256572 grai_graph-0.2.4a0/src/grai_graph/visualizations.py
--rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 grai_graph-0.2.4a0/PKG-INFO
+-rw-r--r--   0        0        0      211 2023-05-19 11:07:12.919359 grai_graph-0.2.4a2/README.md
+-rw-r--r--   0        0        0     1010 2023-06-30 04:56:19.698170 grai_graph-0.2.4a2/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-06-30 04:56:19.703375 grai_graph-0.2.4a2/src/grai_graph/__init__.py
+-rw-r--r--   0        0        0     9328 2023-06-14 21:02:53.363823 grai_graph-0.2.4a2/src/grai_graph/analysis.py
+-rw-r--r--   0        0        0      369 2023-06-14 21:02:53.293703 grai_graph-0.2.4a2/src/grai_graph/client_monkeypatch.py
+-rw-r--r--   0        0        0     5595 2023-06-30 03:54:33.886359 grai_graph-0.2.4a2/src/grai_graph/graph.py
+-rw-r--r--   0        0        0     3494 2023-06-30 04:33:56.941788 grai_graph-0.2.4a2/src/grai_graph/utils.py
+-rw-r--r--   0        0        0     2697 2023-06-01 16:01:43.256572 grai_graph-0.2.4a2/src/grai_graph/visualizations.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 grai_graph-0.2.4a2/PKG-INFO
```

### Comparing `grai_graph-0.2.4a0/pyproject.toml` & `grai_graph-0.2.4a2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "grai-graph"
-version = "0.2.4-alpha"
+version = "0.2.4-alpha2"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-graph"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 networkx = "^2.8.5"
 pydantic = "^1.9.1"
-grai-client = "^0.2.18"
+grai-client = "^0.3.0-alpha3"
 matplotlib = {version = "^3.5.2", optional = true}
 pydot = {version = "^1.4.2", optional = true}
-grai-schemas = "^0.1.15"
+grai-schemas = "^0.2.0-alpha1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 isort = "^5.10.1"
 devtools = "^0.10.0"
```

### Comparing `grai_graph-0.2.4a0/src/grai_graph/analysis.py` & `grai_graph-0.2.4a2/src/grai_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.4a0/src/grai_graph/graph.py` & `grai_graph-0.2.4a2/src/grai_graph/graph.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.4a0/src/grai_graph/utils.py` & `grai_graph-0.2.4a2/src/grai_graph/utils.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.4a0/src/grai_graph/visualizations.py` & `grai_graph-0.2.4a2/src/grai_graph/visualizations.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.4a0/PKG-INFO` & `grai_graph-0.2.4a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-graph
-Version: 0.2.4a0
+Version: 0.2.4a2
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: vis
-Requires-Dist: grai-client (>=0.2.18,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0-alpha3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0-alpha1,<0.3.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "vis"
 Requires-Dist: networkx (>=2.8.5,<3.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "vis"
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-graph
 Description-Content-Type: text/markdown
```

