# Comparing `tmp/apidevtools-4.0.0.tar.gz` & `tmp/apidevtools-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-4.0.0.tar", last modified: Fri Jun 30 12:38:19 2023, max compression
+gzip compressed data, was "apidevtools-4.0.1.tar", last modified: Fri Jun 30 17:55:59 2023, max compression
```

## Comparing `apidevtools-4.0.0.tar` & `apidevtools-4.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.597443 apidevtools-4.0.0/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-06-30 12:38:19.597443 apidevtools-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.0/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-30 12:37:40.000000 apidevtools-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 12:38:19.597443 apidevtools-4.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.555440 apidevtools-4.0.0/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.558443 apidevtools-4.0.0/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.0/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.0/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.568446 apidevtools-4.0.0/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.0/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.0/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.0/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.0/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.572442 apidevtools-4.0.0/src/apidevtools/orm/
--rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.0/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4353 2023-06-30 10:10:21.000000 apidevtools-4.0.0/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.0/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.0/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.575444 apidevtools-4.0.0/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.0/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.580443 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2133 2023-06-30 12:35:54.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      893 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-4.0.0/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.584442 apidevtools-4.0.0/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.0/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.0/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.0/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.587444 apidevtools-4.0.0/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.592444 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.595445 apidevtools-4.0.0/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-06-30 12:35:50.000000 apidevtools-4.0.0/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.563444 apidevtools-4.0.0/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.817048 apidevtools-4.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-06-30 17:55:59.817048 apidevtools-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.1/README.md
+-rw-rw-rw-   0        0        0     2185 2023-06-30 17:55:40.000000 apidevtools-4.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 17:55:59.817048 apidevtools-4.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.773046 apidevtools-4.0.1/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.776046 apidevtools-4.0.1/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.1/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.1/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.786045 apidevtools-4.0.1/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.1/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.1/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.1/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.1/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.790046 apidevtools-4.0.1/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.1/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4842 2023-06-30 17:48:16.000000 apidevtools-4.0.1/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.1/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.1/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.793046 apidevtools-4.0.1/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.1/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-06-30 17:19:13.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.800046 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2583 2023-06-30 17:19:52.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      893 2023-06-30 11:21:27.000000 apidevtools-4.0.1/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      522 2023-06-30 17:03:13.000000 apidevtools-4.0.1/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.803044 apidevtools-4.0.1/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.1/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.1/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.1/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.806045 apidevtools-4.0.1/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.812048 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.815047 apidevtools-4.0.1/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.1/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-06-30 14:42:33.000000 apidevtools-4.0.1/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:55:59.781046 apidevtools-4.0.1/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-06-30 17:55:59.000000 apidevtools-4.0.1/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-06-30 17:55:59.000000 apidevtools-4.0.1/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:55:59.000000 apidevtools-4.0.1/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-06-30 17:55:59.000000 apidevtools-4.0.1/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 17:55:59.000000 apidevtools-4.0.1/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-4.0.0/LICENSE.txt` & `apidevtools-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/PKG-INFO` & `apidevtools-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.0
+Version: 4.0.1
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.0/README.md` & `apidevtools-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/pyproject.toml` & `apidevtools-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "4.0.0"
+version = "4.0.1"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-4.0.0/src/apidevtools/logman.py` & `apidevtools-4.0.1/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-4.0.1/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/media/imgproc.py` & `apidevtools-4.0.1/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/media/telegraph.py` & `apidevtools-4.0.1/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/mysql.py` & `apidevtools-4.0.1/src/apidevtools/orm/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
+from typing import Any, Optional, AsyncGenerator, Callable, Awaitable, Dict
 from functools import cache
 import aiomysql
 
-from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Query, Schema
+from .types import Connector, RecordType, Record, Insert, Select, Update, Delete, Query, Schema, Operation
 from .. import logman
 
 
 class MySQL(Connector, Insert, Select, Update, Delete):
     _placeholder = '%s'
 
     def __init__(self, database: str,
@@ -92,7 +92,14 @@
         async def to_dict(record: Any, _: RecordType) -> dict[str, Any]:
             return record
 
         async def to_schema(record: Any, type: RecordType) -> Schema:
             return await type(**record).from_db()
 
         return to_dict if type is dict else to_schema
+
+    def returning(self, *columns: str, type: RecordType = Dict[str, Any], auto: bool = False) -> Operation:
+        super().returning(*columns, type=type, auto=auto)
+        if all([stmt in self._commands.keys() for stmt in ['update', 'returning']]):
+            tablename = self._commands['update'].split(' ')[1]
+            self._commands['returning'] = f'; SELECT * FROM {tablename} LIMIT ROW_COUNT() OFFSET LAST_INSERT_ID() - ROW_COUNT();'
+        return self
```

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/postgresql.py` & `apidevtools-4.0.1/src/apidevtools/orm/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/sqlite.py` & `apidevtools-4.0.1/src/apidevtools/orm/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/types/_connector.py` & `apidevtools-4.0.1/src/apidevtools/orm/types/_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import suppress
-from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
+from typing import Any, Optional, AsyncGenerator, Callable, Awaitable, Dict
 from abc import abstractmethod
 from copy import copy
 
 from .types import RecordType, Record
 from ._operations import Operation
 from ._operations import Query
 
@@ -64,12 +64,12 @@
         if isinstance(query, Operation):
             commands = {self._mapping[key]: self._commands[key] for key, value in self._commands.items()}  # noqa
             query = f"{' '.join([commands[key] for key in sorted(commands.keys())])};"  # noqa
             args = copy(self._args)  # noqa
 
         self._commands.clear()  # noqa
         self._args.clear()  # noqa
-        self._type = dict
+        self._type = Dict[str, Any]
         with suppress(AttributeError):
             self._placeholder_count = 0
 
         return query, args, type, self._unwrapper(type)
```

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-4.0.1/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional
+from typing import Any, Optional, Dict
 
 from ..types import RecordType, Record
 
 
 class Operation:
     _mapping: dict[str, int] = {
         'insert': 1, 'select': 1, 'update': 1, 'delete': 1,
@@ -13,53 +13,59 @@
         'order': 6,
         'limit': 7,
         'offset': 8,
         'returning': 9,
     }
     _commands: dict[str, str] = {}
     _args: list = []
-    _type: type = dict
+    _type: type = Dict[str, Any]
 
     def fr0m(self, table: str) -> 'Operation':
         c = self._constraint_wrapper  # noqa
-
         self._commands['from'] = f"FROM {c}{table}{c}"
         return self
 
+    # =/LIKE AND/OR
     def where(self, **conditions: Any) -> 'Operation':
         self._args += conditions.values()
         p, c = self._placeholder, self._constraint_wrapper  # noqa
         conditions = ' AND '.join([f'{c}{key}{c} = {p}' for key, value in conditions.items()])
         self._commands['where'] = f"WHERE {conditions}"
         return self
 
     def order(self, **columns: str) -> 'Operation':
         columns = ', '.join([f'{key} {value.upper()}' for key, value in columns.items()])
         self._commands['order'] = f"ORDER BY {columns}"
         return self
 
     def limit(self, value: int) -> 'Operation':
-        self._commands['limit'] = f"LIMIT {value}"
+        p = self._placeholder  # noqa
+        self._args.append(value)
+        self._commands['limit'] = f"LIMIT {p}"
         return self
 
     def offset(self, value: int) -> 'Operation':
-        self._commands['offset'] = f"OFFSET {value}"
+        p = self._placeholder  # noqa
+        self._args.append(value)
+        self._commands['offset'] = f"OFFSET {p}"
         return self
 
-    def returning(self, *columns, type: RecordType = dict) -> 'Operation':
-        if type:
-            self._type = type
+    def returning(self, *columns: str, type: RecordType = Dict[str, Any], auto: bool = False) -> 'Operation':
+        self._type = type
         if columns:
             self._commands['returning'] = f"RETURNING {', '.join(columns)}"
+        if auto and not self._commands.get('returning'):
+            if any([stmt in self._commands.keys() for stmt in ['insert', 'select', 'update', 'delete']]):
+                self.returning('*')
         return self
 
-    async def all(self, type: RecordType = dict) -> list[Record]:
-        return await self.fetchall(self, self._args, type)  # noqa
+    async def all(self, type: RecordType = Dict[str, Any]) -> list[Record]:
+        return await self.fetchall(self.returning(auto=True), self._args, type)  # noqa
 
-    async def one(self, type: RecordType = dict) -> Optional[Record]:
-        return await self.fetchone(self, self._args, type)  # noqa
+    async def one(self, type: RecordType = Dict[str, Any]) -> Optional[Record]:
+        return await self.fetchone(self.returning(auto=True), self._args, type)  # noqa
 
     async def exec(self) -> bool:
         return await self.execute(self, self._args)  # noqa
 
 
 Query: type = type[str, Operation]
```

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/types/_operations/insert.py` & `apidevtools-4.0.1/src/apidevtools/orm/types/_operations/insert.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/types/_operations/update.py` & `apidevtools-4.0.1/src/apidevtools/orm/types/_operations/update.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/orm/types/types.py` & `apidevtools-4.0.1/src/apidevtools/orm/types/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import abstractmethod as _abstractmethod, ABC
 from pydantic import BaseModel
-from typing import Any
+from typing import Any, Dict
 
 
 class Schema(BaseModel, ABC):
     @property
     @_abstractmethod
     def __tablename__(self) -> str:
         ...
@@ -17,9 +17,9 @@
     async def into_db(self) -> 'Schema':
         return self
 
     async def from_db(self) -> 'Schema':
         return self
 
 
-Record = dict[str, Any] | Schema
+Record = Dict[str, Any] | Schema
 RecordType = type[Record]
```

### Comparing `apidevtools-4.0.0/src/apidevtools/security/encryptor.py` & `apidevtools-4.0.1/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/security/hasher.py` & `apidevtools-4.0.1/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/orm.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/redis.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/types/records.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-4.0.1/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools/utils.py` & `apidevtools-4.0.1/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-4.0.0/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-4.0.1/src/apidevtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 4.0.0
+Version: 4.0.1
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-4.0.0/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-4.0.1/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

