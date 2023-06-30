# Comparing `tmp/kaiju_db-2.1.4-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19823 bytes, number of entries: 12
--rw-r--r--  2.0 unx      183 b- defN 23-Jun-29 12:17 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Jun-29 12:17 kaiju_db/functions.py
--rw-r--r--  2.0 unx    58012 b- defN 23-Jun-29 12:17 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jun-29 12:17 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 12:17 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3240 b- defN 23-Jun-29 12:17 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4831 b- defN 23-Jun-29 12:17 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3090 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/RECORD
-12 files, 75124 bytes uncompressed, 18251 bytes compressed:  75.7%
+Zip file size: 19995 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-30 16:21 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3665 b- defN 23-Jun-30 16:21 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    58628 b- defN 23-Jun-30 16:21 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-30 16:21 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 16:21 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3292 b- defN 23-Jun-30 16:21 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4831 b- defN 23-Jun-30 16:21 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/RECORD
+12 files, 75792 bytes uncompressed, 18423 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.4.dist-info/LICENSE
+Filename: kaiju_db-2.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.4.dist-info/METADATA
+Filename: kaiju_db-2.1.5.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.4.dist-info/WHEEL
+Filename: kaiju_db-2.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.4.dist-info/top_level.txt
+Filename: kaiju_db-2.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.4.dist-info/RECORD
+Filename: kaiju_db-2.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.4'
+__version__ = '2.1.5'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/services.py

```diff
@@ -22,15 +22,15 @@
 import sqlalchemy.dialects.postgresql as sa_pg
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.sql.expression import nullslast
 from sqlalchemy import MetaData, text, Table  # noqa pycharm
 from sqlalchemy.ext.asyncio import create_async_engine  # noqa pycharm
 
 from kaiju_tools.app import ContextableService, service_class_registry, Service
-from kaiju_tools.interfaces import DataStore
+from kaiju_tools.interfaces import DataStore, Locks
 from kaiju_tools.exceptions import ValidationError, NotFound, Conflict, InternalError, MethodNotAllowed
 from kaiju_tools.serialization import dumps, loads, load
 from kaiju_db.functions import functions_registry, UserFunction
 
 __all__ = ['DatabaseService', 'SQLService', 'FixtureService', 'DatabaseMigrationService']
 
 
@@ -1377,15 +1377,17 @@
             return
 
         if self.empty_tables_only:
             if await self._table_not_empty(service_name):
                 self.logger.debug('Cannot load fixture: table is not empty', fixture=service_name)
                 return
 
-        data = load(path)
+        with open(path) as f:
+            data = load(f)
+
         if data:
             self.logger.info('Loading fixture', fixture=service_name, filename=str(path))
             await service.m_create(data=data, columns=[], on_conflict='do_nothing')
 
     async def _table_not_empty(self, service_name: str) -> bool:
         service = cast(SQLService, self.app.services[service_name])
         data = await service.list(limit=1, count=False)
@@ -1407,33 +1409,38 @@
     _null_state = -1
 
     def __init__(
         self,
         app,
         *,
         database_service: DatabaseService = None,
+        locks_service: Locks = None,
         migrations_file='./etc/migrations.json',
         migrate_on_start: bool = False,
         logger=None,
     ):
         """Initialize.
 
         :param app:
         :param database_service:
+        :param locks_service:
         :param migrations_file: default migrations file
         :param migrate_on_start: perform an automatic migration from the current state at async init
         :param logger:
         """
         super().__init__(app, logger=logger)
         self._migrations_file = migrations_file
-        self._db = self.discover_service(database_service, cls=DatabaseMigrationService)
+        self._db = self.discover_service(database_service, cls=DatabaseService)
         self._db.add_table(self._state_table)
+        self._locks = locks_service
+        self._lock_key = self.app.namespace.create_namespace('_migrations').get_key('_lock')
         self._migrate_on_start = migrate_on_start
 
     async def init(self):
+        self._locks = self.discover_service(self._locks, cls=Locks)
         if self._migrate_on_start:
             await self.migrate()
 
     async def migrate(self, from_: int = None, to_: int = None, migrations_file: str = None) -> int:
         """Migrate DB from one state to another.
 
         Migration file is expected to be a json file with a number of sorted states containing state id and a list of
@@ -1457,42 +1464,49 @@
         :param migrations_file: optional migrations file path
         :return: current state id
         """
         if migrations_file is None:
             migrations_file = self._migrations_file
         with open(migrations_file) as f:
             migrations: List[DatabaseMigrationService.State] = load(f)
-        state_id = await self.get_state()
-        self.logger.info('Start state: #%d.', state_id)
-        if from_ is None:
-            from_ = state_id
-        if to_ is None:
-            to_ = migrations[-1]['id']
-        self.logger.info('Performing migration: #%d -> #%d', from_, to_)
-        for state in migrations:
-            state_id = state['id']
-            if state_id <= from_:
-                continue
-            elif state_id > to_:
-                break
-            self.logger.info('Migrating state: #%d', state['id'])
-            async with self._db.begin() as conn:
-                for n, cmd in enumerate(state['commands']):
-                    self.logger.info('Migrating state: #%d/%d.', state['id'], n)
-                    await conn.execute(sa.text(cmd))
-                sql = (
-                    self._state_table.update()
-                    .where(self._state_table.c.key == self._state_key)
-                    .values({'value': state['id']})
-                )
-                await conn.execute(sql)
-                await conn.commit()
+        if not migrations:
+            return -1
+        identifier = await self._locks.acquire(self._lock_key)  # TODO: lock context
+        try:
+            state_id = await self.get_state()
+            self.logger.debug('Current state: #%d.', state_id)
+            if from_ is None:
+                from_ = state_id
+            if to_ is None:
+                to_ = migrations[-1]['id']
+            if from_ == to_:
+                return to_
+            self.logger.info('Performing migration: #%d -> #%d', from_, to_)
+            for state in migrations:
+                state_id = state['id']
+                if state_id <= from_:
+                    continue
+                elif state_id > to_:
+                    break
+                async with self._db.begin() as conn:
+                    for n, cmd in enumerate(state['commands']):
+                        self.logger.info('Migrating: #%d/%d.', state['id'], n)
+                        await conn.execute(sa.text(cmd))
+                    sql = (
+                        self._state_table.update()
+                        .where(self._state_table.c.key == self._state_key)
+                        .values({'value': state['id']})
+                    )
+                    await conn.execute(sql)
+                    await conn.commit()
 
-        state_id = await self.get_state()
-        self.logger.info('End state: #%d', state_id)
+            state_id = await self.get_state()
+        finally:
+            await self._locks.release(self._lock_key, identifier)
+        self.logger.debug('Current state: #%d', state_id)
         return state_id
 
     async def get_state(self) -> int:
         """Get current (supposed) database state."""
         sql = self._state_table.select().where(self._state_table.c.key == self._state_key)
         state = await self._db.fetchrow(sql)
         if state is None:
```

## kaiju_db/tests/fixtures.py

```diff
@@ -88,17 +88,19 @@
 @pytest.fixture
 def migrations_file(tmp_path):
     path = tmp_path / 'migrations.json'
     return path
 
 
 @pytest.fixture
-def migrations_service(postgres_glob, app, database_service, migrations_file) -> DatabaseMigrationService:
+def migrations_service(postgres_glob, app, database_service, mock_locks, migrations_file) -> DatabaseMigrationService:
     """Return a new instance of database service."""
-    service = DatabaseMigrationService(app, database_service=database_service, migrations_file=str(migrations_file))
+    service = DatabaseMigrationService(
+        app, database_service=database_service, migrations_file=str(migrations_file), locks_service=mock_locks
+    )
     app.services.add_service(service)
     return service
 
 
 @pytest.fixture
 def test_table(database_service):
     t = sa.Table(
```

## Comparing `kaiju_db-2.1.4.dist-info/LICENSE` & `kaiju_db-2.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.4.dist-info/METADATA` & `kaiju_db-2.1.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.4
+Version: 2.1.5
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

