# Comparing `tmp/gallon-0.0.1.tar.gz` & `tmp/gallon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallon-0.0.1.tar", max compression
+gzip compressed data, was "gallon-0.0.2.tar", max compression
```

## Comparing `gallon-0.0.1.tar` & `gallon-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.1/README.md
--rw-r--r--   0        0        0      257 2023-06-30 03:06:40.530018 gallon-0.0.1/gallon/__init__.py
--rw-r--r--   0        0        0     4023 2023-06-30 03:03:11.079145 gallon-0.0.1/gallon/client.py
--rw-r--r--   0        0        0     9668 2023-06-30 03:02:57.075552 gallon-0.0.1/gallon/data.py
--rw-r--r--   0        0        0     1975 2023-06-30 03:02:44.091937 gallon-0.0.1/gallon/helpers.py
--rw-r--r--   0        0        0     3589 2023-06-30 03:02:55.375602 gallon-0.0.1/gallon/objects.py
--rw-r--r--   0        0        0     3989 2023-06-30 02:42:16.528905 gallon-0.0.1/gallon/server.py
--rw-r--r--   0        0        0      272 2023-06-30 03:07:08.149456 gallon-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 gallon-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.2/README.md
+-rw-r--r--   0        0        0      257 2023-06-30 03:06:40.530018 gallon-0.0.2/gallon/__init__.py
+-rw-r--r--   0        0        0     4023 2023-06-30 03:03:11.079145 gallon-0.0.2/gallon/client.py
+-rw-r--r--   0        0        0     9668 2023-06-30 03:02:57.075552 gallon-0.0.2/gallon/data.py
+-rw-r--r--   0        0        0     1975 2023-06-30 03:02:44.091937 gallon-0.0.2/gallon/helpers.py
+-rw-r--r--   0        0        0     3589 2023-06-30 03:02:55.375602 gallon-0.0.2/gallon/objects.py
+-rw-r--r--   0        0        0     4018 2023-06-30 03:13:50.959250 gallon-0.0.2/gallon/server.py
+-rw-r--r--   0        0        0      296 2023-06-30 03:14:26.358837 gallon-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 gallon-0.0.2/PKG-INFO
```

### Comparing `gallon-0.0.1/gallon/client.py` & `gallon-0.0.2/gallon/client.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.1/gallon/data.py` & `gallon-0.0.2/gallon/data.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.1/gallon/helpers.py` & `gallon-0.0.2/gallon/helpers.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.1/gallon/objects.py` & `gallon-0.0.2/gallon/objects.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.1/gallon/server.py` & `gallon-0.0.2/gallon/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,7 +137,8 @@
     def run(self):
         """Run the server"""
         self.logger.info(
             "%s running on %s",
             self.__class__.__name__,
             f"http://{self.server_name}:{self.server_port}",
         )
+        self.serve_forever()
```

