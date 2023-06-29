# Comparing `tmp/prom-4.4.2.tar.gz` & `tmp/prom-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prom-4.4.2.tar", last modified: Wed Jun 28 00:11:26 2023, max compression
+gzip compressed data, was "prom-4.5.0.tar", last modified: Thu Jun 29 22:43:01 2023, max compression
```

## Comparing `prom-4.4.2.tar` & `prom-4.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.256440 prom-4.4.2/
--rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.4.2/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-28 00:11:26.256303 prom-4.4.2/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.4.2/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.254187 prom-4.4.2/prom/
--rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-06-28 00:11:01.000000 prom-4.4.2/prom/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.4.2/prom/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)    48726 2023-05-01 22:59:39.000000 prom-4.4.2/prom/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.4.2/prom/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.255135 prom-4.4.2/prom/extras/
--rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.4.2/prom/extras/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.4.2/prom/extras/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.4.2/prom/extras/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23069 2023-06-24 20:06:22.000000 prom-4.4.2/prom/extras/testdata.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.255661 prom-4.4.2/prom/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.4.2/prom/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.4.2/prom/interface/base.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.255915 prom-4.4.2/prom/interface/postgres/
--rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.4.2/prom/interface/postgres/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.4.2/prom/interface/postgres/gevent.py
--rw-r--r--   0 jaymon     (501) staff       (20)    34441 2023-05-01 23:10:59.000000 prom-4.4.2/prom/interface/sql.py
--rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-06-27 20:25:40.000000 prom-4.4.2/prom/interface/sqlite.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23833 2023-06-27 23:27:43.000000 prom-4.4.2/prom/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    34778 2023-03-26 19:34:46.000000 prom-4.4.2/prom/query.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.4.2/prom/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-28 00:11:26.254734 prom-4.4.2/prom.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-28 00:11:26.000000 prom-4.4.2/prom.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-06-28 00:11:26.000000 prom-4.4.2/prom.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-28 00:11:26.000000 prom-4.4.2/prom.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-06-28 00:11:26.000000 prom-4.4.2/prom.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-28 00:11:26.000000 prom-4.4.2/prom.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-28 00:11:26.256487 prom-4.4.2/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.4.2/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645992 prom-4.5.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.5.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-29 22:43:01.645854 prom-4.5.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.5.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.643496 prom-4.5.0/prom/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-06-29 22:42:57.000000 prom-4.5.0/prom/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.5.0/prom/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    50364 2023-06-29 22:42:57.000000 prom-4.5.0/prom/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.5.0/prom/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.644677 prom-4.5.0/prom/extras/
+-rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.5.0/prom/extras/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.5.0/prom/extras/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.5.0/prom/extras/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    25477 2023-06-29 22:42:57.000000 prom-4.5.0/prom/extras/testdata.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645172 prom-4.5.0/prom/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.5.0/prom/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.5.0/prom/interface/base.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.645456 prom-4.5.0/prom/interface/postgres/
+-rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.5.0/prom/interface/postgres/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.5.0/prom/interface/postgres/gevent.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35163 2023-06-29 22:42:57.000000 prom-4.5.0/prom/interface/sql.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-06-27 20:25:40.000000 prom-4.5.0/prom/interface/sqlite.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    24278 2023-06-29 22:42:57.000000 prom-4.5.0/prom/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35676 2023-06-29 22:42:57.000000 prom-4.5.0/prom/query.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.5.0/prom/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-29 22:43:01.644251 prom-4.5.0/prom.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-29 22:43:01.000000 prom-4.5.0/prom.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-29 22:43:01.646031 prom-4.5.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.5.0/setup.py
```

### Comparing `prom-4.4.2/LICENSE.txt` & `prom-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/PKG-INFO` & `prom-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.4.2
+Version: 4.5.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.4.2/README.md` & `prom-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/__init__.py` & `prom-4.5.0/prom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     UniqueError,
     CloseError,
 )
 
 from . import utils
 
 
-__version__ = '4.4.2'
+__version__ = '4.5.0'
 
 
 def transaction(connection_name="", **kwargs):
     """Create a transaction 
 
     Sometimes you just need to batch a whole bunch of operation across a whole bunch
     of different models, this allows you to create a transaction outside of any
```

### Comparing `prom-4.4.2/prom/config.py` & `prom-4.5.0/prom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,17 @@
         """
         self.fields = {}
         self.indexes = {}
         self.table_name = String(table_name)
         self.orm_class = None
         self.lookup = {
             "field_names": {},
+            # holds parent's Field.names that have been set to None in children
+            # classes. Basically, if a parent class sets foo and then a child class
+            # later on sets foo = None then foo.names will be here
             "field_names_deleted": {},
         }
 
         for name, val in fields_or_indexes.items():
             self.set(name, val)
 
     def __str__(self):
@@ -336,62 +339,76 @@
         """Return True if schema contains field_name"""
         return field_name in self.lookup["field_names"]
 
     def __contains__(self, field_name):
         return self.has_field(field_name)
 
     def set_field(self, field_name, field):
-        if not field_name: raise ValueError("field_name is empty")
-        if field_name in self.fields: raise ValueError("{} already exists and cannot be changed".format(field_name))
-        if not isinstance(field, Field): raise ValueError("{} is not a Field instance".format(type(field)))
+        if not field_name:
+            raise ValueError("field_name is empty")
+        if field_name in self.fields:
+            raise ValueError(f"{field_name} already exists and cannot be changed")
+        if not isinstance(field, Field):
+            raise ValueError(f"{type(field)} is not a Field instance")
 
         field.__set_name__(self.orm_class, field_name)
-        #field.name = field_name
-        #field.orm_class = self.orm_class
 
         if field.unique:
             self.set_index(field_name, Index(field_name, unique=True))
 
         if field.index:
             self.set_index(field_name, Index(field_name))
 
         self.fields[field_name] = field
 
         for fn in field.names:
-            self.lookup["field_names"][fn] = field
+            if fn in self.lookup["field_names"] and fn in field.aliases:
+                self.lookup["field_names"].pop(fn)
+                logger.warning(
+                    " ".join([
+                        "{} ignored alias {} for {} because it is".format(
+                            self,
+                            fn,
+                            field.name,
+                        ),
+                        "used by another field",
+                    ])
+                )
+
+            else:
+                self.lookup["field_names"][fn] = field
 
         return self
 
     def set_index(self, index_name, index):
-        """
-        add an index to the schema
+        """Add an index to the schema
 
         for the most part, you will use the __getattr__ method of adding indexes for a more fluid interface,
         but you can use this if you want to get closer to the bare metal
 
         index_name -- string -- the name of the index
         index -- Index() -- an Index instance
         """
         if not index_name:
             raise ValueError("index_name must have a value")
         if index_name in self.indexes:
             raise ValueError("index_name {} has already been defined on {}".format(
                 index_name, str(self.indexes[index_name].field_names)
             ))
-        if not isinstance(index, Index): raise ValueError("{} is not an Index instance".format(type(index)))
+        if not isinstance(index, Index):
+            raise ValueError(f"{type(index)} is not an Index instance")
 
         index.name = index_name
         index.orm_class = self.orm_class
 
         self.indexes[index_name] = index
         return self
 
     def field_name(self, field_name, *default):
-        """
-        get the canonical field name of field_name
+        """Get the canonical field name of field_name
 
         most of the time, the field name of field_name will just be field_name,
         but this checks the configured aliases to return the canonical name
 
         :param field_name: str, the field_name you want the canonical field name for
         :param *default: mixed, if present this will be returned instead of AttributeError
             raised if field_name doesn't exist
@@ -406,14 +423,29 @@
             else:
                 if field_name in self.lookup["field_names_deleted"]:
                     return self.lookup["field_names_deleted"][field_name]
 
                 else:
                     raise
 
+    def field_model_name(self, field_name):
+        """Check field_name against all the field's ref model names to see if there
+        is a match, this is separate from .field_name because there are times when
+        this behavior might not be desirable
+
+        :param field_name: str, the field/model name you want the canonical field
+            name for
+        :returns: str, the canonical field name
+        """
+        for fn, field in self.fields.items():
+            if field_name in field.ref_names:
+                return fn
+
+        raise AttributeError(field_name)
+
     def create_orm(self, orm_class=None):
         """If you have a schema but don't have an Orm for it, you can call this method
         and have an orm_class created that will have the fields and table_name of this
         schema
 
         :param orm_class: Orm, if you want your generated class to have a certain
             parent class you can pass in the parent class you want
@@ -660,19 +692,30 @@
     @property
     def ref(self):
         """Returns the FK reference orm class"""
         schema = self.schema
         return schema.orm_class if schema else None
 
     @property
+    def ref_class(self):
+        return self.ref
+
+    @property
     def names(self):
         names = set()
         if self.name:
             names.add(self.name)
 
+        names.update(self.aliases)
+
+        return names
+
+    @property
+    def aliases(self):
+        names = set()
         names.update(self.options.get("names", []))
         names.update(self.options.get("aliases", []))
 
         if alias := self.options.get("alias", ""):
             names.add(alias)
 
         if self.is_pk():
@@ -681,14 +724,22 @@
                 model_name = self.orm_class.model_name
                 names.add(f"{model_name}_id")
                 names.add(f"{model_name}_pk")
 
         return names
 
     @property
+    def ref_names(self):
+        names = set()
+        if ref_class := self.ref:
+            names.add(ref_class.model_name)
+            names.add(ref_class.models_name)
+        return names
+
+    @property
     def interface_options(self):
         """When the interface is doing stuff with the field it might call this
         method to make sure it has all the options it needs to use the field
         """
         if self.is_ref():
             options = self.schema.pk.options
             options.update(self.options)
```

### Comparing `prom-4.4.2/prom/exception.py` & `prom-4.5.0/prom/exception.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/extras/config.py` & `prom-4.5.0/prom/extras/config.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/extras/model.py` & `prom-4.5.0/prom/extras/model.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/extras/testdata.py` & `prom-4.5.0/prom/extras/testdata.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,17 +81,16 @@
     :Example:
         from prom import Orm
 
         class Foobar(Orm):
             model_name = "foo_bar"
             models_name = "foo_bars"
     """
-    method_cache = {}
-
     model_cache = {}
+    """Caches the found models for a given model name"""
 
     def _orm_classes(self):
         """Iterate through a list of orms that should be injected into testdata
 
         by default, we want to ignore any orm classes that are defined in this
         library since they are by definition base classes
 
@@ -126,130 +125,175 @@
         kwargs.setdefault("default_method", self.get_orm)
         return self._find_method(method_name, **kwargs)
 
     def _get(self, orm_class, **kwargs):
         """Internal dispatcher method for get_orm, this will first try and find
         a get_<ORM-NAME> method and fallback to get_orm"""
         method_name, method = self._get_method(orm_class)
-        kwargs.setdefault("orm_class", orm_class)
-        logger.debug(f"Running {method_name} for orm_class {orm_class.__name__}")
-        return method(**kwargs)
+        return self._run_method(method_name, method, orm_class, **kwargs)
+
+    def _gets_count(self, orm_class, **kwargs):
+        """Find how many orm_class should be created
+
+        :param orm_class: Orm
+        :param **kwargs: this will be checked for the correct *_count or count
+            value
+        :returns: int, how many of orm_class is wanted
+        """
+        return kwargs.get(
+            f"{orm_class.model_name}_count",
+            kwargs.get(
+                f"{orm_class.models_name}_count",
+                kwargs.get(
+                    "count",
+                    1
+                )
+            )
+        )
 
     def _gets_method(self, orm_class, **kwargs):
         """Return the .get_orms() type method for orm_class"""
         method_name = f"get_{orm_class.models_name}"
         kwargs.setdefault("default_method", self.get_orms)
         return self._find_method(method_name, **kwargs)
 
     def _gets(self, orm_class, **kwargs):
         """Internal dispatcher method for get_orms, this will first try and find
         a get_<ORM-MODELS-NAME> method and fallback to get_orms"""
         method_name, method = self._gets_method(orm_class)
-        kwargs.setdefault("orm_class", orm_class)
-        logger.debug(f"Running {method_name} for orm_class {orm_class.__name__}")
-        return method(**kwargs)
+        return self._run_method(method_name, method, orm_class, **kwargs)
 
     def _create_method(self, orm_class, **kwargs):
         """Return the .create_orm() type method for orm_class"""
         method_name = f"create_{orm_class.model_name}"
         kwargs.setdefault("default_method", self.create_orm)
         return self._find_method(method_name, **kwargs)
 
     def _create(self, orm_class, **kwargs):
         """Internal dispatcher method for create_orm, this will first try and find
         a create_<ORM-NAME> method and fallback to create_orm"""
         method_name, method = self._create_method(orm_class)
-        kwargs.setdefault("orm_class", orm_class)
-        logger.debug(f"Running {method_name} for orm_class {orm_class.__name__}")
-        return method(**kwargs)
+        return self._run_method(method_name, method, orm_class, **kwargs)
 
     def _creates_method(self, orm_class, **kwargs):
         """Return the .create_orms() type method for orm_class"""
         method_name = f"create_{orm_class.models_name}"
         kwargs.setdefault("default_method", self.create_orms)
         return self._find_method(method_name, **kwargs)
 
     def _creates(self, orm_class, **kwargs):
         """Internal dispatcher method for create_orms, this will first try and find
         a create_<ORM-MODELS-NAME> method and fallback to create_orm"""
         method_name, method = self._creates_method(orm_class)
-        kwargs.setdefault("orm_class", orm_class)
-        logger.debug(f"Running {method_name} for orm_class {orm_class.__name__}")
-        return method(**kwargs)
+        return self._run_method(method_name, method, orm_class, **kwargs)
 
     def _fields_method(self, orm_class, **kwargs):
         """Return the .get_orm_fields() type method for orm_class"""
         method_name = f"get_{orm_class.model_name}_fields"
         kwargs.setdefault("default_method", self.get_orm_fields)
         return self._find_method(method_name, **kwargs)
 
     def _fields(self, orm_class, **kwargs):
         """Internal dispatcher method for get_orm_fields, this will first try and find
         a get_<ORM-NAME>_fields method and fallback to get_orm_fields"""
         method_name, method = self._fields_method(orm_class)
+        return self._run_method(method_name, method, orm_class, **kwargs)
+
+    def _run_method(self, method_name, method, orm_class, **kwargs):
         kwargs.setdefault("orm_class", orm_class)
-        logger.debug(f"Running {method_name} for orm_class {orm_class.__name__}")
+        logger.debug(
+            "Running {} as {} for orm_class {}".format(
+                method.__name__,
+                method_name,
+                orm_class.__name__,
+            )
+        )
         return method(**kwargs)
 
     def _find_attr(self, method_name):
+        """Internal method used by self.__getattr__ to find the orm and create a
+        wrapper method to call
+
+        NOTE -- this method must raise AttributeError on expected errors
+
+        :param method_name: str, the method name that contains the model class
+            we're ultimately looking for
+        :returns: callable, the method that should be ran for the passed in
+            method_name
+        """
+        logger.debug(
+            f"Finding {self.__class__.__name__}.{method_name} method"
+        )
 
-        method = None
+        try:
+            # check for <NAME>_<MODEL_NAME>
+            name, model_name = method_name.split("_", 1)
 
-        if method_name in self.method_cache:
-            method = self.method_cache[method_name]
+            if model_name.endswith("_fields"):
+                name = "fields"
+                model_name, _ = model_name.rsplit("_", 1)
+
+        except ValueError as e:
+            raise AttributeError(
+                f"invalid potential method: {method_name}"
+            ) from e
 
         else:
             try:
-                # check for <NAME>_<MODEL_NAME>
-                name, model_name = method_name.split("_", 1)
-
-                if model_name.endswith("_fields"):
-                    name = "fields"
-                    model_name, _ = model_name.rsplit("_", 1)
+                orm_class = self.get_orm_class(model_name)
 
-            except ValueError:
-                raise AttributeError("invalid potential method: {}".format(method_name))
+            except ValueError as e:
+                raise AttributeError(
+                    f"Could not find orm class from {method_name}"
+                ) from e
 
             else:
-                try:
-                    orm_class = self.get_orm_class(model_name)
+                orm_method = None
+                if name == "get":
+                    if orm_class.model_name == model_name:
+                        orm_method = self.get_orm
 
-                except ValueError as e:
-                    raise AttributeError() from e
+                    else:
+                        orm_method = self.get_orms
 
-                else:
-                    orm_method = None
-                    if name == "get":
-                        if orm_class.model_name == model_name:
-                            orm_method = self.get_orm
-
-                        else:
-                            orm_method = self.get_orms
-
-                    elif name == "create":
-                        if orm_class.model_name == model_name:
-                            orm_method = self.create_orm
-
-                        else:
-                            orm_method = self.create_orms
-
-                    elif name == "fields":
-                        orm_method = self.get_orm_fields
-
-                    if orm_method:
-                        method = functools.partial(
-                            orm_method,
-                            orm_class=orm_class,
-                        )
-                        self.method_cache[method_name] = method
+                elif name == "create":
+                    if orm_class.model_name == model_name:
+                        orm_method = self.create_orm
+
+                    else:
+                        orm_method = self.create_orms
 
-        if not method:
-            raise AttributeError(f"Could not find an orm matching {method_name}")
+                elif name == "fields":
+                    orm_method = self.get_orm_fields
 
-        return method
+                if orm_method:
+                    logger.debug(
+                        f"Found {orm_method.__name__} for {orm_class.__name__}"
+                    )
+
+                    def method(**kwargs):
+                        # https://github.com/Jaymon/prom/issues/166
+                        # we want to override the passed in orm_class if it
+                        # doesn't match our found orm class because this has
+                        # most likely been called internally by another magic
+                        # method that just passed kwargs
+                        kwargs.setdefault("orm_class", orm_class)
+                        if not isinstance(orm_class, kwargs["orm_class"]):
+                            kwargs["orm_class"] = orm_class
+
+                        return orm_method(**kwargs)
+
+                    # could also use functools.wraps here on method instead of
+                    # just setting the name, but I like that it explicitely
+                    # says it is wrapped in the name instead of just
+                    # transparantly using orm_method's name
+                    method.__name__ = f"wrapped_{orm_method.__name__}"
+                    return method
+
+        raise AttributeError(f"Could not find an orm matching {method_name}")
 
     def __getattr__(self, method_name):
         try:
             return self._find_attr(method_name)
 
         except AttributeError:
             return super().__getattr__(method_name)
@@ -399,14 +443,29 @@
         except UniqueError as e:
             logger.warning(" ".join([
                 f"Creating {orm_class.__name__} failed because it exists.",
                 "Fetching the existing instance without updating it",
             ]))
             instance = instance.requery()
 
+        for k in list(kwargs.keys()):
+            # We want to create any orms with FK references to orm_class if  counts
+            # were passed in
+            if k.endswith("_count"):
+                k_model_name = k[0:-6]
+                k_orm_class = self.get_orm_class(k_model_name)
+                if k_orm_class:
+                    logger.debug("Creating {} {} instances tied to {} instance".format(
+                        kwargs[k],
+                        k_orm_class.__name__,
+                        orm_class.__name__,
+                    ))
+                    kwargs.setdefault(instance.model_name, instance)
+                    self.create_orms(k_orm_class, **kwargs)
+
         return instance
 
     def create_orms(self, orm_class, **kwargs):
         """create instances of the orm and save it into the db
 
         :param orm_class: Orm
         :param **kwargs:
@@ -471,22 +530,21 @@
             * count: int, how many instances you want
             * <MODEL_NAME>_count: int, alias for count
             * related_refs: bool, default True, all the orms will have the same
                 foreign key references
         :returns: list, a list of Orm instances
         """
         ret = []
-        orm_field_name = orm_class.model_name
         if kwargs.get("related_refs", True):
             # because we need related refs, we will need to create refs if they
             # don't exist
             kwargs.setdefault("ignore_refs", False)
             kwargs = self.assure_orm_refs(orm_class, **kwargs)
 
-        count = kwargs.get(f"{orm_field_name}_count", kwargs.get("count", 1))
+        count = self._gets_count(orm_class, **kwargs)
         for _ in range(count):
             ret.append(self._get(orm_class, **kwargs))
 
         return ret
 
     def get_orm_fields(self, orm_class, **kwargs):
         """Get the fields of an orm_class
```

### Comparing `prom-4.4.2/prom/interface/__init__.py` & `prom-4.5.0/prom/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/interface/base.py` & `prom-4.5.0/prom/interface/base.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/interface/postgres/__init__.py` & `prom-4.5.0/prom/interface/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/interface/postgres/gevent.py` & `prom-4.5.0/prom/interface/postgres/gevent.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/interface/sql.py` & `prom-4.5.0/prom/interface/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,20 +216,30 @@
         """
         if not conflict_field_names:
             raise ValueError(f"Upsert is missing conflict fields for {schema}")
 
         for field_name in conflict_field_names:
             # conflict fields need to be in the insert fields
             if field_name not in insert_fields:
-                raise ValueError(f"Upsert insert fields on {schema} missing conflict field {field_name}")
+                raise ValueError(
+                    "Upsert insert fields on {} missing conflict field {}".format(
+                        schema,
+                        field_name,
+                    )
+                )
 
-            # conflict fields should not be in the udpate fields (this is more
+            # conflict fields should not be in the update fields (this is more
             # for safety, they should use .update if they want to change them)
             if field_name in update_fields:
-                raise ValueError(f"Upsert update fields on {schema} contains conflict field {field_name}")
+                raise ValueError(
+                    "Upsert update fields on {} contains conflict field {}".format(
+                        schema,
+                        field_name,
+                    )
+                )
 
         insert_sql, insert_args = self.render_insert_sql(
             schema,
             insert_fields,
             ignore_return_clause=True,
             **kwargs,
         )
@@ -247,15 +257,17 @@
             ', '.join(map(self.render_field_name_sql, conflict_field_names)),
             update_sql,
         )
 
         returning_field_names = schema.pk_names
         if returning_field_names:
             # https://www.sqlite.org/lang_returning.html
-            query_str += ' RETURNING {}'.format(', '.join(map(self.render_field_name_sql, returning_field_names)))
+            query_str += ' RETURNING {}'.format(', '.join(
+                map(self.render_field_name_sql, returning_field_names))
+            )
             query_args = insert_args + update_args
 
         r = self._raw(query_str, *query_args, **kwargs)
         if r and returning_field_names:
             if len(returning_field_names) > 1:
                 r = r[0]
             else:
@@ -403,124 +415,14 @@
 
         # now that we know all fk tables exist, create this table
         # !!! This uses the external .set_table so it will run through all the 
         # indexes also
         self.set_table(schema, **kwargs)
         return True
 
-    def render_field_sql(self, schema, symbol_map, field):
-        format_str = ''
-        format_args = []
-        symbol = symbol_map['symbol']
-        is_list = field.is_list
-        field_name = field.name
-        field_val = field.value
-        field_kwargs = field.kwargs
-
-        if field_kwargs:
-            # kwargs take precedence because None is a perfectly valid field_val
-            f = schema.fields[field_name]
-            if issubclass(f.type, (datetime.datetime, datetime.date)):
-                format_strs = self.render_date_field_sql(field_name, field_kwargs, symbol)
-                for fname, fvstr, farg in format_strs:
-                    if format_str:
-                        format_str += ' AND '
-
-                    if is_list:
-                        # you can pass in things like day=..., month=... to
-                        # date fields, this converts those values to lists to
-                        # make sure we can handle something like in_foo(day=1)
-                        # and in_foo(day=[1, 2, 3]) the same way
-                        farg = make_list(farg)
-
-                        format_str += '{} {} ({})'.format(
-                            fname,
-                            symbol,
-                            ', '.join([fvstr] * len(farg))
-                        )
-                        format_args.extend(farg)
-
-                    else:
-                        format_str += '{} {} {}'.format(fname, symbol, fvstr)
-                        format_args.append(farg)
-
-            else:
-                raise ValueError('Field {} does not support extended kwarg values'.format(field_name))
-
-        else:
-            if is_list and not isinstance(field_val, Query):
-                field_val = make_list(field_val) if field_val else []
-                field_name = self.render_field_name_sql(field_name)
-                format_val_str = self.PLACEHOLDER
-
-                if field_val:
-                    format_str = '{} {} ({})'.format(
-                        field_name,
-                        symbol,
-                        ', '.join([format_val_str] * len(field_val))
-                    )
-                    format_args.extend(field_val)
-
-                else:
-                    # field value is empty, so we need to customize the SQL to
-                    # compensate for the empty set since SQL doesn't like empty
-                    # sets
-                    #
-                    # the idea here is this is a condition that will
-                    # automatically cause the query to fail but not necessarily be an error, 
-                    # the best example is the IN (...) queries, if you do self.in_foo([]).get()
-                    # that will fail because the list was empty, but a value error shouldn't
-                    # be raised because a common case is: self.if_foo(Bar.query.is_che(True).pks).get()
-                    # which should result in an empty set if there are no rows where che = TRUE
-                    #
-                    # https://stackoverflow.com/a/58078468/5006
-                    if symbol == "IN":
-                        format_str = '{} <> {}'.format(field_name, field_name)
-
-                    elif symbol == "NOT IN":
-                        format_str = '{} = {}'.format(field_name, field_name)
-
-                    else:
-                        raise ValueError("Unsure what to do here")
-
-            else:
-                field_name = self.render_field_name_sql(field_name)
-                format_val_str = self.PLACEHOLDER
-
-                # special handling for NULL
-                if field_val is None:
-                    symbol = symbol_map['none_symbol']
-
-                if isinstance(field_val, Query):
-                    subquery_schema = field_val.schema
-                    if not subquery_schema:
-                        raise ValueError("{} subquery has no schema".format(field_name))
-
-                    subquery_sql, subquery_args = self.render_sql(
-                        subquery_schema,
-                        field_val
-                    )
-
-                    format_str = '{} {} ({})'.format(
-                        field_name,
-                        symbol,
-                        subquery_sql
-                    )
-                    format_args.extend(subquery_args)
-
-                else:
-                    format_str = '{} {} {}'.format(
-                        field_name,
-                        symbol,
-                        format_val_str,
-                    )
-                    format_args.append(field_val)
-
-        return format_str, format_args
-
     def render_table_name_sql(self, schema):
         return self.render_field_name_sql(schema)
 
     def render_field_name_sql(self, name):
         """normalize a non value name for the query
 
         https://blog.christosoft.de/2012/10/sqlite-escaping-table-acolumn-names/
@@ -601,17 +503,23 @@
                         query_str.append(subquery_str)
 
                     query_args.extend(subquery_args)
 
             query_str.append(") I")
         return query_str, query_args
 
-    def render_where_sql(self, schema, query, **kwargs):
-        query_str = []
-        query_args = []
+    def render_field_raw_sql(self, schema, field):
+        return field.name, field.value
+
+    def render_field_sql(self, schema, field):
+        format_str = ''
+        format_args = []
+        is_list = field.is_list
+        field_name = field.name
+        field_val = field.value
 
         symbol_map = {
             'in': {'symbol': 'IN', 'list': True},
             'nin': {'symbol': 'NOT IN', 'list': True},
             'eq': {'symbol': '=', 'none_symbol': 'IS'},
             'ne': {'symbol': '!=', 'none_symbol': 'IS NOT'},
             'gt': {'symbol': '>'},
@@ -619,32 +527,155 @@
             'lt': {'symbol': '<'},
             'lte': {'symbol': '<='},
             # https://www.tutorialspoint.com/postgresql/postgresql_like_clause.htm
             # https://www.tutorialspoint.com/sqlite/sqlite_like_clause.htm
             'like': {'symbol': 'LIKE'},
             'nlike': {'symbol': 'NOT LIKE'},
         }
+        sd = symbol_map[field.operator]
+        symbol = sd['symbol']
+
+        field_kwargs = field.kwargs
+        if field_kwargs:
+            # kwargs take precedence because None is a perfectly valid field_val
+            f = schema.fields[field_name]
+            if issubclass(f.type, (datetime.datetime, datetime.date)):
+                format_strs = self.render_date_field_sql(
+                    field_name,
+                    field_kwargs,
+                    symbol
+                )
+                for fname, fvstr, farg in format_strs:
+                    if format_str:
+                        format_str += ' AND '
+
+                    if is_list:
+                        # you can pass in things like day=..., month=... to
+                        # date fields, this converts those values to lists to
+                        # make sure we can handle something like in_foo(day=1)
+                        # and in_foo(day=[1, 2, 3]) the same way
+                        farg = make_list(farg)
+
+                        format_str += '{} {} ({})'.format(
+                            fname,
+                            symbol,
+                            ', '.join([fvstr] * len(farg))
+                        )
+                        format_args.extend(farg)
+
+                    else:
+                        format_str += '{} {} {}'.format(fname, symbol, fvstr)
+                        format_args.append(farg)
+
+            else:
+                raise ValueError(
+                    'Field {} does not support extended kwarg values'.format(
+                        field_name
+                    )
+                )
+
+        else:
+            if is_list and not isinstance(field_val, Query):
+                field_val = make_list(field_val) if field_val else []
+                field_name = self.render_field_name_sql(field_name)
+                format_val_str = self.PLACEHOLDER
+
+                if field_val:
+                    format_str = '{} {} ({})'.format(
+                        field_name,
+                        symbol,
+                        ', '.join([format_val_str] * len(field_val))
+                    )
+                    format_args.extend(field_val)
+
+                else:
+                    # field value is empty, so we need to customize the SQL to
+                    # compensate for the empty set since SQL doesn't like empty
+                    # sets
+                    #
+                    # the idea here is this is a condition that will
+                    # automatically cause the query to fail but not necessarily 
+                    # be an error, the best example is the IN (...) queries, if
+                    # you do self.in_foo([]).get() that will fail because the list
+                    # was empty, but a value error shouldn't be raised because a
+                    # common case is: self.if_foo(Bar.query.is_che(True).pks).get()
+                    # which should result in an empty set if there are no rows
+                    # where che = TRUE
+                    #
+                    # https://stackoverflow.com/a/58078468/5006
+                    if symbol == "IN":
+                        format_str = '{} <> {}'.format(field_name, field_name)
+
+                    elif symbol == "NOT IN":
+                        format_str = '{} = {}'.format(field_name, field_name)
+
+                    else:
+                        raise ValueError("Unsure what to do here")
+
+            else:
+                field_name = self.render_field_name_sql(field_name)
+                format_val_str = self.PLACEHOLDER
+
+                # special handling for NULL
+                if field_val is None:
+                    symbol = sd['none_symbol']
+
+                if isinstance(field_val, Query):
+                    subquery_schema = field_val.schema
+                    if not subquery_schema:
+                        raise ValueError(f"{field_name} subquery has no schema")
+
+                    subquery_sql, subquery_args = self.render_sql(
+                        subquery_schema,
+                        field_val
+                    )
+
+                    format_str = '{} {} ({})'.format(
+                        field_name,
+                        symbol,
+                        subquery_sql
+                    )
+                    format_args.extend(subquery_args)
+
+                else:
+                    format_str = '{} {} {}'.format(
+                        field_name,
+                        symbol,
+                        format_val_str,
+                    )
+                    format_args.append(field_val)
+
+        return format_str, format_args
+
+    def render_where_sql(self, schema, query, **kwargs):
+        query_str = []
+        query_args = []
 
         if query.fields_where:
             query_str.append('WHERE')
             or_clause = False
 
             for i, field in enumerate(query.fields_where):
                 if i > 0:
                     query_str.append('OR' if or_clause else 'AND')
 
                 field_str = ''
                 field_args = []
-                sd = symbol_map[field.operator]
 
-                field_str, field_args = self.render_field_sql(
-                    schema,
-                    sd,
-                    field,
-                )
+                if field.raw:
+                    field_str, field_args = self.render_field_raw_sql(
+                        schema,
+                        field,
+                    )
+
+                else:
+                    field_str, field_args = self.render_field_sql(
+                        schema,
+                        field,
+                    )
 
                 if field.or_clause:
                     if not or_clause:
                         query_str.append("(")
                         or_clause = True
 
                 query_str.append('  {}'.format(field_str))
```

### Comparing `prom-4.4.2/prom/interface/sqlite.py` & `prom-4.5.0/prom/interface/sqlite.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom/model.py` & `prom-4.5.0/prom/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,17 @@
 
         :param orm_classpath: string|type, a full python class path (eg, foo.bar.Che) or
             an actual model.Orm python class
         :returns: Orm
         """
         return self.query.ref(orm_classpath).orm_class
 
+    def ref_class(self, orm_classpath):
+        return self.ref(orm_classpath)
+
     def is_hydrated(self):
         """return True if this orm was populated from the interface/db"""
         return self._interface_hydrate
 
     def is_update(self):
         """Return True if .save() will perform an interface update"""
         return self._interface_pk is not None
@@ -431,15 +434,20 @@
         ret = True
 
         schema = self.schema
         fields = self.to_interface()
 
         conflict_fields = self.conflict_fields(fields)
         if not conflict_fields:
-            raise ValueError(f"Upsert failed to find the conflict field names")
+            raise ValueError(
+                "{}.upsert() failed to find conflict field names from: {}".format(
+                    self.__class__.__name__,
+                    list(fields.keys())
+                )
+            )
 
         q = self.query
         q.set(fields)
         pk = q.upsert([t[0] for t in conflict_fields], **kwargs)
         if pk:
             fields = q.fields_set.fields
             pk_name = schema.pk_name
@@ -491,39 +499,42 @@
     def conflict_fields(self, fields):
         """Internal method. This will find fields that can be used for .upsert/.load
 
         :param fields: dict, the fields to check for values that would satisfy
             unique indexes or a primary key
         :returns: list<tuple>, a list of (field_name, field_value) tuples
         """
-        schema = self.schema
-
         conflict_fields = []
 
+        schema = self.schema
+
         # we'll start with checking the primary key
         for field_name in schema.pk_names:
             if field_name in fields:
                 conflict_fields.append((field_name, fields[field_name]))
 
             else:
                 conflict_fields = []
                 break
 
         if not conflict_fields:
-            # no luck with the primary key, so let's check unique indexes 
+            # no luck with the primary key, so let's check unique indexes
             for index in schema.indexes.values():
                 if index.unique:
                     for field_name in index.field_names:
                         if field_name in fields:
                             conflict_fields.append((field_name, fields[field_name]))
 
                         else:
                             conflict_fields = []
                             break
 
+                    if conflict_fields:
+                        break
+
         return conflict_fields
 
     def load(self):
         """Given a partially populated orm try and load any missing fields from
         the db
 
         :returns: bool, True if it loaded from the db, False otherwise
@@ -624,22 +635,24 @@
                     ref_field_value = getattr(self, ref_field_name, None)
                     ret = None
                     if ref_field_value:
                         ret = ref_class.query.eq_pk(ref_field_value).one()
 
                     return ret
 
-            # Go through all the orm_classes looking for a models_name match and
-            # query that model using the field name that matches the FK value in self
+            # Go through all the orm_classes looking for a model_name or models_name
+            # match and query that model using that model's FK field name that
+            # matches self.pk
             for orm_class in self.orm_classes.values():
-                if k == orm_class.models_name:
+                if k == orm_class.models_name or k == orm_class.model_name:
                     for ref_field_name, ref_field in orm_class.schema.ref_fields.items():
                         ref_class = ref_field.ref
                         if ref_class and isinstance(self, ref_class):
-                            return orm_class.query.eq_field(ref_field_name, self.pk).all()
+                            query = orm_class.query.eq_field(ref_field_name, self.pk)
+                            return query.all() if k == orm_class.models_name else query.one()
 
             raise
 
         else:
             ret = getattr(self, field_name)
 
         return ret
```

### Comparing `prom-4.4.2/prom/query.py` & `prom-4.5.0/prom/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,19 +398,25 @@
         return self.query.schema if self.query else None
 
     def __init__(self, query, field_name, field_val=None, **kwargs):
         self.query = query
         self.operator = kwargs.pop("operator", None)
         self.is_list = kwargs.pop("is_list", False)
         self.direction = kwargs.pop("direction", None) # 1 = ASC, -1 = DESC
+        self.raw = kwargs.pop("raw", False)
         self.or_clause = False
         self.kwargs = kwargs
 
-        self.set_name(field_name)
-        self.set_value(field_val)
+        if self.raw:
+            self.name = field_name
+            self.value = field_val
+
+        else:
+            self.set_name(field_name)
+            self.set_value(field_val)
 
     def set_name(self, field_name):
         field_name, function_name = self.parse(field_name, self.schema)
         self.function_name = function_name
         self.name = field_name
 
     def set_value(self, field_val):
@@ -427,27 +433,35 @@
         self.value = field_val
 
     def iquery(self, field_val):
         query = self.query
         schema = self.schema
         if query and schema:
             schema_field = getattr(schema, self.name)
+            if ref_class := schema_field.ref:
+                if isinstance(field_val, ref_class):
+                    field_val = field_val.pk
+
             field_val = schema_field.iquery(query, field_val)
         return field_val
 
     def parse(self, field_name, schema):
         function_name = ""
         if schema:
             function_name = ""
             m = re.match(r"^([^\(]+)\(([^\)]+)\)$", field_name)
             if m:
                 function_name = m.group(1)
                 field_name = m.group(2)
 
-            field_name = schema.field_name(field_name)
+            try:
+                field_name = schema.field_name(field_name)
+
+            except AttributeError:
+                field_name = schema.field_model_name(field_name)
 
         return field_name, function_name
 
 
 class Fields(list):
     @property
     def fields(self):
@@ -538,29 +552,39 @@
 
     @property
     def OR(self):
         """Wraps left and right field statements with an OR clause, you can chain
         as many OR calls as you want to create an any length OR clause
 
         I don't love that I had to use OR instead of or but "or" is a reserved
-        keyword and I thought OR was better than like _or or _or_
+        keyword and I thought OR was better than like _or, or_ or _or_
 
         :Example:
             self.eq_foo(1).OR.eq_foo(5).OR.eq_foo(10) # (foo=1 OR foo=5 OR foo=10)
         """
         self.fields_where[-1].or_clause = True
         return self
 
     @property
+    def or_(self): return self.OR
+    @property
+    def _or(self): return self.OR
+
+    @property
     def AND(self):
         """This is just here for completeness with .OR since, by default, any
         statements will be joined by AND"""
         self.fields_where[-1].or_clause = False
         return self
 
+    @property
+    def and_(self): return self.AND
+    @property
+    def _and(self): return self.AND
+
     def __init__(self, orm_class=None, **kwargs):
         # needed to use the db querying methods like get(), if you just want to build
         # a query then you don't need to bother passing this in
         self.orm_class = orm_class
         self.reset()
 
     def reset(self):
@@ -632,14 +656,17 @@
                 field_method = self.eq_field
                 query_method = getattr(self, name)
 
             elif name in {"get", "values", "all", "cursor"}:
                 field_method = self.in_field
                 query_method = getattr(self, name)
 
+            elif name in {"raw"}:
+                raise AttributeError(method_name)
+
             else:
                 query_method = None
                 field_method_name = "{}_field".format(name)
                 field_method = getattr(self, field_method_name, None)
                 if not field_method:
                     # let's try reversing the split, so <FIELD_NAME>_<NAME>
                     field_name, name = method_name.rsplit("_", 1)
@@ -794,22 +821,22 @@
         keyword.
 
         See .intersect() since this works very similar
         """
         return self.append_compound("except", queries, **kwargs)
 
     def is_field(self, field_name, field_val=None, **field_kwargs):
-        return self.append_operation("eq", field_name, field_val, **field_kwargs)
+        return self.eq_field(field_name, field_val, **field_kwargs)
     def eq_field(self, field_name, field_val=None, **field_kwargs):
-        return self.is_field(field_name, field_val, **field_kwargs)
+        return self.append_operation("eq", field_name, field_val, **field_kwargs)
 
     def not_field(self, field_name, field_val=None, **field_kwargs):
-        return self.append_operation("ne", field_name, field_val, **field_kwargs)
+        return self.ne_field(field_name, field_val, **field_kwargs)
     def ne_field(self, field_name, field_val=None, **field_kwargs):
-        return self.not_field(field_name, field_val, **field_kwargs)
+        return self.append_operation("ne", field_name, field_val, **field_kwargs)
 
     def between_field(self, field_name, low, high):
         self.gte_field(field_name, low)
         self.lte_field(field_name, high)
         return self
 
     def lte_field(self, field_name, field_val=None, **field_kwargs):
@@ -865,14 +892,18 @@
         :param field_val: string, the like query: %val, %val%, val%
         :returns: self, for fluid interface
         """
         if not field_val:
             raise ValueError("Cannot NOT LIKE nothing")
         return self.append_operation("nlike", field_name, field_val, **field_kwargs)
 
+    def raw_field(self, field_name, *field_vals, **field_kwargs):
+        field_kwargs["raw"] = True
+        return self.append_operation("raw", field_name, field_vals, **field_kwargs)
+
     def asc(self, *field_names):
         for field_name in field_names:
             self.asc_field(field_name)
         return self
 
     def asc_field(self, field_name, field_val=None):
         return self.append_sort(1, field_name, field_val)
```

### Comparing `prom-4.4.2/prom/utils.py` & `prom-4.5.0/prom/utils.py`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/prom.egg-info/PKG-INFO` & `prom-4.5.0/prom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.4.2
+Version: 4.5.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.4.2/prom.egg-info/SOURCES.txt` & `prom-4.5.0/prom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prom-4.4.2/setup.py` & `prom-4.5.0/setup.py`

 * *Files identical despite different names*

