# Comparing `tmp/pantherdb-1.2.2.tar.gz` & `tmp/pantherdb-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantherdb-1.2.2.tar", last modified: Sat Mar 18 19:03:24 2023, max compression
+gzip compressed data, was "pantherdb-1.2.3.tar", last modified: Fri Jun 30 09:28:09 2023, max compression
```

## Comparing `pantherdb-1.2.2.tar` & `pantherdb-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:03:24.170753 pantherdb-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-03-18 19:03:24.170753 pantherdb-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-18 19:03:07.000000 pantherdb-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:03:24.170753 pantherdb-1.2.2/pantherdb/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-18 19:03:07.000000 pantherdb-1.2.2/pantherdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-03-18 19:03:07.000000 pantherdb-1.2.2/pantherdb/pantherdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 19:03:24.170753 pantherdb-1.2.2/pantherdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-03-18 19:03:24.000000 pantherdb-1.2.2/pantherdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-18 19:03:24.000000 pantherdb-1.2.2/pantherdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 19:03:24.000000 pantherdb-1.2.2/pantherdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-18 19:03:24.000000 pantherdb-1.2.2/pantherdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-18 19:03:24.000000 pantherdb-1.2.2/pantherdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 19:03:24.170753 pantherdb-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-18 19:03:07.000000 pantherdb-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.869982 pantherdb-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 09:28:09.869982 pantherdb-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-30 09:27:54.000000 pantherdb-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.865982 pantherdb-1.2.3/pantherdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 09:27:54.000000 pantherdb-1.2.3/pantherdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-30 09:27:54.000000 pantherdb-1.2.3/pantherdb/pantherdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:28:09.869982 pantherdb-1.2.3/pantherdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:28:09.000000 pantherdb-1.2.3/pantherdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:28:09.869982 pantherdb-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-30 09:27:54.000000 pantherdb-1.2.3/setup.py
```

### Comparing `pantherdb-1.2.2/PKG-INFO` & `pantherdb-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.2
+Version: 1.2.3
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 ## Introduction
 
-PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use it in your projects.
+PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
 - Written in pure Python +3.11 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
     ```python
-    db: PantherDB = PantherDB('database.pantherdb')
+    db: PantherDB = PantherDB('database.pdb')
     ```
   
 - #### Create an encrypted database:
     ```python
     from cryptography.fernet import Fernet
     key = Fernet.generate_key()  # Should be static (You should not generate new key on every run)
-    db: PantherDB = PantherDB('database.pantherdb', secret_key=key)
+    db: PantherDB = PantherDB('database.pdb', secret_key=key)
     ```
 
 - #### Access to a collection:
     ```python
     user_collection: PantherCollection = db.collection('User')
     ```
```

### Comparing `pantherdb-1.2.2/README.md` & `pantherdb-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ## Introduction
 
-PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use it in your projects.
+PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
 - Written in pure Python +3.11 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
     ```python
-    db: PantherDB = PantherDB('database.pantherdb')
+    db: PantherDB = PantherDB('database.pdb')
     ```
   
 - #### Create an encrypted database:
     ```python
     from cryptography.fernet import Fernet
     key = Fernet.generate_key()  # Should be static (You should not generate new key on every run)
-    db: PantherDB = PantherDB('database.pantherdb', secret_key=key)
+    db: PantherDB = PantherDB('database.pdb', secret_key=key)
     ```
 
 - #### Access to a collection:
     ```python
     user_collection: PantherCollection = db.collection('User')
     ```
```

### Comparing `pantherdb-1.2.2/pantherdb/pantherdb.py` & `pantherdb-1.2.3/pantherdb/pantherdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class PantherDBException(Exception):
     pass
 
 
 class PantherDB:
-    db_name: str = 'database.pantherdb'
+    db_name: str = 'database.pdb'
     __secret_key: bytes | None
     __fernet: Fernet | None
     __return_dict: bool
     __content: dict
 
     def __init__(self, db_name: str | None = None, return_dict: bool = False, secret_key: bytes | None = None):
         self.__return_dict = return_dict
```

### Comparing `pantherdb-1.2.2/pantherdb.egg-info/PKG-INFO` & `pantherdb-1.2.3/pantherdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.2
+Version: 1.2.3
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 ## Introduction
 
-PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use it in your projects.
+PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
 - Written in pure Python +3.11 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
     ```python
-    db: PantherDB = PantherDB('database.pantherdb')
+    db: PantherDB = PantherDB('database.pdb')
     ```
   
 - #### Create an encrypted database:
     ```python
     from cryptography.fernet import Fernet
     key = Fernet.generate_key()  # Should be static (You should not generate new key on every run)
-    db: PantherDB = PantherDB('database.pantherdb', secret_key=key)
+    db: PantherDB = PantherDB('database.pdb', secret_key=key)
     ```
 
 - #### Access to a collection:
     ```python
     user_collection: PantherCollection = db.collection('User')
     ```
```

### Comparing `pantherdb-1.2.2/setup.py` & `pantherdb-1.2.3/setup.py`

 * *Files identical despite different names*

