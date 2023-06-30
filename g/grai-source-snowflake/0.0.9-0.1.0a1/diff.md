# Comparing `tmp/grai_source_snowflake-0.0.9.tar.gz` & `tmp/grai_source_snowflake-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_snowflake-0.0.9.tar", max compression
+gzip compressed data, was "grai_source_snowflake-0.1.0a1.tar", max compression
```

## Comparing `grai_source_snowflake-0.0.9.tar` & `grai_source_snowflake-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      786 2023-01-27 22:50:29.542350 grai_source_snowflake-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      147 2023-01-18 14:35:11.047402 grai_source_snowflake-0.0.9/src/grai_source_snowflake/__init__.py
--rw-r--r--   0        0        0     6102 2023-01-27 22:50:45.345199 grai_source_snowflake-0.0.9/src/grai_source_snowflake/adapters.py
--rw-r--r--   0        0        0     1445 2023-01-27 01:14:06.496945 grai_source_snowflake-0.0.9/src/grai_source_snowflake/base.py
--rw-r--r--   0        0        0     7587 2023-01-27 01:14:06.497042 grai_source_snowflake-0.0.9/src/grai_source_snowflake/loader.py
--rw-r--r--   0        0        0     4231 2023-01-05 00:57:50.897741 grai_source_snowflake-0.0.9/src/grai_source_snowflake/models.py
--rw-r--r--   0        0        0      188 2023-01-27 20:53:45.329460 grai_source_snowflake-0.0.9/src/grai_source_snowflake/package_definitions.py
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.9/setup.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 grai_source_snowflake-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-05-19 11:07:12.943047 grai_source_snowflake-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1113 2023-06-30 03:27:47.552463 grai_source_snowflake-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-06-29 15:34:52.432136 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/__init__.py
+-rw-r--r--   0        0        0     8707 2023-06-29 15:34:52.432255 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/adapters.py
+-rw-r--r--   0        0        0     1204 2023-06-29 15:34:52.432370 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/base.py
+-rw-r--r--   0        0        0    10107 2023-06-14 21:02:53.338748 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/loader.py
+-rw-r--r--   0        0        0     5973 2023-06-01 16:01:43.269618 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/models.py
+-rw-r--r--   0        0        0      201 2023-06-01 16:01:43.269729 grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/package_definitions.py
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 grai_source_snowflake-0.1.0a1/PKG-INFO
```

### Comparing `grai_source_snowflake-0.0.9/src/grai_source_snowflake/base.py` & `grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,41 @@
-from typing import List, Literal, Optional, Tuple
+from typing import Optional
 
 from grai_client.endpoints.client import BaseClient
-from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_client.integrations.base import (
+    ConnectorMixin,
+    GraiIntegrationImplementationV1,
+)
 
 from grai_source_snowflake.adapters import adapt_to_client
 from grai_source_snowflake.loader import SnowflakeConnector
 
 
-def get_nodes_and_edges(
-    connector: SnowflakeConnector, version: Literal["v1"]
-) -> Tuple[List[Node], List[Edge]]:
-    if version != "v1":
-        raise NotImplementedError(
-            f"No available implementation for client version {version}"
+class SnowflakeIntegration(ConnectorMixin, GraiIntegrationImplementationV1):
+    def __init__(
+        self,
+        client: BaseClient,
+        source_name: str,
+        account: Optional[str] = None,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        warehouse: Optional[str] = None,
+        role: Optional[str] = None,
+        database: Optional[str] = None,
+        namespace: Optional[str] = None,
+        **kwargs,
+    ):
+        super().__init__(client, source_name)
+
+        self.connector = SnowflakeConnector(
+            account=account,
+            user=user,
+            password=password,
+            warehouse=warehouse,
+            role=role,
+            database=database,
+            namespace=namespace,
+            **kwargs,
         )
 
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
-    namespace: Optional[str] = None,
-    account: Optional[str] = None,
-    user: Optional[str] = None,
-    password: Optional[str] = None,
-    role: Optional[str] = None,
-    warehouse: Optional[str] = None,
-    database: Optional[str] = None,
-    schema: Optional[str] = None,
-) -> None:
-
-    conn = SnowflakeConnector(
-        account=account,
-        user=user,
-        password=password,
-        role=role,
-        warehouse=warehouse,
-        database=database,
-        schema=schema,
-        namespace=namespace,
-    )
-    nodes, edges = get_nodes_and_edges(conn, client.id)
-    update(client, nodes)
-    update(client, edges)
+    def adapt_to_client(self, objects):
+        return adapt_to_client(objects, self.source, self.client.id)
```

### Comparing `grai_source_snowflake-0.0.9/src/grai_source_snowflake/loader.py` & `grai_source_snowflake-0.1.0a1/src/grai_source_snowflake/loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from functools import cached_property
 from itertools import chain
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import snowflake.connector
 
 from grai_source_snowflake.models import (
     Column,
@@ -10,180 +11,304 @@
     Edge,
     EdgeQuery,
     SnowflakeNode,
     Table,
 )
 
 
+def string_is_quoted(string: str) -> bool:
+    """
+
+    Args:
+        string (str):
+
+    Returns:
+
+    Raises:
+
+    """
+    return string.startswith('"') and string.endswith('"')
+
+
 def get_from_env(
     label: str,
     default: Optional[Any] = None,
     required: bool = True,
     validator: Optional[Callable] = None,
 ):
+    """
+
+    Args:
+        label (str):
+        default (Optional[Any], optional):  (Default value = None)
+        required (bool, optional):  (Default value = True)
+        validator (Optional[Callable], optional):  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     env_key = f"GRAI_SNOWFLAKE_{label.upper()}"
     result = os.getenv(env_key, default)
     if result is None and required:
         message = (
             f"Establishing snowflake connection requires a {label}. "
             f"Either pass a value explicitly or set a {env_key} environment value."
         )
         raise Exception(message)
     return result if validator is None else validator(result)
 
 
 class SnowflakeConnector:
+    """ """
+
     def __init__(
         self,
         account: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         warehouse: Optional[str] = None,
         role: Optional[str] = None,
         database: Optional[str] = None,
-        schema: Optional[str] = None,
         namespace: Optional[str] = None,
         **kwargs,
     ):
         self.account = get_from_env("account") if account is None else account
         self.user = get_from_env("user") if user is None else user
         self.password = get_from_env("password") if password is None else password
         self.warehouse = get_from_env("warehouse") if warehouse is None else warehouse
         self.role = get_from_env("role", required=False) if role is None else role
-        self.database = (
-            get_from_env("database", required=False) if database is None else database
-        )
-        self.schema = (
-            get_from_env("schema", required=False) if schema is None else schema
-        )
-        self.namespace = (
-            get_from_env("namespace", "default") if namespace is None else namespace
-        )
+        self.database = get_from_env("database", required=False) if database is None else database
+        self.namespace = get_from_env("namespace", "default") if namespace is None else namespace
         self.additional_conn_kwargs = kwargs
         self._connection: Optional[snowflake.connector.SnowflakeConnection] = None
 
-        self._tables: Optional[List[Table]] = None
-        self._foreign_keys: Optional[List[Edge]] = None
-
     def __enter__(self):
         return self.connect()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     @property
     def connection_dict(self) -> Dict[str, str]:
+        """Builds connection parameters for Snowflake
+
+        Full documentation of the API available here
+        https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-api#label-snowflake-connector-methods
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         connection_keys = [
             "account",
             "user",
             "password",
             "warehouse",
             "role",
             "database",
-            "schema",
         ]
-        return {
-            key: value
-            for key in connection_keys
-            if (value := getattr(self, key)) is not None
-        }
+        return {key: value for key in connection_keys if (value := getattr(self, key)) is not None}
 
     def connect(self) -> "SnowflakeConnector":
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
-            self._connection = snowflake.connector.connect(
-                **self.connection_dict, **self.additional_conn_kwargs
-            )
+            self._connection = snowflake.connector.connect(**self.connection_dict, **self.additional_conn_kwargs)
         return self
 
     @property
     def connection(self) -> snowflake.connector.SnowflakeConnection:
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
         dict_cursor = self.connection.cursor(snowflake.connector.DictCursor)
         dict_cursor.execute(query, param_dict)
         return dict_cursor.fetchall()  # type: ignore
 
-    def get_tables(self) -> List[Table]:
-        """
-        Create and return a list of dictionaries with the
+    @cached_property
+    def tables(self) -> List[Table]:
+        """Create and return a list of dictionaries with the
         schemas and names of tables in the database
         connected to by the connection argument.
-        """
 
-        if self._tables is not None:
-            return self._tables
+        Args:
+
+        Returns:
+
+        Raises:
 
+        """
         query = """
 	        SELECT table_schema, table_name, table_type
             FROM information_schema.tables
             WHERE table_schema != 'INFORMATION_SCHEMA'
             ORDER BY table_schema, table_name
         """
-        res = (
-            {k.lower(): v for k, v in result.items()}
-            for result in self.query_runner(query)
-        )
+        res = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
 
         additional_args = {
             "namespace": self.namespace,
             "table_database": self.connection_dict["database"],
         }
 
         tables = [Table(**result, **additional_args) for result in res]
         for table in tables:
-            table.columns = self.get_columns(table)
-
-        self._tables = tables
-        return self._tables
+            table.columns = self.get_table_columns(table)
+        return tables
 
-    def get_columns(self, table: Table) -> List[Column]:
-        """
-        Creates and returns a list of dictionaries for the specified
+    @cached_property
+    def columns(self) -> List[Column]:
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
 
+        def quoted_table_name(table_name: str) -> str:
+            """
+
+            Args:
+                table_name (str):
+
+            Returns:
+
+            Raises:
+
+            """
+            return table_name if table_name.startswith('"') and table_name.endswith('"') else f"'{table_name.upper()}'"
+
         query = f"""
-            SELECT column_name, data_type, is_nullable, column_default
+            SELECT column_name, data_type, is_nullable, column_default, table_schema, table_name
             FROM information_schema.columns
-            WHERE table_schema = '{table.table_schema}'
-            AND table_name = '{table.name}'
+            WHERE table_schema != 'INFORMATION_SCHEMA'
         """
 
-        res = (
-            {k.lower(): v for k, v in result.items()}
-            for result in self.query_runner(query)
-        )
+        res = [{k.lower(): v for k, v in result.items()} for result in self.query_runner(query)]
+        for item in res:
+            item.update(
+                {
+                    "table": item["table_name"],
+                    #'table': quoted_table_name(item['table_name']),
+                    "column_schema": item["table_schema"],
+                }
+            )
 
         addtl_args = {
-            "namespace": table.namespace,
-            "schema": table.table_schema,
-            "table": table.name,
+            "namespace": self.namespace,
         }
         return [Column(**result, **addtl_args) for result in res]
 
-    def get_foreign_keys(self) -> List[Edge]:
+    @cached_property
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
+        for col in self.columns:
+            table_id = (col.column_schema, col.table)
+            result_map.setdefault(table_id, [])
+            result_map[table_id].append(col)
+        return result_map
+
+    def get_table_columns(self, table: Table):
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
+        table_id = (table.table_schema, table.name)
+        if table_id in self.column_map:
+            return self.column_map[table_id]
+
+        schema = table_id[0] if string_is_quoted(table_id[0]) else table_id[0].upper()
+        name = table_id[1] if string_is_quoted(table_id[1]) else table_id[1].upper()
+        table_id = (schema, name)
+        if table_id in self.column_map:
+            return self.column_map[table_id]
+        else:
+            raise Exception(f"No columns found for table with schema={schema} and name={name}")
+
+    @cached_property
+    def foreign_keys(self) -> List[Edge]:
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
         # This query only returns foreign keys, there is also exported keys and primary keys.
         # Information schema itself doesn't carry the column for foreign keys
         # show IMPORTED KEYS in database '{self.connection_dict['database']}'
 
-        if self._foreign_keys is not None:
-            return self._foreign_keys
-
         query = f"""
         show IMPORTED KEYS
         """
         addtl_args = {
             "namespace": self.namespace,
         }
 
@@ -204,25 +329,50 @@
             item |= {k: item.pop(v) for k, v in key_rename_map.items()}
             item["constraint_type"] = "f"
             item["definition"] = ""  # Available on another table
             item["self_columns"] = item["self_columns"].split(",")
             item["foreign_columns"] = item["foreign_columns"].split(",")
 
         res = ({k.lower(): v for k, v in result.items()} for result in imported_keys)
-        fks = [EdgeQuery(**fk, **addtl_args).to_edge() for fk in res]
-
-        self._foreign_keys = fks
-        return self._foreign_keys
+        edge_gen = (EdgeQuery(**fk, **addtl_args).to_edge() for fk in res)
+        edges = [edge for edge in edge_gen if edge is not None]
+        return edges
 
     def get_nodes(self) -> List[SnowflakeNode]:
-        tables = self.get_tables()
-        return list(chain(tables, *[t.columns for t in tables]))
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        # return list(chain(self.tables, *[t.columns for t in self.tables]))
+        return list(chain(self.tables, self.columns))
 
     def get_edges(self) -> List[Edge]:
-        tables = self.get_tables()
-        edges = list(chain(*[t.get_edges() for t in tables], self.get_foreign_keys()))
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        edges = [edge for edge in chain(*[t.get_edges() for t in self.tables], self.foreign_keys) if edge is not None]
         return edges
 
     def get_nodes_and_edges(self) -> Tuple[List[SnowflakeNode], List[Edge]]:
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

