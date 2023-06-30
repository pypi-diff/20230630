# Comparing `tmp/sql_deta-0.0.8a3-py3-none-any.whl.zip` & `tmp/sql_deta-0.0.8a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 3875 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       79 b- defN 23-Jun-30 13:03 sql_deta/__init__.py
+Zip file size: 15876 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       79 b- defN 23-Jun-30 13:10 sql_deta/__init__.py
 -rw-rw-rw-  2.0 fat     6017 b- defN 23-Jun-30 08:38 sql_deta/peewee.py
--rw-rw-rw-  2.0 fat     1797 b- defN 23-Jun-30 13:03 sql_deta-0.0.8a3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 13:03 sql_deta-0.0.8a3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-30 13:03 sql_deta-0.0.8a3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      459 b- defN 23-Jun-30 13:03 sql_deta-0.0.8a3.dist-info/RECORD
-6 files, 8453 bytes uncompressed, 3041 bytes compressed:  64.0%
+-rw-rw-rw-  2.0 fat    34523 b- defN 23-Jun-30 13:12 sql_deta-0.0.8a4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1915 b- defN 23-Jun-30 13:12 sql_deta-0.0.8a4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 13:12 sql_deta-0.0.8a4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-30 13:12 sql_deta-0.0.8a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      551 b- defN 23-Jun-30 13:12 sql_deta-0.0.8a4.dist-info/RECORD
+7 files, 43186 bytes uncompressed, 14898 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: sql_deta/__init__.py
 Comment: 
 
 Filename: sql_deta/peewee.py
 Comment: 
 
-Filename: sql_deta-0.0.8a3.dist-info/METADATA
+Filename: sql_deta-0.0.8a4.dist-info/LICENSE
 Comment: 
 
-Filename: sql_deta-0.0.8a3.dist-info/WHEEL
+Filename: sql_deta-0.0.8a4.dist-info/METADATA
 Comment: 
 
-Filename: sql_deta-0.0.8a3.dist-info/top_level.txt
+Filename: sql_deta-0.0.8a4.dist-info/WHEEL
 Comment: 
 
-Filename: sql_deta-0.0.8a3.dist-info/RECORD
+Filename: sql_deta-0.0.8a4.dist-info/top_level.txt
+Comment: 
+
+Filename: sql_deta-0.0.8a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sql_deta/__init__.py

```diff
@@ -1,5 +1,5 @@
 """
 """
-__version__ = "0.0.8-alpha3"
+__version__ = "0.0.8-alpha4"
 
 from .peewee import PeeweeDetaMixin
```

## Comparing `sql_deta-0.0.8a3.dist-info/METADATA` & `sql_deta-0.0.8a4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sql-deta
-Version: 0.0.8a3
+Version: 0.0.8a4
 Summary: Detabase <--> SQL proxy
 Author: d;)
 License: GLWTPL
 Keywords: deta,detabase,sql,mixin,peewee
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: Freeware
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: deta
 Requires-Dist: odetam
 
 
 # Attention! not for production
 ## sql deta
 
@@ -52,9 +53,10 @@
 * It's opensource and free software, see the [LICENSE](LICENSE) for more details
 
 ## similar projects
 * [ssqlite3](https://github.com/jnsougata/space-sqlite3/) store binary `datafile.sqlite3` in DetaBase tables
 * [ODetaM](https://github.com/rickh94/ODetaM/) Object Document Mapper for DetaBase based on pydantic
 * [detadantic](https://github.com/Jay184/detadantic/) Active-Record style wrappers to Deta Base
 * [deta-base-pydantic](https://github.com/papalotis/deta-base-pydantic/) 
+* [csv-deta](https://pypi.org/project/csv-deta/)  
 
 ## TODO
```

