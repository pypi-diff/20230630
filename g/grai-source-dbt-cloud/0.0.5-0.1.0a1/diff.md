# Comparing `tmp/grai_source_dbt_cloud-0.0.5.tar.gz` & `tmp/grai_source_dbt_cloud-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.0.5.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.1.0a1.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.0.5.tar` & `grai_source_dbt_cloud-0.1.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-19 11:07:12.923589 grai_source_dbt_cloud-0.0.5/README.md
--rw-r--r--   0        0        0      999 2023-06-14 22:22:19.811168 grai_source_dbt_cloud-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-14 22:22:09.371760 grai_source_dbt_cloud-0.0.5/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0     1386 2023-06-14 21:02:53.391267 grai_source_dbt_cloud-0.0.5/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     4549 2023-06-14 21:02:53.427243 grai_source_dbt_cloud-0.0.5/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-19 11:07:12.925377 grai_source_dbt_cloud-0.0.5/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1124 2023-06-30 11:11:10.320468 grai_source_dbt_cloud-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-30 11:11:16.371161 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     1089 2023-06-29 12:55:58.976435 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     4549 2023-06-06 17:35:16.800994 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.0.5/pyproject.toml` & `grai_source_dbt_cloud-0.1.0a1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.0.5"
+version = "0.1.0-alpha1"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
@@ -12,17 +12,17 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = "^0.2.18"
-grai-schemas = "^0.1.15"
-grai-source-dbt = "^0.2.9"
+grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
+grai-source-dbt = {version = "^0.3.0a1", allow-prereleases = true}
 dbtc = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.991"
 black = "^22.12.0"
```

### Comparing `grai_source_dbt_cloud-0.0.5/src/grai_source_dbt_cloud/loader.py` & `grai_source_dbt_cloud-0.1.0a1/src/grai_source_dbt_cloud/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt_cloud-0.0.5/PKG-INFO` & `grai_source_dbt_cloud-0.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.0.5
+Version: 0.1.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbtc (>=0.4.2,<0.5.0)
-Requires-Dist: grai-client (>=0.2.18,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
-Requires-Dist: grai-source-dbt (>=0.2.9,<0.3.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
+Requires-Dist: grai-source-dbt (>=0.3.0a1,<0.4.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud
 Description-Content-Type: text/markdown
 
 # Grai dbt Cloud Integration
```

