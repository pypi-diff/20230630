# Comparing `tmp/session-repository-0.1.2.tar.gz` & `tmp/session-repository-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.2.tar", last modified: Fri Jun 30 07:44:46 2023, max compression
+gzip compressed data, was "session-repository-0.1.3.tar", last modified: Fri Jun 30 08:13:47 2023, max compression
```

## Comparing `session-repository-0.1.2.tar` & `session-repository-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:44:46.028357 session-repository-0.1.2/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:44:46.026357 session-repository-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:44:45.979314 session-repository-0.1.2/session_repository/
--rw-rw-rw-   0        0        0     7210 2023-06-30 07:41:17.000000 session-repository-0.1.2/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.2/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.2/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:44:46.019955 session-repository-0.1.2/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:44:45.000000 session-repository-0.1.2/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:44:46.029857 session-repository-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-30 07:44:09.000000 session-repository-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:13:47.378832 session-repository-0.1.3/
+-rw-rw-rw-   0        0        0      599 2023-06-30 08:13:47.376831 session-repository-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 08:13:47.351392 session-repository-0.1.3/session_repository/
+-rw-rw-rw-   0        0        0     7490 2023-06-30 08:13:23.000000 session-repository-0.1.3/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.3/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.3/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:13:47.373832 session-repository-0.1.3/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-06-30 08:13:47.000000 session-repository-0.1.3/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 08:13:47.000000 session-repository-0.1.3/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:13:47.000000 session-repository-0.1.3/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 08:13:47.000000 session-repository-0.1.3/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 08:13:47.000000 session-repository-0.1.3/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:13:47.379834 session-repository-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-30 08:12:32.000000 session-repository-0.1.3/setup.py
```

### Comparing `session-repository-0.1.2/PKG-INFO` & `session-repository-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.2
+Version: 0.1.3
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.2/session_repository/core.py` & `session-repository-0.1.3/session_repository/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,22 +94,36 @@
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
     ) -> Union[Tuple[List[Any], str], List[Any]]:
         def _select_from_session(session: Session):
             query = session.query(model)
-            query = apply_no_load(query=query, relationship_dict=disabled_relationships)
-            query = apply_filters(query=query, filter_dict=filters)
+            query = apply_no_load(
+                query=query,
+                relationship_dict=disabled_relationships,
+            )
+            query = apply_filters(
+                query=query,
+                filter_dict=filters,
+            )
             query = apply_order_by(
-                query=query, model=model, order_by=order_by, direction=direction
+                query=query,
+                model=model,
+                order_by=order_by,
+                direction=direction,
+            )
+            query = apply_limit(
+                query=query,
+                limit=limit,
             )
-            query = apply_limit(query=query, limit=limit)
             query, pagination = apply_pagination(
-                query=query, page=page, per_page=per_page
+                query=query,
+                page=page,
+                per_page=per_page,
             )
 
             results = query.all()
 
             if self._logger is not None:
                 query_compiled = query.statement.compile(
                     compile_kwargs={"literal_binds": self._literal_binds}
@@ -144,15 +158,15 @@
         values: Dict,
         filters: Optional[_FilterType] = None,
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
     ):
         def _update_from_session(session: Session):
-            rows = self._select(
+            rows = self._select_all(
                 model=model,
                 filters=filters,
                 current_session=session,
             )
 
             if len(rows) == 0:
                 return rows
@@ -210,16 +224,18 @@
         model,
         filters: Optional[_FilterType] = None,
         flush: bool = True,
         commit: bool = False,
         current_session: Optional[Session] = None,
     ) -> bool:
         def _delete_from_session(session: Session):
-            rows: List[BaseModel] = self._select(
-                model=model, filters=filters, current_session=session
+            rows: List[BaseModel] = self._select_all(
+                model=model,
+                filters=filters,
+                current_session=session,
             )
 
             if len(rows) == 0:
                 return False
 
             for row in rows:
                 session.delete(row)
```

### Comparing `session-repository-0.1.2/session_repository/utils.py` & `session-repository-0.1.3/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.1.2/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.3/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.2
+Version: 0.1.3
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.2/setup.py` & `session-repository-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.2"
+version = "0.1.3"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

