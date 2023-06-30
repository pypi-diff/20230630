# Comparing `tmp/aiohttp-devtools-1.0.post0.tar.gz` & `tmp/aiohttp-devtools-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-devtools-1.0.post0.tar", last modified: Fri Dec 31 20:45:22 2021, max compression
+gzip compressed data, was "aiohttp-devtools-1.1.tar", last modified: Fri Jun 30 18:58:14 2023, max compression
```

## Comparing `aiohttp-devtools-1.0.post0.tar` & `aiohttp-devtools-1.1.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/aiohttp_devtools/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4625 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    37357 2021-12-31 20:45:15.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/livereload.js
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/log_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    12985 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/serve.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      755 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-31 20:45:22.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 20:45:21.000000 aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-12-31 20:45:22.095523 aiohttp-devtools-1.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2021-12-31 20:45:06.000000 aiohttp-devtools-1.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:58:14.985043 aiohttp-devtools-1.1/aiohttp_devtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/aiohttp_devtools/runserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37357 2023-06-30 18:58:08.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/livereload.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/log_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/aiohttp_devtools/runserver/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:58:14.000000 aiohttp-devtools-1.1/aiohttp_devtools.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:58:14.989044 aiohttp-devtools-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_runserver_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-30 18:58:01.000000 aiohttp-devtools-1.1/tests/test_utils.py
```

### Comparing `aiohttp-devtools-1.0.post0/LICENSE` & `aiohttp-devtools-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp-devtools-1.0.post0/PKG-INFO` & `aiohttp-devtools-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: aiohttp-devtools
-Version: 1.0.post0
+Version: 1.1
 Summary: Dev tools for aiohttp
 Home-page: https://github.com/aio-libs/aiohttp-devtools
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Project-URL: CI: AppVeyor, https://ci.appveyor.com/project/aio-libs/aiohttp-devtools
 Project-URL: CI: Travis, https://travis-ci.com/aio-libs/aiohttp-devtools
 Project-URL: Coverage: codecov, https://codecov.io/github/aio-libs/aiohttp-devtools
 Project-URL: GitHub: issues, https://github.com/aio-libs/aiohttp-devtools/issues
 Project-URL: GitHub: repo, https://github.com/aio-libs/aiohttp-devtools
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -37,17 +36,14 @@
 aiohttp-devtools
 ================
 
 |Coverage| |pypi| |license|
 
 Dev tools for `aiohttp`_.
 
-(Note: ``aiohttp-devtools>=0.8`` only supports ``aiohttp>=3.0``, if you're using older aiohttp, please use
-an older version of ``aiohttp-devtools``, see `History.rst`_ for details.)
-
 **aiohttp-devtools** provides a number of tools useful when developing applications with aiohttp and associated
 libraries.
 
 Installation
 ------------
 
 .. code:: shell
@@ -74,22 +70,22 @@
 **Note:** ``adev runserver <app-path>`` will import the whole file, hence it doesn't work
 with ``web.run_app(app)``. You can however use ``if __name__ == '__main__': web.run_app(app)``.
 
 ``app-path`` can be a path to either a directory containing a recognized default file (``app.py``
 or ``main.py``) or to a specific file. The ``--app-factory`` option can be used to define which method is called
 from the app path file, if not supplied some default method names are tried
 (namely `app`, `app_factory`, `get_app` and `create_app`, which can be
-attributes, functions, or coroutines).
+variables, functions, or coroutines).
 
 All ``runserver`` arguments can be set via environment variables.
 
-``runserver`` has a few of useful features:
+``runserver`` has a few useful features:
 
 * **livereload** will reload resources in the browser as your code changes without having to hit refresh, see `livereload`_ for more details.
-* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally
+* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally.
 
 For more options see ``adev runserver --help``.
 
 serve
 ~~~~~
 
 Similar to `runserver`_ except just serves static files.
@@ -118,28 +114,28 @@
     . env/bin/activate
     pip install aiohttp-devtools create-aio-app
 
 
 We're now ready to build our new application with ``create-aio-app`` and we'll name the
 project ``my_new_app`` after the current directory.
 
-We're going to explicitly choose no database here to make, this tutorial easier but you can remove that option
+We're going to explicitly choose no database here to make this tutorial easier, but you can remove that option
 and choose to use a proper database if you like.
 
 You can just hit return to choose the default for all the options.
 
 
 .. code:: shell
 
     create-aio-app my_new_app --without-postgres
 
 That's it, your app is now created. You might want to have a look through the local directory's file tree.
 
 Before you can run your app you'll need to install the other requirements, luckily they've already been listed in
-``./requirements.txt`` by ``create-aio-app``, to install simply run
+``requirements/development.txt`` by ``create-aio-app``, to install simply run
 
 .. code:: shell
 
     pip install -r requirements/development.txt
 
 You can then run your app with just:
 
@@ -158,12 +154,10 @@
 
 .. |Coverage| image:: https://codecov.io/gh/aio-libs/aiohttp-devtools/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/aio-libs/aiohttp-devtools
 .. |pypi| image:: https://img.shields.io/pypi/v/aiohttp-devtools.svg
    :target: https://pypi.python.org/pypi/aiohttp-devtools
 .. |license| image:: https://img.shields.io/pypi/l/aiohttp-devtools.svg
    :target: https://github.com/aio-libs/aiohttp-devtools
-.. _History.rst: /HISTORY.rst
+.. _Changes.txt: /CHANGES.txt
 .. _livereload: https://github.com/livereload/livereload-js
 .. _aiohttp: http://aiohttp.readthedocs.io/en/stable/
-
-
```

### Comparing `aiohttp-devtools-1.0.post0/README.rst` & `aiohttp-devtools-1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 aiohttp-devtools
 ================
 
 |Coverage| |pypi| |license|
 
 Dev tools for `aiohttp`_.
 
-(Note: ``aiohttp-devtools>=0.8`` only supports ``aiohttp>=3.0``, if you're using older aiohttp, please use
-an older version of ``aiohttp-devtools``, see `History.rst`_ for details.)
-
 **aiohttp-devtools** provides a number of tools useful when developing applications with aiohttp and associated
 libraries.
 
 Installation
 ------------
 
 .. code:: shell
@@ -38,22 +35,22 @@
 **Note:** ``adev runserver <app-path>`` will import the whole file, hence it doesn't work
 with ``web.run_app(app)``. You can however use ``if __name__ == '__main__': web.run_app(app)``.
 
 ``app-path`` can be a path to either a directory containing a recognized default file (``app.py``
 or ``main.py``) or to a specific file. The ``--app-factory`` option can be used to define which method is called
 from the app path file, if not supplied some default method names are tried
 (namely `app`, `app_factory`, `get_app` and `create_app`, which can be
-attributes, functions, or coroutines).
+variables, functions, or coroutines).
 
 All ``runserver`` arguments can be set via environment variables.
 
-``runserver`` has a few of useful features:
+``runserver`` has a few useful features:
 
 * **livereload** will reload resources in the browser as your code changes without having to hit refresh, see `livereload`_ for more details.
-* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally
+* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally.
 
 For more options see ``adev runserver --help``.
 
 serve
 ~~~~~
 
 Similar to `runserver`_ except just serves static files.
@@ -82,28 +79,28 @@
     . env/bin/activate
     pip install aiohttp-devtools create-aio-app
 
 
 We're now ready to build our new application with ``create-aio-app`` and we'll name the
 project ``my_new_app`` after the current directory.
 
-We're going to explicitly choose no database here to make, this tutorial easier but you can remove that option
+We're going to explicitly choose no database here to make this tutorial easier, but you can remove that option
 and choose to use a proper database if you like.
 
 You can just hit return to choose the default for all the options.
 
 
 .. code:: shell
 
     create-aio-app my_new_app --without-postgres
 
 That's it, your app is now created. You might want to have a look through the local directory's file tree.
 
 Before you can run your app you'll need to install the other requirements, luckily they've already been listed in
-``./requirements.txt`` by ``create-aio-app``, to install simply run
+``requirements/development.txt`` by ``create-aio-app``, to install simply run
 
 .. code:: shell
 
     pip install -r requirements/development.txt
 
 You can then run your app with just:
 
@@ -122,10 +119,10 @@
 
 .. |Coverage| image:: https://codecov.io/gh/aio-libs/aiohttp-devtools/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/aio-libs/aiohttp-devtools
 .. |pypi| image:: https://img.shields.io/pypi/v/aiohttp-devtools.svg
    :target: https://pypi.python.org/pypi/aiohttp-devtools
 .. |license| image:: https://img.shields.io/pypi/l/aiohttp-devtools.svg
    :target: https://github.com/aio-libs/aiohttp-devtools
-.. _History.rst: /HISTORY.rst
+.. _Changes.txt: /CHANGES.txt
 .. _livereload: https://github.com/livereload/livereload-js
 .. _aiohttp: http://aiohttp.readthedocs.io/en/stable/
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/cli.py` & `aiohttp-devtools-1.1/aiohttp_devtools/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import traceback
+from typing import Any
 
 import click
 from aiohttp.web import run_app
 
 from . import __version__
 from .exceptions import AiohttpDevException
 from .logs import main_logger, setup_logging
@@ -14,41 +15,49 @@
 _dir_existing = click.Path(exists=True, dir_okay=True, file_okay=False)
 _file_dir_existing = click.Path(exists=True, dir_okay=True, file_okay=True)
 _dir_may_exist = click.Path(dir_okay=True, file_okay=False, writable=True, resolve_path=True)
 
 
 @click.group()
 @click.version_option(__version__, "-V", "--version", prog_name="aiohttp-devtools")
-def cli():
+def cli() -> None:
     pass
 
 
 verbose_help = 'Enable verbose output.'
 livereload_help = ('Whether to inject livereload.js into html page footers to autoreload on changes. '
                    'env variable AIO_LIVERELOAD')
+browser_cache_help = ("When disabled (the default), sends no-cache headers to "
+                      "disable browser caching.")
 
 
 @cli.command()
 @click.argument('path', type=_dir_existing, required=True)
 @click.option('--livereload/--no-livereload', envvar='AIO_LIVERELOAD', default=True, help=livereload_help)
 @click.option('-p', '--port', default=8000, type=int)
 @click.option('-v', '--verbose', is_flag=True, help=verbose_help)
-def serve(path, livereload, port, verbose):
+@click.option("--browser-cache/--no-browser-cache", envvar="AIO_BROWSER_CACHE", default=False,
+              help=browser_cache_help)
+def serve(path: str, livereload: bool, port: int, verbose: bool, browser_cache: bool) -> None:
     """
     Serve static files from a directory.
     """
     setup_logging(verbose)
-    run_app(**serve_static(static_path=path, livereload=livereload, port=port))
+    run_app(**serve_static(static_path=path, livereload=livereload, port=port,
+                           browser_cache=browser_cache))
 
 
 static_help = "Path of static files to serve, if excluded static files aren't served. env variable: AIO_STATIC_STATIC"
 root_help = ('Root directory project used to qualify other paths. '
              'This can be used to watch a parent directory for changes in a more complex application. '
              'env variable: AIO_ROOT')
 static_url_help = 'URL path to serve static files from, default "/static/". env variable: AIO_STATIC_URL'
+shutdown_by_url_help = ("The development server will be stopped via a request to an endpoint that is "
+                        "added to the server, instead of via signals (this is the default on Windows). "
+                        "env variable: AIO_SHUTDOWN_BY_URL")
 host_help = ('host used when referencing livereload and static files, if blank host is taken from the request header '
              'with default of localhost. env variable AIO_HOST')
 app_factory_help = ('name of the app factory to create an aiohttp.web.Application with, if missing default app-factory '
                     'names are tried. This can be either a function with signature '
                     '"def create_app(loop): -> Application" or "def create_app(): -> Application" '
                     'or just an instance of aiohttp.Application. env variable AIO_APP_FACTORY')
 port_help = 'Port to serve app from, default 8000. env variable: AIO_PORT'
@@ -57,22 +66,26 @@
 
 # defaults are all None here so default settings are defined in one place: DEV_DICT validation
 @cli.command()
 @click.argument('app-path', envvar='AIO_APP_PATH', type=_file_dir_existing, required=False)
 @click.option('-s', '--static', 'static_path', envvar='AIO_STATIC_PATH', type=_dir_existing, help=static_help)
 @click.option('--root', 'root_path', envvar='AIO_ROOT', type=_dir_existing, help=root_help)
 @click.option('--static-url', envvar='AIO_STATIC_URL', help=static_url_help)
+@click.option("--shutdown-by-url/--no-shutdown-by-url", default=sys.platform.startswith("win32"),
+              envvar="AIO_SHUTDOWN_BY_URL", help=shutdown_by_url_help)
 @click.option('--livereload/--no-livereload', envvar='AIO_LIVERELOAD', default=None, help=livereload_help)
 @click.option('--host', default=INFER_HOST, help=host_help)
 @click.option('--app-factory', 'app_factory_name', envvar='AIO_APP_FACTORY', help=app_factory_help)
 @click.option('-p', '--port', 'main_port', envvar='AIO_PORT', type=click.INT, help=port_help)
 @click.option('--aux-port', envvar='AIO_AUX_PORT', type=click.INT, help=aux_port_help)
 @click.option('-v', '--verbose', is_flag=True, help=verbose_help)
+@click.option("--browser-cache/--no-browser-cache", envvar="AIO_BROWSER_CACHE", default=None,
+              help=browser_cache_help)
 @click.argument('project_args', nargs=-1)
-def runserver(**config):
+def runserver(**config: Any) -> None:
     """
     Run a development server for an aiohttp apps.
 
     Takes one argument "app-path" which should be a path to either a directory containing a recognized default file
     ("app.py" or "main.py") or to a specific file. Defaults to the environment variable "AIO_APP_PATH" or ".".
 
     The app path is run directly, see the "--app-factory" option for details on how an app is loaded from a python
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/logs.py` & `aiohttp-devtools-1.1/aiohttp_devtools/logs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import json
 import logging
 import logging.config
 import platform
 import re
+import sys
 import traceback
 from io import StringIO
+from types import TracebackType
+from typing import Dict, Optional, Tuple, Type, Union
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Literal
+else:
+    from typing import Literal
 
 import pygments
 from devtools import pformat
-from devtools.ansi import isatty, sformat
+from devtools.ansi import sformat
+from devtools.utils import isatty
 from pygments.formatters import Terminal256Formatter
 from pygments.lexers import Python3TracebackLexer
 
+_Ei = Union[Tuple[Type[BaseException], BaseException, Optional[TracebackType]], Tuple[None, None, None]]
+
 rs_dft_logger = logging.getLogger('adev.server.dft')
 rs_aux_logger = logging.getLogger('adev.server.aux')
 
 tools_logger = logging.getLogger('adev.tools')
 main_logger = logging.getLogger('adev.main')
 
 LOG_FORMATS = {
@@ -24,47 +35,40 @@
     logging.WARN: sformat.yellow,
 }
 pyg_lexer = Python3TracebackLexer()
 pyg_formatter = Terminal256Formatter(style='vim')
 split_log = re.compile(r'^(\[.*?\])')
 
 
-class HighlightStreamHandler(logging.StreamHandler):
-    def setFormatter(self, fmt):
-        self.formatter = fmt
-        self.formatter.stream_is_tty = isatty(self.stream) and platform.system().lower() != 'windows'
-
-
 class DefaultFormatter(logging.Formatter):
-    def __init__(self, fmt=None, datefmt=None, style='%'):
+    def __init__(self, fmt: Optional[str] = None, datefmt: Optional[str] = None, style: Literal["%", "{", "$"] = "%"):
         super().__init__(fmt, datefmt, style)
         self.stream_is_tty = False
 
-    def format(self, record):
+    def format(self, record: logging.LogRecord) -> str:
         msg = super().format(record)
         if not self.stream_is_tty:
             return msg
         m = split_log.match(msg)
         log_color = LOG_FORMATS.get(record.levelno, sformat.red)
         if m:
             time = sformat(m.groups()[0], sformat.magenta)
             return time + sformat(msg[m.end():], log_color)
-        else:
-            return sformat(msg, log_color)
+
+        return sformat(msg, log_color)
 
 
 class AccessFormatter(logging.Formatter):
-    """
-    Used to log aiohttp_access and aiohttp_server
-    """
-    def __init__(self, fmt=None, datefmt=None, style='%'):
+    """Used to log aiohttp_access and aiohttp_server."""
+
+    def __init__(self, fmt: Optional[str] = None, datefmt: Optional[str] = None, style: Literal["%", "{", "$"] = "%"):
         super().__init__(fmt, datefmt, style)
         self.stream_is_tty = False
 
-    def formatMessage(self, record):
+    def formatMessage(self, record: logging.LogRecord) -> str:
         msg = super().formatMessage(record)
         if msg[0] != '{':
             return msg
         # json from AccessLogger
         obj = json.loads(msg)
         if self.stream_is_tty:
             # in future we can do clever things about colouring the message based on status code
@@ -76,26 +80,35 @@
         else:
             msg = '{time} {prefix} {msg}'.format(**obj)
         details = getattr(record, 'details', None)
         if details:
             msg = 'details: {}\n{}'.format(pformat(details, highlight=self.stream_is_tty), msg)
         return msg
 
-    def formatException(self, ei):
+    def formatException(self, ei: _Ei) -> str:
         sio = StringIO()
-        traceback.print_exception(*ei, file=sio)
+        traceback.print_exception(*ei, file=sio)  # type: ignore[misc]
         stack = sio.getvalue()
         sio.close()
         if self.stream_is_tty and pyg_lexer:
-            return pygments.highlight(stack, lexer=pyg_lexer, formatter=pyg_formatter).rstrip('\n')
-        else:
-            return stack
+            return pygments.highlight(stack, lexer=pyg_lexer, formatter=pyg_formatter).rstrip("\n")
+
+        return stack
+
+
+class HighlightStreamHandler(logging.StreamHandler):  # type: ignore[type-arg]
+    def setFormatter(self, fmt: Optional[logging.Formatter]) -> None:
+        stream_is_tty = isatty(self.stream) and platform.system().lower() != "windows"
+        if isinstance(fmt, (DefaultFormatter, AccessFormatter)):
+            fmt.stream_is_tty = stream_is_tty
+
+        self.formatter = fmt
 
 
-def log_config(verbose: bool) -> dict:
+def log_config(verbose: bool) -> Dict[str, object]:
     """
     Setup default config. for dictConfig.
     :param verbose: level: DEBUG if True, INFO if False
     :return: dict suitable for ``logging.config.dictConfig``
     """
     log_level = 'DEBUG' if verbose else 'INFO'
     return {
@@ -163,10 +176,10 @@
                 'handlers': ['aiohttp_server'],
                 'level': log_level,
             },
         },
     }
 
 
-def setup_logging(verbose):
+def setup_logging(verbose: bool) -> None:
     config = log_config(verbose)
     logging.config.dictConfig(config)
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/config.py` & `aiohttp-devtools-1.1/aiohttp_devtools/runserver/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import asyncio
-import inspect
 import re
 import sys
 from importlib import import_module
 from pathlib import Path
-from typing import Optional
+from typing import Awaitable, Callable, Optional, Union
 
 from aiohttp import web
 
+import __main__
 from ..exceptions import AiohttpDevConfigError as AdevConfigError
 from ..logs import rs_dft_logger as logger
 
+AppFactory = Union[web.Application, Callable[[], web.Application], Callable[[], Awaitable[web.Application]]]
+
 STD_FILE_NAMES = [
     re.compile(r'main\.py'),
     re.compile(r'app\.py'),
 ]
 
 
 APP_FACTORY_NAMES = [
@@ -32,18 +34,21 @@
                  app_path: str = '.',
                  root_path: Optional[str] = None,
                  verbose: bool = False,
                  static_path: Optional[str] = None,
                  python_path: Optional[str] = None,
                  static_url: str = '/static/',
                  livereload: bool = True,
+                 shutdown_by_url: bool = sys.platform.startswith("win32"),
+                 path_prefix: str = "/_devtools",
                  app_factory_name: Optional[str] = None,
                  host: str = INFER_HOST,
                  main_port: int = 8000,
-                 aux_port: Optional[int] = None):
+                 aux_port: Optional[int] = None,
+                 browser_cache: bool = False):
         if root_path:
             self.root_path = Path(root_path).resolve()
             logger.debug('Root path specified: %s', self.root_path)
             self.watch_path: Optional[Path] = self.root_path
         else:
             logger.debug('Root path not specified, using current working directory')
             self.root_path = Path('.').resolve()
@@ -52,29 +57,35 @@
         self.app_path = self._find_app_path(app_path)
         if not self.app_path.name.endswith('.py'):
             raise AdevConfigError('Unexpected extension for app_path: %s, should be .py' % self.app_path.name)
         self.verbose = verbose
         self.settings_found = False
 
         self.py_file = self._resolve_path(str(self.app_path), 'is_file', 'app-path')
-        self.python_path = self._resolve_path(python_path, 'is_dir', 'python-path') or self.root_path
+        if python_path:
+            self.python_path = self._resolve_path(python_path, "is_dir", "python-path")
+        else:
+            self.python_path = self.root_path
 
-        self.static_path = self._resolve_path(static_path, 'is_dir', 'static-path')
+        self.static_path = self._resolve_path(static_path, "is_dir", "static-path") if static_path else None
         self.static_url = static_url
         self.livereload = livereload
+        self.shutdown_by_url = shutdown_by_url
+        self.path_prefix = path_prefix
         self.app_factory_name = app_factory_name
         self.infer_host = host == INFER_HOST
         self.host = 'localhost' if self.infer_host else host
         self.main_port = main_port
         self.aux_port = aux_port or (main_port + 1)
+        self.browser_cache = browser_cache
         logger.debug('config loaded:\n%s', self)
 
     @property
     def static_path_str(self) -> Optional[str]:
-        return self.static_path and str(self.static_path)
+        return str(self.static_path) if self.static_path else None
 
     def _find_app_path(self, app_path: str) -> Path:
         # for backwards compatibility try this first
         path = (self.root_path / app_path).resolve()
         if not path.exists():
             path = Path(app_path).resolve()
         if path.is_file():
@@ -90,18 +101,15 @@
                 pass
             else:
                 logger.debug('app_path is a directory with a recognised file %s', file_path)
                 return file_path
         raise AdevConfigError('unable to find a recognised default file ("app.py" or "main.py") '
                               'in the directory "%s"' % app_path)
 
-    def _resolve_path(self, _path: Optional[str], check: str, arg_name: str):
-        if _path is None:
-            return
-
+    def _resolve_path(self, _path: str, check: str, arg_name: str) -> Path:
         if _path.startswith('/'):
             path = Path(_path)
             error_msg = '{arg_name} "{path}" is not a valid path'
         else:
             path = Path(self.root_path / _path)
             error_msg = '{arg_name} "{path}" is not a valid path relative to {root}'
 
@@ -115,25 +123,28 @@
                 raise AdevConfigError('{} is not a file'.format(path))
         else:
             assert check == 'is_dir'
             if not path.is_dir():
                 raise AdevConfigError('{} is not a directory'.format(path))
         return path
 
-    def import_app_factory(self):
-        """
-        Import attribute/class from from a python module. Raise AdevConfigError if the import failed.
+    def import_app_factory(self) -> AppFactory:
+        """Import and return attribute/class from a python module.
 
-        :return: (attribute, Path object for directory of file)
+        Raises:
+            AdevConfigError - If the import failed.
         """
         rel_py_file = self.py_file.relative_to(self.python_path)
         module_path = '.'.join(rel_py_file.with_suffix('').parts)
 
         sys.path.append(str(self.python_path))
         module = import_module(module_path)
+        # Rewrite the package name, so it will appear the same as running the app.
+        if module.__package__:
+            __main__.__package__ = module.__package__
 
         logger.debug('successfully loaded "%s" from "%s"', module_path, self.python_path)
 
         if self.app_factory_name is None:
             try:
                 self.app_factory_name = next(an for an in APP_FACTORY_NAMES if hasattr(module, an))
             except StopIteration as e:
@@ -141,40 +152,43 @@
                                       'found in {s.py_file.name}'.format(s=self)) from e
             else:
                 logger.debug('found default attribute "%s" in module "%s"',
                              self.app_factory_name, module)
 
         try:
             attr = getattr(module, self.app_factory_name)
-        except AttributeError as e:
-            raise AdevConfigError('Module "{s.py_file.name}" '
-                                  'does not define a "{s.app_factory_name}" attribute/class'.format(s=self)) from e
+        except AttributeError:
+            raise AdevConfigError("Module '{}' does not define a '{}' attribute/class".format(
+                self.py_file.name, self.app_factory_name))
+
+        if not isinstance(attr, web.Application) and not callable(attr):
+            raise AdevConfigError("'{}.{}' is not an Application or callable".format(
+                self.py_file.name, self.app_factory_name))
+
+        if hasattr(attr, "__code__"):
+            required_args = attr.__code__.co_argcount - len(attr.__defaults__ or ())
+            if required_args > 0:
+                raise AdevConfigError("'{}.{}' should not have required arguments.".format(
+                    self.py_file.name, self.app_factory_name))
 
-        self.watch_path = self.watch_path or Path(module.__file__).parent
-        return attr
+        self.watch_path = self.watch_path or Path(module.__file__ or ".").parent
+        return attr  # type: ignore[no-any-return]
 
-    async def load_app(self, app_factory):
+    async def load_app(self, app_factory: AppFactory) -> web.Application:
         if isinstance(app_factory, web.Application):
-            app = app_factory
-        else:
-            # app_factory should be a proper factory with signature (loop): -> Application
-            signature = inspect.signature(app_factory)
-            if 'loop' in signature.parameters:
-                loop = asyncio.get_event_loop()
-                app = app_factory(loop=loop)
-            else:
-                # loop argument missing, assume no arguments
-                app = app_factory()
+            return app_factory
+
+        app = app_factory()
 
-            if asyncio.iscoroutine(app):
-                app = await app  # type: ignore[misc]
+        if asyncio.iscoroutine(app):
+            app = await app
 
-            if not isinstance(app, web.Application):
-                raise AdevConfigError('app factory "{.app_factory_name}" returned "{.__class__.__name__}" not an '
-                                      'aiohttp.web.Application'.format(self, app))
+        if not isinstance(app, web.Application):
+            raise AdevConfigError("app factory '{}' returned '{}' not an aiohttp.web.Application".format(
+                self.app_factory_name, app.__class__.__name__))
 
         return app
 
-    def __str__(self):
-        fields = ('py_file', 'static_path', 'static_url', 'livereload',
-                  'app_factory_name', 'host', 'main_port', 'aux_port')
+    def __str__(self) -> str:
+        fields = ("py_file", "static_path", "static_url", "livereload", "shutdown_by_url",
+                  "path_prefix", "app_factory_name", "host", "main_port", "aux_port")
         return 'Config:\n' + '\n'.join('  {0}: {1!r}'.format(f, getattr(self, f)) for f in fields)
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/livereload.js` & `aiohttp-devtools-1.1/aiohttp_devtools/runserver/livereload.js`

 * *Files identical despite different names*

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/log_handlers.py` & `aiohttp-devtools-1.1/aiohttp_devtools/runserver/log_handlers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
 import warnings
 from datetime import datetime, timedelta
-from typing import cast
+from typing import Dict, Optional, Union, cast
 
+from aiohttp import web
 from aiohttp.abc import AbstractAccessLogger
 
 dbtb = '/_debugtoolbar/'
 check = '?_checking_alive=1'
 
 
 class _AccessLogger(AbstractAccessLogger):
     prefix: str
 
-    def get_msg(self, request, response, time):
+    def get_msg(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> Optional[str]:
         raise NotImplementedError()
 
-    def extra(self, request, response, time):
+    def extra(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> Optional[Dict[str, object]]:
         pass
 
-    def log(self, request, response, time):
+    def log(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> None:
         msg = self.get_msg(request, response, time)
         if not msg:
             return
         now = datetime.now()
         start_time = now - timedelta(seconds=time)
         pqs = request.path_qs
         # log messages are encoded to JSON, so they can be easily coloured or not by the logger which knows whether
@@ -35,65 +36,71 @@
         })
         self.logger.info(msg, extra=self.extra(request, response, time))
 
 
 class AccessLogger(_AccessLogger):
     prefix = '●'
 
-    def get_msg(self, request, response, time):
+    def get_msg(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> str:
         return '{method} {path} {code} {size} {ms:0.0f}ms'.format(
             method=request.method,
             path=request.path_qs,
             code=response.status,
             size=fmt_size(response.body_length),
             ms=time * 1000,
         )
 
-    def extra(self, request, response, time: float):
-        if response.status > 310:
-            request_body = request._read_bytes
-            details = dict(
-                request_duration_ms=round(time * 1000, 3),
-                request_headers=dict(request.headers),
-                request_body=parse_body(request_body, 'request body'),
-                request_size=fmt_size(0 if request_body is None else len(request_body)),
-                response_headers=dict(response.headers),
-                response_body=parse_body(response.text or response.body, 'response body'),
-            )
-            return dict(details=details)
+    def extra(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> Optional[Dict[str, object]]:
+        if response.status <= 310:
+            return None
+
+        request_body = request._read_bytes
+        body_text = response.text if isinstance(response, web.Response) else None
+        details = {
+            "request_duration_ms": round(time * 1000, 3),
+            "request_headers": dict(request.headers),
+            "request_body": parse_body(request_body, "request body"),
+            "request_size": fmt_size(0 if request_body is None else len(request_body)),
+            "response_headers": dict(response.headers),
+            "response_body": parse_body(body_text, "response body"),
+        }
+        return {"details": details}
 
 
 class AuxAccessLogger(_AccessLogger):
     prefix = '◆'
 
-    def get_msg(self, request, response, time):
+    def get_msg(self, request: web.BaseRequest, response: web.StreamResponse, time: float) -> Optional[str]:
         # don't log livereload
-        if request.path not in {'/livereload', '/livereload.js'}:
-            return '{method} {path} {code} {size}'.format(
-                method=request.method,
-                path=request.path_qs,
-                code=response.status,
-                size=fmt_size(response.body_length),
-            )
+        if request.path in {"/livereload", "/livereload.js"}:
+            return None
+
+        return "{method} {path} {code} {size}".format(
+            method=request.method,
+            path=request.path_qs,
+            code=response.status,
+            size=fmt_size(response.body_length),
+        )
 
 
-def fmt_size(num):
+def fmt_size(num: int) -> str:
     if not num:
         return ''
     if num < 1024:
         return '{:0.0f}B'.format(num)
     else:
         return '{:0.1f}KB'.format(num / 1024)
 
 
-def parse_body(v, name):
-    if isinstance(v, (str, bytes)):
-        try:
-            return json.loads(v)
-        except UnicodeDecodeError:
-            v = cast(bytes, v)  # UnicodeDecodeError only occurs on bytes.
-            warnings.warn('UnicodeDecodeError parsing ' + name, UserWarning)
-            # bytes which cause UnicodeDecodeError can cause problems later on
-            return v.decode(errors='ignore')
-        except (ValueError, TypeError):
-            pass
-    return v
+def parse_body(v: Union[str, bytes, None], name: str) -> object:
+    if v is None:
+        return v
+
+    try:
+        return json.loads(v)
+    except UnicodeDecodeError:
+        v = cast(bytes, v)  # UnicodeDecodeError only occurs on bytes.
+        warnings.warn("UnicodeDecodeError parsing " + name, UserWarning)
+        # bytes which cause UnicodeDecodeError can cause problems later on
+        return v.decode(errors="ignore")
+    except (ValueError, TypeError):
+        return v
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/main.py` & `aiohttp-devtools-1.1/aiohttp_devtools/runserver/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 import asyncio
 import os
+import sys
 from multiprocessing import set_start_method
+from typing import Any, Type
+
+from aiohttp.abc import AbstractAccessLogger
+from aiohttp.web import Application
 
 from ..logs import rs_dft_logger as logger
 from .config import Config
 from .log_handlers import AuxAccessLogger
 from .serve import HOST, check_port_open, create_auxiliary_app
 from .watch import AppTask, LiveReloadTask
 
+if sys.version_info < (3, 8):
+    from typing_extensions import TypedDict
+else:
+    from typing import TypedDict
+
+
+class RunServer(TypedDict):
+    app: Application
+    host: str
+    port: int
+    shutdown_timeout: float
+    access_log_class: Type[AbstractAccessLogger]
 
-def runserver(**config_kwargs):
-    """
-    Prepare app ready to run development server.
+
+def runserver(**config_kwargs: Any) -> RunServer:
+    """Prepare app ready to run development server.
 
     :param config_kwargs: see config.Config for more details
     :return: tuple (auxiliary app, auxiliary app port, event loop)
     """
     # force a full reload in sub processes so they load an updated version of code, this must be called only once
     set_start_method('spawn')
 
@@ -45,18 +62,20 @@
         rel_path = config.static_path.relative_to(os.getcwd())
         logger.info('serving static files from ./%s/ at %s%s', rel_path, url, config.static_url)
 
     return {"app": aux_app, "host": HOST, "port": config.aux_port,
             "shutdown_timeout": 0.01, "access_log_class": AuxAccessLogger}
 
 
-def serve_static(*, static_path: str, livereload: bool = True, port: int = 8000):
+def serve_static(*, static_path: str, livereload: bool = True, port: int = 8000,
+                 browser_cache: bool = False) -> RunServer:
     logger.debug('Config: path="%s", livereload=%s, port=%s', static_path, livereload, port)
 
-    app = create_auxiliary_app(static_path=static_path, livereload=livereload)
+    app = create_auxiliary_app(static_path=static_path, livereload=livereload,
+                               browser_cache=browser_cache)
 
     if livereload:
         livereload_manager = LiveReloadTask(static_path)
         logger.debug('starting livereload to watch %s', static_path)
         app.cleanup_ctx.append(livereload_manager.cleanup_ctx)
 
     livereload_status = 'ON' if livereload else 'OFF'
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools/runserver/serve.py` & `aiohttp-devtools-1.1/aiohttp_devtools/runserver/serve.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,196 @@
 import asyncio
 import contextlib
 import json
 import mimetypes
 import sys
 from errno import EADDRINUSE
 from pathlib import Path
-from typing import Optional
+from typing import Any, Iterator, Optional, NoReturn
 
 from aiohttp import WSMsgType, web
 from aiohttp.hdrs import LAST_MODIFIED, CONTENT_LENGTH
-from aiohttp.web import FileResponse, Response
+from aiohttp.typedefs import Handler
 from aiohttp.web_exceptions import HTTPNotFound, HTTPNotModified
+from aiohttp.web_runner import GracefulExit
 from aiohttp.web_urldispatcher import StaticResource
 from yarl import URL
 
 from ..exceptions import AiohttpDevException
 from ..logs import rs_aux_logger as aux_logger
 from ..logs import rs_dft_logger as dft_logger
 from ..logs import setup_logging
-from .config import Config
+from .config import AppFactory, Config
 from .log_handlers import AccessLogger
 from .utils import MutableValue
 
 LIVE_RELOAD_HOST_SNIPPET = '\n<script src="http://{}:{}/livereload.js"></script>\n'
 LIVE_RELOAD_LOCAL_SNIPPET = b'\n<script src="/livereload.js"></script>\n'
 HOST = '0.0.0.0'
 
 
-def _set_static_url(app, url):
+def _set_static_url(app: web.Application, url: str) -> None:
     app["static_root_url"] = MutableValue(url)
     for subapp in app._subapps:
         _set_static_url(subapp, url)
 
 
-def _change_static_url(app, url):
+def _change_static_url(app: web.Application, url: str) -> None:
     app["static_root_url"].change(url)
     for subapp in app._subapps:
         _change_static_url(subapp, url)
 
 
-def modify_main_app(app, config: Config):
+def modify_main_app(app: web.Application, config: Config) -> None:  # noqa: C901
     """
     Modify the app we're serving to make development easier, eg.
     * modify responses to add the livereload snippet
-    * set ``static_root_url`` on the app
+    * set ``static_root_url`` on the app (for use with aiohttp-jinja2)
     """
     app._debug = True
     dft_logger.debug('livereload enabled: %s', '✓' if config.livereload else '✖')
 
-    def get_host(request):
+    def get_host(request: web.Request) -> str:
         if config.infer_host:
             return request.headers.get('host', 'localhost').split(':', 1)[0]
         else:
             return config.host
 
     if config.livereload:
-        async def on_prepare(request, response):
-            if (not request.path.startswith('/_debugtoolbar') and
-                    'text/html' in response.content_type and
-                    getattr(response, 'body', False)):
-                lr_snippet = LIVE_RELOAD_HOST_SNIPPET.format(get_host(request), config.aux_port)
-                dft_logger.debug('appending live reload snippet "%s" to body', lr_snippet)
-                response.body += lr_snippet.encode()
-                response.headers[CONTENT_LENGTH] = str(len(response.body))
+        async def on_prepare(request: web.Request, response: web.StreamResponse) -> None:
+            if (not isinstance(response, web.Response)
+                    or not isinstance(response.body, bytes)  # No support for Payload
+                    or request.path.startswith("/_debugtoolbar")
+                    or "text/html" not in response.content_type):
+                return
+            lr_snippet = LIVE_RELOAD_HOST_SNIPPET.format(get_host(request), config.aux_port)
+            dft_logger.debug("appending live reload snippet '%s' to body", lr_snippet)
+            response.body += lr_snippet.encode()
+            response.headers[CONTENT_LENGTH] = str(len(response.body))
         app.on_response_prepare.append(on_prepare)
 
+    if not config.browser_cache:
+        @web.middleware
+        async def no_cache_middleware(request: web.Request, handler: Handler) -> web.StreamResponse:
+            """Add no-cache header to avoid browser caching in local development."""
+            response = await handler(request)
+            response.headers["Cache-Control"] = "no-cache"
+            return response
+
+        app.middlewares.append(no_cache_middleware)
+
     static_path = config.static_url.strip('/')
     if config.infer_host and config.static_path is not None:
         # we set the app key even in middleware to make the switch to production easier and for backwards compat.
         @web.middleware
-        async def static_middleware(request, handler):
+        async def static_middleware(request: web.Request, handler: Handler) -> web.StreamResponse:
             static_url = 'http://{}:{}/{}'.format(get_host(request), config.aux_port, static_path)
             dft_logger.debug('setting app static_root_url to "%s"', static_url)
             _change_static_url(request.app, static_url)
             return await handler(request)
 
         app.middlewares.insert(0, static_middleware)
 
+    # Fallback option to shutdown the application if signals don't work (e.g. Windows).
+    if config.shutdown_by_url:
+        async def do_shutdown(request: web.Request) -> web.Response:
+            def shutdown() -> NoReturn:
+                raise GracefulExit()
+            asyncio.get_running_loop().call_soon(shutdown)
+            return web.Response()
+
+        path = config.path_prefix + "/shutdown"
+        app.router.add_route("GET", path, do_shutdown, name="_devtools.shutdown")
+        dft_logger.debug("Created shutdown endpoint at http://{}:{}{}".format(config.host, config.main_port, path))
+
     if config.static_path is not None:
         static_url = 'http://{}:{}/{}'.format(config.host, config.aux_port, static_path)
         dft_logger.debug('settings app static_root_url to "%s"', static_url)
         _set_static_url(app, static_url)
 
 
-async def check_port_open(port: int, delay: int = 1) -> None:
+async def check_port_open(port: int, delay: float = 1) -> None:
     loop = asyncio.get_running_loop()
     # the "s = socket.socket; s.bind" approach sometimes says a port is in use when it's not
     # this approach replicates aiohttp so should always give the same answer
     for i in range(5, 0, -1):
         try:
-            server = await loop.create_server(asyncio.Protocol(), host=HOST, port=port)
+            server = await loop.create_server(asyncio.Protocol, host=HOST, port=port)
         except OSError as e:
             if e.errno != EADDRINUSE:
                 raise
             dft_logger.warning('port %d is already in use, waiting %d...', port, i)
             await asyncio.sleep(delay)
         else:
             server.close()
             await server.wait_closed()
             return
     raise AiohttpDevException('The port {} is already is use'.format(port))
 
 
 @contextlib.contextmanager
-def set_tty(tty_path):  # pragma: no cover
+def set_tty(tty_path: Optional[str]) -> Iterator[None]:
     try:
         if not tty_path:
             # to match OSError from open
             raise OSError()
         with open(tty_path) as tty:
             sys.stdin = tty
             yield
     except OSError:
         # either tty_path is None (windows) or opening it fails (eg. on pycharm)
         yield
 
 
-def serve_main_app(config: Config, tty_path: Optional[str]):
+def serve_main_app(config: Config, tty_path: Optional[str]) -> None:
     with set_tty(tty_path):
         setup_logging(config.verbose)
         app_factory = config.import_app_factory()
-        loop = asyncio.get_event_loop()
-        runner = loop.run_until_complete(create_main_app(config, app_factory))
-        try:
-            loop.run_until_complete(start_main_app(runner, config.main_port))
-            loop.run_forever()
-        except KeyboardInterrupt:  # pragma: no cover
-            pass
-        finally:
-            with contextlib.suppress(asyncio.TimeoutError, KeyboardInterrupt):
-                loop.run_until_complete(runner.cleanup())
+        if sys.version_info >= (3, 11):
+            with asyncio.Runner() as runner:
+                app_runner = runner.run(create_main_app(config, app_factory))
+                try:
+                    runner.run(start_main_app(app_runner, config.main_port))
+                    runner.get_loop().run_forever()
+                except KeyboardInterrupt:
+                    pass
+                finally:
+                    with contextlib.suppress(asyncio.TimeoutError, KeyboardInterrupt):
+                        runner.run(app_runner.cleanup())
+        else:
+            loop = asyncio.new_event_loop()
+            runner = loop.run_until_complete(create_main_app(config, app_factory))
+            try:
+                loop.run_until_complete(start_main_app(runner, config.main_port))
+                loop.run_forever()
+            except KeyboardInterrupt:  # pragma: no cover
+                pass
+            finally:
+                with contextlib.suppress(asyncio.TimeoutError, KeyboardInterrupt):
+                    loop.run_until_complete(runner.cleanup())
 
 
-async def create_main_app(config: Config, app_factory):
+async def create_main_app(config: Config, app_factory: AppFactory) -> web.AppRunner:
     app = await config.load_app(app_factory)
     modify_main_app(app, config)
 
     await check_port_open(config.main_port)
     return web.AppRunner(app, access_log_class=AccessLogger)
 
 
-async def start_main_app(runner: web.AppRunner, port):
+async def start_main_app(runner: web.AppRunner, port: int) -> None:
     await runner.setup()
     site = web.TCPSite(runner, host=HOST, port=port, shutdown_timeout=0.1)
     await site.start()
 
 
 WS = 'websockets'
 
 
-async def src_reload(app, path: Optional[str] = None):
+async def src_reload(app: web.Application, path: Optional[str] = None) -> int:
     """
     prompt each connected browser to reload by sending websocket message.
 
     :param path: if supplied this must be a path relative to app['static_path'],
         eg. reload of a single file is only supported for static resources.
     :return: number of sources reloaded
     """
@@ -189,20 +226,22 @@
 
     if reloads:
         s = '' if reloads == 1 else 's'
         aux_logger.info('prompted reload of %s on %d client%s', path or 'page', reloads, s)
     return reloads
 
 
-async def cleanup_aux_app(app):
+async def cleanup_aux_app(app: web.Application) -> None:
     aux_logger.debug('closing %d websockets...', len(app[WS]))
     await asyncio.gather(*(ws.close() for ws, _ in app[WS]))
 
 
-def create_auxiliary_app(*, static_path: str, static_url='/', livereload=True):
+def create_auxiliary_app(
+        *, static_path: Optional[str], static_url: str = "/", livereload: bool = True,
+        browser_cache: bool = False) -> web.Application:
     app = web.Application()
     app[WS] = set()
     app.update(
         static_path=static_path,
         static_url=static_url,
     )
     app.on_shutdown.append(cleanup_aux_app)
@@ -216,33 +255,34 @@
 
     if static_path:
         route = CustomStaticResource(
             static_url.rstrip('/'),
             static_path + '/',
             name='static-router',
             add_tail_snippet=livereload,
-            follow_symlinks=True
+            follow_symlinks=True,
+            browser_cache=browser_cache
         )
         app.router.register_resource(route)
 
     return app
 
 
-async def livereload_js(request):
+async def livereload_js(request: web.Request) -> web.Response:
     if request.if_modified_since:
         raise HTTPNotModified()
 
     lr_script = request.app['livereload_script']
     return web.Response(body=lr_script, content_type='application/javascript',
                         headers={LAST_MODIFIED: 'Fri, 01 Jan 2016 00:00:00 GMT'})
 
 WS_TYPE_LOOKUP = {k.value: v for v, k in WSMsgType.__members__.items()}
 
 
-async def websocket_handler(request):
+async def websocket_handler(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse(timeout=0.01)
     url = None
     await ws.prepare(request)
 
     async for msg in ws:
         if msg.type == WSMsgType.TEXT:
             try:
@@ -283,28 +323,30 @@
     else:
         aux_logger.debug('browser disconnected')
         request.app[WS].remove((ws, url))
     return ws
 
 
 class CustomStaticResource(StaticResource):
-    def __init__(self, *args, add_tail_snippet=False, **kwargs):
+    def __init__(self, *args: Any, add_tail_snippet: bool = False,
+                 browser_cache: bool = False, **kwargs: Any):
         self._add_tail_snippet = add_tail_snippet
+        self._browser_cache = browser_cache
         super().__init__(*args, **kwargs)
         self._show_index = True
 
-    def modify_request(self, request):
+    def modify_request(self, request: web.Request) -> Path:
         """
         Apply common path conventions eg. / > /index.html, /foobar > /foobar.html
         """
         filename = URL.build(path=request.match_info['filename'], encoded=True).path
-        raw_path = self._directory.joinpath(filename)
+        raw_path = self._directory / filename
         try:
             filepath = raw_path.resolve(strict=True)
-        except FileNotFoundError:
+        except (FileNotFoundError, NotADirectoryError):
             try:
                 html_file = raw_path.with_name(raw_path.name + '.html').resolve().relative_to(self._directory)
             except (FileNotFoundError, ValueError):
                 pass
             else:
                 request.match_info['filename'] = str(html_file)
         else:
@@ -312,39 +354,49 @@
                 index_file = filepath / 'index.html'
                 if index_file.exists():
                     try:
                         request.match_info['filename'] = str(index_file.relative_to(self._directory))
                     except ValueError:
                         # path is not not relative to self._directory
                         pass
+        return raw_path
 
-    def _insert_footer(self, response):
-        if not isinstance(response, FileResponse) or not self._add_tail_snippet:
+    def _insert_footer(self, response: web.StreamResponse) -> web.StreamResponse:
+        if not isinstance(response, web.FileResponse) or not self._add_tail_snippet:
             return response
 
         filepath = response._path
         ct, encoding = mimetypes.guess_type(str(response._path))
         if ct != 'text/html':
             return response
 
         with filepath.open('rb') as f:
             body = f.read() + LIVE_RELOAD_LOCAL_SNIPPET
 
-        resp = Response(body=body, content_type='text/html')
-        resp.last_modified = filepath.stat().st_mtime
+        resp = web.Response(body=body, content_type="text/html")
+        # Mypy bug: https://github.com/python/mypy/issues/11892
+        resp.last_modified = filepath.stat().st_mtime  # type: ignore[assignment]
         return resp
 
-    async def _handle(self, request):
-        self.modify_request(request)
+    async def _handle(self, request: web.Request) -> web.StreamResponse:
+        raw_path = self.modify_request(request)
         try:
             response = await super()._handle(request)
-            response = self._insert_footer(response)
-        except HTTPNotModified:
-            raise
         except HTTPNotFound:
-            # TODO include list of files in 404 body
-            _404_msg = '404: Not Found\n'
-            response = web.Response(body=_404_msg.encode(), status=404, content_type='text/plain')
+            while not raw_path.is_dir():
+                raw_path = raw_path.parent
+            paths = "\n".join(
+                " {}{}".format(p.relative_to(self._directory), "/" if p.is_dir() else "")
+                for p in raw_path.iterdir())
+            msg = "404: Not Found\n\nAvailable files under '{}/':\n{}\n".format(
+                raw_path.relative_to(self._directory), paths)
+            response = web.Response(text=msg, status=404, content_type="text/plain")
         else:
+            response = self._insert_footer(response)
             # Inject CORS headers to allow webfonts to load correctly
             response.headers['Access-Control-Allow-Origin'] = '*'
+
+        if not self._browser_cache:
+            # Add no-cache header to avoid browser caching in local development.
+            response.headers["Cache-Control"] = "no-cache"
+
         return response
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/PKG-INFO` & `aiohttp-devtools-1.1/aiohttp_devtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: aiohttp-devtools
-Version: 1.0.post0
+Version: 1.1
 Summary: Dev tools for aiohttp
 Home-page: https://github.com/aio-libs/aiohttp-devtools
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Project-URL: CI: AppVeyor, https://ci.appveyor.com/project/aio-libs/aiohttp-devtools
 Project-URL: CI: Travis, https://travis-ci.com/aio-libs/aiohttp-devtools
 Project-URL: Coverage: codecov, https://codecov.io/github/aio-libs/aiohttp-devtools
 Project-URL: GitHub: issues, https://github.com/aio-libs/aiohttp-devtools/issues
 Project-URL: GitHub: repo, https://github.com/aio-libs/aiohttp-devtools
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -37,17 +36,14 @@
 aiohttp-devtools
 ================
 
 |Coverage| |pypi| |license|
 
 Dev tools for `aiohttp`_.
 
-(Note: ``aiohttp-devtools>=0.8`` only supports ``aiohttp>=3.0``, if you're using older aiohttp, please use
-an older version of ``aiohttp-devtools``, see `History.rst`_ for details.)
-
 **aiohttp-devtools** provides a number of tools useful when developing applications with aiohttp and associated
 libraries.
 
 Installation
 ------------
 
 .. code:: shell
@@ -74,22 +70,22 @@
 **Note:** ``adev runserver <app-path>`` will import the whole file, hence it doesn't work
 with ``web.run_app(app)``. You can however use ``if __name__ == '__main__': web.run_app(app)``.
 
 ``app-path`` can be a path to either a directory containing a recognized default file (``app.py``
 or ``main.py``) or to a specific file. The ``--app-factory`` option can be used to define which method is called
 from the app path file, if not supplied some default method names are tried
 (namely `app`, `app_factory`, `get_app` and `create_app`, which can be
-attributes, functions, or coroutines).
+variables, functions, or coroutines).
 
 All ``runserver`` arguments can be set via environment variables.
 
-``runserver`` has a few of useful features:
+``runserver`` has a few useful features:
 
 * **livereload** will reload resources in the browser as your code changes without having to hit refresh, see `livereload`_ for more details.
-* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally
+* **static files** are served separately from your main app (generally on ``8001`` while your app is on ``8000``) so you don't have to contaminate your application to serve static files you only need locally.
 
 For more options see ``adev runserver --help``.
 
 serve
 ~~~~~
 
 Similar to `runserver`_ except just serves static files.
@@ -118,28 +114,28 @@
     . env/bin/activate
     pip install aiohttp-devtools create-aio-app
 
 
 We're now ready to build our new application with ``create-aio-app`` and we'll name the
 project ``my_new_app`` after the current directory.
 
-We're going to explicitly choose no database here to make, this tutorial easier but you can remove that option
+We're going to explicitly choose no database here to make this tutorial easier, but you can remove that option
 and choose to use a proper database if you like.
 
 You can just hit return to choose the default for all the options.
 
 
 .. code:: shell
 
     create-aio-app my_new_app --without-postgres
 
 That's it, your app is now created. You might want to have a look through the local directory's file tree.
 
 Before you can run your app you'll need to install the other requirements, luckily they've already been listed in
-``./requirements.txt`` by ``create-aio-app``, to install simply run
+``requirements/development.txt`` by ``create-aio-app``, to install simply run
 
 .. code:: shell
 
     pip install -r requirements/development.txt
 
 You can then run your app with just:
 
@@ -158,12 +154,10 @@
 
 .. |Coverage| image:: https://codecov.io/gh/aio-libs/aiohttp-devtools/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/aio-libs/aiohttp-devtools
 .. |pypi| image:: https://img.shields.io/pypi/v/aiohttp-devtools.svg
    :target: https://pypi.python.org/pypi/aiohttp-devtools
 .. |license| image:: https://img.shields.io/pypi/l/aiohttp-devtools.svg
    :target: https://github.com/aio-libs/aiohttp-devtools
-.. _History.rst: /HISTORY.rst
+.. _Changes.txt: /CHANGES.txt
 .. _livereload: https://github.com/livereload/livereload-js
 .. _aiohttp: http://aiohttp.readthedocs.io/en/stable/
-
-
```

### Comparing `aiohttp-devtools-1.0.post0/aiohttp_devtools.egg-info/SOURCES.txt` & `aiohttp-devtools-1.1/aiohttp_devtools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,17 @@
 aiohttp_devtools/runserver/__init__.py
 aiohttp_devtools/runserver/config.py
 aiohttp_devtools/runserver/livereload.js
 aiohttp_devtools/runserver/log_handlers.py
 aiohttp_devtools/runserver/main.py
 aiohttp_devtools/runserver/serve.py
 aiohttp_devtools/runserver/utils.py
-aiohttp_devtools/runserver/watch.py
+aiohttp_devtools/runserver/watch.py
+tests/test_cli.py
+tests/test_runserver_cleanup.py
+tests/test_runserver_config.py
+tests/test_runserver_logs.py
+tests/test_runserver_main.py
+tests/test_runserver_serve.py
+tests/test_runserver_watch.py
+tests/test_serve.py
+tests/test_utils.py
```

### Comparing `aiohttp-devtools-1.0.post0/setup.py` & `aiohttp-devtools-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,13 +61,14 @@
         [console_scripts]
         adev=aiohttp_devtools.cli:cli
         aiohttp-devtools=aiohttp_devtools.cli:cli
     """,
     install_requires=[
         'aiohttp>=3.8.0',
         'click>=6.6',
-        'devtools>=0.5',
+        'devtools>=0.6',
         'Pygments>=2.2.0',
-        'watchgod>=0.2',
+        'watchfiles>=0.10',
+        'typing_extensions >= 3.7.4; python_version<"3.8"'
     ],
     python_requires='>=3.7',
 )
```

