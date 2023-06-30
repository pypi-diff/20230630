# Comparing `tmp/clappform-3.0.0a4.tar.gz` & `tmp/clappform-3.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-3.0.0a4.tar", last modified: Wed Jun  7 14:13:50 2023, max compression
+gzip compressed data, was "clappform-3.0.0a5.tar", last modified: Fri Jun  9 13:32:02 2023, max compression
```

## Comparing `clappform-3.0.0a4.tar` & `clappform-3.0.0a5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-07 14:13:39.000000 clappform-3.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 14:13:50.693729 clappform-3.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 14:13:39.000000 clappform-3.0.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-07 14:13:39.000000 clappform-3.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:13:50.693729 clappform-3.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    24656 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:13:50.693729 clappform-3.0.0a4/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 14:13:50.000000 clappform-3.0.0a4/src/clappform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 14:13:39.000000 clappform-3.0.0a4/src/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.456451 clappform-3.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 13:31:53.000000 clappform-3.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 13:32:02.456451 clappform-3.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 13:31:53.000000 clappform-3.0.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 13:31:53.000000 clappform-3.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:32:02.456451 clappform-3.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:32:02.452451 clappform-3.0.0a5/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 13:32:02.000000 clappform-3.0.0a5/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-09 13:31:53.000000 clappform-3.0.0a5/src/debug.py
```

### Comparing `clappform-3.0.0a4/LICENSE` & `clappform-3.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a4/PKG-INFO` & `clappform-3.0.0a5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a4
+Version: 3.0.0a5
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,17 @@
 License-File: LICENSE
 
 # Clappform
 **Clappform** is a wrapper for a Clappform B.V. API written in Python.
 
 ```python
 >>> from clappform import Clappform
+>>> import clappform.dataclasses as r
 >>> c = Clappform("https://app.clappform.com", "j.doe@clappform.com", "S3cr3tP4ssw0rd!")
->>> apps = c.get_apps()
+>>> apps = c.get(r.App())
 >>> for app in apps:
 ...     print(app.name)
 'Clappform'
 'Default'
 ```
 
 Clappform allows you to interact with the Clappform API for a given domain. For many of the resources that the Clappform API provides the simple ``get``, ``create``, ``update`` and ``delete`` methods can be used. Authentication is done transparently, so there is no need to manually authenticate.
```

### Comparing `clappform-3.0.0a4/README.md` & `clappform-3.0.0a5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Clappform
 **Clappform** is a wrapper for a Clappform B.V. API written in Python.
 
 ```python
 >>> from clappform import Clappform
+>>> import clappform.dataclasses as r
 >>> c = Clappform("https://app.clappform.com", "j.doe@clappform.com", "S3cr3tP4ssw0rd!")
->>> apps = c.get_apps()
+>>> apps = c.get(r.App())
 >>> for app in apps:
 ...     print(app.name)
 'Clappform'
 'Default'
 ```
 
 Clappform allows you to interact with the Clappform API for a given domain. For many of the resources that the Clappform API provides the simple ``get``, ``create``, ``update`` and ``delete`` methods can be used. Authentication is done transparently, so there is no need to manually authenticate.
```

### Comparing `clappform-3.0.0a4/pyproject.toml` & `clappform-3.0.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "3.0.0-alpha.4"
+version = "3.0.0-alpha.5"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `clappform-3.0.0a4/src/clappform/__init__.py` & `clappform-3.0.0a5/src/clappform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     HTTPError,
     PaginationTotalError,
     PaginationKeyError,
 )
 
 
 # Metadata
-__version__ = "3.0.0-alpha.4"
+__version__ = "3.0.0-alpha.5"
 __author__ = "Clappform B.V."
 __email__ = "info@clappform.com"
 __license__ = "MIT"
 __doc__ = "Clappform Python API wrapper"
 
 
 class Clappform:
@@ -517,15 +517,18 @@
         for chunk in [df[i : i + size] for i in range(0, df.shape[0], size)]:
             # `TemporaryFile` And `force_ascii=False` force the chunck to be `UTF-8`
             # encoded.
             with tempfile.TemporaryFile(mode="w+", encoding="utf-8") as fd:
                 chunk.to_json(fd, orient="records", force_ascii=False)
                 fd.seek(0)  # Reset pointer to begin of file for reading.
                 self._private_request(
-                    "POST", collection.dataframe_path(), data=fd.read()
+                    "POST",
+                    collection.dataframe_path(),
+                    headers={"Content-Type": "application/json"},
+                    data=fd.read().encode("utf-8"),
                 )
             time.sleep(interval_timeout)
 
     def empty_dataframe(self, collection) -> dc.ApiResponse:
         """Empty a dataframe.
 
         :param collection: Collection to append data to.
```

### Comparing `clappform-3.0.0a4/src/clappform/dataclasses.py` & `clappform-3.0.0a5/src/clappform/dataclasses.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a4/src/clappform/exceptions.py` & `clappform-3.0.0a5/src/clappform/exceptions.py`

 * *Files identical despite different names*

### Comparing `clappform-3.0.0a4/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.0a5/src/clappform.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 3.0.0a4
+Version: 3.0.0a5
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,17 @@
 License-File: LICENSE
 
 # Clappform
 **Clappform** is a wrapper for a Clappform B.V. API written in Python.
 
 ```python
 >>> from clappform import Clappform
+>>> import clappform.dataclasses as r
 >>> c = Clappform("https://app.clappform.com", "j.doe@clappform.com", "S3cr3tP4ssw0rd!")
->>> apps = c.get_apps()
+>>> apps = c.get(r.App())
 >>> for app in apps:
 ...     print(app.name)
 'Clappform'
 'Default'
 ```
 
 Clappform allows you to interact with the Clappform API for a given domain. For many of the resources that the Clappform API provides the simple ``get``, ``create``, ``update`` and ``delete`` methods can be used. Authentication is done transparently, so there is no need to manually authenticate.
```

