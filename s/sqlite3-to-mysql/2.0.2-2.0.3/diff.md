# Comparing `tmp/sqlite3_to_mysql-2.0.2.tar.gz` & `tmp/sqlite3_to_mysql-2.0.3.tar.gz`

## Comparing `sqlite3_to_mysql-2.0.2.tar` & `sqlite3_to_mysql-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/requirements_dev.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/__init__.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/cli.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/py.typed
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/transporter.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/__init__.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/conftest.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/database.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/factories.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/__init__.py
--rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/unit/__init__.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/unit/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/LICENSE
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/README.md
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/requirements_dev.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    30781 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/database.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/factories.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/func/__init__.py
+-rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/README.md
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.3/PKG-INFO
```

### Comparing `sqlite3_to_mysql-2.0.2/CHANGELOG.md` & `sqlite3_to_mysql-2.0.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.0.3
+
+* [FIX] prevent AUTO_INCREMENT-ing fields from having a DEFAULT value
+
 # 2.0.2
 
 * [FIX] properly import CMySQLConnection
 
 # 2.0.1
 
 * [FIX] fix types
```

### Comparing `sqlite3_to_mysql-2.0.2/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.0.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/mysql_utils.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/transporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,23 +322,25 @@
 
             # The "hidden" value is 0 for visible columns, 1 for "hidden" columns,
             # 2 for computed virtual columns and 3 for computed stored columns.
             # Read more on hidden columns here https://www.sqlite.org/pragma.html#pragma_table_xinfo
             if "hidden" in column and column["hidden"] == 1:
                 continue
 
+            auto_increment: bool = (
+                column["pk"] > 0 and column_type.startswith(("INT", "BIGINT")) and not compound_primary_key
+            )
+
             sql += " `{name}` {type} {notnull} {default} {auto_increment}, ".format(
                 name=mysql_safe_name,
                 type=column_type,
                 notnull="NOT NULL" if column["notnull"] or column["pk"] else "NULL",
-                auto_increment="AUTO_INCREMENT"
-                if column["pk"] > 0 and column_type.startswith(("INT", "BIGINT")) and not compound_primary_key
-                else "",
+                auto_increment="AUTO_INCREMENT" if auto_increment else "",
                 default="DEFAULT " + column["dflt_value"]
-                if column["dflt_value"] and column_type not in MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT
+                if column["dflt_value"] and column_type not in MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT and not auto_increment
                 else "",
             )
 
             if column["pk"] > 0:
                 primary_key: t.Dict[str, str] = {
                     "column": mysql_safe_name,
                     "length": "",
```

### Comparing `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/types.py` & `sqlite3_to_mysql-2.0.3/sqlite3_to_mysql/types.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/conftest.py` & `sqlite3_to_mysql-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/database.py` & `sqlite3_to_mysql-2.0.3/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/factories.py` & `sqlite3_to_mysql-2.0.3/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/models.py` & `sqlite3_to_mysql-2.0.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/func/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.3/tests/func/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/func/test_cli.py` & `sqlite3_to_mysql-2.0.3/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.3/tests/unit/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/.gitignore` & `sqlite3_to_mysql-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/LICENSE` & `sqlite3_to_mysql-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/README.md` & `sqlite3_to_mysql-2.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 [![GitHub stars](https://img.shields.io/github/stars/techouse/sqlite3-to-mysql.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/sqlite3-to-mysql/stargazers)
 
 
 # SQLite3 to MySQL
 
 #### A simple Python tool to transfer data from SQLite 3 to MySQL.
 
-I originally wrote this simple program as a standalone script and published it
-as a [gist](https://gist.github.com/techouse/4deb94eee58a02d104c6) as an answer
-to this [Stack Overflow question](https://stackoverflow.com/questions/18671/quick-easy-way-to-migrate-sqlite3-to-mysql/32243979#32243979).
-Since then quite some people have taken interest in it since it's so simple and
-effective. Therefore I finally moved my lazy bones and made a GitHub repository :octopus:.
-
 ### How to run
 
 ```bash
 pip install sqlite3-to-mysql
 sqlite3mysql --help
 ```
```

### Comparing `sqlite3_to_mysql-2.0.2/pyproject.toml` & `sqlite3_to_mysql-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.2/PKG-INFO` & `sqlite3_to_mysql-2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 2.0.2
+Version: 2.0.3
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,20 +49,14 @@
 [![GitHub stars](https://img.shields.io/github/stars/techouse/sqlite3-to-mysql.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/sqlite3-to-mysql/stargazers)
 
 
 # SQLite3 to MySQL
 
 #### A simple Python tool to transfer data from SQLite 3 to MySQL.
 
-I originally wrote this simple program as a standalone script and published it
-as a [gist](https://gist.github.com/techouse/4deb94eee58a02d104c6) as an answer
-to this [Stack Overflow question](https://stackoverflow.com/questions/18671/quick-easy-way-to-migrate-sqlite3-to-mysql/32243979#32243979).
-Since then quite some people have taken interest in it since it's so simple and
-effective. Therefore I finally moved my lazy bones and made a GitHub repository :octopus:.
-
 ### How to run
 
 ```bash
 pip install sqlite3-to-mysql
 sqlite3mysql --help
 ```
```

