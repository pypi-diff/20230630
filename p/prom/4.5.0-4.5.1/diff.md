# Comparing `tmp/prom-4.5.0.tar.gz` & `tmp/prom-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prom-4.5.0.tar", last modified: Thu Jun 29 22:43:01 2023, max compression
+gzip compressed data, was "prom-4.5.1.tar", last modified: Fri Jun 30 00:00:29 2023, max compression
```

## Comparing `prom-4.5.0.tar` & `prom-4.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645992 prom-4.5.0/
--rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.5.0/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-29 22:43:01.645854 prom-4.5.0/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.5.0/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.643496 prom-4.5.0/prom/
--rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-06-29 22:42:57.000000 prom-4.5.0/prom/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.5.0/prom/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)    50364 2023-06-29 22:42:57.000000 prom-4.5.0/prom/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.5.0/prom/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.644677 prom-4.5.0/prom/extras/
--rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.5.0/prom/extras/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.5.0/prom/extras/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.5.0/prom/extras/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    25477 2023-06-29 22:42:57.000000 prom-4.5.0/prom/extras/testdata.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645172 prom-4.5.0/prom/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.5.0/prom/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.5.0/prom/interface/base.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645456 prom-4.5.0/prom/interface/postgres/
--rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.5.0/prom/interface/postgres/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.5.0/prom/interface/postgres/gevent.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35163 2023-06-29 22:42:57.000000 prom-4.5.0/prom/interface/sql.py
--rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-06-27 20:25:40.000000 prom-4.5.0/prom/interface/sqlite.py
--rw-r--r--   0 jaymon     (501) staff       (20)    24278 2023-06-29 22:42:57.000000 prom-4.5.0/prom/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35676 2023-06-29 22:42:57.000000 prom-4.5.0/prom/query.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.5.0/prom/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.644251 prom-4.5.0/prom.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-29 22:43:01.646031 prom-4.5.0/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.5.0/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.424041 prom-4.5.1/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.5.1/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-30 00:00:29.423909 prom-4.5.1/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.5.1/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.421858 prom-4.5.1/prom/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-06-29 23:59:06.000000 prom-4.5.1/prom/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.5.1/prom/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    50364 2023-06-29 23:48:39.000000 prom-4.5.1/prom/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.5.1/prom/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.422798 prom-4.5.1/prom/extras/
+-rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.5.1/prom/extras/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.5.1/prom/extras/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.5.1/prom/extras/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    25477 2023-06-29 22:42:57.000000 prom-4.5.1/prom/extras/testdata.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.423298 prom-4.5.1/prom/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.5.1/prom/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.5.1/prom/interface/base.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.423545 prom-4.5.1/prom/interface/postgres/
+-rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.5.1/prom/interface/postgres/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.5.1/prom/interface/postgres/gevent.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35163 2023-06-29 22:42:57.000000 prom-4.5.1/prom/interface/sql.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-06-27 20:25:40.000000 prom-4.5.1/prom/interface/sqlite.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    24442 2023-06-29 23:58:07.000000 prom-4.5.1/prom/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35676 2023-06-29 22:42:57.000000 prom-4.5.1/prom/query.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.5.1/prom/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.422391 prom-4.5.1/prom.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-30 00:00:29.424081 prom-4.5.1/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.5.1/setup.py
```

### Comparing `prom-4.5.0/LICENSE.txt` & `prom-4.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/PKG-INFO` & `prom-4.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.5.0
+Version: 4.5.1
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.5.0/README.md` & `prom-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/__init__.py` & `prom-4.5.1/prom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     UniqueError,
     CloseError,
 )
 
 from . import utils
 
 
-__version__ = '4.5.0'
+__version__ = '4.5.1'
 
 
 def transaction(connection_name="", **kwargs):
     """Create a transaction 
 
     Sometimes you just need to batch a whole bunch of operation across a whole bunch
     of different models, this allows you to create a transaction outside of any
```

### Comparing `prom-4.5.0/prom/config.py` & `prom-4.5.1/prom/config.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/exception.py` & `prom-4.5.1/prom/exception.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/extras/config.py` & `prom-4.5.1/prom/extras/config.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/extras/model.py` & `prom-4.5.1/prom/extras/model.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/extras/testdata.py` & `prom-4.5.1/prom/extras/testdata.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/__init__.py` & `prom-4.5.1/prom/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/base.py` & `prom-4.5.1/prom/interface/base.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/postgres/__init__.py` & `prom-4.5.1/prom/interface/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/postgres/gevent.py` & `prom-4.5.1/prom/interface/postgres/gevent.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/sql.py` & `prom-4.5.1/prom/interface/sql.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/interface/sqlite.py` & `prom-4.5.1/prom/interface/sqlite.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/model.py` & `prom-4.5.1/prom/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,38 +429,42 @@
         those fields as the conflict fields, it will raise a ValueError if it can't
         find a valid set of conflict fields
 
         :param **kwargs: passed through to the interface
         """
         ret = True
 
-        schema = self.schema
-        fields = self.to_interface()
+        if pk := self._interface_pk:
+            ret = self.update()
 
-        conflict_fields = self.conflict_fields(fields)
-        if not conflict_fields:
-            raise ValueError(
-                "{}.upsert() failed to find conflict field names from: {}".format(
-                    self.__class__.__name__,
-                    list(fields.keys())
+        else:
+            schema = self.schema
+            fields = self.to_interface()
+
+            conflict_fields = self.conflict_fields(fields)
+            if not conflict_fields:
+                raise ValueError(
+                    "{}.upsert() failed to find conflict field names from: {}".format(
+                        self.__class__.__name__,
+                        list(fields.keys())
+                    )
                 )
-            )
 
-        q = self.query
-        q.set(fields)
-        pk = q.upsert([t[0] for t in conflict_fields], **kwargs)
-        if pk:
-            fields = q.fields_set.fields
-            pk_name = schema.pk_name
-            if pk_name:
-                fields[pk_name] = pk
+            q = self.query
+            q.set(fields)
+            pk = q.upsert([t[0] for t in conflict_fields], **kwargs)
+            if pk:
+                fields = q.fields_set.fields
+                pk_name = schema.pk_name
+                if pk_name:
+                    fields[pk_name] = pk
                 self.from_interface(fields)
 
-        else:
-            ret = False
+            else:
+                ret = False
 
         return ret
 
     def save(self, **kwargs):
         """
         persist the fields in this object into the db, this will update if _id is set, otherwise
         it will insert
```

### Comparing `prom-4.5.0/prom/query.py` & `prom-4.5.1/prom/query.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom/utils.py` & `prom-4.5.1/prom/utils.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/prom.egg-info/PKG-INFO` & `prom-4.5.1/prom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.5.0
+Version: 4.5.1
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.5.0/prom.egg-info/SOURCES.txt` & `prom-4.5.1/prom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prom-4.5.0/setup.py` & `prom-4.5.1/setup.py`

 * *Files identical despite different names*

