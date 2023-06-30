# Comparing `tmp/clappform-3.0.0a5.tar.gz` & `tmp/clappform-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.0a5.tar", last modified: Fri Jun  9 13:32:02 2023, max compression
+gzip compressed data, was "clappform-3.0.1.tar", last modified: Fri Jun 30 13:12:36 2023, max compression
```

## Comparing `clappform-3.0.0a5.tar` & `clappform-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.456451 clappform-3.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 13:31:53.000000 clappform-3.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 13:32:02.456451 clappform-3.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 13:31:53.000000 clappform-3.0.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 13:31:53.000000 clappform-3.0.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:32:02.456451 clappform-3.0.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 13:12:27.000000 clappform-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 13:12:36.638102 clappform-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 13:12:27.000000 clappform-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-30 13:12:27.000000 clappform-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:12:36.638102 clappform-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    24897 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 13:12:27.000000 clappform-3.0.1/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:12:36.638102 clappform-3.0.1/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 13:12:36.000000 clappform-3.0.1/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 13:12:27.000000 clappform-3.0.1/src/debug.py
```

### Comparing `clappform-3.0.0a5/LICENSE` & `clappform-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a5/PKG-INFO` & `clappform-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a5
+Version: 3.0.1
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-3.0.0a5/README.md` & `clappform-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a5/pyproject.toml` & `clappform-3.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.0-alpha.5"
+version = "3.0.1"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `clappform-3.0.0a5/src/clappform/__init__.py` & `clappform-3.0.1/src/clappform/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.0-alpha.5"
+__version__ = "3.0.1"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -392,34 +392,36 @@
                 },
                 "deep_dive": {"type": "dict"},
             },
             require_all=True,
         )
         v.validate(options)
 
-        path = "/dataframe/aggregate"
+        path = "/dataframe/read_data?extended=true"
         params = {
             "method": "POST",
-            "path": f"{path}?extended=true",
+            "path": path,
             "json": v.document,
         }
 
         document = self._private_request(**params)
         if "total" not in document:
             raise PaginationKeyError(missing_key="total", data=document)
         if document["total"] == 0:
             raise PaginationTotalError(total=document["total"], data=document)
 
         pages_to_get = math.ceil(document["total"] / options["limit"])
         if pages_to_get == 1:
             yield DataFrame(document["data"])
         else:
-            for _ in range(pages_to_get):
+            for i in range(pages_to_get):
                 yield DataFrame(document["data"])
-                params["path"] = f"{path}?next_page={document['next_page']}"
+                if i >= pages_to_get - 1:
+                    break
+                params["path"] = f"{path}&next_page={document['next_page']}"
                 time.sleep(
                     interval_timeout
                 )  # Prevent Denial Of Service (dos) flagging.
                 document = self._private_request(**params)
 
     def read_dataframe(self, query, limit: int = 100, interval_timeout: int = 0):
         """Read a dataframe.
@@ -449,18 +451,18 @@
             >>> for df in c.read_dataframe(query):
             ...     list_df.append(df)
             >>> master_df = pd.concat(list_df)
 
         :returns: Generator to read dataframe
         :rtype: :class:`generator`
         """
-        path = "/dataframe/read_data"
+        path = "/dataframe/read_data?extended=true"
         params = {
             "method": "POST",
-            "path": f"{path}?extended=true",
+            "path": path,
             "json": {"limit": limit},
         }
         if isinstance(query, dc.Query):
             params["json"]["query"] = query.slug
         elif isinstance(query, dc.Collection):
             params["json"]["app"] = query.app
             params["json"]["collection"] = query.slug
@@ -476,17 +478,19 @@
         if document["total"] == 0:
             raise PaginationTotalError(total=document["total"], data=document)
 
         pages_to_get = math.ceil(document["total"] / limit)
         if pages_to_get == 1:
             yield DataFrame(document["data"])
         else:
-            for _ in range(pages_to_get):
+            for i in range(pages_to_get):
                 yield DataFrame(document["data"])
-                params["path"] = f"{path}?next_page={document['next_page']}"
+                params["path"] = f"{path}&next_page={document['next_page']}"
+                if i >= pages_to_get - 1:
+                    break
                 time.sleep(
                     interval_timeout
                 )  # Prevent Denial Of Service (dos) flagging.
                 document = self._private_request(**params)
 
     def write_dataframe(
         self,
```

### Comparing `clappform-3.0.0a5/src/clappform/dataclasses.py` & `clappform-3.0.1/src/clappform/dataclasses.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a5/src/clappform/exceptions.py` & `clappform-3.0.1/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a5/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.1/src/clappform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a5
+Version: 3.0.1
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

