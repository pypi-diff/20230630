# Comparing `tmp/fyCursor-0.1.2.tar.gz` & `tmp/fyCursor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.2.tar", last modified: Thu Jun  8 20:29:54 2023, max compression
+gzip compressed data, was "fyCursor-0.1.3.tar", last modified: Fri Jun 30 14:01:36 2023, max compression
```

## Comparing `fyCursor-0.1.2.tar` & `fyCursor-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 20:29:34.000000 fyCursor-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-08 20:29:54.347142 fyCursor-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 20:29:34.000000 fyCursor-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:29:54.347142 fyCursor-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 20:29:34.000000 fyCursor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 14:01:25.000000 fyCursor-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 14:01:36.754741 fyCursor-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-30 14:01:25.000000 fyCursor-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:01:36.754741 fyCursor-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 14:01:25.000000 fyCursor-0.1.3/setup.py
```

### Comparing `fyCursor-0.1.2/LICENSE` & `fyCursor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.2/PKG-INFO` & `fyCursor-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.2/README.md` & `fyCursor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.2/fyCursor/__init__.py` & `fyCursor-0.1.3/fyCursor/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sqlite3 as _sq3
+import typing as _typing
 import os as _os
 from .core import (
     fyCursor,
     Table,
     Field,
     TableError
 )
 
 
 def connect(
-    database: _os.PathLike | str,
+    database: _os.PathLike[_typing.Any] | str,
 ) -> 'fyCursor':
     """
     Connect database and return cursor
 
     Alternative to:
     >>> import sqlite3
     ... from fyCursor import fyCursor
@@ -28,15 +29,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.1.2/fyCursor/__main__.py` & `fyCursor-0.1.3/fyCursor/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fyCursor import Table, Field, connect
+'''from fyCursor import Table, Field, connect
 
 cursor = connect("database.db")
 
 # --------------------------------------------------------------------------------------//
 #                                   CREATING A TABLE
 # --------------------------------------------------------------------------------------//
 
@@ -45,7 +45,8 @@
 felixMoney = cursor.select("money", from_="myTable").where(name="felix").one()
 
 # change money of user with id 5
 cursor.update("myTable").set(money=349).where(id=5).commit()
 
 # add 5 to money to all users
 cursor.update("myTable").add(money=5).commit()
+'''
```

### Comparing `fyCursor-0.1.2/fyCursor/core/cursor.py` & `fyCursor-0.1.3/fyCursor/core/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,86 @@
+# pyright: reportPrivateUsage=false
 import sqlite3
 import logging
 
+from .fields import Field
 from typing import Union, Any, Optional
-from .table import Table
+
+
+class TableError(BaseException):
+    """Raised if something went wrong while creating a table class"""
+
+
+class Table():
+    def __init__(
+        self,
+        name: str,
+        cursor: "fyCursor",
+        args_fields: Optional[list[Field]] = None,
+        kwargs_fields: Optional[dict[str, Field]] = None
+    ) -> None:
+        assert kwargs_fields or args_fields, (
+            "you should provide either args_fields or kwargs_fields"
+        )
+        self._table: list[str] = []
+        self._sql = ""
+        self.name = name
+        self.cursor = cursor
+        if kwargs_fields is not None:
+            self._table.extend(
+                f"{value} {value_._generate_field()},"
+                for value, value_ in kwargs_fields.items()
+            )
+
+            for value, value_ in kwargs_fields.items():
+                self._sql += f"{value} {value_._generate_field()},"
+        if args_fields is not None:
+            self._fields = {
+                str(arg.name): arg for arg in args_fields
+            }
+        else:
+            return
+        for value in args_fields:
+            if not value.name:
+                del self._table
+                del self._fields
+
+                raise TableError(
+                    "You must provide name of field if you providing it as "
+                    "args to a table."
+                )
+            self._sql += value._generate_field()
+            self._table.append(value._generate_field())
+
+    def insert(self, **kwargs: Any) -> "Table":
+        names_ = list(kwargs.keys())
+        values_ = list(kwargs.values())
+
+        def generate_name(name: str):
+            return f"{name},"
+
+        names = ""
+        for item in names_:
+            names += generate_name(item)
+
+        values = ""
+        for item in values_:
+            values += generate_name(item)
+
+        self.cursor.execute(
+            f"INSERT INTO {self.name}({names[:-1]}) VALUES ({values[:-1]})"
+        )
+
+        return self
+
+    def get_values(self) -> dict[str, Field]:
+        return self._fields
+
+    def create(self, if_not_exist: bool = False) -> "Table":
+        return self.cursor.create_table(self, if_not_exist)
 
 
 class fyCursor(sqlite3.Cursor):
     """
     Custom `sqlite3.Cursor` that can be used without string query. \n
     I just hate query because it does not have any highlighting in IDE, yeah.
 
@@ -54,15 +128,15 @@
                 "You should use something before `add`"
             )
         column = list(kwargs.keys())[0]
         value = list(kwargs.values())[0]
         self._query += f" SET {column} = {column} + {value}"
         return self
 
-    def set(self, **kwargs: Any) -> 'fyCursor':
+    def set(self, fix: bool = True, **kwargs: Any) -> 'fyCursor':
         """
         Use this as SQL`SET {kwargs.keys} = {kwargs.values}`
 
         :returns: - self
 
         :raises: - `sqlite3.ProgrammingError` if you didn't use
         `fyCursor.update()` or something similar before this statement
@@ -71,49 +145,53 @@
             raise sqlite3.ProgrammingError(
                 "You should use something before `set`"
             )
 
         column = list(kwargs.keys())[0]
         value = str(list(kwargs.values())[0])
         column = column or "NULL"
+
+        if fix:
+            value = f"\"{value}\""
+
         self._query += f" SET {column} = {value}"
         return self
 
-    def select(self, value, from_: Optional[str] = None) -> 'fyCursor':
+    def select(self, value: str, from_: Optional[str] = None) -> 'fyCursor':
         """
         Use this as SQL `SELECT {value} FROM {from_}`
 
         :param value: - value to be selected
         :param from_: - table from which value will be selected
 
         :returns: - self
         """
         self._query = f"SELECT {value}"
         if from_ is not None:
             self._from(from_)
         return self
 
-    def _from(self, table) -> 'fyCursor':
+    def _from(self, table: str) -> 'fyCursor':
         self._query += f" FROM {table}"
         return self
 
-    def where(self, **kwargs) -> 'fyCursor':
+    def where(self, **kwargs: Any) -> 'fyCursor':
         if not self._query:
             raise sqlite3.ProgrammingError(
                 "You should use something before `where`"
             )
         self._query += (
             f" WHERE {list(kwargs.keys())[0]} "
             f"= \"{list(kwargs.values())[0]}\""
         )
         return self
 
     def fetch(
         self, one: bool = False
-    ) -> Optional[Union[tuple[Any], list[Any]]]:
+    ) -> Optional[Union[tuple[Any], list[Any]] | Any]:
         """
         fetch values from cursor query
 
         :param one - if `True` provided, the `cursor.fetchone()`
         function will be used
         """
         if not self._query:
@@ -143,11 +221,12 @@
     def create_table(
         self,
         table: Table,
         if_not_exist: bool = False
     ) -> "Table":
         exist = "IF NOT EXISTS" if if_not_exist else ""
         super().execute(f"""
-            CREATE TABLE {exist} {table.name}({table._sql[:-1]})
+            CREATE TABLE {exist}\
+             {table.name}({table._sql[:-1]})
         """)
 
         return table
```

### Comparing `fyCursor-0.1.2/fyCursor/core/fields.py` & `fyCursor-0.1.3/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.2/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.3/fyCursor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.2/setup.py` & `fyCursor-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.2",
+    version="0.1.3",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

