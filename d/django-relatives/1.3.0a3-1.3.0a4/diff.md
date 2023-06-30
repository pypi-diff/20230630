# Comparing `tmp/django-relatives-1.3.0a3.tar.gz` & `tmp/django-relatives-1.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-relatives-1.3.0a3.tar", last modified: Thu Sep 30 19:13:37 2021, max compression
+gzip compressed data, was "django-relatives-1.3.0a4.tar", last modified: Fri Jun 30 06:22:39 2023, max compression
```

## Comparing `django-relatives-1.3.0a3.tar` & `django-relatives-1.3.0a4.tar`

### file list

```diff
@@ -1,60 +1,28 @@
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/
--rw-r--r--   0 trey      (1001) trey      (1001)      142 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/AUTHORS.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)     1296 2021-09-30 18:46:25.000000 django-relatives-1.3.0a3/CHANGES.rst
--rw-rw-r--   0 trey      (1001) trey      (1001)      948 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/CONTRIBUTING.rst
--rw-r--r--   0 trey      (1001) trey      (1001)     1084 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/LICENSE
--rw-r--r--   0 trey      (1001) trey      (1001)      170 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/MANIFEST.in
--rw-rw-r--   0 trey      (1001) trey      (1001)     4641 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/PKG-INFO
--rw-rw-r--   0 trey      (1001) trey      (1001)     2453 2021-09-14 21:20:00.000000 django-relatives-1.3.0a3/README.rst
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.749757 django-relatives-1.3.0a3/django_relatives.egg-info/
--rw-rw-r--   0 trey      (1001) trey      (1001)     4641 2021-09-30 19:13:37.000000 django-relatives-1.3.0a3/django_relatives.egg-info/PKG-INFO
--rw-rw-r--   0 trey      (1001) trey      (1001)     1349 2021-09-30 19:13:37.000000 django-relatives-1.3.0a3/django_relatives.egg-info/SOURCES.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)        1 2021-09-30 19:13:37.000000 django-relatives-1.3.0a3/django_relatives.egg-info/dependency_links.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)       13 2021-09-30 19:13:37.000000 django-relatives-1.3.0a3/django_relatives.egg-info/requires.txt
--rw-rw-r--   0 trey      (1001) trey      (1001)       10 2021-09-30 19:13:37.000000 django-relatives-1.3.0a3/django_relatives.egg-info/top_level.txt
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.749757 django-relatives-1.3.0a3/docs/
--rw-r--r--   0 trey      (1001) trey      (1001)      204 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/api.rst
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/docs/images/
--rw-r--r--   0 trey      (1001) trey      (1001)    14727 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/images/contents_or_fk_link_example.png
--rw-r--r--   0 trey      (1001) trey      (1001)    20610 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/images/object_edit_link_example.png
--rw-r--r--   0 trey      (1001) trey      (1001)    15749 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/images/object_link_example.png
--rw-r--r--   0 trey      (1001) trey      (1001)    12565 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/images/related_objects_example.png
--rw-r--r--   0 trey      (1001) trey      (1001)      754 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/index.rst
--rw-r--r--   0 trey      (1001) trey      (1001)     4983 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/docs/usage.rst
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/
--rw-rw-r--   0 trey      (1001) trey      (1001)       25 2021-09-30 19:13:17.000000 django-relatives-1.3.0a3/relatives/__init__.py
--rw-r--r--   0 trey      (1001) trey      (1001)      611 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/compat.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.749757 django-relatives-1.3.0a3/relatives/static/
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/static/css/
--rw-r--r--   0 trey      (1001) trey      (1001)      306 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/static/css/relatives.css
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.749757 django-relatives-1.3.0a3/relatives/templates/
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/templates/relatives/
--rw-rw-r--   0 trey      (1001) trey      (1001)      660 2021-09-15 22:57:28.000000 django-relatives-1.3.0a3/relatives/templates/relatives/change_form.html
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/templates/relatives/includes/
--rw-r--r--   0 trey      (1001) trey      (1001)     1444 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/templates/relatives/includes/fieldset.html
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/templatetags/
--rw-r--r--   0 trey      (1001) trey      (1001)        0 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/templatetags/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     3218 2021-09-30 19:12:55.000000 django-relatives-1.3.0a3/relatives/templatetags/relatives.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/tests/
--rw-r--r--   0 trey      (1001) trey      (1001)        0 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)      999 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/relatives/tests/admin.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/tests/migrations/
--rw-r--r--   0 trey      (1001) trey      (1001)     3867 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/migrations/0001_initial.py
--rw-r--r--   0 trey      (1001) trey      (1001)      677 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/migrations/0002_shape.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     2735 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/relatives/tests/migrations/0003_auto_20210927_1618.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     1113 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/relatives/tests/migrations/0004_eater_meal.py
--rw-r--r--   0 trey      (1001) trey      (1001)        0 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/migrations/__init__.py
--rw-rw-r--   0 trey      (1001) trey      (1001)     3088 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/relatives/tests/models.py
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/tests/templates/
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.749757 django-relatives-1.3.0a3/relatives/tests/templates/admin/
-drwxrwxr-x   0 trey      (1001) trey      (1001)        0 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/relatives/tests/templates/admin/includes/
--rw-r--r--   0 trey      (1001) trey      (1001)       49 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/templates/admin/includes/fieldset.html
--rw-rw-r--   0 trey      (1001) trey      (1001)      221 2021-09-27 23:49:38.000000 django-relatives-1.3.0a3/relatives/tests/templates/related_objects_fk_test.html
--rw-r--r--   0 trey      (1001) trey      (1001)      187 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/templates/related_objects_generic_test.html
--rw-r--r--   0 trey      (1001) trey      (1001)      187 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/templates/related_objects_m2m_test.html
--rw-rw-r--   0 trey      (1001) trey      (1001)     9456 2021-09-30 19:07:04.000000 django-relatives-1.3.0a3/relatives/tests/tests.py
--rw-r--r--   0 trey      (1001) trey      (1001)      141 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/tests/urls.py
--rw-r--r--   0 trey      (1001) trey      (1001)     4306 2021-01-18 20:29:36.000000 django-relatives-1.3.0a3/relatives/utils.py
--rwxrwxr-x   0 trey      (1001) trey      (1001)     2425 2021-09-14 21:20:00.000000 django-relatives-1.3.0a3/runtests.py
--rw-r--r--   0 trey      (1001) trey      (1001)      237 2021-09-30 19:13:37.753757 django-relatives-1.3.0a3/setup.cfg
--rw-rw-r--   0 trey      (1001) trey      (1001)     1238 2021-09-14 21:20:00.000000 django-relatives-1.3.0a3/setup.py
+-rw-r--r--   0        0        0      142 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/AUTHORS.rst
+-rw-r--r--   0        0        0     1084 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/LICENSE
+-rw-r--r--   0        0        0     2840 2023-06-30 06:14:24.506582 django-relatives-1.3.0a4/README.rst
+-rw-r--r--   0        0        0     1261 2023-06-30 06:14:24.542582 django-relatives-1.3.0a4/pyproject.toml
+-rw-r--r--   0        0        0      289 2023-06-30 05:44:12.855776 django-relatives-1.3.0a4/relatives/__init__.py
+-rw-r--r--   0        0        0     1114 2023-06-30 06:14:24.506582 django-relatives-1.3.0a4/relatives/model_admin.py
+-rw-r--r--   0        0        0      306 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/static/css/relatives.css
+-rw-r--r--   0        0        0     2549 2023-06-30 06:14:24.506582 django-relatives-1.3.0a4/relatives/template_helpers.py
+-rw-r--r--   0        0        0      660 2021-09-15 22:57:28.415756 django-relatives-1.3.0a4/relatives/templates/relatives/change_form.html
+-rw-r--r--   0        0        0     1444 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/templates/relatives/includes/fieldset.html
+-rw-r--r--   0        0        0        0 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/templatetags/__init__.py
+-rw-r--r--   0        0        0     3303 2023-06-30 06:14:24.506582 django-relatives-1.3.0a4/relatives/templatetags/relatives.py
+-rw-r--r--   0        0        0        0 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/tests/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/admin.py
+-rw-r--r--   0        0        0     6499 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      676 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/migrations/0002_shape.py
+-rw-r--r--   0        0        0     3094 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/migrations/0003_auto_20210927_1618.py
+-rw-r--r--   0        0        0     1776 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/migrations/0004_eater_meal.py
+-rw-r--r--   0        0        0        0 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/tests/migrations/__init__.py
+-rw-r--r--   0        0        0     3102 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/models.py
+-rw-r--r--   0        0        0       49 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/tests/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0      221 2021-09-27 23:49:38.497641 django-relatives-1.3.0a4/relatives/tests/templates/related_objects_fk_test.html
+-rw-r--r--   0        0        0      187 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/tests/templates/related_objects_generic_test.html
+-rw-r--r--   0        0        0      187 2021-01-18 20:29:36.812790 django-relatives-1.3.0a4/relatives/tests/templates/related_objects_m2m_test.html
+-rw-r--r--   0        0        0     9788 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/tests.py
+-rw-r--r--   0        0        0      139 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/tests/urls.py
+-rw-r--r--   0        0        0     1628 2023-06-30 06:14:24.510582 django-relatives-1.3.0a4/relatives/utils.py
+-rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 django-relatives-1.3.0a4/PKG-INFO
```

### Comparing `django-relatives-1.3.0a3/LICENSE` & `django-relatives-1.3.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-relatives-1.3.0a3/README.rst` & `django-relatives-1.3.0a4/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 ================
 django-relatives
 ================
 
-.. image:: https://travis-ci.org/treyhunner/django-relatives.png?branch=master
-   :target: https://travis-ci.org/treyhunner/django-relatives
-   :alt: Test Status
-
-.. image:: https://coveralls.io/repos/treyhunner/django-relatives/badge.png?branch=master
-   :target: https://coveralls.io/r/treyhunner/django-relatives
-   :alt: Coverage Status
-
-.. image:: https://pypip.in/v/django-relatives/badge.png
-   :target: https://crate.io/packages/django-relatives
-   :alt: Latest Version
-
-.. image:: https://pypip.in/d/django-relatives/badge.png
-   :target: https://crate.io/packages/django-relatives
-   :alt: Download Count
+.. image:: https://img.shields.io/pypi/v/django-relatives.svg
+   :target: https://pypi.org/project/django-relatives/
+   :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/pyversions/django-relatives
+   :target: https://pypi.org/project/django-relatives
+   :alt: Python Version
+
+.. image:: https://img.shields.io/pypi/djversions/django-relatives
+   :target: https://pypi.org/project/django-relatives
+   :alt: Django Version
+
+.. image:: https://img.shields.io/readthedocs/django-relatives/latest.svg?label=Read%20the%20Docs
+   :target: https://django-relatives.readthedocs.io/
+   :alt: Read the documentation at https://django-relatives.readthedocs.io/
+
+.. image:: https://github.com/treyhunner/django-relatives/workflows/Tests/badge.svg
+   :target: https://github.com/treyhunner/django-relatives/actions?workflow=Tests
+   :alt: Tests
+
+.. image:: https://codecov.io/gh/treyhunner/django-relatives/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/treyhunner/django-relatives
+   :alt: Codecov
 
 Utilities for linking to related objects in Django admin
 
-This app requires Django 2.2 or greater and Python 3.6 or greater.
+This app requires Django 3.2 or greater and Python 3.8 or greater.
 
 
 Getting Help
 ------------
 
 Documentation for django-relatives is available at
 https://django-relatives.readthedocs.org/
```

### Comparing `django-relatives-1.3.0a3/relatives/templates/relatives/change_form.html` & `django-relatives-1.3.0a4/relatives/templates/relatives/change_form.html`

 * *Files identical despite different names*

### Comparing `django-relatives-1.3.0a3/relatives/templates/relatives/includes/fieldset.html` & `django-relatives-1.3.0a4/relatives/templates/relatives/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-relatives-1.3.0a3/relatives/templatetags/relatives.py` & `django-relatives-1.3.0a4/relatives/templatetags/relatives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from django.template import Library
 from django.urls import reverse, NoReverseMatch
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 from django.utils.safestring import mark_safe
 from django.contrib.admin.utils import lookup_field
 from django.core.exceptions import ObjectDoesNotExist
 
-from ..utils import get_admin_url, GenericObjects
+from ..template_helpers import GenericObjects
+from ..utils import get_admin_url
 
 
 register = Library()
 
 
 @register.filter
 def contents_or_fk_link(field):
@@ -18,29 +19,31 @@
 
     Example Usage::
 
         {% load relatives %}
         {{ field|contents_or_fk_link }}
     """
     contents = field.contents()
-    field_name = field.field['field']
+    field_name = field.field["field"]
     obj = field.form.instance
     if not isinstance(field_name, str):
         return contents
     try:
         related_obj = getattr(obj, field_name)
     except (AttributeError, ObjectDoesNotExist):
         return contents
     else:
         model_field, _, _ = lookup_field(field_name, obj, field.model_admin)
-        if ((model_field is None or model_field.remote_field)
-                and hasattr(related_obj, '_meta')):
+        if (model_field is None or model_field.remote_field) and hasattr(
+            related_obj, "_meta"
+        ):
             try:
-                return mark_safe('<a href="%s">%s</a>' %
-                                 (get_admin_url(related_obj), contents))
+                return mark_safe(
+                    '<a href="%s">%s</a>' % (get_admin_url(related_obj), contents)
+                )
             except NoReverseMatch:
                 pass
         return contents
 
 
 @register.simple_tag
 def related_objects(obj):
@@ -56,40 +59,46 @@
         {% endfor %}
     """
     object_list = []
     all_related_objects = [
         field
         for field in obj._meta.get_fields()
         if (field.one_to_many or field.one_to_one)
-        and field.auto_created and not field.concrete
+        and field.auto_created
+        and not field.concrete
     ]
     all_related_m2m_objects = [
         field
         for field in obj._meta.get_fields(include_hidden=True)
         if field.many_to_many and field.auto_created
     ]
-    related_objects = (all_related_objects
-                       + all_related_m2m_objects
-                       + GenericObjects(obj).get_generic_objects())
+    related_objects = (
+        all_related_objects
+        + all_related_m2m_objects
+        + GenericObjects(obj).get_generic_objects()
+    )
     for related in related_objects:
         try:
-            to_model = getattr(related, 'related_model', related.model)
-            url = reverse('admin:{0}_{1}_changelist'.format(
-                to_model._meta.app_label,
-                to_model._meta.model_name
-            ))
+            to_model = getattr(related, "related_model", related.model)
+            url = reverse(
+                "admin:{0}_{1}_changelist".format(
+                    to_model._meta.app_label, to_model._meta.model_name
+                )
+            )
         except NoReverseMatch:
             continue
-        if getattr(related, 'related_name', None):
+        if getattr(related, "related_name", None):
             plural_name = related.related_name.replace("_", " ")
         else:
             plural_name = to_model._meta.verbose_name_plural
         field = related.field.name
-        if hasattr(related.field, 'm2m_reverse_target_field_name'):
+        if hasattr(related.field, "m2m_reverse_target_field_name"):
             field += "__" + related.field.m2m_reverse_target_field_name()
-        elif hasattr(related.field, 'target_field'):
+        elif hasattr(related.field, "target_field"):
             field += "__" + "".join(related.target_field.name)
-        object_list.append({
-            'plural_name': plural_name,
-            'url': smart_text(f"{url}?{field}__exact={obj.pk}"),
-        })
+        object_list.append(
+            {
+                "plural_name": plural_name,
+                "url": smart_str(f"{url}?{field}__exact={obj.pk}"),
+            }
+        )
     return object_list
```

### Comparing `django-relatives-1.3.0a3/relatives/tests/admin.py` & `django-relatives-1.3.0a4/relatives/tests/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from django.contrib import admin
 
+from .. import RelativesAdmin
 from . import models
 
 
 class ShapeAdmin(admin.ModelAdmin):
-    readonly_fields = ['name', 'lower_name', 'upper_name']
+    readonly_fields = ["name", "lower_name", "upper_name"]
 
     def upper_name(self, obj):
         return obj.name.upper()
 
 
 admin.site.register(models.Shape, ShapeAdmin)
 
 
 class ShipAdmin(admin.ModelAdmin):
-    change_form_template = 'relatives/change_form.html'
-    readonly_fields = ['name']
+    change_form_template = "relatives/change_form.html"
+    readonly_fields = ["name"]
 
 
 admin.site.register(models.Ship, ShipAdmin)
 
 
-class SailorAdmin(admin.ModelAdmin):
-    readonly_fields = ['ship']
+class SailorAdmin(RelativesAdmin):
+    readonly_fields = ["ship"]
+    list_display = ["name", "ship", "ship_name"]
 
 
 admin.site.register(models.Sailor, SailorAdmin)
 
 
 class PetAdmin(admin.ModelAdmin):
-    readonly_fields = ['owner']
+    readonly_fields = ["owner"]
 
 
 admin.site.register(models.Pet, PetAdmin)
 
 
 class ImageAdmin(admin.ModelAdmin):
-    readonly_fields = ['content_object']
+    readonly_fields = ["content_object"]
 
 
 admin.site.register(models.Image, ImageAdmin)
 
 
 admin.site.register(models.Movie)
 admin.site.register(models.Actor)
```

### Comparing `django-relatives-1.3.0a3/relatives/tests/migrations/0003_auto_20210927_1618.py` & `django-relatives-1.3.0a4/relatives/tests/migrations/0003_auto_20210927_1618.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,96 @@
 # Generated by Django 3.2.7 on 2021-09-27 16:18
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('tests', '0002_shape'),
+        ("tests", "0002_shape"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='actor',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="actor",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='book',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="book",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='image',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="image",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='journal',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="journal",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='movie',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="movie",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='notinadmin',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="notinadmin",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='pet',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="pet",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='pirate',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="pirate",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='sailor',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="sailor",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='shape',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="shape",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='ship',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="ship",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
         migrations.AlterField(
-            model_name='something',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="something",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
     ]
```

### Comparing `django-relatives-1.3.0a3/relatives/tests/models.py` & `django-relatives-1.3.0a4/relatives/tests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from __future__ import unicode_literals
-
 from django.db import models
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.contenttypes.fields import (
-    GenericForeignKey, GenericRelation
-)
+from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 
 
 class Pirate(models.Model):
 
     """Pirates have no admin URL"""
 
     name = models.CharField(max_length=80)
@@ -37,24 +33,28 @@
 class Sailor(models.Model):
 
     """Sailors have an admin URL and sometimes link to ships"""
 
     name = models.CharField(max_length=80)
     ship = models.ForeignKey(Ship, null=True, on_delete=models.SET_NULL)
 
+    @property
+    def ship_name(self):
+        self.ship.name
+
     def __str__(self):
         return self.name
 
 
 class Actor(models.Model):
 
     """Actors have an admin URL and a many-to-many relationship with movies"""
 
     name = models.CharField(max_length=80)
-    movies = models.ManyToManyField('Movie', related_name='actors')
+    movies = models.ManyToManyField("Movie", related_name="actors")
 
 
 class Movie(models.Model):
 
     """Movies have an admin URL and are linked to (m2m) by actors"""
 
     name = models.CharField(max_length=80)
@@ -94,15 +94,15 @@
 
 class Image(models.Model):
 
     """Image have an admin URL and link to Book via GenericForeignKey"""
 
     ct = models.ForeignKey(ContentType, on_delete=models.CASCADE, null=True)
     obj_id = models.PositiveIntegerField(null=True)
-    content_object = GenericForeignKey('ct', 'obj_id')
+    content_object = GenericForeignKey("ct", "obj_id")
 
 
 class Journal(models.Model):
 
     """Journal have an admin URL and are linked to images via GenericForeignKey
     also it have GenericRelation link to Images"""
```

### Comparing `django-relatives-1.3.0a3/relatives/tests/tests.py` & `django-relatives-1.3.0a4/relatives/tests/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,48 +3,63 @@
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
 from django.core.cache import cache
 
 from relatives.utils import object_link, object_edit_link
-from .models import (Pirate, Pet, Ship, Sailor, Movie, Actor, NotInAdmin,
-                     Shape, Something, Book, Image, Journal, Eater)
+from .models import (
+    Pirate,
+    Pet,
+    Ship,
+    Sailor,
+    Movie,
+    Actor,
+    NotInAdmin,
+    Shape,
+    Something,
+    Book,
+    Image,
+    Journal,
+    Eater,
+)
 
 
 class ObjectEditLinkTest(TestCase):
-
     def test_default(self):
         ship = Ship.objects.create(id=1, name="Star of India")
         self.assertEqual(
             object_edit_link()(ship),
             '<a href="/adm/tests/ship/1/change/">Star of India</a>',
         )
         pirate = Pirate.objects.create(id=1, name="Lowell Taylor")
         self.assertEqual(object_edit_link()(pirate), "Lowell Taylor")
 
     def test_custom_edit_text(self):
         ship = Ship.objects.create(id=1, name="Star of India")
-        self.assertEqual(object_edit_link("Go There")(ship),
-                         '<a href="/adm/tests/ship/1/change/">Go There</a>')
+        self.assertEqual(
+            object_edit_link("Go There")(ship),
+            '<a href="/adm/tests/ship/1/change/">Go There</a>',
+        )
 
     def test_default_blank_text(self):
         pirate = Pirate.objects.create(id=1, name="Lowell Taylor")
         self.assertEqual(object_edit_link("Edit")(pirate), "")
 
     def test_custom_edit_and_blank_text(self):
         ship = Ship.objects.create(id=1, name="Star of India")
         pirate = Pirate.objects.create(id=1, name="Lowell Taylor")
-        self.assertEqual(object_edit_link("Go There", "N/A")(ship),
-                         '<a href="/adm/tests/ship/1/change/">Go There</a>')
+        self.assertEqual(
+            object_edit_link("Go There", "N/A")(ship),
+            '<a href="/adm/tests/ship/1/change/">Go There</a>',
+        )
         self.assertEqual(object_edit_link("Go There", "N/A")(pirate), "N/A")
 
 
 class ObjectLinkTest(TestCase):
-
     def test_no_admin_url(self):
         pirate = Pirate.objects.create(id=1, name="Lowell Taylor")
         self.assertEqual(object_link(pirate), "Lowell Taylor")
 
     def test_with_primary_key(self):
         ship = Ship.objects.create(id=1, name="Star of India")
         self.assertEqual(
@@ -55,175 +70,187 @@
     def test_no_primary_key(self):
         ship = Ship(name="Star of India")
         self.assertEqual(object_link(ship), "Star of India")
 
 
 class TemplateFilterTest(TestCase):
     def setUp(self):
-        self.user = User.objects.create_superuser('u', 'u@example.com', 'pass')
+        self.user = User.objects.create_superuser("u", "u@example.com", "pass")
 
     def login(self):
-        self.client.login(username=self.user.username, password='pass')
+        self.client.login(username=self.user.username, password="pass")
 
     def test_foreign_key(self):
         self.login()
         ship = Ship.objects.create(id=1, name="Star of India")
         sailor = Sailor.objects.create(name="John Ford", ship=ship)
-        response = self.client.get(reverse('admin:tests_sailor_change',
-                                           args=[sailor.id]))
-        self.assertIn(b'<a href="/adm/tests/ship/1/change/">Star of India</a>',
-                      response.content)
+        response = self.client.get(
+            reverse("admin:tests_sailor_change", args=[sailor.id])
+        )
+        self.assertIn(
+            b'<a href="/adm/tests/ship/1/change/">Star of India</a>', response.content
+        )
 
     def test_property_and_modeladmin_method(self):
         self.login()
         circle = Shape.objects.create(id=1, name="Circle")
-        response = self.client.get(reverse('admin:tests_shape_change',
-                                           args=[circle.id]))
-        self.assertIn(b'<p>Circle</p>', response.content)
-        self.assertIn(b'<p>circle</p>', response.content)
-        self.assertIn(b'<p>CIRCLE</p>', response.content)
+        response = self.client.get(
+            reverse("admin:tests_shape_change", args=[circle.id])
+        )
+        self.assertIn(b"<p>Circle</p>", response.content)
+        self.assertIn(b"<p>circle</p>", response.content)
+        self.assertIn(b"<p>CIRCLE</p>", response.content)
 
     def test_no_foreign_key(self):
         self.login()
         ship = Ship.objects.create(id=1, name="Star of India")
-        response = self.client.get(reverse('admin:tests_ship_change',
-                                           args=[ship.id]))
-        self.assertIn(b'<p>Star of India</p>', response.content)
+        response = self.client.get(reverse("admin:tests_ship_change", args=[ship.id]))
+        self.assertIn(b"<p>Star of India</p>", response.content)
 
     def test_foreign_key_without_admin_url(self):
         self.login()
         pirate = Pirate.objects.create(id=1, name="Kristi Bell")
         pet = Pet.objects.create(owner=pirate)
-        response = self.client.get(reverse('admin:tests_pet_change',
-                                           args=[pet.id]))
-        self.assertIn(b'Kristi Bell', response.content)
-        self.assertNotIn(b'Kristi Bell</a>', response.content)
-        self.assertNotIn(b'Kristi Bell</option>', response.content)
+        response = self.client.get(reverse("admin:tests_pet_change", args=[pet.id]))
+        self.assertIn(b"Kristi Bell", response.content)
+        self.assertNotIn(b"Kristi Bell</a>", response.content)
+        self.assertNotIn(b"Kristi Bell</option>", response.content)
 
     def test_nullable_foreign_key(self):
         self.login()
         sailor = Sailor.objects.create(name="John Ford")
-        response = self.client.get(reverse('admin:tests_sailor_change',
-                                           args=[sailor.id]))
-        self.assertIn(b'<p>-</p>', response.content)
+        response = self.client.get(
+            reverse("admin:tests_sailor_change", args=[sailor.id])
+        )
+        self.assertIn(b"<p>-</p>", response.content)
 
     def test_deleted_foreign_key(self):
         self.login()
         ship = Ship.objects.create(id=1, name="Star of India")
         sailor = Sailor.objects.create(name="John Ford", ship=ship)
         ship.delete()  # Sailor won't get deleted
-        response = self.client.get(reverse('admin:tests_sailor_change',
-                                           args=[sailor.id]))
-        self.assertIn(b'<p>-</p>', response.content)
+        response = self.client.get(
+            reverse("admin:tests_sailor_change", args=[sailor.id])
+        )
+        self.assertIn(b"<p>-</p>", response.content)
 
     def test_add_form_for_non_nullable_fk(self):
         self.login()
-        response = self.client.get(reverse('admin:tests_pet_add'))
-        self.assertIn(b'<p>-</p>', response.content)
+        response = self.client.get(reverse("admin:tests_pet_add"))
+        self.assertIn(b"<p>-</p>", response.content)
 
     def test_generic_foreign_key_present(self):
         book = Book.objects.create(name="Django")
         image = Image.objects.create(content_object=book)
         self.login()
-        response = self.client.get(
-            reverse('admin:tests_image_change', args=[image.id])
-        )
-        self.assertIn(f'/adm/tests/book/{book.id}', response.rendered_content)
-        self.assertIn(f'Book object ({book.id})', response.rendered_content)
-        self.assertNotIn('<p>None</p>', response.rendered_content)
+        response = self.client.get(reverse("admin:tests_image_change", args=[image.id]))
+        self.assertIn(f"/adm/tests/book/{book.id}", response.rendered_content)
+        self.assertIn(f"Book object ({book.id})", response.rendered_content)
+        self.assertNotIn("<p>None</p>", response.rendered_content)
 
     def test_generic_foreign_key_not_present(self):
         image = Image.objects.create()
         self.login()
-        response = self.client.get(
-            reverse('admin:tests_image_change', args=[image.id])
-        )
-        self.assertIn('<p>None</p>', response.rendered_content)
-        self.assertNotIn('Book object', response.rendered_content)
+        response = self.client.get(reverse("admin:tests_image_change", args=[image.id]))
+        self.assertIn("<p>None</p>", response.rendered_content)
+        self.assertNotIn("Book object", response.rendered_content)
 
 
 class RelatedObjectsTagTest(TestCase):
     def test_foreign_keys(self):
         ship = Ship.objects.create(id=1, name="Star of India")
-        body = render_to_string('related_objects_fk_test.html', {'obj': ship})
+        body = render_to_string("related_objects_fk_test.html", {"obj": ship})
         self.assertEqual(
             body.strip(),
             '<a href="/adm/tests/sailor/?ship__id__exact=1">Sailors</a>',
         )
 
     def test_two_foreign_keys(self):
         eater = Eater.objects.create(id=1, name="Cheryl")
-        body = render_to_string('related_objects_fk_test.html', {'obj': eater})
+        body = render_to_string("related_objects_fk_test.html", {"obj": eater})
         self.assertEqual(
             body.strip(),
             '<a href="/adm/tests/meal/?prepared__id__exact=1">'
-            'Meals prepared</a>'
+            "Meals prepared</a>"
             '<a href="/adm/tests/meal/?reviewed__id__exact=1">'
-            'Meals reviewed</a>',
+            "Meals reviewed</a>",
         )
 
     def test_no_admin_url(self):
         thing = Something.objects.create()
         NotInAdmin.objects.create(id=1, fk=thing)
-        body = render_to_string('related_objects_fk_test.html', {'obj': thing})
-        self.assertEqual(body.strip(), '')
+        body = render_to_string("related_objects_fk_test.html", {"obj": thing})
+        self.assertEqual(body.strip(), "")
 
     def test_many_to_many(self):
         movie = Movie.objects.create(id=1, name="Yojimbo")
         actor = Actor.objects.create(name="Tatsuya Nakadai")
         actor.movies.add(movie)
-        body = render_to_string('related_objects_m2m_test.html',
-                                {'obj': movie})
+        body = render_to_string("related_objects_m2m_test.html", {"obj": movie})
         self.assertEqual(
             body.strip(),
             '<a href="/adm/tests/actor/?movies__id__exact=1">Actors</a>',
         )
 
     def test_reverse_many_to_many(self):
         movie = Movie.objects.create(id=1, name="Yojimbo")
         actor = Actor.objects.create(name="Tatsuya Nakadai")
         actor.movies.add(movie)
-        body = render_to_string('related_objects_m2m_test.html',
-                                {'obj': actor})
-        self.assertEqual(body.strip(), '')
+        body = render_to_string("related_objects_m2m_test.html", {"obj": actor})
+        self.assertEqual(body.strip(), "")
 
     def test_generic_foreign_key_not(self):
         book = Book.objects.create(name="Django")
-        body = render_to_string('related_objects_generic_test.html',
-                                {'obj': book})
-        self.assertEqual(body.strip(), '')
+        body = render_to_string("related_objects_generic_test.html", {"obj": book})
+        self.assertEqual(body.strip(), "")
 
     def test_generic_foreign_key_present(self):
         book = Book.objects.create(name="Django")
         Image.objects.create(content_object=book)
         ct_pk = ContentType.objects.get_for_model(book).pk
         expected = (
             '<a href="/adm/tests/image/'
             f'?ct={ct_pk}&amp;obj_id__exact={book.pk}">Images</a>'
         )
         body = render_to_string(
-            'related_objects_generic_test.html',
-            {'obj': book},
+            "related_objects_generic_test.html",
+            {"obj": book},
         )
         self.assertEqual(body.strip(), expected)
 
     def test_generic_relation_and_gfk_present(self):
         journal = Journal.objects.create(name="Django")
         Image.objects.create(content_object=journal)
         ct_pk = ContentType.objects.get_for_model(journal).pk
         expected = (
             '<a href="/adm/tests/image/'
             f'?ct={ct_pk}&amp;obj_id__exact={journal.pk}">Images</a>'
         )
         body = render_to_string(
-            'related_objects_generic_test.html',
-            {'obj': journal},
+            "related_objects_generic_test.html",
+            {"obj": journal},
         )
         self.assertEqual(body.strip(), expected)
 
     def test_with_removed_model(self):
         cache.clear()
         journal = Journal()
-        ContentType.objects.create(model='gone', app_label='gone')
-        body = render_to_string('related_objects_generic_test.html',
-                                {'obj': journal})
-        self.assertEqual(body.strip(), '')
+        ContentType.objects.create(model="gone", app_label="gone")
+        body = render_to_string("related_objects_generic_test.html", {"obj": journal})
+        self.assertEqual(body.strip(), "")
+
+
+class RelativesAdminTests(TestCase):
+    def setUp(self):
+        self.user = User.objects.create_superuser("u", "u@example.com", "pass")
+
+    def login(self):
+        self.client.login(username=self.user.username, password="pass")
+
+    def test_foreign_key_in_change_list(self):
+        self.login()
+        ship = Ship.objects.create(id=1, name="Star of India")
+        Sailor.objects.create(name="John Ford", ship=ship)
+        response = self.client.get(reverse("admin:tests_sailor_changelist"))
+        self.assertIn(
+            b'<a href="/adm/tests/ship/1/change/">Star of India</a>', response.content
+        )
```

