# Comparing `tmp/grai_source_bigquery-0.1.1.tar.gz` & `tmp/grai_source_bigquery-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.1.1.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.1.2a1.tar", max compression
```

## Comparing `grai_source_bigquery-0.1.1.tar` & `grai_source_bigquery-0.1.2a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-19 11:07:12.920740 grai_source_bigquery-0.1.1/README.md
--rw-r--r--   0        0        0     1037 2023-06-14 22:17:28.774356 grai_source_bigquery-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-14 22:11:02.218790 grai_source_bigquery-0.1.1/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8650 2023-06-14 22:10:38.534667 grai_source_bigquery-0.1.1/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     2078 2023-06-14 21:10:34.436953 grai_source_bigquery-0.1.1/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    13790 2023-06-14 21:10:34.437255 grai_source_bigquery-0.1.1/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6222 2023-06-14 21:10:34.437405 grai_source_bigquery-0.1.1/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-01 16:01:43.257500 grai_source_bigquery-0.1.1/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-19 11:07:12.920740 grai_source_bigquery-0.1.2a1/README.md
+-rw-r--r--   0        0        0     1122 2023-06-30 04:52:27.539367 grai_source_bigquery-0.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-30 04:52:27.545730 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8786 2023-06-27 23:26:32.053857 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1892 2023-06-29 15:34:52.418094 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    14133 2023-06-27 23:26:32.058194 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-14 21:10:34.437405 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.257500 grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.2a1/PKG-INFO
```

### Comparing `grai_source_bigquery-0.1.1/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-from typing import Any, Dict, List, Literal, Sequence, Union
+from typing import Any, Dict, List, Literal, Sequence, TypeVar, Union
 
 from grai_client.schemas.schema import Schema
 from grai_schemas import config as base_config
 from grai_schemas.generics import DefaultValue
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
 from pydantic import BaseModel
 
 from grai_source_bigquery.models import (
     ID,
     Column,
     ColumnID,
     Constraint,
     Edge,
     Table,
     TableID,
 )
 from grai_source_bigquery.package_definitions import config
 
+T = TypeVar("T")
+X = TypeVar("X")
+Y = TypeVar("Y")
+
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> BaseModel:
     """
 
     Args:
         current (Any):
@@ -237,15 +246,15 @@
     return {
         base_config.metadata_id: base_metadata,
         config.metadata_id: integration_meta,
     }
 
 
 @multimethod
-def adapt_to_client(current: Any, desired: Any) -> Union[NodeV1, EdgeV1]:
+def adapt_to_client(current: Any, desired: Any) -> Union[SourcedNodeV1, SourcedEdgeV1]:
     """
 
     Args:
         current (Any):
         desired (Any):
 
     Returns:
@@ -253,62 +262,64 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_column_to_client(current: Column, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_column_to_client(current: Column, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Column):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
+        "data_source": source,
         "display_name": current.name,
-        "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_table_to_client(current: Table, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Table):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:
 
     Returns:
 
     Raises:
 
     """
     metadata = {
         "node_type": NodeMetadataTypeLabels.table.value,
         "schema": current.table_schema,
     }
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
+        "data_source": source,
         "display_name": current.name,
-        "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
     metadata.update(current.metadata)
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: ID, node2: ID) -> str:
     """
 
     Args:
         node1 (ID):
@@ -321,50 +332,57 @@
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1") -> EdgeV1:
+def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
     """
 
     Args:
-        current (Edge):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
-        "data_source": config.integration_name,
         "name": make_name(current.source, current.destination),
+        "data_source": source,
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
-def adapt_list_to_client(objs: Sequence, version: Literal["v1"]) -> List:
+def adapt_list_to_client(objs: Sequence, source: SourceSpec, version: Literal["v1"]) -> List:
     """
 
     Args:
-        objs (Sequence):
-        version (Literal["v1"]):
+        objs:
+        version:
+        source:
 
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

### Comparing `grai_source_bigquery-0.1.1/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 from typing import List, Literal, Optional, Tuple, Union
 
 from grai_client.endpoints.client import BaseClient
+from grai_client.integrations.base import (
+    GraiIntegrationImplementationV1,
+    SeparateNodesAndEdgesMixin,
+)
 from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_schemas.base import Edge, Node, Source
 
 from grai_source_bigquery.adapters import adapt_to_client
 from grai_source_bigquery.loader import BigqueryConnector, LoggingConnector
 
 
-def get_nodes_and_edges(connector: BigqueryConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
-    """
-
-    Args:
-        connector (BigqueryConnector):
-        version (Literal["v1"]):
-
-    Returns:
-
-    Raises:
-
-    """
-    if version != "v1":
-        raise NotImplementedError(f"No available implementation for client version {version}")
-
-    with connector.connect() as conn:
-        nodes, edges = conn.get_nodes_and_edges()
-
-    nodes = adapt_to_client(nodes, version)
-    edges = adapt_to_client(edges, version)
-
-    return nodes, edges
-
-
-def update_server(
-    client: BaseClient,
-    namespace: Optional[str] = None,
-    project: Optional[str] = None,
-    dataset: Optional[Union[str, List[str]]] = None,
-    credentials: Optional[str] = None,
-    log_parsing: Optional[bool] = False,
-    log_parsing_window: Optional[int] = 7,
-) -> None:
-    """
-
-    Args:
-        client (BaseClient):
-        namespace (Optional[str], optional):  (Default value = None)
-        project (Optional[str], optional):  (Default value = None)
-        dataset (Optional[str], optional):  (Default value = None)
-        credentials (Optional[str], optional):  (Default value = None)
-
-    Returns:
-
-    Raises:
-
-    """
-    conn = (
-        BigqueryConnector(
-            project=project,
-            namespace=namespace,
-            dataset=dataset,
-            credentials=credentials,
-        )
-        if not log_parsing
-        else LoggingConnector(
-            project=project,
-            namespace=namespace,
-            dataset=dataset,
-            credentials=credentials,
-            window=log_parsing_window,
+class BigQueryIntegration(SeparateNodesAndEdgesMixin, GraiIntegrationImplementationV1):
+    def __init__(
+        self,
+        client: BaseClient,
+        source_name: str,
+        namespace: Optional[str] = None,
+        project: Optional[str] = None,
+        dataset: Optional[Union[str, List[str]]] = None,
+        credentials: Optional[str] = None,
+        log_parsing: Optional[bool] = False,
+        log_parsing_window: Optional[int] = 7,
+    ):
+        super().__init__(client, source_name)
+
+        self.connector = (
+            BigqueryConnector(
+                project=project,
+                namespace=namespace,
+                dataset=dataset,
+                credentials=credentials,
+            )
+            if not log_parsing
+            else LoggingConnector(
+                project=project,
+                namespace=namespace,
+                dataset=dataset,
+                credentials=credentials,
+                window=log_parsing_window,
+            )
         )
-    )
-
-    nodes, edges = get_nodes_and_edges(conn, client.id)
 
-    update(client, nodes)
-    update(client, edges)
+    def nodes(self):
+        with self.connector.connect() as conn:
+            connector_nodes = conn.nodes()
+            grai_nodes = adapt_to_client(connector_nodes, self.source, self.client.id)
+        return grai_nodes
+
+    def edges(self):
+        with self.connector.connect() as conn:
+            connector_edges = conn.edges()
+            grai_edges = adapt_to_client(connector_edges, self.source, self.client.id)
+        return grai_edges
```

### Comparing `grai_source_bigquery-0.1.1/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 from datetime import datetime, timedelta, timezone
-from functools import cached_property, lru_cache
+from functools import cache, cached_property, lru_cache
 from itertools import chain
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from google.cloud import bigquery, logging
 from google.oauth2 import service_account
 
 from grai_source_bigquery.models import (
@@ -58,14 +58,16 @@
         dataset: Optional[Union[str, List[str]]] = None,
         credentials: Optional[str] = None,
         **kwargs,
     ):
         self.namespace = get_from_env("namespace", "default") if namespace is None else namespace
         self.project = get_from_env("project", required=False) if project is None else project
         self.dataset = get_from_env("dataset", required=False) if dataset is None else dataset
+        self.datasets = [self.dataset] if isinstance(self.dataset, str) else self.dataset
+
         self.credentials = get_from_env("credentials", required=False) if credentials is None else credentials
         self._connection: Optional[bigquery.connector.BigqueryConnection] = None
 
         self._tables: Optional[List[Table]] = None
         self._foreign_keys: Optional[List[Edge]] = None
 
     def __enter__(self):
@@ -263,34 +265,40 @@
         Returns:
 
         Raises:
 
         """
         return [item for item in chain(*[t.get_edges() for t in self.tables(dataset)]) if item is not None]
 
+    @cache
+    def nodes(self) -> List[BigqueryNode]:
+        nodes = []
+        for dataset in self.datasets:
+            nodes.extend(self.get_nodes(dataset))
+        return nodes
+
+    @cache
+    def edges(self) -> List[Edge]:
+        edges = []
+        for dataset in self.datasets:
+            edges.extend(self.get_edges(dataset))
+        return edges
+
     def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
         """
 
         Args:
 
         Returns:
 
         Raises:
 
         """
-        datasets = [self.dataset] if isinstance(self.dataset, str) else self.dataset
-
-        nodes = []
-        edges = []
 
-        for dataset in datasets:
-            nodes.extend(self.get_nodes(dataset))
-            edges.extend(self.get_edges(dataset))
-
-        return nodes, edges
+        return self.nodes(), self.edges()
 
 
 class LoggingConnector(BigqueryConnector):
     """ """
 
     def __init__(
         self,
@@ -492,13 +500,18 @@
                         source=source,
                         destination=destination,
                     )
                 )
 
         return list(edges)
 
-    def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
-        nodes, edges = super().get_nodes_and_edges()
+    def nodes(self) -> List[BigqueryNode]:
+        return super().nodes()
 
-        bigquery_edges = self.get_bigquery_edges(nodes)
+    def edges(self) -> List[Edge]:
+        edges = super().edges()
+        bigquery_edges = self.get_bigquery_edges(self.nodes())
 
-        return nodes, edges + bigquery_edges
+        return edges + bigquery_edges
+
+    def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
+        return self.nodes(), self.edges()
```

### Comparing `grai_source_bigquery-0.1.1/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.1.2a1/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.1/PKG-INFO` & `grai_source_bigquery-0.1.2a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.1.1
+Version: 0.1.2a1
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
 Requires-Dist: google-cloud-bigquery (>=3.5.0,<4.0.0)
 Requires-Dist: google-cloud-logging (>=3.5.0,<4.0.0)
-Requires-Dist: grai-client (>=0.2.18,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: setuptools (>=67.1.0,<68.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-bigquery
 Description-Content-Type: text/markdown
```

