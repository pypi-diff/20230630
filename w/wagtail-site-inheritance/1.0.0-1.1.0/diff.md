# Comparing `tmp/wagtail-site-inheritance-1.0.0.tar.gz` & `tmp/wagtail-site-inheritance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-site-inheritance-1.0.0.tar", last modified: Tue May  2 13:31:31 2023, max compression
+gzip compressed data, was "wagtail-site-inheritance-1.1.0.tar", last modified: Fri Jun 30 07:23:36 2023, max compression
```

## Comparing `wagtail-site-inheritance-1.0.0.tar` & `wagtail-site-inheritance-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.839161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-02 13:31:28.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.843161 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 13:31:31.000000 wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.281718 wagtail-site-inheritance-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.281718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.281718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.281718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/wagtail_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-30 07:23:33.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:23:36.285718 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-30 07:23:35.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 07:23:36.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:23:35.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:23:35.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 07:23:35.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 07:23:35.000000 wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/top_level.txt
```

### Comparing `wagtail-site-inheritance-1.0.0/LICENSE` & `wagtail-site-inheritance-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/PKG-INFO` & `wagtail-site-inheritance-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-site-inheritance
-Version: 1.0.0
+Version: 1.1.0
 Summary: Site Inheritance for Wagtail
 Home-page: https://github.com/labd/wagtail-site-inheritance
 Author: Lab Digital
 Author-email: opensource@labdigital.nl
 License: MIT
 Description: 
         # Wagtail Site Inheritance
```

### Comparing `wagtail-site-inheritance-1.0.0/README.md` & `wagtail-site-inheritance-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/pyproject.toml` & `wagtail-site-inheritance-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/setup.py` & `wagtail-site-inheritance-1.1.0/setup.py`

 * *Files identical despite different names*

```diff
@@ -27,15 +27,15 @@
         fh.read(),
         flags=re.M | re.S,
     )
 
 
 setup(
     name="wagtail-site-inheritance",
-    version="1.0.0",
+    version="1.1.0",
     description="Site Inheritance for Wagtail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/labd/wagtail-site-inheritance",
     author="Lab Digital",
     author_email="opensource@labdigital.nl",
     install_requires=[
```

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/admin.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/forms.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/migrations/0001_initial.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/models.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/receivers.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/receivers.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/views.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_forms.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/wagtail_forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance/wagtail_hooks.py` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance/wagtail_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         bool(request.POST.get("action-publish"))
         and parent_page_perms.can_publish_subpage()
     )
     if not is_publishing:
         return
 
     # Mark edited page as modified
-    models.PageInheritanceItem.objects.filter(page=page, modified=False).update(
-        modified=True
-    )
+    models.PageInheritanceItem.objects.filter(
+        inherited_page=page, modified=False
+    ).update(modified=True)
 
     create_non_existing_pages(request, page, parent_page)
     sync_existing_pages(request, page)
 
 
 def create_non_existing_pages(request, page, parent_page):
     # Create non existing pages in other trees.
```

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/PKG-INFO` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-site-inheritance
-Version: 1.0.0
+Version: 1.1.0
 Summary: Site Inheritance for Wagtail
 Home-page: https://github.com/labd/wagtail-site-inheritance
 Author: Lab Digital
 Author-email: opensource@labdigital.nl
 License: MIT
 Description: 
         # Wagtail Site Inheritance
```

### Comparing `wagtail-site-inheritance-1.0.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt` & `wagtail-site-inheritance-1.1.0/src/wagtail_site_inheritance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

