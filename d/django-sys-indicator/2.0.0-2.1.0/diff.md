# Comparing `tmp/django-sys-indicator-2.0.0.tar.gz` & `tmp/django-sys-indicator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sys-indicator-2.0.0.tar", last modified: Thu Nov 24 00:31:33 2022, max compression
+gzip compressed data, was "django-sys-indicator-2.1.0.tar", last modified: Fri Jun 30 12:58:32 2023, max compression
```

## Comparing `django-sys-indicator-2.0.0.tar` & `django-sys-indicator-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      204 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2609 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      500 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.252567 django-sys-indicator-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/src/django_sys_indicator/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.252567 django-sys-indicator-2.0.0/src/django_sys_indicator/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/src/django_sys_indicator/templates/django_sys_indicator/
--rw-r--r--   0 runner    (1001) docker     (122)      709 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/templates/django_sys_indicator/system_indicator.html
--rw-r--r--   0 runner    (1001) docker     (122)      675 2022-11-24 00:31:24.000000 django-sys-indicator-2.0.0/src/django_sys_indicator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 00:31:33.256567 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2609 2022-11-24 00:31:33.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2022-11-24 00:31:33.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 00:31:33.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 00:31:32.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-24 00:31:33.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-24 00:31:33.000000 django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.853718 django-sys-indicator-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/src/django_sys_indicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.853718 django-sys-indicator-2.1.0/src/django_sys_indicator/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/src/django_sys_indicator/templates/django_sys_indicator/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/templates/django_sys_indicator/system_indicator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-30 12:58:23.000000 django-sys-indicator-2.1.0/src/django_sys_indicator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:32.857718 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 12:58:32.000000 django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/top_level.txt
```

### Comparing `django-sys-indicator-2.0.0/LICENSE` & `django-sys-indicator-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/PKG-INFO` & `django-sys-indicator-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-sys-indicator
-Version: 2.0.0
+Version: 2.1.0
 Summary: A system/environment indicator for django
 Home-page: https://github.com/marksweb/django-sys-indicator
 Author: Mark Walker
 Author-email: theshow@gmail.com
 License: MIT License
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-sys-indicator
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/marksweb/django-sys-indicator/main.svg)](https://results.pre-commit.ci/latest/github/marksweb/django-sys-indicator/main)
 [![GitHub license](https://img.shields.io/github/license/marksweb/django-sys-indicator)](https://github.com/marksweb/django-sys-indicator/blob/main/LICENSE)
```

### Comparing `django-sys-indicator-2.0.0/README.md` & `django-sys-indicator-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/setup.cfg` & `django-sys-indicator-2.1.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [metadata]
 name = django-sys-indicator
-version = 2.0.0
+version = 2.1.0
 url = https://github.com/marksweb/django-sys-indicator
 description = A system/environment indicator for django
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mark Walker
 author_email = theshow@gmail.com
 keywords = Django
 license = MIT License
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = django>=3.2
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [coverage:run]
 branch = True
@@ -41,21 +41,15 @@
 source = 
 	django_sys_indicator
 	tests
 
 [coverage:paths]
 source = 
 	src
-	.tox/*/site-packages
 
 [coverage:report]
 show_missing = True
 
-[flake8]
-max-line-length = 119
-extend-ignore = A003,B009,B010,C101,C408,C812,C815,E501,E800,N400,Q000
-exclude = migrations,.venv_*,docs
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator/conf.py` & `django-sys-indicator-2.1.0/src/django_sys_indicator/conf.py`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator/middleware.py` & `django-sys-indicator-2.1.0/src/django_sys_indicator/middleware.py`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator/templates/django_sys_indicator/system_indicator.html` & `django-sys-indicator-2.1.0/src/django_sys_indicator/templates/django_sys_indicator/system_indicator.html`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator/utils.py` & `django-sys-indicator-2.1.0/src/django_sys_indicator/utils.py`

 * *Files identical despite different names*

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/PKG-INFO` & `django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-sys-indicator
-Version: 2.0.0
+Version: 2.1.0
 Summary: A system/environment indicator for django
 Home-page: https://github.com/marksweb/django-sys-indicator
 Author: Mark Walker
 Author-email: theshow@gmail.com
 License: MIT License
 Keywords: Django
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-sys-indicator
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/marksweb/django-sys-indicator/main.svg)](https://results.pre-commit.ci/latest/github/marksweb/django-sys-indicator/main)
 [![GitHub license](https://img.shields.io/github/license/marksweb/django-sys-indicator)](https://github.com/marksweb/django-sys-indicator/blob/main/LICENSE)
```

### Comparing `django-sys-indicator-2.0.0/src/django_sys_indicator.egg-info/SOURCES.txt` & `django-sys-indicator-2.1.0/src/django_sys_indicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

