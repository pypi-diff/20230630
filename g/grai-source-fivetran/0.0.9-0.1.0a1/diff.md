# Comparing `tmp/grai_source_fivetran-0.0.9.tar.gz` & `tmp/grai_source_fivetran-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.9.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.1.0a1.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.9.tar` & `grai_source_fivetran-0.1.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.9/README.md
--rw-r--r--   0        0        0     1092 2023-06-14 22:23:33.925985 grai_source_fivetran-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-14 22:23:33.932002 grai_source_fivetran-0.0.9/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     8750 2023-06-14 22:10:38.525486 grai_source_fivetran-0.0.9/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2937 2023-06-14 21:10:34.441273 grai_source_fivetran-0.0.9/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   451222 2023-06-01 16:01:43.261936 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    69211 2023-06-01 16:01:43.262231 grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    16866 2023-06-14 21:02:53.368839 grai_source_fivetran-0.0.9/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     2173 2023-06-01 16:01:43.262518 grai_source_fivetran-0.0.9/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     5452 2023-06-14 21:02:53.331689 grai_source_fivetran-0.0.9/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      199 2023-06-01 16:01:43.262730 grai_source_fivetran-0.0.9/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.9/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1177 2023-06-30 04:49:28.754498 grai_source_fivetran-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-06-30 04:49:28.760080 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     9094 2023-06-29 15:34:52.423570 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2426 2023-06-29 15:34:52.424077 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   451222 2023-06-01 16:01:43.261936 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    69211 2023-06-01 16:01:43.262231 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    16866 2023-06-14 21:02:53.368839 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     2173 2023-06-01 16:01:43.262518 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     5452 2023-06-14 21:02:53.331689 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.262730 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.9/pyproject.toml` & `grai_source_fivetran-0.1.0a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.9"
+version = "0.1.0-alpha1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
@@ -12,20 +12,20 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
-grai-client = "^0.2.18"
+grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
-grai-schemas = "^0.1.15"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.12.0"
 pytest = "^7.2.0"
 pre-commit = "^3.0.4"
```

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-from typing import Any, Dict, List, Literal, Sequence, Type, Union
+from typing import Any, Dict, List, Literal, Sequence, TypeVar, Union
 
 from grai_schemas import config as base_config
-from grai_schemas.generics import DefaultValue
-from grai_schemas.schema import Schema
-from grai_schemas.v1 import EdgeV1, NodeV1
+from grai_schemas.v1 import SourcedEdgeV1, SourcedNodeV1, SourceV1
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnMetadata,
     EdgeMetadataTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
     TableToTableMetadata,
 )
-from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeMetadataTypeLabels, TableMetadata
+from grai_schemas.v1.metadata.nodes import (
+    ColumnMetadata,
+    NodeMetadataTypeLabels,
+    TableMetadata,
+)
+from grai_schemas.v1.source import SourceSpec
 from multimethod import multimethod
 
 from grai_source_fivetran.models import Column, Edge, NodeTypes, Table
 from grai_source_fivetran.package_definitions import config
 
+T = TypeVar("T")
+X = TypeVar("X")
+Y = TypeVar("Y")
+
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
     """
 
     Args:
         current (Any):
@@ -115,15 +122,21 @@
             return TableToColumnMetadata(**data)
         elif isinstance(current.destination, Table):
             data["edge_type"] = EdgeMetadataTypeLabels.table_to_table.value
             return TableToTableMetadata(**data)
     elif isinstance(current.source, Column):
         if isinstance(current.destination, Column):
             data["edge_type"] = EdgeMetadataTypeLabels.column_to_column.value
-            data.update({"preserves_data_type": True, "preserves_nullable": True, "preserves_unique": True})
+            data.update(
+                {
+                    "preserves_data_type": True,
+                    "preserves_nullable": True,
+                    "preserves_unique": True,
+                }
+            )
             return ColumnToColumnMetadata(**data)
 
     data["edge_type"] = EdgeMetadataTypeLabels.generic.value
     return GenericEdgeMetadataV1(**data)
 
 
 @multimethod
@@ -239,15 +252,15 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_column_to_client(current: Column, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_column_to_client(current: Column, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Column):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -255,22 +268,22 @@
     Raises:
 
     """
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
-        "data_source": config.integration_name,
+        "data_source": source,
         "metadata": build_metadata(current, version),
     }
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_table_to_client(current: Table, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Table):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -278,18 +291,18 @@
     Raises:
 
     """
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
-        "data_source": config.integration_name,
+        "data_source": source,
         "metadata": build_metadata(current, version),
     }
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: NodeTypes, node2: NodeTypes) -> str:
     """
 
     Args:
         node1 (NodeTypes):
@@ -302,66 +315,75 @@
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1") -> EdgeV1:
+def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
-        "data_source": config.integration_name,
+        "data_source": source,
         "name": make_name(current.source, current.destination),
         "namespace": current.source.namespace,
         "source": {
             "name": current.source.full_name,
             "namespace": current.source.namespace,
         },
         "destination": {
             "name": current.destination.full_name,
             "namespace": current.destination.namespace,
         },
         "metadata": build_metadata(current, version),
     }
-    return Schema.to_model(spec_dict, version=version, typing_type="Edge")
+    return SourcedEdgeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_seq_to_client(objs: Sequence, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_seq_to_client(
+    objs: Sequence, source: SourceSpec, version: Literal["v1"]
+) -> List[Union[SourcedNodeV1, SourcedEdgeV1]]:
     """
 
     Args:
         objs (Sequence):
         version (Literal["v1"]):
 
     Returns:
 
     Raises:
 
     """
-    return [adapt_to_client(item, version) for item in objs]
+    return [adapt_to_client(item, source, version) for item in objs]
 
 
 @adapt_to_client.register
-def adapt_list_to_client(objs: List, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_list_to_client(
+    objs: List, source: SourceSpec, version: Literal["v1"]
+) -> List[Union[SourcedNodeV1, SourcedEdgeV1]]:
     """
 
     Args:
         objs (List):
         version (Literal["v1"]):
 
     Returns:
 
     Raises:
 
     """
-    return [adapt_to_client(item, version) for item in objs]
+    return [adapt_to_client(item, source, version) for item in objs]
+
+
+@adapt_to_client.register
+def adapt_source_spec_v1_to_client(obj: X, source: SourceV1, version: Y) -> T:
+    return adapt_to_client(obj, source.spec, version)
```

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,67 @@
-from functools import partial
-from typing import List, Literal, Optional, Tuple
+from typing import List, Optional, Tuple
 
 from grai_client.endpoints.client import BaseClient
-from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_client.integrations.base import (
+    CombinedNodesAndEdgesMixin,
+    GraiIntegrationImplementationV1,
+)
+from grai_schemas.base import SourcedEdge, SourcedNode
 
 from grai_source_fivetran.adapters import adapt_to_client
 from grai_source_fivetran.loader import FivetranConnector, NamespaceTypes
 
 
-def validate_nodes_and_edges(nodes: List[Node], edges: List[Edge]):
-    """
-
-    Args:
-        nodes (List[Node]):
-        edges (List[Edge]):
-
-    Returns:
-
-    Raises:
-
-    """
-    node_hashes = [hash(node) for node in nodes]
-    if (n_hashes := len(set(node_hashes))) == len(nodes):
-        message = (
-            f"The Fivetran connection generated {len(nodes) - n_hashes} duplicated nodes. "
-            f"This is likely because there are multiple Fivetran tables with the same name. "
-            f"You can disambiguate these tables by identifying them with different namespaces. Please "
-            f"see the documentation for more information. https://docs.grai.io/tooling/github-actions#fivetran"
+class FivetranIntegration(CombinedNodesAndEdgesMixin, GraiIntegrationImplementationV1):
+    def __init__(
+        self,
+        client: BaseClient,
+        source_name: str,
+        namespaces: Optional[NamespaceTypes] = None,
+        default_namespace: Optional[str] = None,
+        parallelization: int = 10,
+        api_key: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        endpoint: Optional[str] = None,
+        limit: Optional[int] = None,
+    ):
+        super().__init__(client, source_name)
+
+        self.connector = FivetranConnector(
+            namespaces=namespaces,
+            default_namespace=default_namespace,
+            parallelization=parallelization,
+            api_key=api_key,
+            api_secret=api_secret,
+            endpoint=endpoint,
+            limit=limit,
         )
-        raise ValueError(message)
-
-
-def get_nodes_and_edges(connector: FivetranConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
-    """
-
-    Args:
-        connector (FivetranConnector):
-        version (Literal["v1"]):
-
-    Returns:
-
-    Raises:
-
-    """
-    nodes, edges = connector.get_nodes_and_edges()
-
-    nodes = adapt_to_client(nodes, version)
-    edges = adapt_to_client(edges, version)
-    validate_nodes_and_edges(nodes, edges)
-    return nodes, edges
-
-
-def update_server(
-    client: BaseClient,
-    namespaces: Optional[NamespaceTypes] = None,
-    default_namespace: Optional[str] = None,
-    api_key: Optional[str] = None,
-    api_secret: Optional[str] = None,
-    endpoint: Optional[str] = None,
-    limit: Optional[int] = None,
-    parallelization: Optional[int] = None,
-):
-    """
-
-    Args:
-        client (BaseClient):
-        namespaces (Optional[NamespaceTypes], optional):  (Default value = None)
-        default_namespace (Optional[str], optional):  (Default value = None)
-        api_key (Optional[str], optional):  (Default value = None)
-        api_secret (Optional[str], optional):  (Default value = None)
-        endpoint (Optional[str], optional):  (Default value = None)
-        limit (Optional[int], optional):  (Default value = None)
-        parallelization (Optional[int], optional):  (Default value = None)
-
-    Returns:
-
-    Raises:
-
-    """
-    kwargs = {
-        "namespaces": namespaces,
-        "default_namespace": default_namespace,
-        "api_key": api_key,
-        "api_secret": api_secret,
-        "endpoint": endpoint,
-        "limit": limit,
-        "parallelization": parallelization,
-    }
-    kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
-    conn = FivetranConnector(**kwargs)
-    nodes, edges = get_nodes_and_edges(conn, client.id)
+    def validate_nodes_and_edges(self, nodes: List[SourcedNode], edges: List[SourcedEdge]):
+        """
 
-    update(client, nodes)
-    update(client, edges)
+        Args:
+            nodes (List[Node]):
+            edges (List[Edge]):
+
+        Returns:
+
+        Raises:
+
+        """
+        node_hashes = [hash(node) for node in nodes]
+        if (n_hashes := len(set(node_hashes))) == len(nodes):
+            message = (
+                f"The Fivetran connection generated {len(nodes) - n_hashes} duplicated nodes. "
+                f"This is likely because there are multiple Fivetran tables with the same name. "
+                f"You can disambiguate these tables by identifying them with different namespaces. Please "
+                f"see the documentation for more information. https://docs.grai.io/tooling/github-actions#fivetran"
+            )
+            raise ValueError(message)
+
+    def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
+        nodes, edges = self.connector.get_nodes_and_edges()
+
+        nodes = adapt_to_client(nodes, self.source, self.client.id)
+        edges = adapt_to_client(edges, self.source, self.client.id)
+        self.validate_nodes_and_edges(nodes, edges)
+        return nodes, edges
```

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.9/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.1.0a1/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.9/PKG-INFO` & `grai_source_fivetran-0.1.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.0.9
+Version: 0.1.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fivetran (>=0.7.0,<0.8.0)
-Requires-Dist: grai-client (>=0.2.18,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran
 Description-Content-Type: text/markdown
```

