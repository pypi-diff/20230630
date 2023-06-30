# Comparing `tmp/grai_source_mysql-0.0.9.tar.gz` & `tmp/grai_source_mysql-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mysql-0.0.9.tar", max compression
+gzip compressed data, was "grai_source_mysql-0.1.0a1.tar", max compression
```

## Comparing `grai_source_mysql-0.0.9.tar` & `grai_source_mysql-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      720 2023-03-22 04:18:10.608905 grai_source_mysql-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.725826 grai_source_mysql-0.0.9/src/grai_source_mysql/__init__.py
--rw-r--r--   0        0        0     6109 2023-03-22 03:28:01.338626 grai_source_mysql-0.0.9/src/grai_source_mysql/adapters.py
--rw-r--r--   0        0        0     1054 2023-02-13 20:16:22.726027 grai_source_mysql-0.0.9/src/grai_source_mysql/base.py
--rw-r--r--   0        0        0     7687 2023-03-22 04:13:27.979101 grai_source_mysql-0.0.9/src/grai_source_mysql/loader.py
--rw-r--r--   0        0        0     4089 2023-03-22 03:28:01.339116 grai_source_mysql-0.0.9/src/grai_source_mysql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.726524 grai_source_mysql-0.0.9/src/grai_source_mysql/package_definitions.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.9/setup.py
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 grai_source_mysql-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-05-19 11:07:12.935785 grai_source_mysql-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1063 2023-06-30 03:29:49.116058 grai_source_mysql-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-30 03:29:49.120350 grai_source_mysql-0.1.0a1/src/grai_source_mysql/__init__.py
+-rw-r--r--   0        0        0     8646 2023-06-29 15:34:52.429355 grai_source_mysql-0.1.0a1/src/grai_source_mysql/adapters.py
+-rw-r--r--   0        0        0     1075 2023-06-29 15:34:52.429468 grai_source_mysql-0.1.0a1/src/grai_source_mysql/base.py
+-rw-r--r--   0        0        0     8955 2023-06-14 21:02:53.243358 grai_source_mysql-0.1.0a1/src/grai_source_mysql/loader.py
+-rw-r--r--   0        0        0     4779 2023-06-01 16:01:43.265941 grai_source_mysql-0.1.0a1/src/grai_source_mysql/models.py
+-rw-r--r--   0        0        0      193 2023-06-01 16:01:43.266029 grai_source_mysql-0.1.0a1/src/grai_source_mysql/package_definitions.py
+-rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 grai_source_mysql-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_mysql-0.0.9/pyproject.toml` & `grai_source_mysql-0.1.0a1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "grai_source_mysql"
-version = "0.0.9"
+version = "0.1.0-alpha1"
 description = ""
-authors = ["Tony Lewis <tony@grai.io>"]
+authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mysql", from = "src" },
 ]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-mysql"
+documentation = "https://docs.grai.io/"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
-grai-client = "^0.2.6"
+grai-client = {version = "^0.3.0a3", allow-prereleases = true}
+grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 PyYAML = "^6.0"
 multimethod = "^1.8"
 mysql-connector-python = "^8.0.31"
-grai-schemas = "^0.1.10"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 pytest = "^7.2.0"
@@ -29,7 +34,9 @@
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_source_mysql/__init__.py"]
```

### Comparing `grai_source_mysql-0.0.9/src/grai_source_mysql/base.py` & `grai_source_mysql-0.1.0a1/src/grai_source_mysql/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from typing import List, Literal, Optional, Tuple
+from typing import Optional, Union
 
 from grai_client.endpoints.client import BaseClient
-from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_client.integrations.base import (
+    ConnectorMixin,
+    GraiIntegrationImplementationV1,
+)
 
 from grai_source_mysql.adapters import adapt_to_client
 from grai_source_mysql.loader import MySQLConnector
 
 
-def get_nodes_and_edges(connector: MySQLConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
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
-    dbname: Optional[str] = None,
-    namespace: Optional[str] = None,
-    user: Optional[str] = None,
-    password: Optional[str] = None,
-    host: Optional[str] = None,
-    port: Optional[str] = None,
-):
-    conn = MySQLConnector(dbname=dbname, user=user, password=password, host=host, port=port)
-    nodes, edges = get_nodes_and_edges(conn, client.id)
-    update(client, nodes)
-    update(client, edges)
+class MySQLIntegration(ConnectorMixin, GraiIntegrationImplementationV1):
+    def __init__(
+        self,
+        client: BaseClient,
+        source_name: str,
+        dbname: Optional[str] = None,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        host: Optional[str] = None,
+        port: Optional[Union[str, int]] = None,
+        namespace: Optional[str] = None,
+    ):
+        super().__init__(client, source_name)
+
+        self.connection = MySQLConnector(
+            dbname=dbname,
+            user=user,
+            password=password,
+            host=host,
+            port=port,
+            namespace=namespace,
+        )
+
+    def adapt_to_client(self, objects):
+        return adapt_to_client(objects, self.source, self.client.id)
```

### Comparing `grai_source_mysql-0.0.9/src/grai_source_mysql/loader.py` & `grai_source_mysql-0.1.0a1/src/grai_source_mysql/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,40 @@
 
 import mysql.connector
 
 from grai_source_mysql.models import Column, ColumnID, Edge, EdgeQuery, MysqlNode, Table
 
 
 def get_from_env(label: str, default: Optional[Any] = None, validator: Callable = None):
+    """
+
+    Args:
+        label (str):
+        default (Optional[Any], optional):  (Default value = None)
+        validator (Callable, optional):  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     env_key = f"GRAI_MYSQL_{label.upper()}"
     result = os.getenv(env_key, default)
     if result is None:
         message = (
             f"Establishing mysql connection requires a {label}. "
             f"Either pass a value explicitly or set a {env_key} environment value."
         )
         raise Exception(message)
     return result if validator is None else validator(result)
 
 
 class MySQLConnector:
+    """ """
+
     def __init__(
         self,
         dbname: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         host: Optional[str] = None,
         port: Optional[Union[str, int]] = None,
@@ -42,49 +56,86 @@
         return self.connect()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     @property
     def connection_dict(self) -> dict:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return {
             "host": self.host,
             "database": self.dbname,
             "user": self.user,
             "password": self.password,
             "port": self.port,
         }
 
     def connect(self):
+        """ """
         if self._connection is None:
             self._connection = mysql.connector.connect(**self.connection_dict)
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
 
     def query_runner(self, query: str, param_dict: Dict = {}) -> List[Dict]:
+        """
+
+        Args:
+            query (str):
+            param_dict (Dict, optional):  (Default value = {})
+
+        Returns:
+
+        Raises:
+
+        """
         dict_cursor = self.connection.cursor(dictionary=True)
         dict_cursor.execute(query, param_dict)
         result = dict_cursor.fetchall()
         return [dict(item) for item in result]
 
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
 	    SELECT table_schema, table_name
             FROM information_schema.tables
             WHERE table_schema != 'information_schema'
 		    AND table_schema != 'performance_schema'
@@ -94,17 +145,23 @@
         tables = [Table(**result, namespace=self.namespace) for result in res]
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
             SELECT column_name,
                    table_name as "table",
                    table_schema as "schema",
                    data_type,
@@ -116,36 +173,59 @@
 		    AND table_schema != 'performance_schema'
             ORDER BY ordinal_position
         """
         res = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
 
         return [Column(**result, namespace=self.namespace) for result in res]
 
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
         # Only need constraint_types == 'f' for foreign keys but the others might be useful someday.
         # Removed schemas, no schemas in mysql
         query = """
         select
             tc.CONSTRAINT_NAME as constraint_name,
             case when tc.CONSTRAINT_TYPE='PRIMARY KEY' then 'p'
@@ -179,24 +259,51 @@
 
         res = self.query_runner(query)
 
         for item in res:
             item["self_columns"] = list(item["self_columns"].split(",")) if item["self_columns"] else []
             item["foreign_columns"] = list(item["foreign_columns"].split(",")) if item["foreign_columns"] else []
 
-        res = ({k.lower(): v for k, v in result.items()} for result in res)
+        res_gen = ({k.lower(): v for k, v in result.items()} for result in res)
+        filtered_results = (result for result in res_gen if result["constraint_type"] == "f")
+        edge_query_gen = (EdgeQuery(**fk, **addtl_args).to_edge() for fk in filtered_results)
+        edges = [edge for edge in edge_query_gen if edge is not None]
+        return edges
 
-        filtered_results = (result for result in res if result["constraint_type"] == "f")
+    def get_nodes(self) -> List[MysqlNode]:
+        """
 
-        return [EdgeQuery(**fk, **addtl_args).to_edge() for fk in filtered_results]
+        Args:
 
-    def get_nodes(self) -> List[MysqlNode]:
+        Returns:
+
+        Raises:
+
+        """
         return list(chain(self.tables, self.columns))
 
     def get_edges(self) -> List[Edge]:
-        return list(chain(*[t.get_edges() for t in self.tables], self.foreign_keys))
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        return [edge for edge in chain(*[t.get_edges() for t in self.tables], self.foreign_keys) if edge is not None]
 
     def get_nodes_and_edges(self) -> Tuple[List[MysqlNode], List[Edge]]:
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

### Comparing `grai_source_mysql-0.0.9/src/grai_source_mysql/models.py` & `grai_source_mysql-0.1.0a1/src/grai_source_mysql/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,175 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class MysqlNode(BaseModel):
+    """ """
+
     pass
 
 
 class ID(MysqlNode):
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
 
 
 # https://dev.mysql.com/doc/mysql-infoschema-excerpt/8.0/en/information-schema-columns-table.html
 class ColumnKey(Enum):
+    """ """
+
     NOT_INDEXED = ""
     PRIMARY_KEY = "PRI"
     UNIQUE = "UNI"
     NON_UNIQUE_INDEX = "MUL"
 
 
 UNIQUE_COLUMN_CONSTRAINTS = {ColumnKey.PRIMARY_KEY.value, ColumnKey.UNIQUE.value}
 
 
 class Column(MysqlNode):
+    """ """
+
     name: str = Field(alias="column_name")
     table: str
     column_schema: str = Field(alias="schema")
     data_type: str
     is_nullable: bool
     namespace: str
     default_value: Any = Field(alias="column_default")
     column_key: ColumnKey
 
     class Config:
+        """ """
+
         allow_population_by_field_name = True
 
     @property
     def full_name(self) -> str:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return f"{self.column_schema}.{self.table}.{self.name}"
 
 
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
 
 
 class Table(MysqlNode):
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
@@ -117,27 +182,39 @@
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
         destination = ColumnID(
             table_schema=self.self_schema,
             table_name=self.self_table,
             name=self.self_columns[0],
             namespace=self.namespace,
         )
         source = ColumnID(
```

