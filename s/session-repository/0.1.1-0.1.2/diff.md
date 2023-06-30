# Comparing `tmp/session-repository-0.1.1.tar.gz` & `tmp/session-repository-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.1.tar", last modified: Fri Jun 30 07:34:22 2023, max compression
+gzip compressed data, was "session-repository-0.1.2.tar", last modified: Fri Jun 30 07:44:46 2023, max compression
```

## Comparing `session-repository-0.1.1.tar` & `session-repository-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.148038 session-repository-0.1.1/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:34:22.145667 session-repository-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.122518 session-repository-0.1.1/session_repository/
--rw-rw-rw-   0        0        0     7241 2023-06-30 07:31:39.000000 session-repository-0.1.1/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.1/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.1/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.141339 session-repository-0.1.1/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:34:22.148538 session-repository-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-30 07:33:39.000000 session-repository-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:44:46.028357 session-repository-0.1.2/
+-rw-rw-rw-   0        0        0      599 2023-06-30 07:44:46.026357 session-repository-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:44:45.979314 session-repository-0.1.2/session_repository/
+-rw-rw-rw-   0        0        0     7210 2023-06-30 07:41:17.000000 session-repository-0.1.2/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.2/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.2/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:44:46.019955 session-repository-0.1.2/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:44:46.029857 session-repository-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-30 07:44:09.000000 session-repository-0.1.2/setup.py
```

### Comparing `session-repository-0.1.1/PKG-INFO` & `session-repository-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.1
+Version: 0.1.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.1/session_repository/core.py` & `session-repository-0.1.2/session_repository/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def _select(
         self,
         model,
         model_returned: Optional[Type[T]] = None,
         filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         current_session: Optional[Session] = None,
-    ) -> Union[Tuple[List[Any], str], List[Any], Any]:
+    ) -> Optional[Any]:
         def _select_from_session(session: Session):
             query = session.query(model)
             query = apply_no_load(query=query, relationship_dict=disabled_relationships)
             query = apply_filters(query=query, filter_dict=filters)
             results = query.first()
 
             if self._logger is not None:
```

### Comparing `session-repository-0.1.1/session_repository/utils.py` & `session-repository-0.1.2/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.1.1/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.2/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.1
+Version: 0.1.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.1/setup.py` & `session-repository-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.1"
+version = "0.1.2"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

