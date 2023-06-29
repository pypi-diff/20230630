# Comparing `tmp/django_model_import-0.7.1.tar.gz` & `tmp/django_model_import-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_model_import-0.7.1.tar", max compression
+gzip compressed data, was "django_model_import-0.7.2.tar", max compression
```

## Comparing `django_model_import-0.7.1.tar` & `django_model_import-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0     3976 2022-11-10 00:29:59.375497 django_model_import-0.7.1/README.md
--rwxr-xr-x   0        0        0      282 2023-02-16 22:27:38.570122 django_model_import-0.7.1/djangomodelimport/__init__.py
--rw-r--r--   0        0        0      173 2022-11-10 00:29:59.376699 django_model_import-0.7.1/djangomodelimport/caches.py
--rw-r--r--   0        0        0     7006 2022-12-07 04:01:32.877215 django_model_import-0.7.1/djangomodelimport/core.py
--rw-r--r--   0        0        0     7733 2022-11-15 22:49:58.055394 django_model_import-0.7.1/djangomodelimport/fields.py
--rw-r--r--   0        0        0     3804 2022-11-15 22:49:58.055568 django_model_import-0.7.1/djangomodelimport/formclassbuilder.py
--rw-r--r--   0        0        0     6615 2022-11-15 22:49:58.055742 django_model_import-0.7.1/djangomodelimport/forms.py
--rw-r--r--   0        0        0     1536 2022-11-15 22:49:58.055893 django_model_import-0.7.1/djangomodelimport/loaders.py
--rw-r--r--   0        0        0     7336 2022-11-14 01:42:13.378100 django_model_import-0.7.1/djangomodelimport/magic.py
--rw-r--r--   0        0        0     2766 2022-11-10 00:29:59.378713 django_model_import-0.7.1/djangomodelimport/parsers.py
--rw-r--r--   0        0        0     2703 2022-01-31 04:49:09.805613 django_model_import-0.7.1/djangomodelimport/resultset.py
--rw-r--r--   0        0        0      612 2022-11-15 22:49:58.055999 django_model_import-0.7.1/djangomodelimport/utils.py
--rw-r--r--   0        0        0     2541 2022-11-10 00:29:59.378882 django_model_import-0.7.1/djangomodelimport/widgets.py
--rw-r--r--   0        0        0      876 2023-02-16 22:27:28.572564 django_model_import-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5028 1970-01-01 00:00:00.000000 django_model_import-0.7.1/setup.py
--rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 django_model_import-0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0     3976 2022-11-10 00:29:59.375497 django_model_import-0.7.2/README.md
+-rwxr-xr-x   0        0        0      282 2023-02-16 22:27:38.570122 django_model_import-0.7.2/djangomodelimport/__init__.py
+-rw-r--r--   0        0        0      173 2022-11-10 00:29:59.376699 django_model_import-0.7.2/djangomodelimport/caches.py
+-rw-r--r--   0        0        0     7006 2022-12-07 04:01:32.877215 django_model_import-0.7.2/djangomodelimport/core.py
+-rw-r--r--   0        0        0     7746 2023-06-29 23:24:47.491255 django_model_import-0.7.2/djangomodelimport/fields.py
+-rw-r--r--   0        0        0     3804 2022-11-15 22:49:58.055568 django_model_import-0.7.2/djangomodelimport/formclassbuilder.py
+-rw-r--r--   0        0        0     6615 2022-11-15 22:49:58.055742 django_model_import-0.7.2/djangomodelimport/forms.py
+-rw-r--r--   0        0        0     1536 2022-11-15 22:49:58.055893 django_model_import-0.7.2/djangomodelimport/loaders.py
+-rw-r--r--   0        0        0     7336 2022-11-14 01:42:13.378100 django_model_import-0.7.2/djangomodelimport/magic.py
+-rw-r--r--   0        0        0     2766 2022-11-10 00:29:59.378713 django_model_import-0.7.2/djangomodelimport/parsers.py
+-rw-r--r--   0        0        0     2703 2022-01-31 04:49:09.805613 django_model_import-0.7.2/djangomodelimport/resultset.py
+-rw-r--r--   0        0        0      612 2022-11-15 22:49:58.055999 django_model_import-0.7.2/djangomodelimport/utils.py
+-rw-r--r--   0        0        0     2541 2022-11-10 00:29:59.378882 django_model_import-0.7.2/djangomodelimport/widgets.py
+-rw-r--r--   0        0        0      876 2023-06-29 23:24:47.491625 django_model_import-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 django_model_import-0.7.2/PKG-INFO
```

### Comparing `django_model_import-0.7.1/README.md` & `django_model_import-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/core.py` & `django_model_import-0.7.2/djangomodelimport/core.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/fields.py` & `django_model_import-0.7.2/djangomodelimport/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,10 +218,10 @@
             value = json.dumps(value, sort_keys=True, indent=4)
         return super().render(name, value, attrs)
 
 
 class SourceFieldSwitcher(forms.Field):
     fields = None
 
-    def __init__(self, *fields: Iterable[Field]) -> None:
+    def __init__(self, *fields: Field, **kwargs: Any) -> None:
         self.fields = fields
-        super().__init__()
+        super().__init__(**kwargs)
```

### Comparing `django_model_import-0.7.1/djangomodelimport/formclassbuilder.py` & `django_model_import-0.7.2/djangomodelimport/formclassbuilder.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/forms.py` & `django_model_import-0.7.2/djangomodelimport/forms.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/loaders.py` & `django_model_import-0.7.2/djangomodelimport/loaders.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/magic.py` & `django_model_import-0.7.2/djangomodelimport/magic.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/parsers.py` & `django_model_import-0.7.2/djangomodelimport/parsers.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/resultset.py` & `django_model_import-0.7.2/djangomodelimport/resultset.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/utils.py` & `django_model_import-0.7.2/djangomodelimport/utils.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/djangomodelimport/widgets.py` & `django_model_import-0.7.2/djangomodelimport/widgets.py`

 * *Files identical despite different names*

### Comparing `django_model_import-0.7.1/pyproject.toml` & `django_model_import-0.7.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-model-import"
-version = "0.7.1"
+version = "0.7.2"
 description = "A Django library for importing CSVs and other structured data quickly using Django's ModelForm for validation and deserialisation into an instance."
 authors = ["Aidan Lister <aidan@uptickhq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/uptick/django-model-import"
 repository = "https://github.com/uptick/django-model-import"
 documentation = "https://github.com/uptick/django-model-import/tree/master/tests/djangoexample"
```

### Comparing `django_model_import-0.7.1/PKG-INFO` & `django_model_import-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-import
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Django library for importing CSVs and other structured data quickly using Django's ModelForm for validation and deserialisation into an instance.
 Home-page: https://github.com/uptick/django-model-import
 License: MIT
 Author: Aidan Lister
 Author-email: aidan@uptickhq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

