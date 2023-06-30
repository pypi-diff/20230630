# Comparing `tmp/axsqlalchemy-0.0.5.tar.gz` & `tmp/axsqlalchemy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axsqlalchemy-0.0.5.tar", last modified: Mon Jun 26 09:08:17 2023, max compression
+gzip compressed data, was "axsqlalchemy-0.0.6.tar", last modified: Fri Jun 30 17:47:11 2023, max compression
```

## Comparing `axsqlalchemy-0.0.5.tar` & `axsqlalchemy-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/repository.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/uow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/axsqlalchemy/utils/creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 09:08:17.000000 axsqlalchemy-0.0.5/axsqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 09:08:17.532245 axsqlalchemy-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-26 09:07:51.000000 axsqlalchemy-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 17:47:11.503602 axsqlalchemy-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-30 17:47:11.499602 axsqlalchemy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 17:47:11.499602 axsqlalchemy-0.0.6/axsqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/repository.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 17:47:11.499602 axsqlalchemy-0.0.6/axsqlalchemy/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/axsqlalchemy/utils/creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 17:47:11.499602 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-30 17:47:11.000000 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-30 17:47:11.000000 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 17:47:11.000000 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-30 17:47:11.000000 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-30 17:47:11.000000 axsqlalchemy-0.0.6/axsqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 17:47:11.503602 axsqlalchemy-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-06-30 17:46:45.000000 axsqlalchemy-0.0.6/setup.py
```

### Comparing `axsqlalchemy-0.0.5/axsqlalchemy/model.py` & `axsqlalchemy-0.0.6/axsqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.5/axsqlalchemy/repository.py` & `axsqlalchemy-0.0.6/axsqlalchemy/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,26 @@
             return tuple(ids)
 
         for column in columns:
             ids.append(getattr(obj, column.name))
 
         return tuple(ids)
 
-
     async def get(self, *ids: Any) -> Any:
         filters = self.__get_filters(ids)
 
         if self.DBModel.ids is None:
             raise NotImplementedError
 
         obj = (
             (
                 await self.session.execute(
                     select(self.DBModel)
                     .where(and_(*filters))
-                    .order_by(self.DBModel.created_at),
+                    .order_by(self.DBModel.created_at.desc()),
                 )
             )
             .scalars()
             .first()
         )
 
         if obj:
```

### Comparing `axsqlalchemy-0.0.5/axsqlalchemy/settings.py` & `axsqlalchemy-0.0.6/axsqlalchemy/settings.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.5/axsqlalchemy/uow.py` & `axsqlalchemy-0.0.6/axsqlalchemy/uow.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.5/axsqlalchemy/utils/creation.py` & `axsqlalchemy-0.0.6/axsqlalchemy/utils/creation.py`

 * *Files identical despite different names*

### Comparing `axsqlalchemy-0.0.5/setup.py` & `axsqlalchemy-0.0.6/setup.py`

 * *Files identical despite different names*

