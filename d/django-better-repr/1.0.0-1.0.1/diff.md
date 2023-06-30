# Comparing `tmp/django-better-repr-1.0.0.tar.gz` & `tmp/django-better-repr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-better-repr-1.0.0.tar", last modified: Fri Jun 30 20:34:05 2023, max compression
+gzip compressed data, was "django-better-repr-1.0.1.tar", last modified: Fri Jun 30 21:04:36 2023, max compression
```

## Comparing `django-better-repr-1.0.0.tar` & `django-better-repr-1.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.752130 django-better-repr-1.0.0/
--rw-r--r--   0 collinsage   (501) staff       (20)      601 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/.coveragerc
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.739374 django-better-repr-1.0.0/.github/
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.743138 django-better-repr-1.0.0/.github/workflows/
--rw-r--r--   0 collinsage   (501) staff       (20)     4361 2023-06-30 20:13:10.000000 django-better-repr-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 collinsage   (501) staff       (20)      593 2023-06-30 20:26:29.000000 django-better-repr-1.0.0/.gitignore
--rw-r--r--   0 collinsage   (501) staff       (20)       66 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/.isort.cfg
--rw-r--r--   0 collinsage   (501) staff       (20)     1844 2023-06-30 20:11:20.000000 django-better-repr-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 collinsage   (501) staff       (20)      530 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/.readthedocs.yml
--rw-r--r--   0 collinsage   (501) staff       (20)       96 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/AUTHORS.rst
--rw-r--r--   0 collinsage   (501) staff       (20)      128 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/CHANGELOG.rst
--rw-r--r--   0 collinsage   (501) staff       (20)    13957 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 collinsage   (501) staff       (20)     1078 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/LICENSE.txt
--rw-r--r--   0 collinsage   (501) staff       (20)     2719 2023-06-30 20:34:05.752213 django-better-repr-1.0.0/PKG-INFO
--rw-r--r--   0 collinsage   (501) staff       (20)     2238 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/README.rst
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.744475 django-better-repr-1.0.0/docs/
--rw-r--r--   0 collinsage   (501) staff       (20)     1154 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/Makefile
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.744692 django-better-repr-1.0.0/docs/_static/
--rw-r--r--   0 collinsage   (501) staff       (20)       18 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/_static/.gitignore
--rw-r--r--   0 collinsage   (501) staff       (20)       41 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/authors.rst
--rw-r--r--   0 collinsage   (501) staff       (20)       43 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/changelog.rst
--rw-r--r--   0 collinsage   (501) staff       (20)     9787 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/conf.py
--rw-r--r--   0 collinsage   (501) staff       (20)       33 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/contributing.rst
--rw-r--r--   0 collinsage   (501) staff       (20)     2357 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/index.rst
--rw-r--r--   0 collinsage   (501) staff       (20)       67 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/license.rst
--rw-r--r--   0 collinsage   (501) staff       (20)       39 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/readme.rst
--rw-r--r--   0 collinsage   (501) staff       (20)      233 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/docs/requirements.txt
--rw-r--r--   0 collinsage   (501) staff       (20)     1088 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/manage.py
--rw-r--r--   0 collinsage   (501) staff       (20)      346 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/pyproject.toml
--rw-r--r--   0 collinsage   (501) staff       (20)     1331 2023-06-30 20:34:05.752663 django-better-repr-1.0.0/setup.cfg
--rw-r--r--   0 collinsage   (501) staff       (20)      713 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/setup.py
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.739675 django-better-repr-1.0.0/src/
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.745482 django-better-repr-1.0.0/src/django_better_repr/
--rw-r--r--   0 collinsage   (501) staff       (20)      870 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/src/django_better_repr/__init__.py
--rw-r--r--   0 collinsage   (501) staff       (20)     1388 2023-06-30 20:11:23.000000 django-better-repr-1.0.0/src/django_better_repr/bases.py
--rw-r--r--   0 collinsage   (501) staff       (20)      273 2023-06-30 20:11:23.000000 django-better-repr-1.0.0/src/django_better_repr/config.py
--rw-r--r--   0 collinsage   (501) staff       (20)       46 2023-06-30 19:02:18.000000 django-better-repr-1.0.0/src/django_better_repr/exceptions.py
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.746845 django-better-repr-1.0.0/src/django_better_repr.egg-info/
--rw-r--r--   0 collinsage   (501) staff       (20)     2719 2023-06-30 20:34:05.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/PKG-INFO
--rw-r--r--   0 collinsage   (501) staff       (20)     1755 2023-06-30 20:34:05.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/SOURCES.txt
--rw-r--r--   0 collinsage   (501) staff       (20)        1 2023-06-30 20:34:05.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/dependency_links.txt
--rw-r--r--   0 collinsage   (501) staff       (20)        1 2023-06-30 19:15:54.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/not-zip-safe
--rw-r--r--   0 collinsage   (501) staff       (20)      100 2023-06-30 20:34:05.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/requires.txt
--rw-r--r--   0 collinsage   (501) staff       (20)       19 2023-06-30 20:34:05.000000 django-better-repr-1.0.0/src/django_better_repr.egg-info/top_level.txt
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.747223 django-better-repr-1.0.0/tests/
--rw-r--r--   0 collinsage   (501) staff       (20)        0 2023-06-30 19:13:57.000000 django-better-repr-1.0.0/tests/__init__.py
--rw-r--r--   0 collinsage   (501) staff       (20)      286 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/tests/conftest.py
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.747897 django-better-repr-1.0.0/tests/example_project/
--rw-r--r--   0 collinsage   (501) staff       (20)        0 2023-06-30 19:13:49.000000 django-better-repr-1.0.0/tests/example_project/__init__.py
--rwxr-xr-x   0 collinsage   (501) staff       (20)      693 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/__main__.py
--rw-r--r--   0 collinsage   (501) staff       (20)   180224 2023-06-30 20:00:03.000000 django-better-repr-1.0.0/tests/example_project/db.sqlite3
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.749931 django-better-repr-1.0.0/tests/example_project/example_project/
--rw-r--r--   0 collinsage   (501) staff       (20)        0 2023-06-30 19:05:55.000000 django-better-repr-1.0.0/tests/example_project/example_project/__init__.py
--rw-r--r--   0 collinsage   (501) staff       (20)      407 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/example_project/asgi.py
--rw-r--r--   0 collinsage   (501) staff       (20)     3327 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/example_project/settings.py
--rw-r--r--   0 collinsage   (501) staff       (20)      771 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/example_project/urls.py
--rw-r--r--   0 collinsage   (501) staff       (20)      407 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/example_project/wsgi.py
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.751051 django-better-repr-1.0.0/tests/example_project/myapp/
--rw-r--r--   0 collinsage   (501) staff       (20)        0 2023-06-30 19:06:03.000000 django-better-repr-1.0.0/tests/example_project/myapp/__init__.py
--rw-r--r--   0 collinsage   (501) staff       (20)       29 2023-06-30 20:11:26.000000 django-better-repr-1.0.0/tests/example_project/myapp/admin.py
--rw-r--r--   0 collinsage   (501) staff       (20)      164 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/myapp/apps.py
-drwxr-xr-x   0 collinsage   (501) staff       (20)        0 2023-06-30 20:34:05.752042 django-better-repr-1.0.0/tests/example_project/myapp/migrations/
--rw-r--r--   0 collinsage   (501) staff       (20)     2038 2023-06-30 20:11:23.000000 django-better-repr-1.0.0/tests/example_project/myapp/migrations/0001_initial.py
--rw-r--r--   0 collinsage   (501) staff       (20)      410 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/myapp/migrations/0002_alter_fourorlessfields_two.py
--rw-r--r--   0 collinsage   (501) staff       (20)      429 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/myapp/migrations/0003_alter_fourormorefields_two.py
--rw-r--r--   0 collinsage   (501) staff       (20)      432 2023-06-30 20:11:02.000000 django-better-repr-1.0.0/tests/example_project/myapp/migrations/0004_fourormorefields_six.py
--rw-r--r--   0 collinsage   (501) staff       (20)        0 2023-06-30 19:06:03.000000 django-better-repr-1.0.0/tests/example_project/myapp/migrations/__init__.py
--rw-r--r--   0 collinsage   (501) staff       (20)      826 2023-06-30 20:11:23.000000 django-better-repr-1.0.0/tests/example_project/myapp/models.py
--rw-r--r--   0 collinsage   (501) staff       (20)       26 2023-06-30 20:11:26.000000 django-better-repr-1.0.0/tests/example_project/myapp/tests.py
--rw-r--r--   0 collinsage   (501) staff       (20)       26 2023-06-30 20:11:26.000000 django-better-repr-1.0.0/tests/example_project/myapp/views.py
--rw-r--r--   0 collinsage   (501) staff       (20)     2287 2023-06-30 20:11:23.000000 django-better-repr-1.0.0/tests/test_better_repr.py
--rw-r--r--   0 collinsage   (501) staff       (20)     2851 2023-06-30 18:57:09.000000 django-better-repr-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.667644 django-better-repr-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.679644 django-better-repr-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.667644 django-better-repr-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.683644 django-better-repr-1.0.1/src/django_better_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/src/django_better_repr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/src/django_better_repr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:04:36.000000 django-better-repr-1.0.1/src/django_better_repr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.687644 django-better-repr-1.0.1/tests/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/db.sqlite3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.691644 django-better-repr-1.0.1/tests/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/example_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.691644 django-better-repr-1.0.1/tests/example_project/myapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:36.695644 django-better-repr-1.0.1/tests/example_project/myapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0002_alter_fourorlessfields_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0003_alter_fourormorefields_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/0004_fourormorefields_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/example_project/myapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tests/test_better_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 21:03:55.000000 django-better-repr-1.0.1/tox.ini
```

### Comparing `django-better-repr-1.0.0/.coveragerc` & `django-better-repr-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/.github/workflows/ci.yml` & `django-better-repr-1.0.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
           retention-days: 1
 
   test:
     needs: prepare
     strategy:
       matrix:
         python:
-        - "3.7"  # oldest Python supported by PSF
+        - "3.8"  # oldest Python supported by PSF
         - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
```

### Comparing `django-better-repr-1.0.0/.gitignore` & `django-better-repr-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/.pre-commit-config.yaml` & `django-better-repr-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/.readthedocs.yml` & `django-better-repr-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/CONTRIBUTING.rst` & `django-better-repr-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/LICENSE.txt` & `django-better-repr-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/PKG-INFO` & `django-better-repr-1.0.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: django-better-repr
-Version: 1.0.0
-Summary: Django model reprs for humans!
-Home-page: https://github.com/MrSage
-Author: Collin Sage
-Author-email: 3229549+MrSage@users.noreply.github.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/django-better-repr.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
@@ -49,15 +33,60 @@
 django-better-repr
 ==================
 
 
     Django model reprs for humans!
 
 
-A longer description of your project goes here...
+This project seeks to make reprs of Django models more human-friendly. This
+project is heavily inspired by https://github.com/dan-passaro/django-auto-repr .
+
+How to use:
+===========
+
+::
+
+   from django_better_repr import better_repr
+
+   @better_repr
+   class MyDjangoModel(models.Model):
+       my_field = models.CharField(max_length=16)
+
+Or, if class inheritance is more your speed:
+
+::
+
+   from django_better_repr.bases import BetterRepr
+
+   class MyDjangoModel(BetterRepr, models.Model):
+       my_field = models.CharField(max_length=16)
+
+Then load up your favorite shell and run:
+
+::
+
+   MyDjangoModel.objects.create(my_field='Hello, world!')
+   >>> MyDjangoModel(my_field='Hello, world!')
+
+If your model has a lot of fields then the repr will automatically switch to
+pretty printing. This can be configured via settings.
+
+Configuration
+=============
+
+If you want to customize the behavior of the library, below are all the options.
+
+::
+
+   # settings.py
+   BETTER_REPR_CONFIG = {
+      'ENABLE_MULTILINE_REPRS': True,  # bool (default: True), whether or not to allow multiline reprs
+      'SINGLE_LINE_PARTS_LIMIT': 4,  # int (default: 4), the number of fields a repr can have before switching to multi line
+      'MULTILINE_WHITESPACE': '\t',  # str (default: '\t'), the whitespace string to use for multiline reprs
+   }
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
```

### Comparing `django-better-repr-1.0.0/docs/Makefile` & `django-better-repr-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/docs/conf.py` & `django-better-repr-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/docs/index.rst` & `django-better-repr-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/manage.py` & `django-better-repr-1.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/setup.cfg` & `django-better-repr-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	django
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `django-better-repr-1.0.0/setup.py` & `django-better-repr-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/src/django_better_repr/__init__.py` & `django-better-repr-1.0.1/src/django_better_repr/__init__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/src/django_better_repr.egg-info/SOURCES.txt` & `django-better-repr-1.0.1/src/django_better_repr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/__main__.py` & `django-better-repr-1.0.1/tests/example_project/__main__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/db.sqlite3` & `django-better-repr-1.0.1/tests/example_project/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/example_project/settings.py` & `django-better-repr-1.0.1/tests/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/example_project/urls.py` & `django-better-repr-1.0.1/tests/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/myapp/migrations/0001_initial.py` & `django-better-repr-1.0.1/tests/example_project/myapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/example_project/myapp/models.py` & `django-better-repr-1.0.1/tests/example_project/myapp/models.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tests/test_better_repr.py` & `django-better-repr-1.0.1/tests/test_better_repr.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.0/tox.ini` & `django-better-repr-1.0.1/tox.ini`

 * *Files identical despite different names*

