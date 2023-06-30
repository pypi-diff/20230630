# Comparing `tmp/grai_source_postgres-0.1.9.tar.gz` & `tmp/grai_source_postgres-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_postgres-0.1.9.tar", max compression
+gzip compressed data, was "grai_source_postgres-0.2.0a1.tar", max compression
```

## Comparing `grai_source_postgres-0.1.9.tar` & `grai_source_postgres-0.2.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      706 2023-01-27 12:50:31.332417 grai_source_postgres-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      145 2023-01-23 19:51:17.814721 grai_source_postgres-0.1.9/src/grai_source_postgres/__init__.py
--rw-r--r--   0        0        0     5861 2023-01-27 11:11:33.559126 grai_source_postgres-0.1.9/src/grai_source_postgres/adapters.py
--rw-r--r--   0        0        0     1171 2023-01-27 12:45:33.465685 grai_source_postgres-0.1.9/src/grai_source_postgres/base.py
--rw-r--r--   0        0        0     7185 2023-01-11 10:42:34.274803 grai_source_postgres-0.1.9/src/grai_source_postgres/loader.py
--rw-r--r--   0        0        0     4144 2022-12-07 15:33:50.248250 grai_source_postgres-0.1.9/src/grai_source_postgres/models.py
--rw-r--r--   0        0        0      148 2023-01-23 19:51:17.815063 grai_source_postgres-0.1.9/src/grai_source_postgres/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.9/setup.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_postgres-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-05-19 11:07:12.938428 grai_source_postgres-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1118 2023-06-30 03:31:34.039845 grai_source_postgres-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-06-30 03:31:34.045950 grai_source_postgres-0.2.0a1/src/grai_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8780 2023-06-29 15:34:52.430294 grai_source_postgres-0.2.0a1/src/grai_source_postgres/adapters.py
+-rw-r--r--   0        0        0     1142 2023-06-29 15:34:52.430389 grai_source_postgres-0.2.0a1/src/grai_source_postgres/base.py
+-rw-r--r--   0        0        0    10194 2023-06-14 21:02:53.412976 grai_source_postgres-0.2.0a1/src/grai_source_postgres/loader.py
+-rw-r--r--   0        0        0     5200 2023-06-01 16:01:43.266903 grai_source_postgres-0.2.0a1/src/grai_source_postgres/models.py
+-rw-r--r--   0        0        0      199 2023-06-01 16:01:43.266998 grai_source_postgres-0.2.0a1/src/grai_source_postgres/package_definitions.py
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 grai_source_postgres-0.2.0a1/PKG-INFO
```

### Comparing `grai_source_postgres-0.1.9/src/grai_source_postgres/models.py` & `grai_source_postgres-0.2.0a1/src/grai_source_postgres/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,111 +1,194 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class PostgresNode(BaseModel):
+    """ """
+
     pass
 
 
 class ID(PostgresNode):
+    """ """
+
     name: str
     namespace: str
     full_name: str
 
+    class Config:
+        """ """
+
+        extra = "forbid"
+
 
 class TableID(ID):
+    """ """
+
     table_schema: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values):
+        """
+
+        Args:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         full_name = values.get("full_name", None)
         if values.get("full_name", None) is None:
             values["full_name"] = f"{values['table_schema']}.{values['name']}"
         return values
 
 
 class ColumnID(ID):
+    """ """
+
     table_schema: str
     table_name: str
 
     @root_validator(pre=True)
     def make_full_name(cls, values):
+        """
+
+        Args:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         full_name = values.get("full_name", None)
         if values.get("full_name", None) is None:
-            values[
-                "full_name"
-            ] = f"{values['table_schema']}.{values['table_name']}.{values['name']}"
+            values["full_name"] = f"{values['table_schema']}.{values['table_name']}.{values['name']}"
         return values
 
 
+class ColumnConstraint(Enum):
+    """ """
+
+    primary_key = "p"
+    unique = "u"
+    foreign_key = "f"
+    check = "c"
+    trigger = "t"
+    exclusion = "x"
+
+
+UNIQUE_COLUMN_CONSTRAINTS = {ColumnConstraint.primary_key.value, ColumnConstraint.unique.value}
+
+
 class Column(PostgresNode):
+    """ """
+
     name: str = Field(alias="column_name")
     table: str
     column_schema: str = Field(alias="schema")
     data_type: str
     is_nullable: bool
     namespace: str
     default_value: Any = Field(alias="column_default")
+    column_constraint: Optional[ColumnConstraint]
     is_pk: Optional[bool] = False
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name, values):
+        """
+
+        Args:
+            full_name:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
         result = f"{values['column_schema']}.{values['table']}.{values['name']}"
         return result
 
 
 class Constraint(str, Enum):
+    """ """
+
     foreign_key = "f"
     primary_key = "p"
     belongs_to = "bt"
 
 
 class Edge(BaseModel):
-    source: Union[TableID, ColumnID]
-    destination: Union[TableID, ColumnID]
+    """ """
+
+    source: Union[ColumnID, TableID]
+    destination: Union[ColumnID, TableID]
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
 
 
 class TableType(str, Enum):
+    """ """
+
     Table = "BASE TABLE"
     View = "VIEW"
     ForeignTable = "FOREIGN"
     TemporaryTable = "LOCAL TEMPORARY"
 
 
 class Table(PostgresNode):
+    """ """
+
     name: str = Field(alias="table_name")
     table_schema: str = Field(alias="schema")
     table_type: TableType
     namespace: str
     columns: Optional[List[Column]] = []
     metadata: Dict = {}
     full_name: Optional[str] = None
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name, values):
+        """
+
+        Args:
+            full_name:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         if full_name is not None:
             return full_name
 
         return f"{values['table_schema']}.{values['name']}"
 
     def get_edges(self):
+        """ """
         return [
             Edge(
                 constraint_type=Constraint("bt"),
                 source=TableID(
                     table_schema=self.table_schema,
                     name=self.name,
                     namespace=self.namespace,
@@ -118,27 +201,40 @@
                 ),
             )
             for column in self.columns
         ]
 
 
 class EdgeQuery(BaseModel):
+    """ """
+
     namespace: str
     constraint_name: str
     constraint_type: str
     self_schema: str
     self_table: str
     self_columns: List[str]
     foreign_schema: str
     foreign_table: str
     foreign_columns: List[str]
     definition: str
 
-    def to_edge(self) -> Edge:
-        assert len(self.self_columns) == 1 and len(self.foreign_columns) == 1
+    def to_edge(self) -> Optional[Edge]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        if not len(self.self_columns) == 1 and len(self.foreign_columns) == 1:
+            return None
+
         destination = ColumnID(
             table_schema=self.self_schema,
             table_name=self.self_table,
             name=self.self_columns[0],
             namespace=self.namespace,
         )
         source = ColumnID(
```

