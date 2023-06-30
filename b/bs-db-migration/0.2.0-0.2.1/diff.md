# Comparing `tmp/bs_db_migration-0.2.0.tar.gz` & `tmp/bs_db_migration-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_db_migration-0.2.0.tar", last modified: Wed Jun 28 11:34:58 2023, max compression
+gzip compressed data, was "bs_db_migration-0.2.1.tar", last modified: Fri Jun 30 06:21:02 2023, max compression
```

## Comparing `bs_db_migration-0.2.0.tar` & `bs_db_migration-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.110407 bs_db_migration-0.2.0/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     1063 2023-02-03 01:32:29.000000 bs_db_migration-0.2.0/LICENSE
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      639 2023-06-28 11:34:58.110549 bs_db_migration-0.2.0/PKG-INFO
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     6745 2023-06-28 10:34:56.000000 bs_db_migration-0.2.0/README.md
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       79 2023-06-28 11:34:58.110897 bs_db_migration-0.2.0/setup.cfg
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     1128 2023-06-28 11:34:53.000000 bs_db_migration-0.2.0/setup.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.106619 bs_db_migration-0.2.0/src/
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.108400 bs_db_migration-0.2.0/src/bs_db_migration/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       63 2023-06-28 11:34:37.000000 bs_db_migration-0.2.0/src/bs_db_migration/__init__.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.109784 bs_db_migration-0.2.0/src/bs_db_migration/common/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:39.000000 bs_db_migration-0.2.0/src/bs_db_migration/common/__init__.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      382 2023-02-08 09:51:41.000000 bs_db_migration-0.2.0/src/bs_db_migration/common/debug.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     2262 2023-06-28 08:46:10.000000 bs_db_migration-0.2.0/src/bs_db_migration/config.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      240 2023-06-28 06:29:21.000000 bs_db_migration-0.2.0/src/bs_db_migration/domain_dictionary.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.110238 bs_db_migration-0.2.0/src/bs_db_migration/logger/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:31.000000 bs_db_migration-0.2.0/src/bs_db_migration/logger/__init__.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     2254 2023-02-08 09:51:41.000000 bs_db_migration-0.2.0/src/bs_db_migration/logger/logger.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)    22596 2023-06-28 10:04:25.000000 bs_db_migration-0.2.0/src/bs_db_migration/ms2postgres.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     3259 2023-06-28 08:46:05.000000 bs_db_migration-0.2.0/src/bs_db_migration/ms2postgres_type_mapping.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:34:58.109448 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      639 2023-06-28 11:34:58.000000 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/PKG-INFO
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      587 2023-06-28 11:34:58.000000 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/SOURCES.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        1 2023-06-28 11:34:58.000000 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/dependency_links.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       24 2023-06-28 11:34:58.000000 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/requires.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       16 2023-06-28 11:34:58.000000 bs_db_migration-0.2.0/src/bs_db_migration.egg-info/top_level.txt
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.136063 bs_db_migration-0.2.1/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     1063 2023-02-03 01:32:29.000000 bs_db_migration-0.2.1/LICENSE
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 06:21:02.136180 bs_db_migration-0.2.1/PKG-INFO
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     6868 2023-06-30 06:10:48.000000 bs_db_migration-0.2.1/README.md
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       79 2023-06-30 06:21:02.136549 bs_db_migration-0.2.1/setup.cfg
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     1128 2023-06-30 06:19:56.000000 bs_db_migration-0.2.1/setup.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.131380 bs_db_migration-0.2.1/src/
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.133998 bs_db_migration-0.2.1/src/bs_db_migration/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       63 2023-06-30 06:20:10.000000 bs_db_migration-0.2.1/src/bs_db_migration/__init__.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.135284 bs_db_migration-0.2.1/src/bs_db_migration/common/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:39.000000 bs_db_migration-0.2.1/src/bs_db_migration/common/__init__.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      382 2023-02-08 09:51:41.000000 bs_db_migration-0.2.1/src/bs_db_migration/common/debug.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     2290 2023-06-30 06:12:35.000000 bs_db_migration-0.2.1/src/bs_db_migration/config.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      240 2023-06-28 06:29:21.000000 bs_db_migration-0.2.1/src/bs_db_migration/domain_dictionary.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.135717 bs_db_migration-0.2.1/src/bs_db_migration/logger/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:31.000000 bs_db_migration-0.2.1/src/bs_db_migration/logger/__init__.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     2254 2023-02-08 09:51:41.000000 bs_db_migration-0.2.1/src/bs_db_migration/logger/logger.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)    22357 2023-06-30 06:19:21.000000 bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     3259 2023-06-28 08:46:05.000000 bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres_type_mapping.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.134921 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/PKG-INFO
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      587 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        1 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       24 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/requires.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       16 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/top_level.txt
```

### Comparing `bs_db_migration-0.2.0/LICENSE` & `bs_db_migration-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.0/PKG-INFO` & `bs_db_migration-0.2.1/src/bs_db_migration.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 1.1
-Name: bs_db_migration
-Version: 0.2.0
+Metadata-Version: 2.1
+Name: bs-db-migration
+Version: 0.2.1
 Summary: BS DB Migration
 Home-page: https://github.com/vincent841/ms2postgres.git
 Author: Jinwon Choi
 Author-email: jinwon@hatiolab.com
 License: MIT
-Description: BS DB Migration
 Keywords: database migration
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+BS DB Migration
```

### Comparing `bs_db_migration-0.2.0/README.md` & `bs_db_migration-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,36 @@
   use: false
   connection:
     host: localhost
     port: 5432
     id: postgres
     pw: password
     db: devmanager
-  migration_table: migration_info
-  migration_detail_table: migration_info_detail
 ```
 
 ## unit test
 
 ```bash
 cd src
 python3 -m unittest discover -s unit_test -p "*_test.py"
 ```
 
+## PyPL
+
+```bash
+# run once
+pip install --upgrade pip
+pip install twine
+
+# upload new version based on setup.py
+python setup.py install
+python setup.py sdist bdist_wheel
+python -m twine upload dist/*
+```
+
 ## API
 
 ### create_table_without_migration_info
 create a table in the target database(postgres) using the table information of the source database(mssql).
 
 ### migrate_table_without_migration_info
 copy all records of the myssql table into the postgres table but this api doesn't create a table in the target database(postgres).
```

### Comparing `bs_db_migration-0.2.0/setup.py` & `bs_db_migration-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """BS DB Migration"""
 
 INSTALL_REQUIRES = ["psycopg2", "pymssql", "pyyaml"]
 
 setup(
     name="bs_db_migration",
-    version="0.2.0",
+    version="0.2.1",
     author="Jinwon Choi",
     author_email="jinwon@hatiolab.com",
     url="https://github.com/vincent841/ms2postgres.git",
     install_requires=INSTALL_REQUIRES,
     packages=find_packages(
         where="src", include=["bs_db_migration", "bs_db_migration.*"]
     ),
@@ -26,12 +26,12 @@
         "database migration",
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration/config.py` & `bs_db_migration-0.2.1/src/bs_db_migration/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from enum import Enum
 
 
 class ConfigDBType(Enum):
     MSSQL = "mssql"
     POSTGRES = "postgres"
+    MIGRATION = "migration"
 
 
 class Configuration:
     CONFIG_DATA: dict = {}
 
     def __init__(self, config_yaml_file=None, config_data=None):
         Configuration.CONFIG_DATA: dict = {}
```

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration/logger/logger.py` & `bs_db_migration-0.2.1/src/bs_db_migration/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration/ms2postgres.py` & `bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,35 +51,33 @@
                 connection_info
             )
             self.postgres = pg2.connect(
                 user=id, password=pw, host=host, port=port, database=db
             )
 
             # TODO:
-            migration_info = self.configuration.migration_info()
+            migration_connection = self.configuration.db_info(ConfigDBType.MIGRATION)
             self.migraiton_table_list: list = []
-            self.migration_info_available = migration_info.get("use", False)
-            if self.migration_info_available:
-                migration_connection_info = migration_info["connection"]
-                (host, port, id, pw, db) = self.configuration.get_connection_info(
-                    migration_connection_info
-                )
-                self.mginfo = pg2.connect(
-                    user=id,
-                    password=pw,
-                    host=host,
-                    port=port,
-                    database=db,
-                )
 
-                with self.mginfo.cursor() as cursor:
-                    cursor.execute(
-                        f"SELECT id, type, source_table_name, target_table_name FROM migration_info;"
-                    )
-                    self.migraiton_table_list = cursor.fetchall()
+            (host, port, id, pw, db) = self.configuration.get_connection_info(
+                migration_connection
+            )
+            self.mginfo = pg2.connect(
+                user=id,
+                password=pw,
+                host=host,
+                port=port,
+                database=db,
+            )
+
+            with self.mginfo.cursor() as cursor:
+                cursor.execute(
+                    f"SELECT id, type, source_table_name, target_table_name FROM migration_info;"
+                )
+                self.migraiton_table_list = cursor.fetchall()
 
         except Exception as ex:
             log_error(f"Can't connect databases: {ex}")
             raise ex
 
     def close(self):
         self.mssql.close()
```

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration/ms2postgres_type_mapping.py` & `bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres_type_mapping.py`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration.egg-info/PKG-INFO` & `bs_db_migration-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 1.1
-Name: bs-db-migration
-Version: 0.2.0
+Metadata-Version: 2.1
+Name: bs_db_migration
+Version: 0.2.1
 Summary: BS DB Migration
 Home-page: https://github.com/vincent841/ms2postgres.git
 Author: Jinwon Choi
 Author-email: jinwon@hatiolab.com
 License: MIT
-Description: BS DB Migration
 Keywords: database migration
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
+BS DB Migration
```

### Comparing `bs_db_migration-0.2.0/src/bs_db_migration.egg-info/SOURCES.txt` & `bs_db_migration-0.2.1/src/bs_db_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

