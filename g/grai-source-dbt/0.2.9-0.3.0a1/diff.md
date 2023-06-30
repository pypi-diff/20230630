# Comparing `tmp/grai_source_dbt-0.2.9.tar.gz` & `tmp/grai_source_dbt-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.2.9.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.3.0a1.tar", max compression
```

## Comparing `grai_source_dbt-0.2.9.tar` & `grai_source_dbt-0.3.0a1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0      124 2023-04-29 00:58:02.883723 grai_source_dbt-0.2.9/README.md
--rw-r--r--   0        0        0      924 2023-04-30 17:37:05.392599 grai_source_dbt-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.9/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     5993 2023-04-29 00:19:10.365667 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      531 2023-04-17 19:49:39.119946 grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.9/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.9/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.9/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.9/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     5493 2023-04-17 19:21:38.342251 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.9/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.9/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.9/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.9/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.9/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.9/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.9/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.9/setup.py
--rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a1/README.md
+-rw-r--r--   0        0        0     1077 2023-06-29 13:31:54.879881 grai_source_dbt-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-06-29 09:02:55.964007 grai_source_dbt-0.3.0a1/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a1/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     8357 2023-06-29 12:17:12.998756 grai_source_dbt-0.3.0a1/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a1/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      934 2023-06-29 12:55:58.962310 grai_source_dbt-0.3.0a1/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a1/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a1/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a1/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a1/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a1/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a1/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a1/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     2631 2023-06-29 13:30:53.867579 grai_source_dbt-0.3.0a1/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a1/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a1/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a1/PKG-INFO
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/adapters/v5.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ParsedSourceDefinition
 
 from grai_source_dbt.adapters.adapters import build_app_metadata
 
 
 @build_app_metadata.register
 def build_metadata_from_node(current: ParsedSourceDefinition, version: Literal["v1"] = "v1") -> Dict:
+    """
+
+    Args:
+        current (ParsedSourceDefinition):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
     data = {
         "description": current.description,
         "dbt_resource_type": current.resource_type,
         "table_name": current.name,
         "dbt_model_name": current.unique_id,
     }
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,19 +27,39 @@
 AllDbtNodeTypes = Union[NodeTypes, SourceTypes]
 AllDbtNodeInstances = get_args(AllDbtNodeTypes)
 set_extra_fields(AllDbtNodeInstances)
 
 
 @full_name.register
 def node_full_name(obj: NodeTypes) -> str:
+    """
+
+    Args:
+        obj (NodeTypes):
+
+    Returns:
+
+    Raises:
+
+    """
     return f"{obj.schema_}.{obj.name}"
 
 
 @full_name.register
 def source_full_name(obj: SourceTypes) -> str:
+    """
+
+    Args:
+        obj (SourceTypes):
+
+    Returns:
+
+    Raises:
+
+    """
     return f"{obj.schema_}.{obj.identifier}"
 
 
 MANIFEST_MAP = {
     ArtifactTypes.MANIFEST_V1.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V2.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V3.value.dbt_schema_version: ManifestLoaderV1,
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 from grai_source_dbt.utils import full_name
 
 if typing.TYPE_CHECKING:
     from grai_source_dbt.loaders import ManifestTypes
 
 
 class BaseManifestLoader(ABC):
+    """ """
+
     def __init__(self, manifest: ManifestTypes, namespace: str, *args, **kwargs):
         self.manifest = manifest
         self.namespace = namespace
 
         for node in self.manifest.nodes.values():
             node.grai_ = GraiExtras(full_name=full_name(node), namespace=self.namespace)
         for node in self.manifest.sources.values():
             node.grai_ = GraiExtras(full_name=full_name(node), namespace=self.namespace)
 
     @property
     @abstractmethod
     def nodes(self):
+        """ """
         raise NotImplementedError
 
     @property
     @abstractmethod
     def edges(self):
+        """ """
         raise NotImplementedError
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v7.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,31 @@
     ParsedSeedNode,
     ParsedSnapshotNode,
 ]
 SourceTypes = Union[ParsedSourceDefinition]
 
 
 class ManifestLoaderV7(ManifestLoaderV1):
+    """ """
+
     def make_edge(self, source, destination, constraint_type, edge_type, definition: bool = False) -> Edge:
+        """
+
+        Args:
+            source:
+            destination:
+            constraint_type:
+            edge_type:
+            definition (bool, optional):  (Default value = False)
+
+        Returns:
+
+        Raises:
+
+        """
         source_terminus = EdgeTerminus(name=full_name(source), namespace=self.namespace)
         destination_terminus = EdgeTerminus(name=full_name(destination), namespace=self.namespace)
         if definition:
             return Edge(
                 constraint_type=constraint_type,
                 source=source_terminus,
                 destination=destination_terminus,
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/models/grai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing
 from enum import Enum
 from typing import Dict, List, Literal, Optional, Union
 
-from grai_schemas.v1.metadata.edges import EdgeTypeLabels
+from grai_schemas.v1.metadata.edges import EdgeMetadataTypeLabels
 from pydantic import BaseModel, Field
 
 from grai_source_dbt.models.shared import (
     ID,
     Constraint,
     DBTNode,
     DBTNodeColumn,
@@ -16,14 +16,16 @@
 )
 
 if typing.TYPE_CHECKING:
     from grai_source_dbt.loaders import NodeTypes
 
 
 class Column(ID):
+    """ """
+
     name: str
     description: Optional[str]
     meta: Dict
     data_type: Optional[str]
     quote: Optional[str]
     tags: List
     table_unique_id: str
@@ -33,62 +35,88 @@
     resource_type: Literal["column"] = "column"
 
     #### Grai Specific ####
     tests: List = []
 
     @property
     def full_name(self):
+        """ """
         return f"{self.table_schema}.{self.table_name}.{self.name}"
 
     @classmethod
     def from_table_column(cls, table: NodeTypes, column, namespace) -> "Column":
+        """
+
+        Args:
+            table (NodeTypes):
+            column:
+            namespace:
+
+        Returns:
+
+        Raises:
+
+        """
         attrs = {
             "table_unique_id": table.unique_id,
             "table_name": table.name,
             "table_schema": table.schema_,
             "database": table.database,
             "namespace": namespace,
             "package_name": table.package_name,
         }
         attrs.update(column.dict())
         return cls(**attrs)
 
     @property
     def unique_id(self):
+        """ """
         return self.table_unique_id, self.name
 
     def __hash__(self):
         return hash((self.table_unique_id, self.name))
 
     class Config:
+        """ """
+
         validate_assignment = True
 
 
 class EdgeTerminus(BaseModel):
+    """ """
+
     name: str
     namespace: str
 
     @property
     def identifier(self):
+        """ """
         return f"{self.namespace}:{self.name}"
 
     class Config:
+        """ """
+
         validate_assignment = True
 
 
 class Edge(BaseModel):
+    """ """
+
     source: EdgeTerminus
     destination: EdgeTerminus
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
-    edge_type: EdgeTypeLabels
+    edge_type: EdgeMetadataTypeLabels
 
     def __hash__(self):
         return hash((self.source, self.destination))
 
     @property
     def name(self):
+        """ """
         return f"{self.source.identifier} -> {self.destination.identifier}"
 
     class Config:
+        """ """
+
         validate_assignment = True
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/models/shared.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,82 +4,104 @@
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, Field
 
 
 class ManifestMetadata(BaseModel):
+    """ """
+
     dbt_schema_version: str
     dbt_version: str
     generated_at: str
     invocation_id: str
     env: Dict
     project_id: UUID
     user_id: UUID
     send_anonymous_usage_stats: bool
     adapter_type: str
 
 
 class ID(BaseModel):
+    """ """
+
     name: str
     namespace: Optional[str]
     package_name: str
 
 
 class Constraint(str, Enum):
+    """ """
+
     belongs_to = "bt"
     dbt_model = "dbtm"
 
 
 class DbtResourceType(str, Enum):
+    """ """
+
     model = "model"
     seed = "seed"
     source = "source"
     analysis = "analysis"
     test = "test"
     operation = "operation"
 
 
 class DbtMaterializationType(str, Enum):
+    """ """
+
     table = "table"
     view = "view"
     incremental = "incremental"
     ephemeral = "ephemeral"
     seed = "seed"
     snapshot = "snapshot"
 
 
 class NodeDeps(BaseModel):
+    """ """
+
     nodes: List[str]
     macros: List[str]  # TODO: macros not currently tested
 
 
 class NodeConfig(BaseModel):
+    """ """
+
     materialized: Optional[DbtMaterializationType]
 
 
 class DBTNodeColumn(BaseModel):
+    """ """
+
     name: str
     description: Optional[str]
     meta: Dict
     data_type: Optional[str]
     quote: Optional[str]
     tags: List
 
 
 class NodeChecksum(BaseModel):
+    """ """
+
     name: str
     checksum: str
 
 
 class NodeDocs(BaseModel):
+    """ """
+
     show: bool
 
 
 class DBTNode(ID):
+    """ """
+
     unique_id: str
     root_path: str
     path: Optional[str]
     original_file_path: Optional[str]
     node_schema: str = Field(alias="schema")
     description: str
     depends_on: NodeDeps
@@ -99,15 +121,25 @@
     compiled_path: Any
     deferred: Optional[bool]
     unrendered_config: Dict[Any, Any]
     created_at: float
 
     @property
     def tag_list(self) -> List[str]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return [self.tags] if isinstance(self.tags, str) else self.tags
 
     def __hash__(self):
         return hash(self.unique_id)
 
     @property
     def full_name(self):
+        """ """
         return f"{self.node_schema}.{self.name}"
```

### Comparing `grai_source_dbt-0.2.9/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.3.0a1/src/grai_source_dbt/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,59 @@
 
 from multimethod import multimethod
 from pydantic import BaseModel, Extra
 
 
 @multimethod
 def full_name(obj: Any) -> str:
+    """
+
+    Args:
+        obj (Any):
+
+    Returns:
+
+    Raises:
+
+    """
     # This is a fallback method that will be called if no other method is found
     try:
         return obj.full_name
     except AttributeError as e:
         message = (
             f"The `full_name` function requires objects to either have a `full_name` attribute or a custom "
             f"implementation for their type. No implementation was found for objects of type {type(obj)}"
         )
         raise NotImplementedError(message) from e
 
 
 def set_loader_config_fields(obj: BaseModel):
+    """
+
+    Args:
+        obj (BaseModel):
+
+    Returns:
+
+    Raises:
+
+    """
     obj.Config.extra = Extra.allow
     obj.Config.use_enum_values = True
 
 
 def set_extra_fields(obj: Union[BaseModel, Sequence[BaseModel]]) -> None:
+    """
+
+    Args:
+        obj (Union[BaseModel, Sequence[BaseModel]]):
+
+    Returns:
+
+    Raises:
+
+    """
     if isinstance(obj, BaseModel):
         set_loader_config_fields(obj)
     elif isinstance(obj, Sequence):
         for item in obj:
             set_loader_config_fields(item)
```

### Comparing `grai_source_dbt-0.2.9/PKG-INFO` & `grai_source_dbt-0.3.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.2.9
+Version: 0.3.0a1
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
 Requires-Dist: dbt-artifacts-parser (>=0.2.4,<0.3.0)
-Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.10,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt
 Description-Content-Type: text/markdown
 
 # Grai dbt Integration
```

