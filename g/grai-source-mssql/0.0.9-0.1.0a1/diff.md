# Comparing `tmp/grai_source_mssql-0.0.9.tar.gz` & `tmp/grai_source_mssql-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mssql-0.0.9.tar", max compression
+gzip compressed data, was "grai_source_mssql-0.1.0a1.tar", max compression
```

## Comparing `grai_source_mssql-0.0.9.tar` & `grai_source_mssql-0.1.0a1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      145 2023-04-29 00:58:02.883807 grai_source_mssql-0.0.9/README.md
--rw-r--r--   0        0        0      876 2023-04-30 17:37:24.495159 grai_source_mssql-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.9/src/grai_source_mssql/__init__.py
--rw-r--r--   0        0        0     6461 2023-04-29 00:19:10.367254 grai_source_mssql-0.0.9/src/grai_source_mssql/adapters.py
--rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.9/src/grai_source_mssql/base.py
--rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.9/src/grai_source_mssql/loader.py
--rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.9/src/grai_source_mssql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.9/src/grai_source_mssql/package_definitions.py
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.9/setup.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1727 2023-05-19 11:07:12.934170 grai_source_mssql-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1031 2023-06-30 03:29:39.493787 grai_source_mssql-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-30 03:29:39.499035 grai_source_mssql-0.1.0a1/src/grai_source_mssql/__init__.py
+-rw-r--r--   0        0        0     8770 2023-06-29 15:34:52.427765 grai_source_mssql-0.1.0a1/src/grai_source_mssql/adapters.py
+-rw-r--r--   0        0        0     1484 2023-06-29 15:34:52.427938 grai_source_mssql-0.1.0a1/src/grai_source_mssql/base.py
+-rw-r--r--   0        0        0    12098 2023-06-29 15:34:52.428298 grai_source_mssql-0.1.0a1/src/grai_source_mssql/loader.py
+-rw-r--r--   0        0        0     5032 2023-06-01 16:01:43.264695 grai_source_mssql-0.1.0a1/src/grai_source_mssql/models.py
+-rw-r--r--   0        0        0      193 2023-06-01 16:01:43.264786 grai_source_mssql-0.1.0a1/src/grai_source_mssql/package_definitions.py
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 grai_source_mssql-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_mssql-0.0.9/src/grai_source_mssql/base.py` & `grai_source_mssql-0.1.0a1/src/grai_source_mssql/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-from typing import List, Literal, Optional, Tuple
+from typing import List, Optional, Tuple
 
 from grai_client.endpoints.client import BaseClient
-from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_client.integrations.base import (
+    ConnectorMixin,
+    GraiIntegrationImplementationV1,
+)
 
 from grai_source_mssql.adapters import adapt_to_client
 from grai_source_mssql.loader import MsSQLConnector
 
 
-def get_nodes_and_edges(connector: MsSQLConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
-    with connector.connect() as conn:
-        nodes, edges = conn.get_nodes_and_edges()
-
-    nodes = adapt_to_client(nodes, version)
-    edges = adapt_to_client(edges, version)
-    return nodes, edges
-
-
-def update_server(
-    client: BaseClient,
-    database: Optional[str] = None,
-    namespace: Optional[str] = None,
-    user: Optional[str] = None,
-    password: Optional[str] = None,
-    protocol: Optional[str] = None,
-    host: Optional[str] = None,
-    port: Optional[str] = None,
-    additional_connection_strings: Optional[List[str]] = None,
-):
-    conn = MsSQLConnector(
-        database=database,
-        user=user,
-        password=password,
-        protocol=protocol,
-        host=host,
-        port=port,
-        additional_connection_strings=additional_connection_strings,
-    )
-    nodes, edges = get_nodes_and_edges(conn, client.id)
-    update(client, nodes)
-    update(client, edges)
+class MsSQLIntegration(ConnectorMixin, GraiIntegrationImplementationV1):
+    def __init__(
+        self,
+        client: BaseClient,
+        source_name: str,
+        driver: Optional[str] = None,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        database: Optional[str] = None,
+        server: Optional[str] = None,
+        protocol: Optional[str] = None,
+        host: Optional[str] = None,
+        port: Optional[str] = None,
+        encrypt: Optional[bool] = None,
+        namespace: Optional[str] = None,
+        additional_connection_strings: Optional[List[str]] = None,
+    ):
+        super().__init__(client, source_name)
+
+        self.connector = MsSQLConnector(
+            driver=driver,
+            user=user,
+            password=password,
+            database=database,
+            server=server,
+            protocol=protocol,
+            host=host,
+            port=port,
+            encrypt=encrypt,
+            namespace=namespace,
+            additional_connection_strings=additional_connection_strings,
+        )
+
+    def adapt_to_client(self, objects):
+        return adapt_to_client(objects, self.source, self.client.id)
```

### Comparing `grai_source_mssql-0.0.9/src/grai_source_mssql/loader.py` & `grai_source_mssql-0.1.0a1/src/grai_source_mssql/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-import os
 import warnings
 from enum import Enum
 from functools import cached_property
 from itertools import chain
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple
 
 import pydantic
 import pyodbc
 from pydantic import SecretStr, root_validator, validator
 
-from grai_source_mssql.models import Column, ColumnID, Edge, EdgeQuery, MsSqlNode, Table
+from grai_source_mssql.models import Column, Edge, EdgeQuery, MsSqlNode, Table
 
 ENV_PREFIX = "GRAI_MSSQL_"
 
 
 class BaseSettings(pydantic.BaseSettings):
+    """ """
+
     class Config:
+        """ """
+
         env_prefix = ENV_PREFIX
 
 
 class Protocol(Enum):
+    """ """
+
     TCP = "tcp"
     ICP = "Icp"
     NP = "NP"
 
 
 class MsSqlSettings(BaseSettings):
+    """ """
+
     driver: Optional[str] = None
     database: Optional[str] = None
     server: Optional[str] = None
     protocol: Optional[Protocol] = None
     host: Optional[str] = None
     port: Optional[str] = None
     trusted_connection: Optional[bool] = None
@@ -37,20 +44,31 @@
     user: Optional[str]
     password: Optional[SecretStr]
     encrypt: Optional[bool]
     additional_connection_strings: Optional[List[str]] = None
 
     @validator("protocol")
     def validate_protocol(cls, value):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         if value is None:
             return Protocol.TCP
 
         return Protocol(value)
 
     def connection_string(self):
+        """ """
         connection_attributes = [f"DRIVER={self.driver}"]
         if self.trusted_connection:
             connection_attributes.append("Trusted_Connection=yes")
         else:
             connection_attributes.extend([f"UID={self.user}", f"Pwd={self.password.get_secret_value()}"])
         if self.encrypt is not None:
             connection_attributes.append(f"Encrypt={'yes' if self.encrypt else 'no'}")
@@ -72,44 +90,69 @@
         if self.additional_connection_strings is not None:
             connection_attributes.extend(self.additional_connection_strings)
 
         return "; ".join(connection_attributes)
 
     @validator("driver")
     def validate_driver(cls, value):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         available_drivers = pyodbc.drivers()
         if value is None:
             message = f"Running the MS Server connector requires either a `driver` parameter or {ENV_PREFIX}DRIVER environment variable. Normally we would attempt to detect an available driver installed on your system, however, in this case none were found. "
             assert len(available_drivers) >= 1, message
             return available_drivers[0]
         elif value not in available_drivers:
             warnings.warn(
                 f"Specified driver {value} not found in the list of available pyodbc drivers {available_drivers}"
             )
         return value
 
     @root_validator(pre=True)
     def parse_empty_values(cls, values):
-        """Empty strings should be treated as missing"""
+        """Empty strings should be treated as missing
+
+        Args:
+            values:
+
+        Returns:
+
+        Raises:
+
+        """
         new_values = values.copy()
         for k, v in values.items():
             if v == "":
                 new_values.pop(k)
         return new_values
 
 
 class MsSqlGraiSettings(BaseSettings):
+    """ """
+
     namespace: str = "default"
 
 
 class ConnectorSettings(MsSqlSettings, MsSqlGraiSettings):
+    """ """
+
     pass
 
 
 class MsSQLConnector:
+    """ """
+
     def __init__(
         self,
         driver: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         database: Optional[str] = None,
         server: Optional[str] = None,
@@ -130,69 +173,111 @@
             "host": host,
             "port": port,
             "encrypt": encrypt,
             "namespace": namespace,
             "additional_connection_strings": additional_connection_strings,
         }
         user_provided_connection_params = {k: v for k, v in connection_values.items() if v is not None}
-        self.config = ConnectorSettings(**user_provided_connection_params)
-        self._connection = None
+        self.config: ConnectorSettings = ConnectorSettings(**user_provided_connection_params)
+        self._connection: Optional[pyodbc.connect] = None
 
     def __enter__(self):
         return self.connect()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
-    def connect(self):
+    def connect(self) -> pyodbc.connect:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         if self._connection is None:
             self._connection = pyodbc.connect(self.config.connection_string())
         return self
 
     @property
     def connection(self):
+        """ """
         if self._connection is None:
             raise Exception("Not connected, call `.connect()")
         return self._connection
 
     def close(self) -> None:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         self.connection.close()
         self._connection = None
 
     def query_runner(self, query: str, params: List = []) -> List[Dict]:
+        """
+
+        Args:
+            query (str):
+            params (List, optional):  (Default value = [])
+
+        Returns:
+
+        Raises:
+
+        """
         cursor = self.connection.cursor()
         # queries must be parameterized with ?
         # https://github.com/mkleehammer/pyodbc/wiki/Getting-started#parameters
         cursor.execute(query, *params)
         columns = [col[0] for col in cursor.description]
         return [dict(zip(columns, row)) for row in cursor.fetchall()]
 
     @cached_property
     def tables(self) -> List[Table]:
-        """
-        Create and return a list of dictionaries with the
+        """Create and return a list of dictionaries with the
         schemas and names of tables in the database
         connected to by the connection argument.
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
 
         query = """
 	        SELECT TABLE_SCHEMA, TABLE_NAME, TABLE_TYPE
             FROM INFORMATION_SCHEMA.TABLES
         """
-        tables = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
-        tables = [Table(**result, namespace=self.config.namespace) for result in tables]
+        table_gen = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
+        tables = [Table(**result, namespace=self.config.namespace) for result in table_gen]
         for table in tables:
             table.columns = self.get_table_columns(table)
         return tables
 
     @cached_property
     def columns(self) -> List[Column]:
-        """
-        Creates and returns a list of dictionaries for the specified
+        """Creates and returns a list of dictionaries for the specified
         schema.table in the database connected to.
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
         query = f"""
             SELECT c.COLUMN_NAME,
                    c.DATA_TYPE,
                    c.IS_NULLABLE,
                    c.COLUMN_DEFAULT,
                    c.TABLE_NAME,
@@ -215,35 +300,58 @@
                 }
             )
 
         result = [Column(**result, namespace=self.config.namespace) for result in res]
         return result
 
     @cached_property
-    def column_map(self):
-        result_map = {}
+    def column_map(self) -> Dict[Tuple[str, str], List[Column]]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        result_map: Dict[Tuple[str, str], List[Column]] = {}
         for col in self.columns:
             table_id = (col.column_schema, col.table)
             result_map.setdefault(table_id, [])
             result_map[table_id].append(col)
         return result_map
 
-    def get_table_columns(self, table: Table):
+    def get_table_columns(self, table: Table) -> List[Column]:
+        """
+
+        Args:
+            table (Table):
+
+        Returns:
+
+        Raises:
+
+        """
         table_id = (table.table_schema, table.name)
         if table_id in self.column_map:
             return self.column_map[table_id]
         else:
             raise Exception(f"No columns found for table with schema={table.table_schema} and name={table.name}")
 
     @cached_property
     def foreign_keys(self) -> List[Edge]:
         """This needs to be tested / evaluated
-        :param connection:
-        :param table:
-        :return:
+
+        Args:
+
+        Returns:
+
+        Raises:
+
         """
 
         query = """
             SELECT sch.name AS [self_schema],
                 tab1.name AS [self_table],
                 col1.name AS [self_columns],
                 tab2.name AS [foreign_table],
@@ -273,20 +381,48 @@
                     "foreign_schema": item["self_schema"],  # TODO: This is not necessarily true
                     "namespace": self.config.namespace,
                     "constraint_name": "",
                     "self_columns": list(item["self_columns"].split(",")),
                     "foreign_columns": list(item["foreign_columns"].split(",")),
                 }
             )
-        return [EdgeQuery(**fk).to_edge() for fk in res]
+        result = [EdgeQuery(**fk).to_edge() for fk in res]
+        return [r for r in result if r is not None]
 
     def get_nodes(self) -> List[MsSqlNode]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return list(chain(self.tables, self.columns))
 
-    def get_edges(self):
-        return list(chain(*[t.get_edges() for t in self.tables], self.foreign_keys))
+    def get_edges(self) -> List[Edge]:
+        """
+
+        Args:
 
-    def get_nodes_and_edges(self):
+        Returns:
+
+        Raises:
+
+        """
+        return [edge for edge in chain(*[t.get_edges() for t in self.tables], self.foreign_keys) if edge is not None]
+
+    def get_nodes_and_edges(self) -> Tuple[List[MsSqlNode], List[Edge]]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         nodes = self.get_nodes()
         edges = self.get_edges()
 
         return nodes, edges
```

### Comparing `grai_source_mssql-0.0.9/src/grai_source_mssql/models.py` & `grai_source_mssql-0.1.0a1/src/grai_source_mssql/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,181 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class MsSqlNode(BaseModel):
+    """ """
+
     pass
 
 
 class ID(MsSqlNode):
+    """ """
+
     name: str
     namespace: str
     full_name: str
 
     class Config:
+        """ """
+
         extra = "forbid"
 
 
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
             values["full_name"] = f"{values['table_schema']}.{values['table_name']}.{values['name']}"
         return values
 
 
 class ColumnConstraint(Enum):
+    """ """
+
     primary_key = "PRIMARY KEY"
     unique = "UNIQUE"
     foreign_key = "FOREIGN KEY"
     check = "CHECK"
 
 
 UNIQUE_COLUMN_CONSTRAINTS = {ColumnConstraint.primary_key.value, ColumnConstraint.unique.value}
 
 
 class Column(MsSqlNode):
+    """ """
+
     name: str = Field(alias="column_name")
     table: str = Field(alias="table_name")
     column_schema: str = Field(alias="table_schema")
     data_type: str
     is_nullable: bool
     namespace: str
     default_value: Any = Field(alias="column_default")
     column_constraint: Optional[ColumnConstraint]
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
+    """ """
+
     source: Union[ColumnID, TableID]
     destination: Union[ColumnID, TableID]
     definition: Optional[str]
     constraint_type: Constraint
     metadata: Optional[Dict] = None
 
 
 class Table(MsSqlNode):
+    """ """
+
     name: str = Field(alias="table_name")
     table_schema: str = Field(alias="schema")
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
@@ -121,27 +188,40 @@
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

