# Comparing `tmp/django-structlog-5.1.0.tar.gz` & `tmp/django-structlog-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-structlog-5.1.0.tar", last modified: Sun Apr 23 02:54:08 2023, max compression
+gzip compressed data, was "django-structlog-5.2.0.tar", last modified: Fri Jun 30 01:26:51 2023, max compression
```

## Comparing `django-structlog-5.1.0.tar` & `django-structlog-5.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-23 02:53:57.000000 django-structlog-5.1.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 02:53:57.000000 django-structlog-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-23 02:54:08.865115 django-structlog-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-04-23 02:53:57.000000 django-structlog-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/celery/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/middlewares/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 02:53:57.000000 django-structlog-5.1.0/django_structlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 02:54:08.865115 django-structlog-5.1.0/django_structlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 02:54:08.000000 django-structlog-5.1.0/django_structlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-23 02:53:57.000000 django-structlog-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-23 02:54:08.865115 django-structlog-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:26:51.688402 django-structlog-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 01:26:37.000000 django-structlog-5.2.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 01:26:37.000000 django-structlog-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-06-30 01:26:51.688402 django-structlog-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-30 01:26:37.000000 django-structlog-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:26:51.684402 django-structlog-5.2.0/django_structlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:26:51.688402 django-structlog-5.2.0/django_structlog/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/celery/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/celery/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/celery/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/celery/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:26:51.688402 django-structlog-5.2.0/django_structlog/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/middlewares/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-30 01:26:37.000000 django-structlog-5.2.0/django_structlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:26:51.684402 django-structlog-5.2.0/django_structlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-06-30 01:26:51.000000 django-structlog-5.2.0/django_structlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 01:26:51.000000 django-structlog-5.2.0/django_structlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:26:51.000000 django-structlog-5.2.0/django_structlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 01:26:51.000000 django-structlog-5.2.0/django_structlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 01:26:51.000000 django-structlog-5.2.0/django_structlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-30 01:26:37.000000 django-structlog-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 01:26:51.688402 django-structlog-5.2.0/setup.cfg
```

### Comparing `django-structlog-5.1.0/LICENSE.rst` & `django-structlog-5.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/PKG-INFO` & `django-structlog-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 5.1.0
+Version: 5.2.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Classifier: Framework :: Django
```

### Comparing `django-structlog-5.1.0/README.rst` & `django-structlog-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog/celery/middlewares.py` & `django-structlog-5.2.0/django_structlog/celery/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog/celery/receivers.py` & `django-structlog-5.2.0/django_structlog/celery/receivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     structlog.contextvars.clear_contextvars()
     structlog.contextvars.bind_contextvars(task_id=task_id)
     metadata = getattr(task.request, "__django_structlog__", {})
     structlog.contextvars.bind_contextvars(**metadata)
     signals.bind_extra_task_metadata.send(
         sender=receiver_task_pre_run, task=task, logger=logger
     )
+    logger.info("task_started", task=task.name)
 
 
 def receiver_task_retry(request=None, reason=None, einfo=None, **kwargs):
     logger.warning("task_retrying", reason=reason)
 
 
 def receiver_task_success(result=None, **kwargs):
```

### Comparing `django-structlog-5.1.0/django_structlog/celery/signals.py` & `django-structlog-5.2.0/django_structlog/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog/celery/steps.py` & `django-structlog-5.2.0/django_structlog/celery/steps.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog/middlewares/request.py` & `django-structlog-5.2.0/django_structlog/middlewares/request.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog/signals.py` & `django-structlog-5.2.0/django_structlog/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/django_structlog.egg-info/PKG-INFO` & `django-structlog-5.2.0/django_structlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 5.1.0
+Version: 5.2.0
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Classifier: Framework :: Django
```

### Comparing `django-structlog-5.1.0/django_structlog.egg-info/SOURCES.txt` & `django-structlog-5.2.0/django_structlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-structlog-5.1.0/pyproject.toml` & `django-structlog-5.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     [tox]
     # Test against latest supported version of each of python for each Django version.
     #
     # Also, make sure that all python versions used here are included in ./github/worksflows/main.yml
     envlist =
         py37-django32-celery51-redis{3,4}-kombu5-importlibmetadata4,
         py{38,39,310}-django32-celery51-redis{3,4}-kombu5,
-        py{38,39,310,311}-django4{0,1,2}-celery52-redis{3,4}-kombu5,
+        py{38,39,310,311}-django4{0,1,2}-celery5{2,3}-redis{3,4}-kombu5,
     pip_pre = True
 
     [gh-actions]
     python =
         3.7: py37
         3.8: py38
         3.9: py39
@@ -102,14 +102,15 @@
     deps =
         importlibmetadata4: importlib-metadata<5
         redis3: redis>=3, <4
         redis4: redis>=4, <5
         kombu5: kombu<6
         celery51: Celery >=5.1, <5.2
         celery52: Celery >=5.2, <5.3
+        celery53: Celery >=5.3, <5.4
         django32: Django >=3.2, <4.0
         django40: Django >=4.0, <4.1
         django41: Django >=4.1, <4.2
         django42: Django >=4.2, <5.0
         -r{toxinidir}/requirements/ci.txt
 
     commands = pytest --cov=./test_app --cov=./django_structlog --cov-append test_app
```

