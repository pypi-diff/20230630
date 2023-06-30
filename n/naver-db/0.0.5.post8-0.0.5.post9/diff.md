# Comparing `tmp/naver-db-0.0.5.post8.tar.gz` & `tmp/naver-db-0.0.5.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver-db-0.0.5.post8.tar", last modified: Fri Jun 30 01:59:45 2023, max compression
+gzip compressed data, was "naver-db-0.0.5.post9.tar", last modified: Fri Jun 30 02:15:20 2023, max compression
```

## Comparing `naver-db-0.0.5.post8.tar` & `naver-db-0.0.5.post9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:59:45.530150 naver-db-0.0.5.post8/
--rw-rw-rw-   0        0        0      412 2023-06-30 01:59:45.528168 naver-db-0.0.5.post8/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 01:59:45.478548 naver-db-0.0.5.post8/naver_db/
--rw-rw-rw-   0        0        0      345 2023-06-05 04:16:55.000000 naver-db-0.0.5.post8/naver_db/__init__.py
--rw-rw-rw-   0        0        0    15209 2023-06-30 01:59:06.000000 naver-db-0.0.5.post8/naver_db/persistence.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:59:45.506452 naver-db-0.0.5.post8/naver_db.egg-info/
--rw-rw-rw-   0        0        0      412 2023-06-30 01:59:45.000000 naver-db-0.0.5.post8/naver_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-30 01:59:45.000000 naver-db-0.0.5.post8/naver_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:59:45.000000 naver-db-0.0.5.post8/naver_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 01:59:45.000000 naver-db-0.0.5.post8/naver_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 01:59:45.000000 naver-db-0.0.5.post8/naver_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 01:59:45.530150 naver-db-0.0.5.post8/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-06-30 01:59:21.000000 naver-db-0.0.5.post8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:59:45.525128 naver-db-0.0.5.post8/test/
--rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/__init__.py
--rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_getprops.py
--rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_nextval.py
--rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_param.py
--rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_query.py
--rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_userpermission.py
--rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_write.py
--rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post8/test/naver_writelog.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:15:20.926202 naver-db-0.0.5.post9/
+-rw-rw-rw-   0        0        0      412 2023-06-30 02:15:20.924226 naver-db-0.0.5.post9/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 02:15:20.880718 naver-db-0.0.5.post9/naver_db/
+-rw-rw-rw-   0        0        0      345 2023-06-05 04:16:55.000000 naver-db-0.0.5.post9/naver_db/__init__.py
+-rw-rw-rw-   0        0        0    15212 2023-06-30 02:15:04.000000 naver-db-0.0.5.post9/naver_db/persistence.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:15:20.906201 naver-db-0.0.5.post9/naver_db.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-06-30 02:15:20.000000 naver-db-0.0.5.post9/naver_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-30 02:15:20.000000 naver-db-0.0.5.post9/naver_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:15:20.000000 naver-db-0.0.5.post9/naver_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 02:15:20.000000 naver-db-0.0.5.post9/naver_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 02:15:20.000000 naver-db-0.0.5.post9/naver_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:15:20.926202 naver-db-0.0.5.post9/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-06-30 02:14:11.000000 naver-db-0.0.5.post9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:15:20.922200 naver-db-0.0.5.post9/test/
+-rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_getprops.py
+-rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_nextval.py
+-rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_param.py
+-rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_query.py
+-rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_userpermission.py
+-rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_write.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post9/test/naver_writelog.py
```

### Comparing `naver-db-0.0.5.post8/naver_db/persistence.py` & `naver-db-0.0.5.post9/naver_db/persistence.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
             table (str): Tabla de la base de datos
 
         Returns:
             int: Siguiente valor
         """
         seq_name = f"{schema}.{table}_{field}_seq"
         stm = f'''
-        SELECT last_value  nextval
+        SELECT last_value + 1 nextval
             FROM {seq_name};
         '''
         res = self.getQuery(stm, table)
         res = res[0]["nextval"] or 1
         return res
     # TESTED
```

### Comparing `naver-db-0.0.5.post8/setup.py` & `naver-db-0.0.5.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='naver-db',
-    version='0.0.5-8',
+    version='0.0.5-9',
     packages=setuptools.find_packages(),
     author="Jose Cuevas",
     author_email="jose.cuevas.cv@gmail.com",
     description="A DB Persistence Ancestor Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jacr6/naver-db",
```

