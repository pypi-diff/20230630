# Comparing `tmp/grai_graph-0.2.3.tar.gz` & `tmp/grai_graph-0.2.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_graph-0.2.3.tar", max compression
+gzip compressed data, was "grai_graph-0.2.4a0.tar", max compression
```

## Comparing `grai_graph-0.2.3.tar` & `grai_graph-0.2.4a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      211 2023-05-19 11:07:12.919359 grai_graph-0.2.3/README.md
--rw-r--r--   0        0        0      991 2023-06-14 22:53:01.212296 grai_graph-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-14 22:53:01.217484 grai_graph-0.2.3/src/grai_graph/__init__.py
--rw-r--r--   0        0        0     9328 2023-06-14 21:02:53.363823 grai_graph-0.2.3/src/grai_graph/analysis.py
--rw-r--r--   0        0        0      369 2023-06-14 21:02:53.293703 grai_graph-0.2.3/src/grai_graph/client_monkeypatch.py
--rw-r--r--   0        0        0     5594 2023-06-01 16:01:43.256304 grai_graph-0.2.3/src/grai_graph/graph.py
--rw-r--r--   0        0        0     3941 2023-06-14 22:10:38.552183 grai_graph-0.2.3/src/grai_graph/utils.py
--rw-r--r--   0        0        0     2697 2023-06-01 16:01:43.256572 grai_graph-0.2.3/src/grai_graph/visualizations.py
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 grai_graph-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      211 2023-05-19 11:07:12.919359 grai_graph-0.2.4a0/README.md
+-rw-r--r--   0        0        0      997 2023-06-30 04:44:12.057351 grai_graph-0.2.4a0/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-15 00:41:57.145583 grai_graph-0.2.4a0/src/grai_graph/__init__.py
+-rw-r--r--   0        0        0     9328 2023-06-14 21:02:53.363823 grai_graph-0.2.4a0/src/grai_graph/analysis.py
+-rw-r--r--   0        0        0      369 2023-06-14 21:02:53.293703 grai_graph-0.2.4a0/src/grai_graph/client_monkeypatch.py
+-rw-r--r--   0        0        0     5595 2023-06-30 03:54:33.886359 grai_graph-0.2.4a0/src/grai_graph/graph.py
+-rw-r--r--   0        0        0     3494 2023-06-30 04:33:56.941788 grai_graph-0.2.4a0/src/grai_graph/utils.py
+-rw-r--r--   0        0        0     2697 2023-06-01 16:01:43.256572 grai_graph-0.2.4a0/src/grai_graph/visualizations.py
+-rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 grai_graph-0.2.4a0/PKG-INFO
```

### Comparing `grai_graph-0.2.3/pyproject.toml` & `grai_graph-0.2.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-graph"
-version = "0.2.3"
+version = "0.2.4-alpha"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-graph"
 documentation = "https://docs.grai.io/"
```

### Comparing `grai_graph-0.2.3/src/grai_graph/analysis.py` & `grai_graph-0.2.4a0/src/grai_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.3/src/grai_graph/graph.py` & `grai_graph-0.2.4a0/src/grai_graph/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,12 +228,13 @@
         version (str):
 
     Returns:
 
     Raises:
 
     """
+
     nodes = process_items(nodes, version, "Node")
     edges = process_items(edges, version, "Edge")
     manifest = GraphManifest(nodes, edges)
 
     return Graph(manifest)
```

### Comparing `grai_graph-0.2.3/src/grai_graph/utils.py` & `grai_graph-0.2.4a0/src/grai_graph/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-from grai_schemas.v1 import EdgeV1, NodeV1
+from grai_schemas.v1 import EdgeV1, NodeV1, mock
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnAttributes,
     ColumnToColumnMetadata,
     EdgeMetadataTypeLabels,
     GenericEdgeMetadataV1,
 )
 from grai_schemas.v1.metadata.nodes import (
@@ -21,14 +21,15 @@
 
 class TestNodeObj(BaseModel):
     """ """
 
     name: str
     namespace: Optional[str] = DEFAULT_NAMESPACE
     node_attributes: Optional[ColumnAttributes] = None
+    data_sources: List[Any] = []
 
     def __hash__(self):
         return hash((self.name, self.namespace))
 
 
 def mock_v1_node(node: Union[str, TestNodeObj]):
     """
@@ -40,31 +41,23 @@
 
     Raises:
 
     """
     if isinstance(node, str):
         node = TestNodeObj(name=node)
 
-    metadata = node.node_attributes if node.node_attributes is not None else {}
-    node_dict = {
-        "type": "Node",
-        "version": "v1",
-        "spec": {
-            "id": None,
-            "name": node.name,
-            "namespace": node.namespace,
-            "data_source": "test_source",
-            "display_name": node.name,
-            "is_active": True,
-            "metadata": {
-                "grai": ColumnMetadata(node_type=NodeMetadataTypeLabels.column.value, node_attributes=metadata).dict()
-            },
-        },
+    node_attributes = node.node_attributes if node.node_attributes is not None else {}
+    metadata = {
+        "grai": ColumnMetadata(node_type=NodeMetadataTypeLabels.column.value, node_attributes=node_attributes).dict()
     }
-    return NodeV1(**node_dict)
+
+    node = mock.MockV1.node.node(
+        id=None, name=node.name, namespace=node.namespace, data_source="test_source", is_active=True, metadata=metadata
+    )
+    return node
 
 
 def mock_v1_edge(
     source_node: Union[str, TestNodeObj],
     destination_node: Union[str, TestNodeObj],
     metadata={},
 ):
@@ -81,37 +74,31 @@
 
     """
     if isinstance(source_node, str):
         source_node = TestNodeObj(name=source_node)
     if isinstance(destination_node, str):
         destination_node = TestNodeObj(name=destination_node)
 
-    edge_dict = {
-        "type": "Edge",
-        "version": "v1",
-        "spec": {
-            "id": None,
-            "name": f"{source_node.namespace}.{source_node.name} -> {destination_node.namespace}.{destination_node.name}",
-            "namespace": source_node.namespace,
-            "data_source": "test_source",
-            "source": {"name": source_node.name, "namespace": source_node.namespace},
-            "destination": {
-                "name": destination_node.name,
-                "namespace": destination_node.namespace,
-            },
-            "is_active": True,
-            "metadata": {
-                "grai": ColumnToColumnMetadata(
-                    edge_type=EdgeMetadataTypeLabels.column_to_column.value,
-                    edge_attributes=metadata,
-                ).dict()
-            },
-        },
+    metadata = {
+        "grai": ColumnToColumnMetadata(
+            edge_type=EdgeMetadataTypeLabels.column_to_column.value,
+            edge_attributes=metadata,
+        )
     }
-    return EdgeV1(**edge_dict)
+    name = f"{source_node.namespace}.{source_node.name} -> {destination_node.namespace}.{destination_node.name}"
+    edge = mock.MockV1.edge.edge(
+        id=None,
+        name=name,
+        namespace=source_node.namespace,
+        source=source_node.dict(),
+        destination=destination_node.dict(),
+        is_active=True,
+        metadata=metadata,
+    )
+    return edge
 
 
 def build_graph_from_map(map: Dict[Union[str, TestNodeObj], List[Tuple[str, ColumnToColumnAttributes]]]) -> graph.Graph:
     """
 
     Args:
         map (Dict[Union[str, TestNodeObj]):
```

### Comparing `grai_graph-0.2.3/src/grai_graph/visualizations.py` & `grai_graph-0.2.4a0/src/grai_graph/visualizations.py`

 * *Files identical despite different names*

### Comparing `grai_graph-0.2.3/PKG-INFO` & `grai_graph-0.2.4a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-graph
-Version: 0.2.3
+Version: 0.2.4a0
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

