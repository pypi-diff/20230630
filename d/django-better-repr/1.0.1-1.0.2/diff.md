# Comparing `tmp/django-better-repr-1.0.1.tar.gz` & `tmp/django-better-repr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-better-repr-1.0.1.tar", last modified: Fri Jun 30 21:04:36 2023, max compression
+gzip compressed data, was "django-better-repr-1.0.2.tar", last modified: Fri Jun 30 21:39:54 2023, max compression
```

## Comparing `django-better-repr-1.0.1.tar` & `django-better-repr-1.0.2.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.667644 django-better-repr-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.679644 django-better-repr-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.667644 django-better-repr-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/src/django_better_repr/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/src/django_better_repr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/tests/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/db.sqlite3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.691644 django-better-repr-1.0.1/tests/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.691644 django-better-repr-1.0.1/tests/example_project/myapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/tests/example_project/myapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0002_alter_fourorlessfields_two.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0003_alter_fourormorefields_two.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0004_fourormorefields_six.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/test_better_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.710146 django-better-repr-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.722147 django-better-repr-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/pyscaffold.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.710146 django-better-repr-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/src/django_better_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.730148 django-better-repr-1.0.2/src/django_better_repr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.730148 django-better-repr-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.734148 django-better-repr-1.0.2/tests/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/db.sqlite3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.738149 django-better-repr-1.0.2/tests/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.738149 django-better-repr-1.0.2/tests/example_project/myapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/tests/example_project/myapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/test_better_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tox.ini
```

### Comparing `django-better-repr-1.0.1/.coveragerc` & `django-better-repr-1.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/.github/workflows/ci.yml` & `django-better-repr-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/.gitignore` & `django-better-repr-1.0.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -52,7 +52,10 @@
 .venv*/
 .conda*/
 .python-version
 
 # Environment
 .env
 .envrc
+
+# Exclusions
+!pyscaffold.cfg
```

### Comparing `django-better-repr-1.0.1/.pre-commit-config.yaml` & `django-better-repr-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/.readthedocs.yml` & `django-better-repr-1.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/CONTRIBUTING.rst` & `django-better-repr-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/LICENSE.txt` & `django-better-repr-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/PKG-INFO` & `django-better-repr-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django model reprs for humans!
-Home-page: https://github.com/MrSage
+Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://github.com/MrSage/django-better-repr
+Project-URL: Source, https://github.com/MrSage/django-better-repr
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -53,17 +54,30 @@
 
     Django model reprs for humans!
 
 
 This project seeks to make reprs of Django models more human-friendly. This
 project is heavily inspired by https://github.com/dan-passaro/django-auto-repr .
 
+Installation
+============
+
+::
+
+   pip install django-better-repr
+
+And that's it!
+
 How to use:
 ===========
 
+The repr logic in this library is designed to produce the smallest, most meaningful repr possible
+for your Django models. That means that fields which aren't set won't show up in the repr. This
+should reduce noise and let you get the most value out of your reprs.
+
 ::
 
    from django_better_repr import better_repr
 
    @better_repr
    class MyDjangoModel(models.Model):
        my_field = models.CharField(max_length=16)
@@ -114,15 +128,14 @@
     cd django-better-repr
     pre-commit install
 
 It is a good idea to update the hooks to the latest version::
 
     pre-commit autoupdate
 
-Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.5. For details and usage
```

### Comparing `django-better-repr-1.0.1/README.rst` & `django-better-repr-1.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,30 @@
 
     Django model reprs for humans!
 
 
 This project seeks to make reprs of Django models more human-friendly. This
 project is heavily inspired by https://github.com/dan-passaro/django-auto-repr .
 
+Installation
+============
+
+::
+
+   pip install django-better-repr
+
+And that's it!
+
 How to use:
 ===========
 
+The repr logic in this library is designed to produce the smallest, most meaningful repr possible
+for your Django models. That means that fields which aren't set won't show up in the repr. This
+should reduce noise and let you get the most value out of your reprs.
+
 ::
 
    from django_better_repr import better_repr
 
    @better_repr
    class MyDjangoModel(models.Model):
        my_field = models.CharField(max_length=16)
@@ -97,15 +110,14 @@
     cd django-better-repr
     pre-commit install
 
 It is a good idea to update the hooks to the latest version::
 
     pre-commit autoupdate
 
-Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.5. For details and usage
```

### Comparing `django-better-repr-1.0.1/docs/Makefile` & `django-better-repr-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/docs/conf.py` & `django-better-repr-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/docs/index.rst` & `django-better-repr-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/manage.py` & `django-better-repr-1.0.2/manage.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/setup.cfg` & `django-better-repr-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 description = Django model reprs for humans!
 author = Collin Sage
 author_email = 3229549+MrSage@users.noreply.github.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/MrSage
+url = https://github.com/MrSage/django-better-repr
 project_urls = 
-	Documentation = https://pyscaffold.org/
+	Documentation = https://github.com/MrSage/django-better-repr
+	Source = https://github.com/MrSage/django-better-repr
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `django-better-repr-1.0.1/setup.py` & `django-better-repr-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/src/django_better_repr/__init__.py` & `django-better-repr-1.0.2/src/django_better_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/src/django_better_repr/bases.py` & `django-better-repr-1.0.2/src/django_better_repr/bases.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/src/django_better_repr.egg-info/PKG-INFO` & `django-better-repr-1.0.2/src/django_better_repr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django model reprs for humans!
-Home-page: https://github.com/MrSage
+Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://github.com/MrSage/django-better-repr
+Project-URL: Source, https://github.com/MrSage/django-better-repr
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
@@ -53,17 +54,30 @@
 
     Django model reprs for humans!
 
 
 This project seeks to make reprs of Django models more human-friendly. This
 project is heavily inspired by https://github.com/dan-passaro/django-auto-repr .
 
+Installation
+============
+
+::
+
+   pip install django-better-repr
+
+And that's it!
+
 How to use:
 ===========
 
+The repr logic in this library is designed to produce the smallest, most meaningful repr possible
+for your Django models. That means that fields which aren't set won't show up in the repr. This
+should reduce noise and let you get the most value out of your reprs.
+
 ::
 
    from django_better_repr import better_repr
 
    @better_repr
    class MyDjangoModel(models.Model):
        my_field = models.CharField(max_length=16)
@@ -114,15 +128,14 @@
     cd django-better-repr
     pre-commit install
 
 It is a good idea to update the hooks to the latest version::
 
     pre-commit autoupdate
 
-Don't forget to tell your contributors to also install and use pre-commit.
 
 .. _pre-commit: https://pre-commit.com/
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.5. For details and usage
```

### Comparing `django-better-repr-1.0.1/src/django_better_repr.egg-info/SOURCES.txt` & `django-better-repr-1.0.2/src/django_better_repr.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 manage.py
 pyproject.toml
+pyscaffold.cfg
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
@@ -48,11 +49,8 @@
 tests/example_project/myapp/__init__.py
 tests/example_project/myapp/admin.py
 tests/example_project/myapp/apps.py
 tests/example_project/myapp/models.py
 tests/example_project/myapp/tests.py
 tests/example_project/myapp/views.py
 tests/example_project/myapp/migrations/0001_initial.py
-tests/example_project/myapp/migrations/0002_alter_fourorlessfields_two.py
-tests/example_project/myapp/migrations/0003_alter_fourormorefields_two.py
-tests/example_project/myapp/migrations/0004_fourormorefields_six.py
 tests/example_project/myapp/migrations/__init__.py
```

### Comparing `django-better-repr-1.0.1/tests/example_project/__main__.py` & `django-better-repr-1.0.2/tests/example_project/__main__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tests/example_project/db.sqlite3` & `django-better-repr-1.0.2/tests/example_project/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tests/example_project/example_project/settings.py` & `django-better-repr-1.0.2/tests/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tests/example_project/example_project/urls.py` & `django-better-repr-1.0.2/tests/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tests/example_project/myapp/migrations/0001_initial.py` & `django-better-repr-1.0.2/tests/example_project/myapp/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.2 on 2023-06-30 19:24
+# Generated by Django 4.2.2 on 2023-06-30 21:09
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 import src.django_better_repr.bases
 
 
@@ -27,26 +27,27 @@
             ],
         ),
         migrations.CreateModel(
             name='FourOrMoreFields',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
-                ('two', models.CharField(default='Default', max_length=32)),
+                ('two', models.CharField(default='Default', max_length=32, null=True)),
                 ('three', models.IntegerField(null=True)),
+                ('six', models.FloatField()),
                 ('five', models.ManyToManyField(to='myapp.justform2ms')),
                 ('four', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='myapp.justforfks')),
             ],
             bases=(src.django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='FourOrLessFields',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
-                ('two', models.CharField(default='Default', max_length=32)),
+                ('two', models.CharField(default='Default', max_length=32, null=True)),
                 ('three', models.IntegerField(null=True)),
                 ('four', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='myapp.justforfks')),
             ],
             bases=(src.django_better_repr.bases.BetterRepr, models.Model),
         ),
     ]
```

### Comparing `django-better-repr-1.0.1/tests/example_project/myapp/models.py` & `django-better-repr-1.0.2/tests/example_project/myapp/models.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tests/test_better_repr.py` & `django-better-repr-1.0.2/tests/test_better_repr.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.1/tox.ini` & `django-better-repr-1.0.2/tox.ini`

 * *Files identical despite different names*

