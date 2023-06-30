# Comparing `tmp/grai_client-0.3.0a4.tar.gz` & `tmp/grai_client-0.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.3.0a4.tar", max compression
+gzip compressed data, was "grai_client-0.3.0a5.tar", max compression
```

## Comparing `grai_client-0.3.0a4.tar` & `grai_client-0.3.0a5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      168 2023-05-19 11:07:12.865820 grai_client-0.3.0a4/README.md
--rw-r--r--   0        0        0     1239 2023-06-30 05:39:58.363390 grai_client-0.3.0a4/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-30 05:39:56.864944 grai_client-0.3.0a4/src/grai_client/__init__.py
--rw-r--r--   0        0        0      643 2023-06-01 16:01:43.248134 grai_client-0.3.0a4/src/grai_client/authentication.py
--rw-r--r--   0        0        0      265 2023-06-01 16:01:43.248265 grai_client-0.3.0a4/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0    24172 2023-06-21 18:49:43.776824 grai_client-0.3.0a4/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0     1011 2023-06-23 08:42:59.012279 grai_client-0.3.0a4/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     7282 2023-06-23 08:42:59.422640 grai_client-0.3.0a4/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.3.0a4/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     3947 2023-06-20 17:08:01.030243 grai_client-0.3.0a4/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0     5369 2023-06-23 20:47:34.369379 grai_client-0.3.0a4/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0      121 2023-06-23 08:42:59.032276 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-23 20:47:34.378573 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/edge.py
--rw-r--r--   0        0        0     4895 2023-06-23 20:47:34.374014 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/node.py
--rw-r--r--   0        0        0      838 2023-06-22 21:15:12.449726 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/organisation.py
--rw-r--r--   0        0        0     2501 2023-06-23 08:42:59.006274 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/source.py
--rw-r--r--   0        0        0     1953 2023-06-23 20:47:34.390041 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/utils.py
--rw-r--r--   0        0        0     2622 2023-06-23 08:42:59.019314 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/workspace.py
--rw-r--r--   0        0        0     6704 2023-06-23 20:47:34.376525 grai_client-0.3.0a4/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     8301 2023-06-23 20:47:34.387631 grai_client-0.3.0a4/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0     3167 2023-06-23 20:47:34.371648 grai_client-0.3.0a4/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0     1102 2023-06-23 08:42:56.457027 grai_client-0.3.0a4/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0      307 2023-06-21 23:05:57.332295 grai_client-0.3.0a4/src/grai_client/errors.py
--rw-r--r--   0        0        0       42 2023-06-27 19:01:12.016896 grai_client-0.3.0a4/src/grai_client/integrations/__init__.py
--rw-r--r--   0        0        0     2155 2023-06-29 15:34:52.416731 grai_client-0.3.0a4/src/grai_client/integrations/base.py
--rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.3.0a4/src/grai_client/py.typed
--rw-r--r--   0        0        0       47 2023-06-19 23:02:00.694709 grai_client-0.3.0a4/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-23 18:41:02.198472 grai_client-0.3.0a4/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      417 2023-06-01 16:01:43.249849 grai_client-0.3.0a4/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.3.0a4/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-15 00:41:57.143647 grai_client-0.3.0a4/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     3516 2023-06-23 20:47:34.690459 grai_client-0.3.0a4/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.3.0a4/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      518 2023-06-01 16:01:43.250336 grai_client-0.3.0a4/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a4/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a5/README.md
+-rw-r--r--   0        0        0     1239 2023-06-30 08:56:19.976546 grai_client-0.3.0a5/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-30 08:56:29.594370 grai_client-0.3.0a5/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a5/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a5/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a5/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a5/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a5/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a5/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a5/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a5/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a5/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a5/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a5/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a5/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a5/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a5/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     2097 2023-06-30 08:51:37.620301 grai_client-0.3.0a5/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a5/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a5/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a5/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a5/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a5/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a5/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a5/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a5/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a5/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a5/PKG-INFO
```

### Comparing `grai_client-0.3.0a4/pyproject.toml` & `grai_client-0.3.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.3.0-alpha4"
+version = "0.3.0-alpha5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_client-0.3.0a4/src/grai_client/authentication.py` & `grai_client-0.3.0a5/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/client.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/rest.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/rest.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/utilities.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/client.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/edge.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/edge.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/node.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/node.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/organisation.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/organisation.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/source.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/source.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/utils.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/workspace.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/get/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/post.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/post.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/url.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.3.0a5/src/grai_client/endpoints/v1/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/integrations/base.py` & `grai_client-0.3.0a5/src/grai_client/integrations/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,10 +65,10 @@
 
 
 class ConnectorMixin(CombinedNodesAndEdgesMixin):
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         with self.connector.connect() as conn:
             nodes, edges = conn.get_nodes_and_edges()
 
-        nodes = self.adapt_to_client(nodes, self.source, self.client.id)
-        edges = self.adapt_to_client(edges, self.source, self.client.id)
+        nodes = self.adapt_to_client(nodes)
+        edges = self.adapt_to_client(edges)
         return nodes, edges
```

### Comparing `grai_client-0.3.0a4/src/grai_client/schemas/labels.py` & `grai_client-0.3.0a5/src/grai_client/schemas/labels.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/testing/schema.py` & `grai_client-0.3.0a5/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/update.py` & `grai_client-0.3.0a5/src/grai_client/update.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/src/grai_client/utilities/tests.py` & `grai_client-0.3.0a5/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a4/PKG-INFO` & `grai_client-0.3.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.3.0a4
+Version: 0.3.0a5
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

