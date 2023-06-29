# Comparing `tmp/sniimapp-0.0.5.tar.gz` & `tmp/sniimapp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.5.tar", last modified: Thu Jun 29 21:40:09 2023, max compression
+gzip compressed data, was "sniimapp-0.0.6.tar", last modified: Thu Jun 29 22:14:51 2023, max compression
```

## Comparing `sniimapp-0.0.5.tar` & `sniimapp-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:40:09.747492 sniimapp-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-06-29 21:40:09.747492 sniimapp-0.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      869 2023-06-29 21:39:32.000000 sniimapp-0.0.5/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 21:27:51.000000 sniimapp-0.0.5/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 21:40:09.747492 sniimapp-0.0.5/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 21:40:09.747492 sniimapp-0.0.5/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-06-29 21:40:09.000000 sniimapp-0.0.5/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 21:40:09.000000 sniimapp-0.0.5/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 21:40:09.000000 sniimapp-0.0.5/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 21:40:09.000000 sniimapp-0.0.5/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1951 2023-06-29 21:19:11.000000 sniimapp-0.0.5/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 22:14:51.287767 sniimapp-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-29 22:14:51.287767 sniimapp-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-06-29 22:13:57.000000 sniimapp-0.0.6/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2023-06-29 22:14:37.000000 sniimapp-0.0.6/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 22:14:51.287767 sniimapp-0.0.6/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 22:14:51.287767 sniimapp-0.0.6/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1369 2023-06-29 22:14:51.000000 sniimapp-0.0.6/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-29 22:14:51.000000 sniimapp-0.0.6/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 22:14:51.000000 sniimapp-0.0.6/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-29 22:14:51.000000 sniimapp-0.0.6/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1951 2023-06-29 21:19:11.000000 sniimapp-0.0.6/sniimapp.py
```

### Comparing `sniimapp-0.0.5/LICENSE` & `sniimapp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.5/PKG-INFO` & `sniimapp-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,23 @@
 
 ### Descripcion:
 
 - Libreria para la extraccion de precios de granos, frutas y hortalizas del SNIIM.
 
 ### Requerimientos:
 
-- pip install sniimapp
+- pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
 - data = sniim.get_data()
 
 - print(data[1])
-- print(len(list(data)))
 - print(data.explain())
 
 Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
 - sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.5/README.md` & `sniimapp-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 ### Descripcion:
 
 - Libreria para la extraccion de precios de granos, frutas y hortalizas del SNIIM.
 
 ### Requerimientos:
 
-- pip install sniimapp
+- pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
 - data = sniim.get_data()
 
 - print(data[1])
-- print(len(list(data)))
 - print(data.explain())
 
 Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
 - sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.5/pyproject.toml` & `sniimapp-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.5/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.6/sniimapp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,23 @@
 
 ### Descripcion:
 
 - Libreria para la extraccion de precios de granos, frutas y hortalizas del SNIIM.
 
 ### Requerimientos:
 
-- pip install sniimapp
+- pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
 - data = sniim.get_data()
 
 - print(data[1])
-- print(len(list(data)))
 - print(data.explain())
 
 Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
 - sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.5/sniimapp.py` & `sniimapp-0.0.6/sniimapp.py`

 * *Files identical despite different names*

