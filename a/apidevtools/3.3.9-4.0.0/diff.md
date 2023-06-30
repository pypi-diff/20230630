# Comparing `tmp/apidevtools-3.3.9.tar.gz` & `tmp/apidevtools-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.3.9.tar", last modified: Thu Jun 29 21:14:40 2023, max compression
+gzip compressed data, was "apidevtools-4.0.0.tar", last modified: Fri Jun 30 12:38:19 2023, max compression
```

## Comparing `apidevtools-3.3.9.tar` & `apidevtools-4.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.932526 apidevtools-3.3.9/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-06-29 21:14:40.931527 apidevtools-3.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.9/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-29 21:14:26.000000 apidevtools-3.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 21:14:40.932526 apidevtools-3.3.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.899552 apidevtools-3.3.9/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.902551 apidevtools-3.3.9/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.9/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-3.3.9/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.909527 apidevtools-3.3.9/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.9/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.9/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.9/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.9/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.912527 apidevtools-3.3.9/src/apidevtools/orm/
--rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-3.3.9/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4353 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.915528 apidevtools-3.3.9/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-3.3.9/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2049 2023-06-28 21:40:46.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.919527 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2297 2023-06-29 18:55:11.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      491 2023-06-29 16:30:07.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0     1581 2023-06-29 18:55:35.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      385 2023-06-29 18:55:37.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      885 2023-06-29 20:52:22.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-3.3.9/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.922527 apidevtools-3.3.9/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.9/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.9/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.9/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.924527 apidevtools-3.3.9/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.928527 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.930527 apidevtools-3.3.9/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.9/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.906527 apidevtools-3.3.9/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.597443 apidevtools-4.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-4.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-06-30 12:38:19.597443 apidevtools-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-4.0.0/README.md
+-rw-rw-rw-   0        0        0     2185 2023-06-30 12:37:40.000000 apidevtools-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 12:38:19.597443 apidevtools-4.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.555440 apidevtools-4.0.0/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-4.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.558443 apidevtools-4.0.0/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-4.0.0/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-4.0.0/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.568446 apidevtools-4.0.0/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-4.0.0/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-4.0.0/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-4.0.0/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-4.0.0/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.572442 apidevtools-4.0.0/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-4.0.0/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4353 2023-06-30 10:10:21.000000 apidevtools-4.0.0/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-4.0.0/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-4.0.0/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.575444 apidevtools-4.0.0/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-4.0.0/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.580443 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2133 2023-06-30 12:35:54.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      506 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1180 2023-06-30 11:32:44.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      336 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      893 2023-06-30 11:21:27.000000 apidevtools-4.0.0/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-4.0.0/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.584442 apidevtools-4.0.0/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-4.0.0/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-4.0.0/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-4.0.0/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.587444 apidevtools-4.0.0/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.592444 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.595445 apidevtools-4.0.0/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-4.0.0/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-06-30 12:35:50.000000 apidevtools-4.0.0/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:19.563444 apidevtools-4.0.0/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 12:38:19.000000 apidevtools-4.0.0/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.3.9/LICENSE.txt` & `apidevtools-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/PKG-INFO` & `apidevtools-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.9
+Version: 4.0.0
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.9/README.md` & `apidevtools-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/pyproject.toml` & `apidevtools-4.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.3.9"
+version = "4.0.0"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-3.3.9/src/apidevtools/logman.py` & `apidevtools-4.0.0/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-4.0.0/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/media/imgproc.py` & `apidevtools-4.0.0/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/media/telegraph.py` & `apidevtools-4.0.0/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/mysql.py` & `apidevtools-4.0.0/src/apidevtools/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/postgresql.py` & `apidevtools-4.0.0/src/apidevtools/orm/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/sqlite.py` & `apidevtools-4.0.0/src/apidevtools/orm/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/types/_connector.py` & `apidevtools-4.0.0/src/apidevtools/orm/types/_connector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from contextlib import suppress
 from typing import Any, Optional, AsyncGenerator, Callable, Awaitable
 from abc import abstractmethod
+from copy import copy
 
 from .types import RecordType, Record
 from ._operations import Operation
 from ._operations import Query
 
 
 class Connector:
@@ -20,34 +22,14 @@
         ...
 
     # @abstractmethod
     # async def columns(self, tablename: str) -> list[str]:
     #     ...
 
     @abstractmethod
-    def __aiter__(self):
-        return self.records(f'{self._query[:-1]};', self._qargs, self._type)  # noqa
-
-    @abstractmethod
-    def __anext__(self) -> Record:
-        try:
-            return anext(self)
-        except StopIteration:
-            raise StopAsyncIteration
-
-    @abstractmethod
-    def _unwrapper(self, type: RecordType) -> Callable[[Any, RecordType], Awaitable[Record]]:
-        ...
-
-    async def _parameters(self, query: Query, args: tuple[Any, ...], type: RecordType):
-        if isinstance(query, Operation):
-            query, args, type = f'{self._query[:-1]};', self._qargs, self._type  # noqa
-        return query, args, type, self._unwrapper(type)
-
-    @abstractmethod
     async def execute(self, query: Query, args: tuple[Any, ...] = ()) -> bool:
         ...
 
     async def fetchall(self, query: Query, args: tuple[Any, ...] = (), type: RecordType = dict) -> list[Record]:
         try:
             return [record async for record in self.records(query, args, type)]  # noqa
         except Exception as error:
@@ -57,7 +39,37 @@
     @abstractmethod
     async def fetchone(self, query: Query, args: tuple[Any, ...] = (), type: RecordType = dict) -> Optional[Record]:
         ...
 
     @abstractmethod
     async def records(self, query: Query, args: tuple[Any, ...] = (), type: RecordType = dict) -> AsyncGenerator[Record, None]:
         ...
+
+    @abstractmethod
+    def __aiter__(self):
+        return self.records(f'{self._query[:-1]};', self._qargs, self._type)  # noqa
+
+    @abstractmethod
+    def __anext__(self) -> Record:
+        try:
+            return anext(self)
+        except StopIteration:
+            raise StopAsyncIteration
+
+    @abstractmethod
+    def _unwrapper(self, type: RecordType) -> Callable[[Any, RecordType], Awaitable[Record]]:
+        ...
+
+    async def _parameters(self, query: Query, args: tuple[Any, ...], type: RecordType) \
+            -> tuple[str, list[Any, ...], type, Callable[[Any, RecordType], Awaitable[Record]]]:
+        if isinstance(query, Operation):
+            commands = {self._mapping[key]: self._commands[key] for key, value in self._commands.items()}  # noqa
+            query = f"{' '.join([commands[key] for key in sorted(commands.keys())])};"  # noqa
+            args = copy(self._args)  # noqa
+
+        self._commands.clear()  # noqa
+        self._args.clear()  # noqa
+        self._type = dict
+        with suppress(AttributeError):
+            self._placeholder_count = 0
+
+        return query, args, type, self._unwrapper(type)
```

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-4.0.0/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,65 @@
-from typing import Any, Iterable, Optional
+from typing import Any, Optional
 
 from ..types import RecordType, Record
 
 
 class Operation:
-    _query: str
-    _qargs: list
-    _type: type
+    _mapping: dict[str, int] = {
+        'insert': 1, 'select': 1, 'update': 1, 'delete': 1,
+        'from': 2, 'into': 2,
+        'columns': 3,
+        'values': 4, 'set': 4,
+        'where': 5,
+        'order': 6,
+        'limit': 7,
+        'offset': 8,
+        'returning': 9,
+    }
+    _commands: dict[str, str] = {}
+    _args: list = []
+    _type: type = dict
 
     def fr0m(self, table: str) -> 'Operation':
         c = self._constraint_wrapper  # noqa
-        self._query += f"FROM {c}{table}{c} "
+
+        self._commands['from'] = f"FROM {c}{table}{c}"
         return self
 
     def where(self, **conditions: Any) -> 'Operation':
-        self._qargs += conditions.values()
+        self._args += conditions.values()
         p, c = self._placeholder, self._constraint_wrapper  # noqa
         conditions = ' AND '.join([f'{c}{key}{c} = {p}' for key, value in conditions.items()])
-        self._query += f"WHERE {conditions} "
+        self._commands['where'] = f"WHERE {conditions}"
         return self
 
     def order(self, **columns: str) -> 'Operation':
         columns = ', '.join([f'{key} {value.upper()}' for key, value in columns.items()])
-        self._query += f"ORDER BY {columns} "
+        self._commands['order'] = f"ORDER BY {columns}"
         return self
 
     def limit(self, value: int) -> 'Operation':
-        self._query += f"LIMIT {value} "
+        self._commands['limit'] = f"LIMIT {value}"
         return self
 
     def offset(self, value: int) -> 'Operation':
-        self._query += f"OFFSET {value} "
+        self._commands['offset'] = f"OFFSET {value}"
         return self
 
     def returning(self, *columns, type: RecordType = dict) -> 'Operation':
         if type:
             self._type = type
         if columns:
-            self._query += f"RETURNING {', '.join(columns)} "
+            self._commands['returning'] = f"RETURNING {', '.join(columns)}"
         return self
 
     async def all(self, type: RecordType = dict) -> list[Record]:
-        # if not (query := self._query.lower()).startswith('select'):
-        #     if 'returning' not in query:
-        #         self.returning('*')
-        return await self.fetchall(f'{self._query[:-1]};', tuple(self._qargs), type)
+        return await self.fetchall(self, self._args, type)  # noqa
 
     async def one(self, type: RecordType = dict) -> Optional[Record]:
-        # if not (query := self._query.lower()).startswith('select'):
-        #     if 'returning' not in query:
-        #         self.returning('*')
-        return await self.fetchone(f'{self._query[:-1]};', tuple(self._qargs), type)
+        return await self.fetchone(self, self._args, type)  # noqa
 
     async def exec(self) -> bool:
-        return await self.execute(f'{self._query[:-1]};', tuple(self._qargs))
-
-    def _refresh(self):
-        self._qargs = []
-        self._type = dict
-        try:
-            self._placeholder_count = 0
-        except AttributeError:
-            ...
+        return await self.execute(self, self._args)  # noqa
 
 
-Query: type = type[str | Operation]
+Query: type = type[str, Operation]
```

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/types/_operations/insert.py` & `apidevtools-4.0.0/src/apidevtools/orm/types/_operations/insert.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,42 +2,31 @@
 
 from ._operation import Operation
 from ..types import Schema, Record
 
 
 class Insert(Operation):
     def insert(self, record: Record | list[Record] = None) -> 'Insert':
-        self._refresh()
-
-        self._query = 'INSERT '
+        self._commands['insert'] = 'INSERT'
         if record:
             if isinstance(record, list):
-                for instance in record:
-                    if isinstance(instance, Schema):
-                        self.into(instance.__tablename__)
-                        instance = dict(instance)
-                    self.values(**instance)
+                self.insert(record)
             elif isinstance(record, Schema):
                 self.into(record.__tablename__)
                 self.values(**dict(record))
             elif isinstance(record, dict):
                 self.values(**record)
         return self
 
     def into(self, table: str) -> 'Insert':
-        if 'into' in self._query.lower():
-            self.logger.warning('`INTO {tablename}` specified twice')  # noqa
-        else:
-            self._query += f"INTO {table} "
+        self._commands['into'] = f"INTO {table}"
         return self
 
-    # def values(self, *values: Any) -> 'Insert':
-    def values(self, *values: Any, **columns: Any) -> 'Insert':
-        if columns:
-            self._query += f"({', '.join(columns.keys())}) "
-            values = columns.values()
+    def values(self, **columns: Any) -> 'Insert':
+        self._commands['columns'] = f"({', '.join(columns.keys())})"
+        self._args += (values := columns.values())
         placeholders = ', '.join([self._placeholder for i in range(len(values))])  # noqa
-        if 'values' in self._query.lower():
-            self._query += '\b, '
-        self._qargs += values
-        self._query += f"VALUES ({placeholders}) "
+        if self._commands.get('values'):
+            self._commands['values'] += f", ({placeholders})"
+        else:
+            self._commands['values'] = f"VALUES ({placeholders})"
         return self
```

### Comparing `apidevtools-3.3.9/src/apidevtools/orm/types/types.py` & `apidevtools-4.0.0/src/apidevtools/orm/types/types.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/security/encryptor.py` & `apidevtools-4.0.0/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/security/hasher.py` & `apidevtools-4.0.0/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/orm.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/redis.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/types/records.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-4.0.0/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools/utils.py` & `apidevtools-4.0.0/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.9/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-4.0.0/src/apidevtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.9
+Version: 4.0.0
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.9/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-4.0.0/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

