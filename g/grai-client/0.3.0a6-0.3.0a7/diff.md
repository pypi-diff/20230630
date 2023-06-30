# Comparing `tmp/grai_client-0.3.0a6.tar.gz` & `tmp/grai_client-0.3.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.3.0a6.tar", max compression
+gzip compressed data, was "grai_client-0.3.0a7.tar", max compression
```

## Comparing `grai_client-0.3.0a6.tar` & `grai_client-0.3.0a7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a6/README.md
--rw-r--r--   0        0        0     1239 2023-06-30 11:22:03.773897 grai_client-0.3.0a6/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-30 11:22:10.751754 grai_client-0.3.0a6/src/grai_client/__init__.py
--rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a6/src/grai_client/authentication.py
--rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a6/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a6/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a6/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a6/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a6/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a6/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a6/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/edge.py
--rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/node.py
--rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/organisation.py
--rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/source.py
--rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/utils.py
--rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/workspace.py
--rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a6/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a6/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a6/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a6/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a6/src/grai_client/errors.py
--rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a6/src/grai_client/integrations/__init__.py
--rw-r--r--   0        0        0     2654 2023-06-30 10:48:59.169885 grai_client-0.3.0a6/src/grai_client/integrations/base.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a6/src/grai_client/py.typed
--rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a6/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a6/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a6/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a6/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a6/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a6/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a6/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a6/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a6/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a7/README.md
+-rw-r--r--   0        0        0     1239 2023-06-30 11:50:18.659289 grai_client-0.3.0a7/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-30 11:50:14.898948 grai_client-0.3.0a7/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a7/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a7/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a7/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a7/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a7/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a7/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a7/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a7/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a7/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a7/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a7/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a7/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a7/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a7/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     2901 2023-06-30 11:52:08.294285 grai_client-0.3.0a7/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a7/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a7/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a7/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a7/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a7/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a7/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a7/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a7/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a7/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a7/PKG-INFO
```

### Comparing `grai_client-0.3.0a6/pyproject.toml` & `grai_client-0.3.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.3.0-alpha6"
+version = "0.3.0-alpha7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_client-0.3.0a6/src/grai_client/authentication.py` & `grai_client-0.3.0a7/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/client.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/rest.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/rest.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/utilities.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/client.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/edge.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/edge.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/node.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/node.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/organisation.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/organisation.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/source.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/source.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/utils.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/get/workspace.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/get/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/post.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/post.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/url.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.3.0a7/src/grai_client/endpoints/v1/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/integrations/base.py` & `grai_client-0.3.0a7/src/grai_client/integrations/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,47 +6,57 @@
 
 from grai_client.endpoints.v1.client import ClientV1
 from grai_client.update import update
 
 
 class EventMixin(ABC):
     def __init__(self):
-        raise NotImplementedError("The EventMixin is not yet stable or ready for production use.")
+        raise NotImplementedError(
+            "The EventMixin is not yet stable or ready for production use."
+        )
 
     @abstractmethod
     def events(self) -> List[Event]:
         pass
 
     def update(self):
         super().update()
         update(self.client, self.events())
 
 
 class GraiIntegrationImplementationV1(ABC):
     client: Optional[ClientV1]
     source: SourceV1
+    version: str
 
     def __init__(
         self,
         client: Optional[ClientV1] = None,
         source_name: Optional[str] = None,
         source: Optional[SourceSpec] = None,
+        version: Optional[str] = None,
     ):
         if source:
             self.source = SourceV1.from_spec(source)
+            self.version = version if version else "v1"
 
         elif client:
             if not source_name:
-                raise Exception("A source name must be provided if a client is provided")
+                raise Exception(
+                    "A source name must be provided if a client is provided"
+                )
 
             if client.id != "v1":
-                raise NotImplementedError(f"No available implementation for client version {client.id}")
+                raise NotImplementedError(
+                    f"No available implementation for client version {client.id}"
+                )
 
             self.client = client
             self.source = client.get("Source", name=source_name)
+            self.version = client.id
 
         else:
             raise Exception("Either a client or a source must be provided")
 
     @abstractmethod
     def nodes(self) -> List[SourcedNode]:
         pass
```

### Comparing `grai_client-0.3.0a6/src/grai_client/schemas/labels.py` & `grai_client-0.3.0a7/src/grai_client/schemas/labels.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/testing/schema.py` & `grai_client-0.3.0a7/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/update.py` & `grai_client-0.3.0a7/src/grai_client/update.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/src/grai_client/utilities/tests.py` & `grai_client-0.3.0a7/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a6/PKG-INFO` & `grai_client-0.3.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.3.0a6
+Version: 0.3.0a7
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

