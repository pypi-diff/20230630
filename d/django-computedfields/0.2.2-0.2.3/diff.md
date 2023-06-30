# Comparing `tmp/django-computedfields-0.2.2.tar.gz` & `tmp/django-computedfields-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-computedfields-0.2.2.tar", last modified: Thu Apr 13 14:26:14 2023, max compression
+gzip compressed data, was "dist/django-computedfields-0.2.3.tar", last modified: Fri Jun 30 11:58:09 2023, max compression
```

## Comparing `django-computedfields-0.2.2.tar` & `django-computedfields-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    40930 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/resolver.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/migrations/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      656 2020-04-24 12:52:14.000000 django-computedfields-0.2.2/computedfields/migrations/0001_initial.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      703 2020-04-24 12:52:14.000000 django-computedfields-0.2.2/computedfields/migrations/0002_contributingmodelsmodel.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/migrations/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      537 2020-07-14 19:41:57.000000 django-computedfields-0.2.2/computedfields/migrations/0003_auto_20200713_2212.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/management/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/management/__init__.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/management/commands/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/management/commands/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     9735 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/management/commands/updatedata.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1900 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/management/commands/showdependencies.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2063 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/management/commands/_helpers.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8420 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/management/commands/checkdata.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2367 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/computedfields/management/commands/rendergraph.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     9129 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/admin.py
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/templates/
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      991 2020-05-22 18:15:10.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/change_list.html
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      750 2020-05-22 18:15:10.000000 django-computedfields-0.2.2/computedfields/templates/computedfields/graph.html
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/static/
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/computedfields/static/computedfields/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)  1441964 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/computedfields/static/computedfields/viz-lite.js
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/__init__.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    35600 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/graph.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      902 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/settings.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5505 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/computedfields/models.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8633 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/computedfields/handlers.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     2751 2022-04-18 09:39:28.000000 django-computedfields-0.2.2/computedfields/helper.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1880 2022-04-17 14:52:45.000000 django-computedfields-0.2.2/computedfields/apps.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1834 2023-04-13 14:19:50.000000 django-computedfields-0.2.2/setup.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/setup.cfg
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/docs/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    30903 2022-08-03 15:44:26.000000 django-computedfields-0.2.2/docs/manual.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)    54109 2022-04-18 12:52:27.000000 django-computedfields-0.2.2/docs/examples.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      618 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/docs/Makefile
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2022-04-15 08:50:44.000000 django-computedfields-0.2.2/docs/reference.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2020-05-29 20:53:10.000000 django-computedfields-0.2.2/docs/index.rst
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5517 2022-01-26 15:45:25.000000 django-computedfields-0.2.2/docs/conf.py
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      789 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/docs/make.bat
-drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/
--rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/dependency_links.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1296 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/SOURCES.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8366 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       59 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/requires.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)       15 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/django_computedfields.egg-info/top_level.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)      150 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/MANIFEST.in
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     1023 2019-03-10 14:07:26.000000 django-computedfields-0.2.2/LICENSE.txt
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     8366 2023-04-13 14:26:14.000000 django-computedfields-0.2.2/PKG-INFO
--rw-rw-r--   0 jerch     (1000) jerch     (1000)     5912 2023-04-13 14:04:02.000000 django-computedfields-0.2.2/README.md
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    41036 2023-06-30 11:49:11.000000 django-computedfields-0.2.3/computedfields/resolver.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/migrations/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      656 2020-04-24 12:52:14.000000 django-computedfields-0.2.3/computedfields/migrations/0001_initial.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      703 2020-04-24 12:52:14.000000 django-computedfields-0.2.3/computedfields/migrations/0002_contributingmodelsmodel.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/computedfields/migrations/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      537 2020-07-14 19:41:57.000000 django-computedfields-0.2.3/computedfields/migrations/0003_auto_20200713_2212.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/management/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/computedfields/management/__init__.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/management/commands/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        0 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/computedfields/management/commands/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     9735 2023-04-13 14:04:02.000000 django-computedfields-0.2.3/computedfields/management/commands/updatedata.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1900 2022-04-17 14:52:45.000000 django-computedfields-0.2.3/computedfields/management/commands/showdependencies.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2063 2022-04-17 14:52:45.000000 django-computedfields-0.2.3/computedfields/management/commands/_helpers.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8420 2023-04-13 14:04:02.000000 django-computedfields-0.2.3/computedfields/management/commands/checkdata.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2367 2022-04-15 08:50:44.000000 django-computedfields-0.2.3/computedfields/management/commands/rendergraph.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     9129 2023-04-13 14:04:02.000000 django-computedfields-0.2.3/computedfields/admin.py
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/templates/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/templates/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      991 2020-05-22 18:15:10.000000 django-computedfields-0.2.3/computedfields/templates/computedfields/change_list.html
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      750 2020-05-22 18:15:10.000000 django-computedfields-0.2.3/computedfields/templates/computedfields/graph.html
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/static/
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/computedfields/static/computedfields/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)  1441964 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/computedfields/static/computedfields/viz-lite.js
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       22 2023-06-30 11:53:22.000000 django-computedfields-0.2.3/computedfields/__init__.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    35600 2023-04-13 14:04:02.000000 django-computedfields-0.2.3/computedfields/graph.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      902 2022-04-17 14:52:45.000000 django-computedfields-0.2.3/computedfields/settings.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5505 2022-04-15 08:50:44.000000 django-computedfields-0.2.3/computedfields/models.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8633 2023-04-13 14:04:02.000000 django-computedfields-0.2.3/computedfields/handlers.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     2751 2022-04-18 09:39:28.000000 django-computedfields-0.2.3/computedfields/helper.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1880 2022-04-17 14:52:45.000000 django-computedfields-0.2.3/computedfields/apps.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1834 2023-06-30 11:53:36.000000 django-computedfields-0.2.3/setup.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       79 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/setup.cfg
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/docs/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    31084 2023-06-30 11:56:04.000000 django-computedfields-0.2.3/docs/manual.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)    54109 2022-04-18 12:52:27.000000 django-computedfields-0.2.3/docs/examples.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      618 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/docs/Makefile
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2022-04-15 08:50:44.000000 django-computedfields-0.2.3/docs/reference.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      512 2020-05-29 20:53:10.000000 django-computedfields-0.2.3/docs/index.rst
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     5517 2022-01-26 15:45:25.000000 django-computedfields-0.2.3/docs/conf.py
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      789 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/docs/make.bat
+drwxrwxr-x   0 jerch     (1000) jerch     (1000)        0 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)        1 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1296 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8480 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       59 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/requires.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)       15 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/django_computedfields.egg-info/top_level.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)      150 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/MANIFEST.in
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     1023 2019-03-10 14:07:26.000000 django-computedfields-0.2.3/LICENSE.txt
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     8480 2023-06-30 11:58:09.000000 django-computedfields-0.2.3/PKG-INFO
+-rw-rw-r--   0 jerch     (1000) jerch     (1000)     6002 2023-06-30 11:53:10.000000 django-computedfields-0.2.3/README.md
```

### Comparing `django-computedfields-0.2.2/computedfields/resolver.py` & `django-computedfields-0.2.3/computedfields/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                 m_fields, m_paths = model_updates.setdefault(model, (set(), set()))
                 m_fields.update(fields)
                 m_paths.update(paths)
         for model, data in model_updates.items():
             fields, paths = data
             queryset: Any = model._base_manager.none()
             for path in paths:
-                queryset |= model._base_manager.filter(**{path+subquery: instance})
+                queryset = queryset.union(model._base_manager.filter(**{path+subquery: instance}))
             if pk_list:
                 # need pks for post_delete since the real queryset will be empty
                 # after deleting the instance in question
                 # since we need to interact with the db anyways
                 # we can already drop empty results here
                 queryset = set(queryset.values_list('pk', flat=True).iterator())
                 if not queryset:
@@ -512,15 +512,16 @@
         # distinct issue workaround
         # the workaround is needed for already sliced/distinct querysets coming from outside
         # TODO: distinct is a major query perf smell, and is in fact only needed on back relations
         #       may need some rework in _querysets_for_update
         #       ideally we find a way to avoid it for forward relations
         #       also see #101
         if queryset.query.can_filter() and not queryset.query.distinct_fields:
-            queryset = queryset.distinct()
+            if queryset.query.combinator != "union":
+                queryset = queryset.distinct()
         else:
             queryset = model._base_manager.filter(pk__in=subquery_pk(queryset, queryset.db))
 
         # correct update_fields by local mro
         mro = self.get_local_mro(model, update_fields)
         fields: Any = set(mro)  # FIXME: narrow type once issue in django-stubs is resolved
         if update_fields:
@@ -546,18 +547,18 @@
                     if new_value != getattr(elem, comp_field):
                         has_changed = True
                         setattr(elem, comp_field, new_value)
                 if has_changed:
                     change.append(elem)
                     pks.append(elem.pk)
                 if len(change) >= self._batchsize:
-                    self._update(queryset, change, fields)
+                    self._update(model._base_manager.all(), change, fields)
                     change = []
             if change:
-                self._update(queryset, change, fields)
+                self._update(model._base_manager.all(), change, fields)
 
         # trigger dependent comp field updates from changed records
         # other than before we exit the update tree early, if we have no changes at all
         # also cuts the update tree for recursive deps (tree-like)
         if not local_only and pks:
             self.update_dependent(model._base_manager.filter(pk__in=pks), model, fields, update_local=False)
         return set(pks) if return_pks else None
```

### Comparing `django-computedfields-0.2.2/computedfields/migrations/0001_initial.py` & `django-computedfields-0.2.3/computedfields/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/migrations/0002_contributingmodelsmodel.py` & `django-computedfields-0.2.3/computedfields/migrations/0002_contributingmodelsmodel.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/migrations/0003_auto_20200713_2212.py` & `django-computedfields-0.2.3/computedfields/migrations/0003_auto_20200713_2212.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/management/commands/updatedata.py` & `django-computedfields-0.2.3/computedfields/management/commands/updatedata.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/management/commands/showdependencies.py` & `django-computedfields-0.2.3/computedfields/management/commands/showdependencies.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/management/commands/_helpers.py` & `django-computedfields-0.2.3/computedfields/management/commands/_helpers.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/management/commands/checkdata.py` & `django-computedfields-0.2.3/computedfields/management/commands/checkdata.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/management/commands/rendergraph.py` & `django-computedfields-0.2.3/computedfields/management/commands/rendergraph.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/admin.py` & `django-computedfields-0.2.3/computedfields/admin.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/templates/computedfields/change_list.html` & `django-computedfields-0.2.3/computedfields/templates/computedfields/change_list.html`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/templates/computedfields/graph.html` & `django-computedfields-0.2.3/computedfields/templates/computedfields/graph.html`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/static/computedfields/viz-lite.js` & `django-computedfields-0.2.3/computedfields/static/computedfields/viz-lite.js`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/graph.py` & `django-computedfields-0.2.3/computedfields/graph.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/settings.py` & `django-computedfields-0.2.3/computedfields/settings.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/models.py` & `django-computedfields-0.2.3/computedfields/models.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/handlers.py` & `django-computedfields-0.2.3/computedfields/handlers.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/helper.py` & `django-computedfields-0.2.3/computedfields/helper.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/computedfields/apps.py` & `django-computedfields-0.2.3/computedfields/apps.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/setup.py` & `django-computedfields-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     license='MIT',
     description='autoupdated database fields for model methods',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='netzkolchose',
     author_email='j.breitbart@netzkolchose.de',
     url='https://github.com/netzkolchose/django-computedfields',
-    download_url='https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz',
+    download_url='https://github.com/netzkolchose/django-computedfields/archive/0.2.3.tar.gz',
     keywords=['django', 'method', 'decorator',
               'autoupdate', 'persistent', 'field'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Database',
         'Topic :: Database :: Front-Ends',
```

### Comparing `django-computedfields-0.2.2/docs/manual.rst` & `django-computedfields-0.2.3/docs/manual.rst`

 * *Files 1% similar despite different names*

```diff
@@ -579,14 +579,19 @@
 :mod:`django-computedfields` is inspired by odoo's computed fields and the lack of
 a similar feature in Django's ORM.
 
 
 Changelog
 ---------
 
+- 0.2.3
+    - performance improvement: use UNION for multi dependency query construction
+- 0.2.2
+    - Django 4.2 support
+    - Use `model._base_manager` instead of `model.objects`
 - 0.2.1
     - Django 4.1 support
 - 0.2.0 - next beta release
     - new features:
         - better memory control for the update resolver via
           ``COMPUTEDFIELDS_QUERYSIZE`` or as argument on ``@computed``
         - update optimization - early update-tree exit
```

### Comparing `django-computedfields-0.2.2/docs/examples.rst` & `django-computedfields-0.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/docs/Makefile` & `django-computedfields-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/docs/reference.rst` & `django-computedfields-0.2.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/docs/index.rst` & `django-computedfields-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/docs/conf.py` & `django-computedfields-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/docs/make.bat` & `django-computedfields-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/django_computedfields.egg-info/SOURCES.txt` & `django-computedfields-0.2.3/django_computedfields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/django_computedfields.egg-info/PKG-INFO` & `django-computedfields-0.2.3/django_computedfields.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-computedfields
-Version: 0.2.2
+Version: 0.2.3
 Summary: autoupdated database fields for model methods
 Home-page: https://github.com/netzkolchose/django-computedfields
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz
+Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.3.tar.gz
 Description: [![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
         
         
         ### django-computedfields ###
         
         django-computedfields provides autoupdated database fields
@@ -87,14 +87,17 @@
         #### Documentation ####
         
         The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
         
         
         #### Changelog ####
         
+        - 0.2.3
+            - performance improvement: use UNION for multi dependency query construction
+        
         - 0.2.2
             - Django 4.2 support
             - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
         
         - 0.2.1
             - Django 4.1 support
```

### Comparing `django-computedfields-0.2.2/LICENSE.txt` & `django-computedfields-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-computedfields-0.2.2/PKG-INFO` & `django-computedfields-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-computedfields
-Version: 0.2.2
+Version: 0.2.3
 Summary: autoupdated database fields for model methods
 Home-page: https://github.com/netzkolchose/django-computedfields
 Author: netzkolchose
 Author-email: j.breitbart@netzkolchose.de
 License: MIT
-Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.2.tar.gz
+Download-URL: https://github.com/netzkolchose/django-computedfields/archive/0.2.3.tar.gz
 Description: [![build](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml/badge.svg)](https://github.com/netzkolchose/django-computedfields/actions/workflows/build.yml)
         [![Coverage Status](https://coveralls.io/repos/github/netzkolchose/django-computedfields/badge.svg?branch=master)](https://coveralls.io/github/netzkolchose/django-computedfields?branch=master)
         
         
         ### django-computedfields ###
         
         django-computedfields provides autoupdated database fields
@@ -87,14 +87,17 @@
         #### Documentation ####
         
         The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
         
         
         #### Changelog ####
         
+        - 0.2.3
+            - performance improvement: use UNION for multi dependency query construction
+        
         - 0.2.2
             - Django 4.2 support
             - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
         
         - 0.2.1
             - Django 4.1 support
```

### Comparing `django-computedfields-0.2.2/README.md` & `django-computedfields-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 #### Documentation ####
 
 The documentation can be found [here](https://django-computedfields.readthedocs.io/en/latest/index.html).
 
 
 #### Changelog ####
 
+- 0.2.3
+    - performance improvement: use UNION for multi dependency query construction
+
 - 0.2.2
     - Django 4.2 support
     - Use `model._base_manager` instead of `model.objects` to prevent using overridden `models.objects` with a custom manager
 
 - 0.2.1
     - Django 4.1 support
```

