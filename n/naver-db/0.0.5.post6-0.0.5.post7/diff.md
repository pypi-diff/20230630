# Comparing `tmp/naver-db-0.0.5.post6.tar.gz` & `tmp/naver-db-0.0.5.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver-db-0.0.5.post6.tar", last modified: Mon Jun  5 04:19:44 2023, max compression
+gzip compressed data, was "naver-db-0.0.5.post7.tar", last modified: Thu Jun 29 18:47:45 2023, max compression
```

## Comparing `naver-db-0.0.5.post6.tar` & `naver-db-0.0.5.post7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.357256 naver-db-0.0.5.post6/
--rw-rw-rw-   0        0        0      412 2023-06-05 04:19:44.356135 naver-db-0.0.5.post6/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.314845 naver-db-0.0.5.post6/naver_db/
--rw-rw-rw-   0        0        0      345 2023-06-05 04:16:55.000000 naver-db-0.0.5.post6/naver_db/__init__.py
--rw-rw-rw-   0        0        0    15028 2023-06-05 04:16:07.000000 naver-db-0.0.5.post6/naver_db/persistence.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.332337 naver-db-0.0.5.post6/naver_db.egg-info/
--rw-rw-rw-   0        0        0      412 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 04:19:44.000000 naver-db-0.0.5.post6/naver_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 04:19:44.358735 naver-db-0.0.5.post6/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-06-05 04:17:49.000000 naver-db-0.0.5.post6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:19:44.354143 naver-db-0.0.5.post6/test/
--rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/__init__.py
--rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_getprops.py
--rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_nextval.py
--rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_param.py
--rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_query.py
--rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_userpermission.py
--rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_write.py
--rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post6/test/naver_writelog.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:47:45.183170 naver-db-0.0.5.post7/
+-rw-rw-rw-   0        0        0      412 2023-06-29 18:47:45.182170 naver-db-0.0.5.post7/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 18:47:45.131730 naver-db-0.0.5.post7/naver_db/
+-rw-rw-rw-   0        0        0      345 2023-06-05 04:16:55.000000 naver-db-0.0.5.post7/naver_db/__init__.py
+-rw-rw-rw-   0        0        0    15123 2023-06-29 18:46:21.000000 naver-db-0.0.5.post7/naver_db/persistence.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:47:45.160019 naver-db-0.0.5.post7/naver_db.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-06-29 18:47:44.000000 naver-db-0.0.5.post7/naver_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-29 18:47:44.000000 naver-db-0.0.5.post7/naver_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:47:44.000000 naver-db-0.0.5.post7/naver_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-29 18:47:44.000000 naver-db-0.0.5.post7/naver_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 18:47:44.000000 naver-db-0.0.5.post7/naver_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:47:45.183170 naver-db-0.0.5.post7/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-06-29 18:47:14.000000 naver-db-0.0.5.post7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:47:45.180166 naver-db-0.0.5.post7/test/
+-rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_getprops.py
+-rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_nextval.py
+-rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_param.py
+-rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_query.py
+-rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_userpermission.py
+-rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_write.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post7/test/naver_writelog.py
```

### Comparing `naver-db-0.0.5.post6/naver_db/persistence.py` & `naver-db-0.0.5.post7/naver_db/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,31 +453,32 @@
                                        "\'" if value is not None else "NULL")
             stm += "INSERT INTO " + str(schema)+"."+str(table).lower(
             ) + " (" + columns[:-1] + ")" + " VALUES (" + values[:-1] + "); \n "
         return stm
 
     # UPDATE DTO
 
-    def updateDto(self, dto, table, pk, schema="entities"):
+    def updateDto(self, dto, table, schema, pk):
         """Método para actualizar un dto
 
         Args:
             dto (dto): DTO
             table (str): Tabla de la base de datos
 
         Returns:
             res: Resultado de la consulta
         """
         stm = f"UPDATE  {schema}.{table}  SET "
-        if isinstance(dto, dict):
-            dto_items = dto.items()
-        else:
-            dto_items = dto.__dict__().items()
+        table_columns = self.listColumns(table, schema)
+        dto_items = dto.__dict__().items()
         for key, value in dto_items:
-            stm += " {}={} ,".format(key, "\'"+str(value) +
-                                     "\'" if value is not None else "NULL")
+            value = value or "NULL"
+            if (str(value).__contains__("{") or str(value).__contains__("-") or isinstance(value, str)) and value != "NULL":
+                value = f"'{value}'"
+            stm += f" {key}={value} ,"
         stm = stm[:-1]
-        id = dto.__dict__()[pk]
-        where = " WHERE {}=\'{}\'".format(pk, id)
-        stm += where
+        id = dto.toDict()[pk]
+        stm += f" WHERE {pk}='{id}'"
+        stm = stm.replace("\n","")
+        stm = stm.replace("\\'","'")
         res = self.setWrite(stm, table)
         return res
```

### Comparing `naver-db-0.0.5.post6/setup.py` & `naver-db-0.0.5.post7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='naver-db',
-    version='0.0.5-6',
+    version='0.0.5-7',
     packages=setuptools.find_packages(),
     author="Jose Cuevas",
     author_email="jose.cuevas.cv@gmail.com",
     description="A DB Persistence Ancestor Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jacr6/naver-db",
```

