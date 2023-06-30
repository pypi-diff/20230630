# Comparing `tmp/asphalt-web-1.1.0.tar.gz` & `tmp/asphalt-web-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphalt-web-1.1.0.tar", last modified: Wed May  4 19:13:34 2022, max compression
+gzip compressed data, was "asphalt-web-1.2.0.tar", last modified: Fri Jun 30 17:30:17 2023, max compression
```

## Comparing `asphalt-web-1.1.0.tar` & `asphalt-web-1.2.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/integrations.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/modules/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/modules/asgi.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/modules/django.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/modules/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/modules/starlette.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/py-modindex.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/docs/versionhistory.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/examples/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/aiohttp/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/aiohttp/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/aiohttp/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/aiohttp/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/examples/asgi3/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/asgi3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/asgi3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/asgi3/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/examples/django/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/examples/django/django_example/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/django_example/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      670 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/django/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/examples/fastapi/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/fastapi/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/fastapi/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/fastapi/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/fastapi/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/examples/starlette/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/starlette/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/starlette/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/starlette/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/examples/starlette/static.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.130508 asphalt-web-1.1.0/src/asphalt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/src/asphalt/web/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5092 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/asgi3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/django.py
--rw-r--r--   0 runner    (1001) docker     (121)     5111 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/src/asphalt/web/starlette.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/src/asphalt_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-05-04 19:13:33.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-05-04 19:13:34.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 19:13:33.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-04 19:13:33.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-05-04 19:13:33.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-04 19:13:34.000000 asphalt-web-1.1.0/src/asphalt_web.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:34.134508 asphalt-web-1.1.0/tests/django_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/django_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/django_app/asgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/django_app/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/django_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/django_app/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6623 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/test_asgi3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-05-04 19:13:22.000000 asphalt-web-1.1.0/tests/test_starlette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/integrations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/asgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/starlette.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/py-modindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/versionhistory.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/asgi3/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/django/django_example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.121054 asphalt-web-1.2.0/examples/starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/src/asphalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.121054 asphalt-web-1.2.0/src/asphalt/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/asgi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/starlette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.125054 asphalt-web-1.2.0/src/asphalt_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.125054 asphalt-web-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/tests/django_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_asgi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_starlette.py
```

### Comparing `asphalt-web-1.1.0/.github/workflows/publish.yml` & `asphalt-web-1.2.0/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 name: Publish packages to PyPI
 
 on:
   push:
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
+      - "[0-9]+.[0-9]+.[0-9]+.post[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+[a-b][0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+rc[0-9]+"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
-      run: python -m build -s -w .
+      run: python -m build
     - name: Upload packages
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_password }}
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `asphalt-web-1.1.0/.github/workflows/test.yml` & `asphalt-web-1.2.0/.github/workflows/test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -6,56 +6,40 @@
   pull_request:
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11-dev", "pypy-3.8"]
-        exclude:
-        - os: macos-latest
-          python-version: "3.8"
-        - os: macos-latest
-          python-version: "3.9"
-        - os: macos-latest
-          python-version: "pypy-3.8"
-        - os: windows-latest
-          python-version: "3.8"
-        - os: windows-latest
-          python-version: "3.9"
-        - os: windows-latest
-          python-version: "pypy-3.8"
+        os: [ubuntu-latest]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12", "pypy-3.10"]
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    - uses: actions/cache@v2
-      with:
-        path: ~/.cache/pip
-        key: pip-test-${{ matrix.python-version }}-${{ matrix.os }}
+        allow-prereleases: true
+        cache: pip
+        cache-dependency-path: pyproject.toml
     - name: Install dependencies
-      run: pip install .[test] coveralls
+      run: pip install .[test] coverage
     - name: Test with pytest
-      run: coverage run -m pytest
+      run: |
+        coverage run -m pytest
+        coverage xml
     - name: Upload Coverage
-      run: coveralls --service=github
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
-        COVERALLS_PARALLEL: true
+      uses: coverallsapp/github-action@v2
+      with:
+        parallel: true
+        file: coverage.xml
 
   coveralls:
     name: Finish Coveralls
     needs: test
     runs-on: ubuntu-latest
-    container: python:3-slim
     steps:
     - name: Finished
-      run: |
-        pip install coveralls
-        coveralls --service=github --finish
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      uses: coverallsapp/github-action@v2
+      with:
+        parallel-finished: true
```

### Comparing `asphalt-web-1.1.0/LICENSE` & `asphalt-web-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/PKG-INFO` & `asphalt-web-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: asphalt-web
-Version: 1.1.0
+Version: 1.2.0
 Summary: Web framework integrations for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Documentation, https://asphalt-web.readthedocs.org/en/latest/
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt-web
 Project-URL: Issue tracker, https://github.com/asphalt-framework/asphalt-web/issues
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: doc
 Provides-Extra: aiohttp
+Provides-Extra: asgi3
 Provides-Extra: django
 Provides-Extra: fastapi
 Provides-Extra: starlette
+Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/asphalt-framework/asphalt-web/actions/workflows/test.yml/badge.svg
   :target: https://github.com/asphalt-framework/asphalt-web/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/github/asphalt-framework/asphalt-web/badge.svg?branch=master
   :target: https://coveralls.io/github/asphalt-framework/asphalt-web?branch=master
@@ -66,9 +66,7 @@
 Project links
 -------------
 
 * `Documentation <http://asphalt-web.readthedocs.org/en/latest/>`_
 * `Help and support <https://github.com/asphalt-framework/asphalt/wiki/Help-and-support>`_
 * `Source code <https://github.com/asphalt-framework/asphalt-web>`_
 * `Issue tracker <https://github.com/asphalt-framework/asphalt-web/issues>`_
-
-
```

### Comparing `asphalt-web-1.1.0/README.rst` & `asphalt-web-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/docs/conf.py` & `asphalt-web-1.2.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from importlib.metadata import version
+from importlib import metadata
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.extlinks",
@@ -14,29 +14,28 @@
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "asphalt-web"
 author = "Alex Grönholm"
 copyright = "2022, " + author
 
-v = parse(version(project))
+v = parse(metadata.version(project))
 version = v.base_version
 release = v.public
 
-language = None
+language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 highlight_language = "python3"
 todo_include_todos = False
 autodoc_inherit_docstrings = False
 autodoc_default_options = {"show-inheritance": True}
 
 html_theme = "sphinx_rtd_theme"
-html_static_path = ["_static"]
 htmlhelp_basename = project.replace("-", "") + "doc"
 
 extlinks = {
     "github": (
         f"https://github.com/asphalt-framework/{project}/tree/{release}/%s",
         None,
     )
```

### Comparing `asphalt-web-1.1.0/docs/contributing.rst` & `asphalt-web-1.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/docs/integrations.rst` & `asphalt-web-1.2.0/docs/integrations.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/docs/usage.rst` & `asphalt-web-1.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/examples/asgi3/static.py` & `asphalt-web-1.2.0/examples/asgi3/static.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/examples/django/django_example/settings.py` & `asphalt-web-1.2.0/examples/django/django_example/settings.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/examples/django/django_example/urls.py` & `asphalt-web-1.2.0/examples/django/django_example/urls.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/examples/django/manage.py` & `asphalt-web-1.2.0/examples/django/manage.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/pyproject.toml` & `asphalt-web-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools >= 61",
+    "setuptools >= 64",
     "setuptools_scm[toml] >= 6.4"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asphalt-web"
 description = "Web framework integrations for the Asphalt framework"
@@ -17,97 +17,115 @@
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-    "aiohttp >= 3.8; (extra == 'test' or extra == 'doc' or extra == 'aiohttp') and python_version < '3.11'",
-    "asgiref ~= 3.5; extra == 'test' or extra == 'doc' or extra == 'asgi3' or extra == 'starlette' or extra == 'fastapi' or extra == 'django'",
     "asphalt ~= 4.8",
-    "Django >= 3.2; (extra == 'test' and platform_python_implementation == 'CPython') or extra == 'doc' or extra == 'django'",
-    "fastapi >= 0.75; extra == 'test' or extra == 'doc' or extra == 'fastapi'",
-    "starlette >= 0.17; extra == 'test' or extra == 'doc' or extra == 'starlette'",
-    "uvicorn >= 0.17.6; extra == 'test' or extra == 'doc' or extra == 'asgi3' or extra == 'starlette' or extra == 'fastapi' or extra == 'django'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://asphalt-web.readthedocs.org/en/latest/"
 "Source code" = "https://github.com/asphalt-framework/asphalt-web"
 "Issue tracker" = "https://github.com/asphalt-framework/asphalt-web/issues"
 "Help and support" = "https://github.com/asphalt-framework/asphalt/wiki/Help-and-support"
 
 [project.optional-dependencies]
+aiohttp = [
+    "aiohttp >= 3.8"
+]
+asgi3 = [
+    "asgiref ~= 3.5",
+    "uvicorn >= 0.17.6",
+]
+django = [
+    "Django >= 3.2",
+    "uvicorn >= 0.17.6",
+]
+fastapi = [
+    "fastapi >= 0.75",
+    "uvicorn >= 0.17.6",
+]
+starlette = [
+    "starlette >= 0.17",
+    "uvicorn >= 0.17.6",
+]
 test = [
     "pytest",
     "pytest-asyncio",
     "httpx",
-    "websockets"
+    "websockets",
+    "aiohttp >= 3.8; python_version < '3.12'",
+    "Django >= 3.2; python_implementation == 'CPython'",
+    "asphalt-web[asgi3,starlette,fastapi]",
 ]
 doc = [
-    "Sphinx",
-    "sphinx_rtd_theme",
-    "sphinx-autodoc-typehints >= 1.2.0",
-    "sphinx-tabs >= 3.3.1"
-]
-aiohttp = []
-django = []
-fastapi = []
-starlette = []
+    "Sphinx >= 6.0",
+    "sphinx_rtd_theme >= 1.2.0",
+    "sphinx-autodoc-typehints >= 1.22",
+    "sphinx-tabs >= 3.3.1",
+    "asphalt-web[aiohttp,asgi3,starlette,django,fastapi]",
+]
 
 [project.entry-points."asphalt.components"]
 aiohttp = "asphalt.web.aiohttp:AIOHTTPComponent"
 asgi3 = "asphalt.web.asgi3:ASGIComponent"
 django = "asphalt.web.django:DjangoComponent"
 fastapi = "asphalt.web.fastapi:FastAPIComponent"
 starlette = "asphalt.web.starlette:StarletteComponent"
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
-[tool.isort]
-src_paths = ["src"]
-skip_gitignore = true
-profile = "black"
-
-[tool.flake8]
-max-line-length = 99
-
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short"
 asyncio_mode = "strict"
 testpaths = ["tests"]
 
+[tool.ruff]
+line-length = 99
+select = [
+    "E", "F", "W",  # default flake-8
+    "I",            # isort
+    "PGH",          # pygrep-hooks
+    "UP",           # pyupgrade
+]
+target-version = "py38"
+
+[tool.ruff.isort]
+known-first-party = ["asphalt.web"]
+
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 
 [tool.coverage.run]
 source = ["asphalt.web"]
 relative_files = true
 branch = true
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37, py38, py39, py310, py311, pypy3
+envlist = py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
-isolated_build = true
+minversion = 4.0
 
 [testenv]
 extras = test
 commands = python -m pytest {posargs}
 
 [testenv:docs]
 extras = doc
```

### Comparing `asphalt-web-1.1.0/src/asphalt/web/aiohttp.py` & `asphalt-web-1.2.0/src/asphalt/web/aiohttp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import AsyncIterator, Awaitable, Callable, Coroutine, Sequence
+from collections.abc import AsyncGenerator, Awaitable, Callable, Coroutine, Sequence
 from inspect import iscoroutinefunction
 from typing import Any
 
 from aiohttp.web_app import Application
 from aiohttp.web_middlewares import middleware
 from aiohttp.web_request import Request
 from aiohttp.web_response import Response
@@ -35,15 +35,15 @@
     :param port: the port to bind to
     :param middlewares: list of compatible coroutine functions or dicts to be added as
         middleware using :meth:`add_middleware`
     """
 
     def __init__(
         self,
-        components: dict[str, dict[str, Any] | None] = None,
+        components: dict[str, dict[str, Any] | None] | None = None,
         *,
         app: Application | str | None = None,
         host: str = "127.0.0.1",
         port: int = 8000,
         middlewares: Sequence[
             Callable[..., Coroutine[Any, Any, Any]] | dict[str, Any]
         ] = (),
@@ -91,15 +91,17 @@
 
     async def start(self, ctx: Context) -> None:
         ctx.add_resource(self.app)
         await super().start(ctx)
         await self.start_server(ctx)
 
     @context_teardown
-    async def start_server(self, ctx: Context) -> AsyncIterator[None]:
+    async def start_server(
+        self, ctx: Context
+    ) -> AsyncGenerator[None, Exception | None]:
         """
         Start the HTTP server.
 
         This method is called by the component after the subcomponents have been
         started. If you need to add any middleware that requires resources provided by
         subcomponents, you can override this method and call the superclass
         implementation after the middleware has been added.
```

### Comparing `asphalt-web-1.1.0/src/asphalt/web/asgi3.py` & `asphalt-web-1.2.0/src/asphalt/web/asgi3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from asyncio import create_task, sleep
-from collections.abc import AsyncIterator, Callable, Sequence
+from collections.abc import AsyncGenerator, Callable, Sequence
 from dataclasses import dataclass
 from inspect import isfunction
 from typing import Any, Generic, TypeVar
 
 import uvicorn
 from asgiref.typing import (
     ASGI3Application,
@@ -61,15 +61,15 @@
     :param port: the port to bind to
     :param middlewares: list of callables or dicts to be added as middleware using
         :meth:`add_middleware`
     """
 
     def __init__(
         self,
-        components: dict[str, dict[str, Any] | None] = None,
+        components: dict[str, dict[str, Any] | None] | None = None,
         *,
         app: T_Application | str,
         host: str = "127.0.0.1",
         port: int = 8000,
         middlewares: Sequence[Callable[..., ASGI3Application] | dict[str, Any]] = (),
     ) -> None:
         super().__init__(components)
@@ -118,15 +118,17 @@
             types.append(type(self.original_app))
 
         ctx.add_resource(self.original_app, types=types)
         await super().start(ctx)
         await self.start_server(ctx)
 
     @context_teardown
-    async def start_server(self, ctx: Context) -> AsyncIterator[None]:
+    async def start_server(
+        self, ctx: Context
+    ) -> AsyncGenerator[None, Exception | None]:
         """
         Start the HTTP server.
 
         This method is called by the component after the subcomponents have been
         started. If you need to add any middleware that requires resources provided by
         subcomponents, you can override this method and call the superclass
         implementation after the middleware has been added.
```

### Comparing `asphalt-web-1.1.0/src/asphalt/web/django.py` & `asphalt-web-1.2.0/src/asphalt/web/django.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/src/asphalt/web/fastapi.py` & `asphalt-web-1.2.0/src/asphalt/web/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         ignored if an application object is explicitly passed in)
     :param middlewares: list of callables or dicts to be added as middleware using
         :meth:`add_middleware`
     """
 
     def __init__(
         self,
-        components: dict[str, dict[str, Any] | None] = None,
+        components: dict[str, dict[str, Any] | None] | None = None,
         *,
         app: FastAPI | str | None = None,
         host: str = "127.0.0.1",
         port: int = 8000,
         debug: bool | None = None,
         middlewares: Sequence[Callable[..., ASGI3Application] | dict[str, Any]] = (),
     ) -> None:
```

### Comparing `asphalt-web-1.1.0/src/asphalt/web/starlette.py` & `asphalt-web-1.2.0/src/asphalt/web/starlette.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         ignored if an application object is explicitly passed in)
     :param middlewares: list of callables or dicts to be added as middleware using
         :meth:`add_middleware`
     """
 
     def __init__(
         self,
-        components: dict[str, dict[str, Any] | None] = None,
+        components: dict[str, dict[str, Any] | None] | None = None,
         *,
         app: Starlette | None = None,
         host: str = "127.0.0.1",
         port: int = 8000,
         debug: bool | None = None,
         middlewares: Sequence[Callable[..., ASGI3Application] | dict[str, Any]] = (),
     ) -> None:
```

### Comparing `asphalt-web-1.1.0/src/asphalt_web.egg-info/PKG-INFO` & `asphalt-web-1.2.0/src/asphalt_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: asphalt-web
-Version: 1.1.0
+Version: 1.2.0
 Summary: Web framework integrations for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Documentation, https://asphalt-web.readthedocs.org/en/latest/
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt-web
 Project-URL: Issue tracker, https://github.com/asphalt-framework/asphalt-web/issues
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: doc
 Provides-Extra: aiohttp
+Provides-Extra: asgi3
 Provides-Extra: django
 Provides-Extra: fastapi
 Provides-Extra: starlette
+Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/asphalt-framework/asphalt-web/actions/workflows/test.yml/badge.svg
   :target: https://github.com/asphalt-framework/asphalt-web/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/github/asphalt-framework/asphalt-web/badge.svg?branch=master
   :target: https://coveralls.io/github/asphalt-framework/asphalt-web?branch=master
@@ -66,9 +66,7 @@
 Project links
 -------------
 
 * `Documentation <http://asphalt-web.readthedocs.org/en/latest/>`_
 * `Help and support <https://github.com/asphalt-framework/asphalt/wiki/Help-and-support>`_
 * `Source code <https://github.com/asphalt-framework/asphalt-web>`_
 * `Issue tracker <https://github.com/asphalt-framework/asphalt-web/issues>`_
-
-
```

### Comparing `asphalt-web-1.1.0/src/asphalt_web.egg-info/SOURCES.txt` & `asphalt-web-1.2.0/src/asphalt_web.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/integrations.rst
 docs/py-modindex.rst
```

### Comparing `asphalt-web-1.1.0/tests/django_app/settings.py` & `asphalt-web-1.2.0/tests/django_app/settings.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/tests/django_app/urls.py` & `asphalt-web-1.2.0/tests/django_app/urls.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/tests/test_aiohttp.py` & `asphalt-web-1.2.0/tests/test_aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         await ws.send_json(
             {
                 "message": f"Hello {message}",
                 "my resource": my_resource,
                 "another resource": another_resource,
             }
         )
+        return ws
 
     application = Application()
     if method == "static":
         application.router.add_route("GET", "/", ws_root)
         components = {}
     else:
```

### Comparing `asphalt-web-1.1.0/tests/test_asgi3.py` & `asphalt-web-1.2.0/tests/test_asgi3.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/tests/test_django.py` & `asphalt-web-1.2.0/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/tests/test_fastapi.py` & `asphalt-web-1.2.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.1.0/tests/test_starlette.py` & `asphalt-web-1.2.0/tests/test_starlette.py`

 * *Files identical despite different names*

