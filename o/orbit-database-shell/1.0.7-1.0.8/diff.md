# Comparing `tmp/orbit_database_shell-1.0.7.tar.gz` & `tmp/orbit_database_shell-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database_shell-1.0.7.tar", max compression
+gzip compressed data, was "orbit_database_shell-1.0.8.tar", max compression
```

## Comparing `orbit_database_shell-1.0.7.tar` & `orbit_database_shell-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.7/LICENSE.md
--rw-r--r--   0        0        0     2272 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.7/README.md
--rwxr-xr-x   0        0        0        0 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.7/orbit_database_shell/__init__.py
--rwxr-xr-x   0        0        0     1887 2023-06-27 15:21:47.019586 orbit_database_shell-1.0.7/orbit_database_shell/__main__.py
--rwxr-xr-x   0        0        0    24838 2023-06-21 17:01:34.537701 orbit_database_shell-1.0.7/orbit_database_shell/odb_actions.py
--rwxr-xr-x   0        0        0     4169 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.7/orbit_database_shell/odb_completers.py
--rw-r--r--   0        0        0     1988 2023-06-23 14:54:20.350769 orbit_database_shell-1.0.7/orbit_database_shell/odb_decorators.py
--rwxr-xr-x   0        0        0     7071 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.7/orbit_database_shell/odb_grammar.py
--rwxr-xr-x   0        0        0    46376 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.7/orbit_database_shell/odb_help.py
--rw-r--r--   0        0        0     1313 2023-06-27 15:21:47.019586 orbit_database_shell-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 orbit_database_shell-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0     2272 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/orbit_database_shell/__init__.py
+-rwxr-xr-x   0        0        0     1887 2023-06-29 22:19:46.643208 orbit_database_shell-1.0.8/orbit_database_shell/__main__.py
+-rwxr-xr-x   0        0        0    24788 2023-06-28 13:28:56.984810 orbit_database_shell-1.0.8/orbit_database_shell/odb_actions.py
+-rwxr-xr-x   0        0        0     4169 2023-05-30 15:20:01.323993 orbit_database_shell-1.0.8/orbit_database_shell/odb_completers.py
+-rw-r--r--   0        0        0     1988 2023-06-23 14:54:20.350769 orbit_database_shell-1.0.8/orbit_database_shell/odb_decorators.py
+-rwxr-xr-x   0        0        0     7071 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.8/orbit_database_shell/odb_grammar.py
+-rwxr-xr-x   0        0        0    46376 2023-05-30 15:20:01.327993 orbit_database_shell-1.0.8/orbit_database_shell/odb_help.py
+-rw-r--r--   0        0        0     1313 2023-06-29 22:19:46.643208 orbit_database_shell-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 orbit_database_shell-1.0.8/PKG-INFO
```

### Comparing `orbit_database_shell-1.0.7/LICENSE.md` & `orbit_database_shell-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/README.md` & `orbit_database_shell-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/__main__.py` & `orbit_database_shell-1.0.8/orbit_database_shell/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from orbit_database_shell.odb_decorators import banner
 
 __author__ = 'Gareth Bult'
 __banner__ = 'Orbit-DB'
 __copyright__ = 'Copyright 2023, Mad Penguin Consulting Ltd'
 __credits__ = ['Gareth Bult']
 __license__ = 'MIT'
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 __maintainer__ = 'Gareth Bult'
 __email__ = 'gareth@madpenguin.uk'
 __status__ = 'Development'
 
 
 def main ():
     actions = Actions().notice(banner)
```

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/odb_actions.py` & `orbit_database_shell-1.0.8/orbit_database_shell/odb_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,17 +325,16 @@
     @selected
     def show_tables(self):
         """Display a list of tables available within this database"""
         tab = self.richTable(['Table name', '#Recs', 'Codec', 'Depth', 'Oflow%', 'Index names'])
         for name in self._db.tables(self._mode):
             table = self.get_table(name)
             try:
-                db = self._db.env.open_db(name.encode())
                 with self._db.env.begin() as txn:
-                    stat = txn.stat(db)
+                    stat = txn.stat(table._db)
                 leaf = int(stat['leaf_pages'])
                 indexes = ', '.join(table.indexes())
                 names, indexes = indexes[:60], indexes[60:]
                 codec = str(table._codec.value)
             except Exception as e:
                 self.error(str(e))
                 stat = {}
```

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/odb_completers.py` & `orbit_database_shell-1.0.8/orbit_database_shell/odb_completers.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/odb_decorators.py` & `orbit_database_shell-1.0.8/orbit_database_shell/odb_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/odb_grammar.py` & `orbit_database_shell-1.0.8/orbit_database_shell/odb_grammar.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/orbit_database_shell/odb_help.py` & `orbit_database_shell-1.0.8/orbit_database_shell/odb_help.py`

 * *Files identical despite different names*

### Comparing `orbit_database_shell-1.0.7/pyproject.toml` & `orbit_database_shell-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-database-shell"
-version = "1.0.7"
+version = "1.0.8"
 description = "Orbit-DB Shell"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `orbit_database_shell-1.0.7/PKG-INFO` & `orbit_database_shell-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-database-shell
-Version: 1.0.7
+Version: 1.0.8
 Summary: Orbit-DB Shell
 Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: orbit-database-shell Version: 1.0.7 Summary: Orbit-
+Metadata-Version: 2.1 Name: orbit-database-shell Version: 1.0.8 Summary: Orbit-
 DB Shell Home-page: https://gitlab.com/madpenguin/orbit-database-shell
 Keywords: database,shell Author: Gareth Bult Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console :: Curses Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

