# Comparing `tmp/session-repository-0.1.0.tar.gz` & `tmp/session-repository-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.1.0.tar", last modified: Fri Jun 30 07:21:43 2023, max compression
+gzip compressed data, was "session-repository-0.1.1.tar", last modified: Fri Jun 30 07:34:22 2023, max compression
```

## Comparing `session-repository-0.1.0.tar` & `session-repository-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:21:43.365862 session-repository-0.1.0/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:21:43.363858 session-repository-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:21:43.340652 session-repository-0.1.0/session_repository/
--rw-rw-rw-   0        0        0     5999 2023-06-30 07:14:23.000000 session-repository-0.1.0/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.0/session_repository/enum.py
--rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.0/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:21:43.359306 session-repository-0.1.0/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-06-30 07:21:43.000000 session-repository-0.1.0/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 07:21:43.000000 session-repository-0.1.0/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:21:43.000000 session-repository-0.1.0/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:21:43.000000 session-repository-0.1.0/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-30 07:21:43.000000 session-repository-0.1.0/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:21:43.367856 session-repository-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-30 07:21:08.000000 session-repository-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.148038 session-repository-0.1.1/
+-rw-rw-rw-   0        0        0      599 2023-06-30 07:34:22.145667 session-repository-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.122518 session-repository-0.1.1/session_repository/
+-rw-rw-rw-   0        0        0     7241 2023-06-30 07:31:39.000000 session-repository-0.1.1/session_repository/core.py
+-rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.1.1/session_repository/enum.py
+-rw-rw-rw-   0        0        0     7274 2023-06-30 07:14:32.000000 session-repository-0.1.1/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:34:22.141339 session-repository-0.1.1/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 07:34:22.000000 session-repository-0.1.1/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:34:22.148538 session-repository-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-30 07:33:39.000000 session-repository-0.1.1/setup.py
```

### Comparing `session-repository-0.1.0/PKG-INFO` & `session-repository-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.0
+Version: 0.1.1
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.0/session_repository/core.py` & `session-repository-0.1.1/session_repository/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,51 +46,85 @@
 
     def _select(
         self,
         model,
         model_returned: Optional[Type[T]] = None,
         filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
+        current_session: Optional[Session] = None,
+    ) -> Union[Tuple[List[Any], str], List[Any], Any]:
+        def _select_from_session(session: Session):
+            query = session.query(model)
+            query = apply_no_load(query=query, relationship_dict=disabled_relationships)
+            query = apply_filters(query=query, filter_dict=filters)
+            results = query.first()
+
+            if self._logger is not None:
+                query_compiled = query.statement.compile(
+                    compile_kwargs={"literal_binds": self._literal_binds}
+                )
+                self._logger.info(query_compiled.string)
+
+            if results is None:
+                return
+
+            mapped_results = (
+                model_returned.from_orm(results)
+                if model_returned is not None
+                else results
+            )
+
+            return mapped_results
+
+        if current_session is not None:
+            results = _select_from_session(session=current_session)
+        else:
+            with self._session_factory() as session:
+                results = _select_from_session(session=session)
+
+        return results
+
+    def _select_all(
+        self,
+        model,
+        model_returned: Optional[Type[T]] = None,
+        filters: Optional[_FilterType] = None,
+        disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         page: Optional[int] = None,
         per_page: Optional[int] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
-        first: bool = False,
         limit: int = None,
         current_session: Optional[Session] = None,
-    ) -> Union[Tuple[List[Any], str], List[Any], Any]:
+    ) -> Union[Tuple[List[Any], str], List[Any]]:
         def _select_from_session(session: Session):
             query = session.query(model)
             query = apply_no_load(query=query, relationship_dict=disabled_relationships)
             query = apply_filters(query=query, filter_dict=filters)
             query = apply_order_by(
                 query=query, model=model, order_by=order_by, direction=direction
             )
             query = apply_limit(query=query, limit=limit)
             query, pagination = apply_pagination(
                 query=query, page=page, per_page=per_page
             )
 
-            results = query.first() if first else query.all()
+            results = query.all()
 
             if self._logger is not None:
                 query_compiled = query.statement.compile(
                     compile_kwargs={"literal_binds": self._literal_binds}
                 )
                 self._logger.info(query_compiled.string)
 
             if results is None:
                 return
 
             mapped_results = (
-                (
-                    model_returned.from_orm(results)
-                    if first
-                    else [model_returned.from_orm(res) for res in results]
-                )
+                [model_returned.from_orm(res) for res in results]
                 if model_returned is not None
                 else results
             )
 
             if pagination is None:
                 return mapped_results
```

### Comparing `session-repository-0.1.0/session_repository/utils.py` & `session-repository-0.1.1/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.1.0/session_repository.egg-info/PKG-INFO` & `session-repository-0.1.1/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.1.0
+Version: 0.1.1
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.1.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.1.0/setup.py` & `session-repository-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.1.0"
+version = "0.1.1"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

