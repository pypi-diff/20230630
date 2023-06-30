# Comparing `tmp/django-lazy-srcset-0.2.0.tar.gz` & `tmp/django-lazy-srcset-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-0.2.0.tar", last modified: Tue Jun 27 21:15:42 2023, max compression
+gzip compressed data, was "django-lazy-srcset-0.2.1.tar", last modified: Fri Jun 30 12:30:30 2023, max compression
```

## Comparing `django-lazy-srcset-0.2.0.tar` & `django-lazy-srcset-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.566515 django-lazy-srcset-0.2.0/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.0/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)       49 2023-06-27 17:54:23.000000 django-lazy-srcset-0.2.0/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-27 21:15:42.566631 django-lazy-srcset-0.2.0/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.0/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.560594 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      445 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-06-27 21:15:42.000000 django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.562817 django-lazy-srcset-0.2.0/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.0/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.0/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.0/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.0/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-27 21:15:42.566002 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     8879 2023-06-27 16:04:10.000000 django-lazy-srcset-0.2.0/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.0/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-06-27 21:15:42.570431 django-lazy-srcset-0.2.0/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.0/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.835195 django-lazy-srcset-0.2.1/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.1/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-0.2.1/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-30 12:30:30.835304 django-lazy-srcset-0.2.1/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.1/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.830690 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      576 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-06-30 12:30:30.000000 django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.832149 django-lazy-srcset-0.2.1/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.1/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.1/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.1/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.1/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.832940 django-lazy-srcset-0.2.1/lazy_srcset/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.833974 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-0.2.1/lazy_srcset/management/commands/imagekit_cleanup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-30 12:30:30.834933 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8879 2023-06-27 16:04:10.000000 django-lazy-srcset-0.2.1/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.1/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-06-30 12:30:30.839863 django-lazy-srcset-0.2.1/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.1/setup.py
```

### Comparing `django-lazy-srcset-0.2.0/LICENSE` & `django-lazy-srcset-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.0/PKG-INFO` & `django-lazy-srcset-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
```

### Comparing `django-lazy-srcset-0.2.0/README.rst` & `django-lazy-srcset-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.0/django_lazy_srcset.egg-info/PKG-INFO` & `django-lazy-srcset-0.2.1/django_lazy_srcset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
```

### Comparing `django-lazy-srcset-0.2.0/lazy_srcset/conf.py` & `django-lazy-srcset-0.2.1/lazy_srcset/conf.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.0/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-0.2.1/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.0/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-0.2.1/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.0/setup.cfg` & `django-lazy-srcset-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-lazy-srcset
-version = 0.2.0
+version = 0.2.1
 description = Lazy srcset and image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

