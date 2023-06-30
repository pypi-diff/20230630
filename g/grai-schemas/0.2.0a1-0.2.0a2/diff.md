# Comparing `tmp/grai_schemas-0.2.0a1.tar.gz` & `tmp/grai_schemas-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a1.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a2.tar", max compression
```

## Comparing `grai_schemas-0.2.0a1.tar` & `grai_schemas-0.2.0a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a1/README.md
--rw-r--r--   0        0        0      834 2023-06-29 09:52:52.322058 grai_schemas-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      203 2023-06-29 08:12:22.804283 grai_schemas-0.2.0a1/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      590 2023-06-29 08:12:22.804823 grai_schemas-0.2.0a1/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3715 2023-06-29 08:12:22.804993 grai_schemas-0.2.0a1/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a1/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a1/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a1/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      701 2023-06-06 17:35:16.829170 grai_schemas-0.2.0a1/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2568 2023-06-16 16:15:18.436927 grai_schemas-0.2.0a1/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      440 2023-06-29 08:12:22.805122 grai_schemas-0.2.0a1/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     2786 2023-06-29 08:12:22.805233 grai_schemas-0.2.0a1/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0        0 2023-06-29 08:12:22.805263 grai_schemas-0.2.0a1/src/grai_schemas/v1/events
--rw-r--r--   0        0        0      845 2023-06-29 08:12:22.805491 grai_schemas-0.2.0a1/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      858 2023-06-29 08:12:22.805602 grai_schemas-0.2.0a1/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-29 08:12:22.805723 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      321 2023-06-16 16:15:18.437462 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0      779 2023-06-29 08:12:22.805839 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     1873 2023-06-29 08:12:22.805942 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     6925 2023-06-29 08:12:22.806053 grai_schemas-0.2.0a1/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     2776 2023-06-29 08:12:22.806146 grai_schemas-0.2.0a1/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-06-29 08:12:22.806213 grai_schemas-0.2.0a1/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1325 2023-06-29 08:12:22.806285 grai_schemas-0.2.0a1/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3686 2023-06-29 08:12:22.806382 grai_schemas-0.2.0a1/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a2/README.md
+-rw-r--r--   0        0        0      834 2023-06-30 04:33:29.224911 grai_schemas-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-06-23 20:49:31.413799 grai_schemas-0.2.0a2/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-30 04:32:44.479884 grai_schemas-0.2.0a2/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3715 2023-06-19 19:58:41.663555 grai_schemas-0.2.0a2/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a2/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a2/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a2/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      671 2023-06-30 04:31:27.905478 grai_schemas-0.2.0a2/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2568 2023-06-15 00:41:57.157492 grai_schemas-0.2.0a2/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      440 2023-06-21 00:58:14.451681 grai_schemas-0.2.0a2/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     2786 2023-06-23 08:42:59.409297 grai_schemas-0.2.0a2/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:53:35.574143 grai_schemas-0.2.0a2/src/grai_schemas/v1/events
+-rw-r--r--   0        0        0      845 2023-06-21 00:58:14.478004 grai_schemas-0.2.0a2/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      858 2023-06-23 06:29:43.639982 grai_schemas-0.2.0a2/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-19 19:58:41.664190 grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      321 2023-06-15 00:41:57.158515 grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      779 2023-06-19 19:58:41.664345 grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     2024 2023-06-30 03:38:58.072088 grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     6925 2023-06-23 20:47:34.762065 grai_schemas-0.2.0a2/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     2776 2023-06-23 07:31:48.438313 grai_schemas-0.2.0a2/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-06-23 08:42:59.385413 grai_schemas-0.2.0a2/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1325 2023-06-21 19:43:14.334934 grai_schemas-0.2.0a2/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3686 2023-06-23 06:29:43.642768 grai_schemas-0.2.0a2/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a2/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a1/LICENSE` & `grai_schemas-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/pyproject.toml` & `grai_schemas-0.2.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha1"
+version = "0.2.0-alpha2"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
```

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/base.py` & `grai_schemas-0.2.0a2/src/grai_schemas/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,10 +16,13 @@
 Edge = v1.edge.EdgeV1
 
 
 SourcedNode = v1.node.SourcedNodeV1
 SourcedEdge = v1.edge.SourcedEdgeV1
 Source = v1.source.SourceV1
 Event = v1.events.EventV1
+Workspace = v1.workspace.WorkspaceV1
+Organisation = v1.organization.OrganisationV1
 
+GraiType = Union[Node, Edge, SourcedNode, SourcedEdge, Source, Event, Workspace, Organisation]
 
-__all__ = ["GraiMetadata", "Node", "Edge", "SourcedNode", "SourcedEdge", "Source"]
+__all__ = ["GraiMetadata", "Node", "Edge", "SourcedNode", "SourcedEdge", "Source", "Workspace", "Organisation", "GraiType"]
```

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a2/src/grai_schemas/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a2/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a2/src/grai_schemas/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Literal, Union
 
-from grai_schemas.base import Edge, Node
+from grai_schemas.base import GraiType
 from grai_schemas.generics import GraiBaseModel
 
-GraiType = Union[Node, Edge]
+
 
 
 class Schema(GraiBaseModel):
     """ """
 
     entity: GraiType
```

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a2/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/edges.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/metadata/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,8 +70,16 @@
 class TableMetadata(BaseNodeMetadataV1):
     """ """
 
     node_type: Literal["Table"]
     node_attributes: TableAttributes = TableAttributes()
 
 
+x = {
+    'version': 'v1',
+    'node_type': NodeMetadataTypeLabels.table.value,
+    'node_attributes': {},
+    'tags': ['a_tag']
+}
+TableMetadata(**x)
+
 Metadata = Union[ColumnMetadata, TableMetadata, GenericNodeMetadataV1]
```

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/mock.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/mock.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/source.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a2/src/grai_schemas/v1/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a1/PKG-INFO` & `grai_schemas-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

