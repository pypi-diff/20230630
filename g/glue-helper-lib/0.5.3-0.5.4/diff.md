# Comparing `tmp/glue_helper_lib-0.5.3.tar.gz` & `tmp/glue_helper_lib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_helper_lib-0.5.3.tar", max compression
+gzip compressed data, was "glue_helper_lib-0.5.4.tar", max compression
```

## Comparing `glue_helper_lib-0.5.3.tar` & `glue_helper_lib-0.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.5.3/LICENSE
--rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.5.3/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.5.3/glue_helper_lib/__init__.py
--rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.5.3/glue_helper_lib/arguments.py
--rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.5.3/glue_helper_lib/hudi/__init__.py
--rw-r--r--   0        0        0     8992 2023-06-29 07:05:20.967941 glue_helper_lib-0.5.3/glue_helper_lib/hudi/config.py
--rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.5.3/glue_helper_lib/hudi/session.py
--rw-r--r--   0        0        0     2334 2023-06-27 11:54:34.233678 glue_helper_lib-0.5.3/glue_helper_lib/hudi/table.py
--rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.5.3/glue_helper_lib/logging.py
--rw-r--r--   0        0        0      714 2023-06-17 15:39:16.309191 glue_helper_lib-0.5.3/glue_helper_lib/session.py
--rw-r--r--   0        0        0     1562 2023-06-27 07:40:10.813610 glue_helper_lib-0.5.3/glue_helper_lib/table.py
--rw-r--r--   0        0        0      711 2023-06-29 07:06:07.037941 glue_helper_lib-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.5.4/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.5.4/glue_helper_lib/__init__.py
+-rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.5.4/glue_helper_lib/arguments.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.5.4/glue_helper_lib/hudi/__init__.py
+-rw-r--r--   0        0        0     8963 2023-06-30 09:12:56.795617 glue_helper_lib-0.5.4/glue_helper_lib/hudi/config.py
+-rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.5.4/glue_helper_lib/hudi/session.py
+-rw-r--r--   0        0        0     2334 2023-06-27 11:54:34.233678 glue_helper_lib-0.5.4/glue_helper_lib/hudi/table.py
+-rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.5.4/glue_helper_lib/logging.py
+-rw-r--r--   0        0        0      714 2023-06-17 15:39:16.309191 glue_helper_lib-0.5.4/glue_helper_lib/session.py
+-rw-r--r--   0        0        0     1562 2023-06-27 07:40:10.813610 glue_helper_lib-0.5.4/glue_helper_lib/table.py
+-rw-r--r--   0        0        0      711 2023-06-30 09:13:22.425617 glue_helper_lib-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.5.4/PKG-INFO
```

### Comparing `glue_helper_lib-0.5.3/LICENSE` & `glue_helper_lib-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/arguments.py` & `glue_helper_lib-0.5.4/glue_helper_lib/arguments.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/hudi/config.py` & `glue_helper_lib-0.5.4/glue_helper_lib/hudi/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     partitioning: bool,
     partitioned_on_datetime: bool,
 ):
     if n_record_key_columns == 1 and not partitioned_on_datetime:
         return KeyGenerator.COMPLEX
     elif n_record_key_columns > 1 and not partitioned_on_datetime:
         return KeyGenerator.COMPLEX
-    elif n_record_key_columns > 1 and partitioning and partitioned_on_datetime:
+    elif partitioning and partitioned_on_datetime:
         return KeyGenerator.CUSTOM
     else:
         raise KeyGeneratorNotKnownException(
             "number of record key columns:",
             n_record_key_columns,
             "partitioning:",
             partitioning,
```

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/hudi/session.py` & `glue_helper_lib-0.5.4/glue_helper_lib/hudi/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/hudi/table.py` & `glue_helper_lib-0.5.4/glue_helper_lib/hudi/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/logging.py` & `glue_helper_lib-0.5.4/glue_helper_lib/logging.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/session.py` & `glue_helper_lib-0.5.4/glue_helper_lib/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/glue_helper_lib/table.py` & `glue_helper_lib-0.5.4/glue_helper_lib/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.5.3/pyproject.toml` & `glue_helper_lib-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-helper-lib"
-version = "0.5.3"
+version = "0.5.4"
 description = "A library containing multiple helper and utility functionalities for AWS Glue"
 authors = ["Martijn Sturm <martijn.sturm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glue_helper_lib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `glue_helper_lib-0.5.3/PKG-INFO` & `glue_helper_lib-0.5.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-helper-lib
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library containing multiple helper and utility functionalities for AWS Glue
 License: MIT
 Author: Martijn Sturm
 Author-email: martijn.sturm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

