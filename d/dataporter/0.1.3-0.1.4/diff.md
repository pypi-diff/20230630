# Comparing `tmp/dataporter-0.1.3.tar.gz` & `tmp/dataporter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataporter-0.1.3.tar", max compression
+gzip compressed data, was "dataporter-0.1.4.tar", max compression
```

## Comparing `dataporter-0.1.3.tar` & `dataporter-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.3/README.md
--rw-r--r--   0        0        0      177 2023-06-14 11:19:16.055673 dataporter-0.1.3/dataporter/__init__.py
--rw-r--r--   0        0        0     6360 2023-06-14 10:55:40.759968 dataporter-0.1.3/dataporter/csv2sql.py
--rw-r--r--   0        0        0     3532 2023-06-14 08:14:15.148442 dataporter-0.1.3/dataporter/sql2csv.py
--rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.3/dataporter/sql_schema2txt.py
--rw-r--r--   0        0        0      502 2023-06-14 11:20:23.374180 dataporter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 dataporter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-06-14 10:59:50.072481 dataporter-0.1.4/README.md
+-rw-r--r--   0        0        0      177 2023-06-14 11:19:16.055673 dataporter-0.1.4/dataporter/__init__.py
+-rw-r--r--   0        0        0     6351 2023-06-30 11:00:53.891585 dataporter-0.1.4/dataporter/csv2sql.py
+-rw-r--r--   0        0        0     3582 2023-06-14 13:44:28.242148 dataporter-0.1.4/dataporter/sql2csv.py
+-rw-r--r--   0        0        0     1828 2023-06-14 11:17:06.906524 dataporter-0.1.4/dataporter/sql_schema2txt.py
+-rw-r--r--   0        0        0      502 2023-06-30 12:13:53.746523 dataporter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 dataporter-0.1.4/PKG-INFO
```

### Comparing `dataporter-0.1.3/dataporter/csv2sql.py` & `dataporter-0.1.4/dataporter/csv2sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     :param quotechar: quote char, '"' default.
     :param escapechar: escape char, None default.
     :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
     :param sql_data_exists: action on data exist in sql db, can be 'fail' or 'replace' or 'append', default 'fail'.
     :param sql_schema_file: schema on create table, default None (auto generate with no index).
     :param read_chunk_line: if csv file is large, to reduce the memory usage, read csv to memory by trunk of lines.
-    :param pandas_exprs: exec multiple pandas expr in order.
+    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['expr1 xxxxx','expr2 xxx']".
     :param debug: if debug mod on, will print every result after exec pandas exprs.
     :param ignore_error: if ignore sql insert error, it may cause loss chunks of data.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
 
     Session = sessionmaker(engine)
     # handle sql schema
@@ -78,17 +78,16 @@
             sql_data_exists = "append"
     elif sql_schema_file:
         with open(sql_schema_file) as f:
             schema = f.read()
 
         with Session() as session:
             try:
-                create_res = session.execute(text(schema))
+                session.execute(text(schema))
                 logger.info("creating table according to schema(if not exist)...")
-                logger.info(create_res.all())
             except exc.OperationalError as e:
                 if e.orig.args[0] == 1050:
                     logger.info("table already exist.")
                 else:
                     raise e
 
     if read_chunk_size is None:
```

### Comparing `dataporter-0.1.3/dataporter/sql2csv.py` & `dataporter-0.1.4/dataporter/sql2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     :param header: if contains header in result.
     :param sep: sep symbol, ',' default.
     :param quotechar: quote char, '"' default.
     :param escapechar: escape char, None default.
     :param lineterminator: line terminator, related to system ('\\n' for linux, '\\r\\n' for Windows, i.e.).
     :param read_chunk_size: if sql table is large, to reduce the memory usage, read sql to memory by trunk of lines, then write to local csv.
     :param sql_kwargs: other kwargs for sql, it will be pass to sqlalchemy 'create_engine' function.
-    :param pandas_exprs: exec multiple pandas expr in order.
+    :param pandas_exprs: exec multiple pandas expr in order, e.g.--pandas_exprs="['expr1 xxxxx','expr2 xxx']".
     :param debug: if debug mod on, will print every result after exec pandas exprs.
     """
     engine = create_engine(url=sql_uri, **sql_kwargs)
     if read_chunk_size is None:
         with engine.begin() as conn:
             df = pd.read_sql(sql, conn)
         if pandas_exprs:
```

### Comparing `dataporter-0.1.3/dataporter/sql_schema2txt.py` & `dataporter-0.1.4/dataporter/sql_schema2txt.py`

 * *Files identical despite different names*

### Comparing `dataporter-0.1.3/PKG-INFO` & `dataporter-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataporter
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: AuthorPlaceholder
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=40.0.2,<41.0.0)
```

