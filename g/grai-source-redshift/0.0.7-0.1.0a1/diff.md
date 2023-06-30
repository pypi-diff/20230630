# Comparing `tmp/grai_source_redshift-0.0.7.tar.gz` & `tmp/grai_source_redshift-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.7.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.1.0a1.tar", max compression
```

## Comparing `grai_source_redshift-0.0.7.tar` & `grai_source_redshift-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-19 11:07:12.940719 grai_source_redshift-0.0.7/README.md
--rw-r--r--   0        0        0     1066 2023-06-14 22:46:26.213086 grai_source_redshift-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-14 21:10:34.451009 grai_source_redshift-0.0.7/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     8770 2023-06-14 22:10:38.520511 grai_source_redshift-0.0.7/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1749 2023-06-14 21:02:53.255449 grai_source_redshift-0.0.7/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     8092 2023-06-14 21:02:53.295511 grai_source_redshift-0.0.7/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     5080 2023-06-01 16:01:43.268316 grai_source_redshift-0.0.7/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      199 2023-06-01 16:01:43.268442 grai_source_redshift-0.0.7/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-19 11:07:12.940719 grai_source_redshift-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1151 2023-06-30 03:28:57.030933 grai_source_redshift-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-29 15:34:52.431101 grai_source_redshift-0.1.0a1/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     9040 2023-06-29 15:34:52.431205 grai_source_redshift-0.1.0a1/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1078 2023-06-29 15:34:52.431310 grai_source_redshift-0.1.0a1/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     8092 2023-06-14 21:02:53.295511 grai_source_redshift-0.1.0a1/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     5080 2023-06-01 16:01:43.268316 grai_source_redshift-0.1.0a1/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.268442 grai_source_redshift-0.1.0a1/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 grai_source_redshift-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.7/pyproject.toml` & `grai_source_redshift-0.1.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.7"
+version = "0.1.0-alpha1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-grai-client = "^0.2.18"
+grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
-grai-schemas = "^0.1.15"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 botocore = "^1.29.153"
 redshift-connector = "^2.0.911"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
```

### Comparing `grai_source_redshift-0.0.7/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.1.0a1/src/grai_source_redshift/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-from typing import Any, Dict, List, Literal, Sequence
+from typing import Any, Dict, List, Literal, Sequence, TypeVar
 from warnings import warn
 
-from grai_client.schemas.schema import Schema
 from grai_schemas import config as base_config
 from grai_schemas.generics import DefaultValue
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
 
 from grai_source_redshift.models import (
     ID,
     UNIQUE_COLUMN_CONSTRAINTS,
     Column,
     ColumnConstraint,
     ColumnID,
-    Constraint,
     Edge,
     Table,
     TableID,
 )
 from grai_source_redshift.package_definitions import config
 
+T = TypeVar("T")
+X = TypeVar("X")
+Y = TypeVar("Y")
+
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
     """
 
     Args:
         current (Any):
@@ -257,15 +265,15 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_column_to_client(current: Column, version: Literal["v1"] = "v1"):
+def adapt_column_to_client(current: Column, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Column):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -273,22 +281,22 @@
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
-def adapt_table_to_client(current: Table, version: Literal["v1"] = "v1"):
+def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Table):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -296,18 +304,18 @@
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
 
 
 def make_name(node1: ID, node2: ID) -> str:
     """
 
     Args:
         node1 (ID):
@@ -320,51 +328,56 @@
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1"):
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
-def adapt_list_to_client(objs: Sequence, version: Literal["v1"]) -> List:
+def adapt_list_to_client(objs: Sequence, source: SourceSpec, version: Literal["v1"]) -> List:
     """
 
     Args:
         objs (Sequence):
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

### Comparing `grai_source_redshift-0.0.7/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.1.0a1/src/grai_source_redshift/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.7/src/grai_source_redshift/models.py` & `grai_source_redshift-0.1.0a1/src/grai_source_redshift/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.7/PKG-INFO` & `grai_source_redshift-0.1.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.0.7
+Version: 0.1.0a1
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
 Requires-Dist: botocore (>=1.29.153,<2.0.0)
-Requires-Dist: grai-client (>=0.2.18,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0a3,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: redshift-connector (>=2.0.911,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-redshift
 Description-Content-Type: text/markdown
```

