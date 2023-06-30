# Comparing `tmp/pymongo-migrate-0.9.1.tar.gz` & `tmp/pymongo-migrate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymongo-migrate-0.9.1.tar", last modified: Mon Mar  4 17:31:51 2019, max compression
+gzip compressed data, was "pymongo-migrate-1.0.0.tar", last modified: Fri Jun 30 07:52:16 2023, max compression
```

## Comparing `pymongo-migrate-0.9.1.tar` & `pymongo-migrate-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 rooter    (1000) rooter    (1000)        0 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/
--rw-r--r--   0 rooter    (1000) rooter    (1000)     1107 2019-03-04 17:30:38.000000 pymongo-migrate-0.9.1/setup.py
-drwxr-xr-x   0 rooter    (1000) rooter    (1000)        0 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/
-drwxr-xr-x   0 rooter    (1000) rooter    (1000)        0 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/
--rw-rw-r--   0 rooter    (1000) rooter    (1000)     1332 2019-03-04 13:25:27.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/generate.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)     5738 2019-03-04 15:32:41.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/mongo_migrate.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)     3260 2019-03-04 13:16:14.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/cli.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)     2969 2019-03-04 08:46:09.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/migrations.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)      804 2019-03-04 08:46:09.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/loader.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)       22 2019-02-26 11:34:26.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/__init__.py
--rw-r--r--   0 rooter    (1000) rooter    (1000)      662 2019-02-26 11:34:26.000000 pymongo-migrate-0.9.1/src/pymongo_migrate/graph_draw.py
-drwxr-xr-x   0 rooter    (1000) rooter    (1000)        0 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/
--rw-r--r--   0 rooter    (1000) rooter    (1000)      556 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 rooter    (1000) rooter    (1000)      688 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/PKG-INFO
--rw-r--r--   0 rooter    (1000) rooter    (1000)       16 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/top_level.txt
--rw-r--r--   0 rooter    (1000) rooter    (1000)        1 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 rooter    (1000) rooter    (1000)       68 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/requires.txt
--rw-r--r--   0 rooter    (1000) rooter    (1000)        1 2019-02-21 15:35:26.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/not-zip-safe
--rw-r--r--   0 rooter    (1000) rooter    (1000)       61 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/src/pymongo_migrate.egg-info/entry_points.txt
--rw-r--r--   0 rooter    (1000) rooter    (1000)      688 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/PKG-INFO
--rw-r--r--   0 rooter    (1000) rooter    (1000)      468 2019-03-04 17:31:51.000000 pymongo-migrate-0.9.1/setup.cfg
--rw-r--r--   0 rooter    (1000) rooter    (1000)     2382 2019-03-04 08:46:09.000000 pymongo-migrate-0.9.1/README.md
+drwxrwxr-x   0 rooter    (1000) rooter    (1000)        0 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/
+-rw-r--r--   0 rooter    (1000) rooter    (1000)    11357 2019-02-26 11:34:26.000000 pymongo-migrate-1.0.0/LICENSE
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     3286 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/PKG-INFO
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     2349 2023-06-29 20:45:30.000000 pymongo-migrate-1.0.0/README.md
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     1502 2023-06-30 07:42:35.000000 pymongo-migrate-1.0.0/pyproject.toml
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)       38 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/setup.cfg
+drwxrwxr-x   0 rooter    (1000) rooter    (1000)        0 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/src/
+drwxrwxr-x   0 rooter    (1000) rooter    (1000)        0 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/src/pymongo_migrate/
+-rw-r--r--   0 rooter    (1000) rooter    (1000)       22 2019-02-26 11:34:26.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/__init__.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     5585 2023-06-29 20:44:22.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/cli.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     1490 2023-06-30 07:47:24.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/generate.py
+-rw-r--r--   0 rooter    (1000) rooter    (1000)      662 2019-02-26 11:34:26.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/graph_draw.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)      861 2023-05-31 12:58:10.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/loader.py
+-rw-r--r--   0 rooter    (1000) rooter    (1000)     2969 2020-07-21 10:05:04.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/migrations.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     7737 2023-06-29 20:44:22.000000 pymongo-migrate-1.0.0/src/pymongo_migrate/mongo_migrate.py
+drwxrwxr-x   0 rooter    (1000) rooter    (1000)        0 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     3286 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/PKG-INFO
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)      650 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/SOURCES.txt
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)        1 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/dependency_links.txt
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)       60 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/entry_points.txt
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)       24 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/requires.txt
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)       16 2023-06-30 07:52:16.000000 pymongo-migrate-1.0.0/src/pymongo_migrate.egg-info/top_level.txt
+drwxrwxr-x   0 rooter    (1000) rooter    (1000)        0 2023-06-30 07:52:16.641709 pymongo-migrate-1.0.0/tests/
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     2159 2023-06-30 07:47:24.000000 pymongo-migrate-1.0.0/tests/test_cli.py
+-rw-r--r--   0 rooter    (1000) rooter    (1000)      365 2023-06-30 06:14:08.000000 pymongo-migrate-1.0.0/tests/test_generate.py
+-rw-r--r--   0 rooter    (1000) rooter    (1000)     1338 2023-06-30 06:14:08.000000 pymongo-migrate-1.0.0/tests/test_main_status.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     3261 2023-06-30 06:14:08.000000 pymongo-migrate-1.0.0/tests/test_mongo_migrate.py
+-rw-rw-r--   0 rooter    (1000) rooter    (1000)     2091 2023-06-30 07:47:24.000000 pymongo-migrate-1.0.0/tests/test_mongo_migrate_generate.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pymongo-migrate-0.9.1/setup.py` & `pymongo-migrate-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,55 @@
-from setuptools import find_packages, setup
+[build-system]
+requires = ["setuptools>=61", "wheel"]
+build-backend = "setuptools.build_meta"
 
-setup(
-    name="pymongo-migrate",
-    version="0.9.1",
-    description="MongoDB data migration tool in Python",
-    url="https://github.com/stxnext/pymongo-migrate",
-    license="Apache",
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
-    platforms="any",
-    include_package_data=True,
-    zip_safe=False,
-    python_requires=">=3.6",
-    install_requires=[
-        "pymongo>=3.7.2",
-        "Click>=7",
-        "dataclasses>=0.6; python_version<'3.7'",
-    ],
-    entry_points={"console_scripts": ["pymongo-migrate=pymongo_migrate.cli:cli"]},
-    keywords=["mongo", "mongodb", "pymongo", "migrate", "migration"],
-    classifiers=[
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Database",
-    ],
-)
+[project]
+name = "pymongo-migrate"
+version = "1.0.0"
+description = "MongoDB data migration tool in Python"
+license = {text="Apache Software License"}
+readme = "README.md"  # assuming you have a README.md file
+requires-python = ">=3.8"
+keywords = ["mongo", "mongodb", "pymongo", "migrate", "migration"]
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Database",
+]
+
+dependencies = [
+"pymongo>=3.7.2",
+    "Click>=7",
+]
+
+[project.urls]
+Homepage = "https://github.com/stxnext/pymongo-migrate"
+Changelog = "https://github.com/stxnext/pymongo-migrate/blob/main/CHANGELOG.md"
+
+[project.scripts]
+pymongo-migrate = "pymongo_migrate.cli:cli"
+
+[tool.setuptools]
+package-dir = {"" = "src"}
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
+exclude = ["tests"]
+
+[tool.ruff]
+select = ["E", "F", "I", "UP"]
+ignore = ["E203", "E266", "E501"]
+exclude = [".git", "__pycache__", ".venv", "build", "dist"]
+
+[tool.pytest.env]
+env_files = ".env"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/generate.py` & `pymongo-migrate-1.0.0/src/pymongo_migrate/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pathlib import Path
 from typing import List, Optional
 
 MIGRATION_MODULE_TMPL = '''\
 """
 {description}
 """
+import pymongo
+
 name = {name!r}
 dependencies = {dependencies!r}
 
 
 def upgrade(db: "pymongo.database.Database"):
     pass
 
@@ -40,17 +42,22 @@
         name=name, description=description, dependencies=dependencies
     )
     fp.write(content)
 
 
 def generate_migration_module_in_dir(
     migration_dir: Path, name: str = "", *args, **kwargs
-):
+) -> Path:
     now = datetime.datetime.utcnow()
     if not name:
         name = f"{now:%Y%m%d%H%M%S}"
         description = kwargs.get("description")
         if description:
             name = f"{name}_{slugify(description)}"
         name = name[:MAX_NAME_LEN]
-    with (migration_dir / f"{name}.py").open("w") as f:
+    file_path = migration_dir / f"{name}.py"
+    if file_path.exists():
+        raise FileExistsError(f"{file_path} already exists")
+
+    with file_path.open("w") as f:
         generate_migration_module(f, name=name, *args, **kwargs)  # type: ignore
+    return file_path
```

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/mongo_migrate.py` & `pymongo-migrate-1.0.0/src/pymongo_migrate/mongo_migrate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import logging
+import time
 from dataclasses import asdict, dataclass
 from pathlib import Path
-from typing import Optional
+from typing import Iterator, Optional
 
 import pymongo
 from bson import CodecOptions
 
 from pymongo_migrate.generate import generate_migration_module_in_dir
 from pymongo_migrate.loader import load_module_migrations
 from pymongo_migrate.migrations import Migration, MigrationsGraph, MigrationState
@@ -28,43 +29,77 @@
 
 def _deserialize(data, cls):
     data = {**data}
     del data["_id"]
     return cls(**data)
 
 
+class _MeasureTime:
+    """
+    Class to measure the time of execution of code block.
+    usage:
+
+     with MeasureTime() as mt:
+         # code block ...
+         print(f"Execution time: {mt.elapsed}s")
+    """
+
+    def __init__(self):
+        self.start = None
+        self.stop = None
+
+    @staticmethod
+    def time() -> float:
+        return time.time()
+
+    @property
+    def elapsed(self) -> Optional[float]:
+        if self.start is None:
+            return None
+        return (self.stop or self.time()) - self.start
+
+    def __enter__(self):
+        self.start = self.time()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.stop = self.time()
+
+
 @dataclass
 class MongoMigrate:
-    mongo_uri: str  # https://docs.mongodb.com/manual/reference/connection-string/
+    client: pymongo.MongoClient
+    database: str
     migrations_dir: str = "./pymongo_migrations"
     migrations_collection: str = "pymongo_migrate"
     logger: logging.Logger = LOGGER
 
     def __post_init__(self):
-        self.client = pymongo.MongoClient(self.mongo_uri)
         self.graph = MigrationsGraph()
         for migration in load_module_migrations(self.migrations_path):
             self.graph.add_migration(migration)
         self.graph.verify()
 
     @property
     def migrations_path(self):
         return Path(self.migrations_dir)
 
     @property
     def db(self):
-        return self.client.get_database()
+        return self.client.get_database(self.database)
 
     @property
     def db_collection(self):
-        return self.client.get_database()[self.migrations_collection].with_options(
+        return self.client.get_database(self.database)[
+            self.migrations_collection
+        ].with_options(
             codec_options=CodecOptions(tz_aware=True, tzinfo=datetime.timezone.utc)
         )
 
-    def get_migrations(self):
+    def get_migrations(self) -> Iterator[Migration]:
         yield from self.graph
 
     def get_state(self, migration: Migration) -> MigrationState:
         data = self.db_collection.find_one({"name": migration.name})
         if data:
             return _deserialize(data, MigrationState)
         return MigrationState(name=migration.name)
@@ -80,84 +115,111 @@
         if migration_name is None:
             return None
         migration = self.graph.migrations.get(migration_name)
         if migration is None:
             raise ValueError(f"No such migration: {migration_name}")
         return migration
 
-    def migrate(self, migration_name: Optional[str] = None):
+    def migrate(self, migration_name: Optional[str] = None, fake: bool = False):
         """
         Automatically detects if upgrades or downgrades should be applied to
         reach target migration state.
 
         :param migration_name:
             target migration
             None if all upgrades should be applied
+        :param fake:
+            If True, only migration state in database will be modified and
+            no actual migration will be run.
         """
         if migration_name is None:
             self.logger.debug("Migration target not specified, assuming upgrade")
-            self.upgrade()
+            self.upgrade(fake=fake)
             return
         migration = self._check_for_migration(migration_name)
         assert migration, "No matching migration, something went wrong"
         migration_state = self.get_state(migration)
         if migration_state.applied:
             self.logger.debug("Migration target already applied, assuming downgrade")
-            self.downgrade(migration_name)
+            self.downgrade(migration_name, fake)
         else:
-            self.logger.debug("Migration target already applied, assuming upgrade")
-            self.upgrade(migration_name)
+            self.logger.debug("Migration target not applied, assuming upgrade")
+            self.upgrade(migration_name, fake)
 
-    def upgrade(self, migration_name: Optional[str] = None):
+    def upgrade(self, migration_name: Optional[str] = None, fake: bool = False):
         """
         Apply upgrade migrations.
 
         :param migration_name:
             name of migration up to which (including) upgrades should be executed
             None if all migrations should be run
+        :param fake:
+            If True, only migration state in database will be modified and
+            no actual migration will be run.
         """
         self._check_for_migration(migration_name)
         for migration in self.graph:
             migration_state = self.get_state(migration)
             if migration_state.applied:
-                LOGGER.debug("Migration %r already applied, skipping")
+                self.logger.debug(
+                    "Migration %r already applied, skipping", migration.name
+                )
                 continue
-            LOGGER.info("Running upgrade migration %r", migration.name)
-            migration.upgrade(self.db)
+            if fake:
+                self.logger.info("Fake running upgrade migration %r", migration.name)
+            else:
+                self.logger.info("Running upgrade migration %r", migration.name)
+                with _MeasureTime() as mt:
+                    migration.upgrade(self.db)
+                    self.logger.info(
+                        "Execution time of %r: %s seconds", migration.name, mt.elapsed
+                    )
             migration_state.applied = dt()
             self.set_state(migration_state)
             if migration.name == migration_name:
                 break
 
-    def downgrade(self, migration_name: Optional[str]):
+    def downgrade(self, migration_name: Optional[str] = None, fake: bool = False):
         """
         Reverse migrations.
 
         :param migration_name:
             name of migration down to which (excluding) downgrades should be executed
             None if all migrations should be run
+        :param fake:
+            If True, only migration state in database will be modified and
+            no actual migration will be run.
         """
         self._check_for_migration(migration_name)
         for migration in reversed(list(self.get_migrations())):
             if migration.name == migration_name:
                 break
             migration_state = self.get_state(migration)
             if not migration_state.applied:
-                LOGGER.debug("Migration %r not yet applied, skipping")
+                self.logger.debug(
+                    "Migration %r not yet applied, skipping", migration.name
+                )
                 continue
-            LOGGER.info("Running downgrade migration %r", migration.name)
-            migration.downgrade(self.db)
+            if fake:
+                self.logger.info("Fake running downgrade migration %r", migration.name)
+            else:
+                self.logger.info("Running downgrade migration %r", migration.name)
+                with _MeasureTime() as mt:
+                    migration.downgrade(self.db)
+                    self.logger.info(
+                        "Execution time of %r: %s seconds", migration.name, mt.elapsed
+                    )
             migration_state.applied = None
             self.set_state(migration_state)
 
-    def generate(self, name: str = "", **kwargs):
+    def generate(self, name: str = "", **kwargs) -> Path:
         last_migration_name = None
         for migration in self.get_migrations():
             last_migration_name = migration.name
         self.migrations_path.mkdir(exist_ok=True)
         dependencies = [last_migration_name] if last_migration_name else []
-        generate_migration_module_in_dir(
+        return generate_migration_module_in_dir(
             self.migrations_path,
             name=name,
             dependencies=dependencies,
             **{k: v for k, v in kwargs.items() if v is not None},
         )
```

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/cli.py` & `pymongo-migrate-1.0.0/tests/test_mongo_migrate_generate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,114 +1,86 @@
-from functools import wraps
-from typing import Optional
+import freezegun
+import pymongo
+import pytest
+from pymongo_migrate.mongo_migrate import MongoMigrate
 
-import click
 
-from pymongo_migrate.graph_draw import dump
-from pymongo_migrate.mongo_migrate import MongoMigrate
+@freezegun.freeze_time("2019-02-25 01:13:56")
+def test_generate(mongo_migrate, tmp_path):
+    tmp_migrations_path = tmp_path / "test_generate_migrations"
+    mongo_migrate.migrations_dir = str(tmp_migrations_path)
+    filename = mongo_migrate.generate().name
+    assert filename == "20190225011356.py"
+    files = {f.name: f for f in tmp_migrations_path.iterdir()}
+    assert set(files) == {filename}
+    with files[filename].open() as f:
+        content = f.read()
+        assert (
+            content
+            == '''\
+"""
+Migration description here!
+"""
+import pymongo
 
+name = '20190225011356'
+dependencies = ['20181123000000_gt_500']
 
-@click.group()
-def cli():
+
+def upgrade(db: "pymongo.database.Database"):
     pass
 
 
-def mongo_migrate_decor(f):
-    @wraps(f)
-    def wrap_with_client(uri, migrations, collection, *args, **kwargs):
-        mongo_migrate = MongoMigrate(
-            mongo_uri=uri, migrations_dir=migrations, migrations_collection=collection
+def downgrade(db: "pymongo.database.Database"):
+    pass
+'''
         )
-        return f(mongo_migrate, *args, **kwargs)
 
-    return wrap_with_client
 
+@pytest.fixture
+def empty_migrations_dir(tmp_path):
+    yield tmp_path / "migrations"
 
-def mongo_migration_options(f):
-    decorators = [
-        click.option(
-            "-u",
-            "--uri",
-            default=None,
-            envvar="PYMONGO_MIGRATE_URI",
-            help="mongodb URI",
-        ),
-        click.option(
-            "-m",
-            "--migrations",
-            default=MongoMigrate.migrations_dir,
-            envvar="PYMONGO_MIGRATE_MIGRATIONS",
-            help="migration script directory",
-            show_default=True,
-        ),
-        click.option(
-            "-c",
-            "--collection",
-            default=MongoMigrate.migrations_collection,
-            envvar="PYMONGO_MIGRATE_COLLECTION",
-            help="mongodb collection used for storing migration states",
-            show_default=True,
-        ),
-        mongo_migrate_decor,
-    ]
-    for decorator in reversed(decorators):
-        f = decorator(f)
-    return f
-
-
-@cli.command(short_help="show migrations and their status")
-@mongo_migration_options
-def show(mongo_migrate):
-    name_len_max = max(
-        (len(migration.name) for migration in mongo_migrate.get_migrations()), default=0
+
+@pytest.fixture
+def mongo_migrate_with_empty_dir(db_uri, db_name, db, empty_migrations_dir):
+    mm = MongoMigrate(
+        pymongo.MongoClient(db_uri), db_name, migrations_dir=str(empty_migrations_dir)
     )
+    yield mm
+    mm.client.close()
+
+
+@freezegun.freeze_time("2019-02-03 04:05:06")
+def test_generate_initial_migration(mongo_migrate_with_empty_dir, empty_migrations_dir):
+    mongo_migrate = mongo_migrate_with_empty_dir
+    filename = mongo_migrate.generate().name
+    assert filename == "20190203040506.py"
+    files = {f.name: f for f in empty_migrations_dir.iterdir()}
+    assert set(files) == {filename}
+    with files[filename].open() as f:
+        content = f.read()
+        assert (
+            content
+            == '''\
+"""
+Migration description here!
+"""
+import pymongo
 
-    migration_column_name = "Migration name".ljust(name_len_max)
-    click.secho(f"{migration_column_name}\tApplied timestamp", fg="yellow")
-    for migration in mongo_migrate.get_migrations():
-        migration_state = mongo_migrate.get_state(migration)
-        if migration_state.applied:
-            applied_text = click.style(migration_state.applied.isoformat(), fg="green")
-        else:
-            applied_text = click.style("Not applied", fg="red")
-        click.echo(f"{migration.name.ljust(name_len_max)}\t" + applied_text)
-
-
-@cli.command(
-    short_help="automagically apply necessary upgrades or downgrades to reach target migration"
-)
-@mongo_migration_options
-@click.argument("migration", required=False)
-def migrate(mongo_migrate, migration=None):
-    mongo_migrate.migrate(migration)
-
-
-@cli.command(short_help="apply necessary upgrades to reach target migration")
-@mongo_migration_options
-@click.argument("migration", required=False)
-def upgrade(mongo_migrate, migration=None):
-    mongo_migrate.upgrade(migration)
-
-
-@cli.command(short_help="apply necessary downgrades to reach target migration")
-@mongo_migration_options
-@click.argument("migration")
-def downgrade(mongo_migrate, migration):
-    mongo_migrate.downgrade(migration)
-
-
-@cli.command()
-@mongo_migration_options
-@click.argument("name", required=False)
-def generate(mongo_migrate, name: Optional[str] = None):
-    mongo_migrate.generate(name)
-
-
-@cli.command()
-@mongo_migration_options
-def graph(mongo_migrate):
-    stdout = click.get_text_stream("stdout")
-    dump(mongo_migrate.graph, stdout)
+name = '20190203040506'
+dependencies = []
+
+
+def upgrade(db: "pymongo.database.Database"):
+    pass
+
+
+def downgrade(db: "pymongo.database.Database"):
+    pass
+'''
+        )
 
 
-if __name__ == "__main__":
-    cli()
+def test_generate_should_fail_when_name_collides(mongo_migrate):
+    with pytest.raises(FileExistsError):
+        mongo_migrate.generate("20181123000000_gt_500")
```

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/migrations.py` & `pymongo-migrate-1.0.0/src/pymongo_migrate/migrations.py`

 * *Files identical despite different names*

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/loader.py` & `pymongo-migrate-1.0.0/src/pymongo_migrate/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import importlib.util
 from pathlib import Path
-from typing import Generator
+from typing import Generator, cast
 
-from pymongo_migrate.migrations import MigrationModuleWrapper
+from pymongo_migrate.migrations import MigrationModuleType, MigrationModuleWrapper
 
 
 def load_module_migrations(
     path: Path, namespace=f"{__name__}._migrations"
 ) -> Generator[MigrationModuleWrapper, None, None]:
-
     for module_file in path.glob("*.py"):
         if module_file.name.startswith("__"):
             continue
         migration_name = module_file.stem
         spec = importlib.util.spec_from_file_location(
             f"{namespace}.{migration_name}", str(module_file)
         )
+        assert spec
         migration_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(migration_module)  # type: ignore
-        yield MigrationModuleWrapper(  # type: ignore
-            name=migration_name, module=migration_module
+        yield MigrationModuleWrapper(
+            name=migration_name, module=cast(MigrationModuleType, migration_module)
         )
```

### Comparing `pymongo-migrate-0.9.1/src/pymongo_migrate/graph_draw.py` & `pymongo-migrate-1.0.0/src/pymongo_migrate/graph_draw.py`

 * *Files identical despite different names*

### Comparing `pymongo-migrate-0.9.1/README.md` & `pymongo-migrate-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,32 +33,31 @@
 
 Use `pymongo-migrate command --help` to learn more about particular command.
 
 ## Development & contributing to the project
 
 Contributions and raising Issues is welcome; standard netiquette rules apply.
 
-Use `pipenv install --dev` to setup the project for development.
+Use `make init` to setup the project for development.
 To format your code & test your changes run:
 
     make check
 
 ## Alternatives
 
 ATM there seem only two active python projects like this:
  * https://github.com/DoubleCiti/mongodb-migrations
  * https://github.com/skynyrd/cikilop
- 
+
 So if something already existed, why then another project?
 
-Goals of this project, where at least one of them were not fullfilled by above:
+Goals of this project, where at least one of them were not fulfilled by above:
  * tests and CI pipeline for ensuring that tool indeed works
  * keeping it usable both as standalone tool and as python dependency
- * use of modern Python version (3.6 and above)
-   * which allows use of type annotations, dataclasses, f-strings and other goodies
+ * use of modern Python version, which allows use of type annotations, dataclasses, f-strings and other goodies
 
 ## Inspiration and design
 
 Other than Alternatives mentioned above, both `alembic` and `django` were used as references when designing this tool.
 
 For now only linear revision history is supported.
 The support for squash migrations is planned.
```

