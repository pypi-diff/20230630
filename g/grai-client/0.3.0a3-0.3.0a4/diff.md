# Comparing `tmp/grai_client-0.3.0a3.tar.gz` & `tmp/grai_client-0.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.3.0a3.tar", max compression
+gzip compressed data, was "grai_client-0.3.0a4.tar", max compression
```

## Comparing `grai_client-0.3.0a3.tar` & `grai_client-0.3.0a4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a3/README.md
--rw-r--r--   0        0        0     1239 2023-06-29 10:21:40.167754 grai_client-0.3.0a3/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-29 08:12:22.777016 grai_client-0.3.0a3/src/grai_client/__init__.py
--rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a3/src/grai_client/authentication.py
--rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a3/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a3/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a3/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a3/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a3/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a3/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a3/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/edge.py
--rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/node.py
--rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/organisation.py
--rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/source.py
--rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/utils.py
--rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/workspace.py
--rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a3/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a3/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a3/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a3/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a3/src/grai_client/errors.py
--rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a3/src/grai_client/integrations/__init__.py
--rw-r--r--   0        0        0     2149 2023-06-29 10:21:30.925245 grai_client-0.3.0a3/src/grai_client/integrations/base.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a3/src/grai_client/py.typed
--rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a3/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a3/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a3/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a3/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a3/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a3/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a3/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a3/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a3/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-19 11:07:12.865820 grai_client-0.3.0a4/README.md
+-rw-r--r--   0        0        0     1239 2023-06-30 05:39:58.363390 grai_client-0.3.0a4/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-30 05:39:56.864944 grai_client-0.3.0a4/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-01 16:01:43.248134 grai_client-0.3.0a4/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-01 16:01:43.248265 grai_client-0.3.0a4/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    24172 2023-06-21 18:49:43.776824 grai_client-0.3.0a4/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-06-23 08:42:59.012279 grai_client-0.3.0a4/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7282 2023-06-23 08:42:59.422640 grai_client-0.3.0a4/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.3.0a4/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     3947 2023-06-20 17:08:01.030243 grai_client-0.3.0a4/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-06-23 20:47:34.369379 grai_client-0.3.0a4/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-06-23 08:42:59.032276 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-23 20:47:34.378573 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4895 2023-06-23 20:47:34.374014 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0      838 2023-06-22 21:15:12.449726 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2501 2023-06-23 08:42:59.006274 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-06-23 20:47:34.390041 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     2622 2023-06-23 08:42:59.019314 grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     6704 2023-06-23 20:47:34.376525 grai_client-0.3.0a4/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8301 2023-06-23 20:47:34.387631 grai_client-0.3.0a4/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-06-23 20:47:34.371648 grai_client-0.3.0a4/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1102 2023-06-23 08:42:56.457027 grai_client-0.3.0a4/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-06-21 23:05:57.332295 grai_client-0.3.0a4/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-06-27 19:01:12.016896 grai_client-0.3.0a4/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     2155 2023-06-29 15:34:52.416731 grai_client-0.3.0a4/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.3.0a4/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-06-19 23:02:00.694709 grai_client-0.3.0a4/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-23 18:41:02.198472 grai_client-0.3.0a4/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-01 16:01:43.249849 grai_client-0.3.0a4/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.3.0a4/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-15 00:41:57.143647 grai_client-0.3.0a4/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3516 2023-06-23 20:47:34.690459 grai_client-0.3.0a4/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.3.0a4/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-01 16:01:43.250336 grai_client-0.3.0a4/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a4/PKG-INFO
```

### Comparing `grai_client-0.3.0a3/pyproject.toml` & `grai_client-0.3.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.3.0-alpha3"
+version = "0.3.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_client-0.3.0a3/src/grai_client/authentication.py` & `grai_client-0.3.0a4/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/client.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/rest.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/rest.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/utilities.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/client.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/edge.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/edge.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/node.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/node.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/organisation.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/organisation.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/source.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/source.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/utils.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/workspace.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/get/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/post.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/post.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/url.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.3.0a4/src/grai_client/endpoints/v1/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/integrations/base.py` & `grai_client-0.3.0a4/src/grai_client/integrations/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 from grai_client.endpoints.v1.client import ClientV1
 from grai_client.update import update
 
 
 class EventMixin(ABC):
     def __init__(self):
-        raise NotImplementedError(
-            "The EventMixin is not yet stable or ready for production use."
-        )
+        raise NotImplementedError("The EventMixin is not yet stable or ready for production use.")
 
     @abstractmethod
     def events(self) -> List[Event]:
         pass
 
     def update(self):
         update(self.client, self.events())
@@ -25,17 +23,15 @@
 
 class GraiIntegrationImplementationV1(ABC):
     client: ClientV1
     source: SourceV1
 
     def __init__(self, client: ClientV1, source_name: str):
         if client.id != "v1":
-            raise NotImplementedError(
-                f"No available implementation for client version {client.id}"
-            )
+            raise NotImplementedError(f"No available implementation for client version {client.id}")
 
         self.client = client
         self.source = client.get("Source", name=source_name)
 
     @abstractmethod
     def nodes(self) -> List[SourcedNode]:
         pass
@@ -69,10 +65,10 @@
 
 
 class ConnectorMixin(CombinedNodesAndEdgesMixin):
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         with self.connector.connect() as conn:
             nodes, edges = conn.get_nodes_and_edges()
 
-        nodes = self.adapt_to_client(nodes)
-        edges = self.adapt_to_client(edges)
+        nodes = self.adapt_to_client(nodes, self.source, self.client.id)
+        edges = self.adapt_to_client(edges, self.source, self.client.id)
         return nodes, edges
```

### Comparing `grai_client-0.3.0a3/src/grai_client/schemas/labels.py` & `grai_client-0.3.0a4/src/grai_client/schemas/labels.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/testing/schema.py` & `grai_client-0.3.0a4/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/update.py` & `grai_client-0.3.0a4/src/grai_client/update.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/src/grai_client/utilities/tests.py` & `grai_client-0.3.0a4/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a3/PKG-INFO` & `grai_client-0.3.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.3.0a3
+Version: 0.3.0a4
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

