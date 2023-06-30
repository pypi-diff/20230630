# Comparing `tmp/bs_db_migration-0.2.1.tar.gz` & `tmp/bs_db_migration-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_db_migration-0.2.1.tar", last modified: Fri Jun 30 06:21:02 2023, max compression
+gzip compressed data, was "bs_db_migration-0.2.2.tar", last modified: Fri Jun 30 07:07:27 2023, max compression
```

## Comparing `bs_db_migration-0.2.1.tar` & `bs_db_migration-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.136063 bs_db_migration-0.2.1/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     1063 2023-02-03 01:32:29.000000 bs_db_migration-0.2.1/LICENSE
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 06:21:02.136180 bs_db_migration-0.2.1/PKG-INFO
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     6868 2023-06-30 06:10:48.000000 bs_db_migration-0.2.1/README.md
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       79 2023-06-30 06:21:02.136549 bs_db_migration-0.2.1/setup.cfg
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     1128 2023-06-30 06:19:56.000000 bs_db_migration-0.2.1/setup.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.131380 bs_db_migration-0.2.1/src/
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.133998 bs_db_migration-0.2.1/src/bs_db_migration/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       63 2023-06-30 06:20:10.000000 bs_db_migration-0.2.1/src/bs_db_migration/__init__.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.135284 bs_db_migration-0.2.1/src/bs_db_migration/common/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:39.000000 bs_db_migration-0.2.1/src/bs_db_migration/common/__init__.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      382 2023-02-08 09:51:41.000000 bs_db_migration-0.2.1/src/bs_db_migration/common/debug.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     2290 2023-06-30 06:12:35.000000 bs_db_migration-0.2.1/src/bs_db_migration/config.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      240 2023-06-28 06:29:21.000000 bs_db_migration-0.2.1/src/bs_db_migration/domain_dictionary.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.135717 bs_db_migration-0.2.1/src/bs_db_migration/logger/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:31.000000 bs_db_migration-0.2.1/src/bs_db_migration/logger/__init__.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     2254 2023-02-08 09:51:41.000000 bs_db_migration-0.2.1/src/bs_db_migration/logger/logger.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)    22357 2023-06-30 06:19:21.000000 bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres.py
--rw-r--r--   0 jinwonchoi   (501) staff       (20)     3259 2023-06-28 08:46:05.000000 bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres_type_mapping.py
-drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 06:21:02.134921 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/PKG-INFO
--rw-r--r--   0 jinwonchoi   (501) staff       (20)      587 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/SOURCES.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)        1 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/dependency_links.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       24 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/requires.txt
--rw-r--r--   0 jinwonchoi   (501) staff       (20)       16 2023-06-30 06:21:02.000000 bs_db_migration-0.2.1/src/bs_db_migration.egg-info/top_level.txt
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.606734 bs_db_migration-0.2.2/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     1063 2023-02-03 01:32:29.000000 bs_db_migration-0.2.2/LICENSE
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 07:07:27.606822 bs_db_migration-0.2.2/PKG-INFO
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     6868 2023-06-30 06:10:48.000000 bs_db_migration-0.2.2/README.md
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       79 2023-06-30 07:07:27.607310 bs_db_migration-0.2.2/setup.cfg
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     1128 2023-06-30 07:06:32.000000 bs_db_migration-0.2.2/setup.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.602554 bs_db_migration-0.2.2/src/
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.604880 bs_db_migration-0.2.2/src/bs_db_migration/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       63 2023-06-30 07:06:32.000000 bs_db_migration-0.2.2/src/bs_db_migration/__init__.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.606245 bs_db_migration-0.2.2/src/bs_db_migration/common/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:39.000000 bs_db_migration-0.2.2/src/bs_db_migration/common/__init__.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      382 2023-02-08 09:51:41.000000 bs_db_migration-0.2.2/src/bs_db_migration/common/debug.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     2290 2023-06-30 07:05:34.000000 bs_db_migration-0.2.2/src/bs_db_migration/config.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      240 2023-06-28 06:29:21.000000 bs_db_migration-0.2.2/src/bs_db_migration/domain_dictionary.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.606582 bs_db_migration-0.2.2/src/bs_db_migration/logger/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        0 2023-06-28 11:33:31.000000 bs_db_migration-0.2.2/src/bs_db_migration/logger/__init__.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     2254 2023-02-08 09:51:41.000000 bs_db_migration-0.2.2/src/bs_db_migration/logger/logger.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)    22357 2023-06-30 06:19:21.000000 bs_db_migration-0.2.2/src/bs_db_migration/ms2postgres.py
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)     3259 2023-06-28 08:46:05.000000 bs_db_migration-0.2.2/src/bs_db_migration/ms2postgres_type_mapping.py
+drwxr-xr-x   0 jinwonchoi   (501) staff       (20)        0 2023-06-30 07:07:27.605816 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      631 2023-06-30 07:07:27.000000 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/PKG-INFO
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)      587 2023-06-30 07:07:27.000000 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)        1 2023-06-30 07:07:27.000000 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       24 2023-06-30 07:07:27.000000 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/requires.txt
+-rw-r--r--   0 jinwonchoi   (501) staff       (20)       16 2023-06-30 07:07:27.000000 bs_db_migration-0.2.2/src/bs_db_migration.egg-info/top_level.txt
```

### Comparing `bs_db_migration-0.2.1/LICENSE` & `bs_db_migration-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.1/PKG-INFO` & `bs_db_migration-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs_db_migration
-Version: 0.2.1
+Version: 0.2.2
 Summary: BS DB Migration
 Home-page: https://github.com/vincent841/ms2postgres.git
 Author: Jinwon Choi
 Author-email: jinwon@hatiolab.com
 License: MIT
 Keywords: database migration
 Classifier: Intended Audience :: Developers
```

### Comparing `bs_db_migration-0.2.1/README.md` & `bs_db_migration-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.1/setup.py` & `bs_db_migration-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """BS DB Migration"""
 
 INSTALL_REQUIRES = ["psycopg2", "pymssql", "pyyaml"]
 
 setup(
     name="bs_db_migration",
-    version="0.2.1",
+    version="0.2.2",
     author="Jinwon Choi",
     author_email="jinwon@hatiolab.com",
     url="https://github.com/vincent841/ms2postgres.git",
     install_requires=INSTALL_REQUIRES,
     packages=find_packages(
         where="src", include=["bs_db_migration", "bs_db_migration.*"]
     ),
```

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration/config.py` & `bs_db_migration-0.2.2/src/bs_db_migration/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     @classmethod
     def get(cls, key):
         return cls.CONFIG_DATA.get(key, None)
 
     @classmethod
     def db_info(cls, db_type: ConfigDBType):
         try:
-            config_data = cls.CONFIG_DATA.get("db_connection").get(db_type.value, None)
+            config_data = cls.CONFIG_DATA.get("db-connection").get(db_type.value, None)
         except Exception as ex:
             log_error(f"invalid configuration: \n{ex}")
             config_data = None
 
         return config_data if config_data != None else None
 
     @classmethod
```

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration/logger/logger.py` & `bs_db_migration-0.2.2/src/bs_db_migration/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres.py` & `bs_db_migration-0.2.2/src/bs_db_migration/ms2postgres.py`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration/ms2postgres_type_mapping.py` & `bs_db_migration-0.2.2/src/bs_db_migration/ms2postgres_type_mapping.py`

 * *Files identical despite different names*

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration.egg-info/PKG-INFO` & `bs_db_migration-0.2.2/src/bs_db_migration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-db-migration
-Version: 0.2.1
+Version: 0.2.2
 Summary: BS DB Migration
 Home-page: https://github.com/vincent841/ms2postgres.git
 Author: Jinwon Choi
 Author-email: jinwon@hatiolab.com
 License: MIT
 Keywords: database migration
 Classifier: Intended Audience :: Developers
```

### Comparing `bs_db_migration-0.2.1/src/bs_db_migration.egg-info/SOURCES.txt` & `bs_db_migration-0.2.2/src/bs_db_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

