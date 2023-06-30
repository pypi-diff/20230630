# Comparing `tmp/marshmallow_peewee-4.3.0.tar.gz` & `tmp/marshmallow_peewee-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow_peewee-4.3.0.tar", max compression
+gzip compressed data, was "marshmallow_peewee-4.3.1.tar", max compression
```

## Comparing `marshmallow_peewee-4.3.0.tar` & `marshmallow_peewee-4.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4452 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/README.md
--rw-r--r--   0        0        0      302 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/__init__.py
--rw-r--r--   0        0        0      255 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/config.py
--rw-r--r--   0        0        0     5727 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/convert.py
--rw-r--r--   0        0        0     2786 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/fields.py
--rw-r--r--   0        0        0        0 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/py.typed
--rw-r--r--   0        0        0     4514 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/schema.py
--rw-r--r--   0        0        0      264 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/marshmallow_peewee/types.py
--rw-r--r--   0        0        0     1355 2023-05-25 06:54:47.569647 marshmallow_peewee-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 marshmallow_peewee-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4452 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/README.md
+-rw-r--r--   0        0        0      302 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/__init__.py
+-rw-r--r--   0        0        0      255 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/config.py
+-rw-r--r--   0        0        0     5782 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/convert.py
+-rw-r--r--   0        0        0     2836 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/fields.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/py.typed
+-rw-r--r--   0        0        0     4514 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/schema.py
+-rw-r--r--   0        0        0      264 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/marshmallow_peewee/types.py
+-rw-r--r--   0        0        0     1355 2023-06-30 13:22:05.636203 marshmallow_peewee-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 marshmallow_peewee-4.3.1/PKG-INFO
```

### Comparing `marshmallow_peewee-4.3.0/README.md` & `marshmallow_peewee-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.3.0/marshmallow_peewee/convert.py` & `marshmallow_peewee-4.3.1/marshmallow_peewee/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         self.opts = opts
 
     def get_fields(self, model: pw.Model) -> OrderedDict[str, fields.Field]:
         result = OrderedDict()
         meta = cast(pw.Metadata, model._meta)  # type: ignore[]
         for field in meta.sorted_fields:
             name = field.name
-            if self.opts.id_keys and isinstance(field, pw.ForeignKeyField):
+            if self.opts.id_keys and isinstance(
+                field, (pw.ForeignKeyField, pw.DeferredForeignKey)
+            ):
                 name = field.column_name
 
             ma_field = self.convert(field)
             if ma_field:
                 result[name] = ma_field
 
         return result
```

### Comparing `marshmallow_peewee-4.3.0/marshmallow_peewee/fields.py` & `marshmallow_peewee-4.3.1/marshmallow_peewee/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,12 +78,13 @@
                 model = model_cls
                 fields = kwargs.get("only", ())
                 exclude = kwargs.get("exclude", ())
 
         return Schema
 
     def get_value(self, obj: pw.Model, attr: str, accessor=None, default=None):
-        fk = obj.__data__.get(attr)
+        data_key = self.attribute or attr
+        fk = obj.__data__.get(data_key)
         if fk is None:
             return None
 
-        return obj.__rel__[attr]
+        return obj.__rel__[data_key]
```

### Comparing `marshmallow_peewee-4.3.0/marshmallow_peewee/schema.py` & `marshmallow_peewee-4.3.1/marshmallow_peewee/schema.py`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.3.0/pyproject.toml` & `marshmallow_peewee-4.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marshmallow-peewee"
-version = "4.3.0"
+version = "4.3.1"
 description = "Peewee ORM integration with the Marshmallow (de)serialization library"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klen/marshmallow-peewee"
 repository = "https://github.com/klen/marshmallow-peewee"
 keywords = ["marshmallow", "peewee", "orm", "serialization", "deserialization"]
```

### Comparing `marshmallow_peewee-4.3.0/PKG-INFO` & `marshmallow_peewee-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow-peewee
-Version: 4.3.0
+Version: 4.3.1
 Summary: Peewee ORM integration with the Marshmallow (de)serialization library
 Home-page: https://github.com/klen/marshmallow-peewee
 License: MIT
 Keywords: marshmallow,peewee,orm,serialization,deserialization
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

