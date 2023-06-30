# Comparing `tmp/pyauxlib-0.0.1.tar.gz` & `tmp/pyauxlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauxlib-0.0.1.tar", last modified: Mon Jun  5 01:35:10 2023, max compression
+gzip compressed data, was "pyauxlib-0.0.2.tar", last modified: Fri Jun 30 03:59:28 2023, max compression
```

## Comparing `pyauxlib-0.0.1.tar` & `pyauxlib-0.0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.503582 pyauxlib-0.0.1/
--rw-rw-rw-   0        0        0      761 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2007 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/.cookiecutterrc
--rw-rw-rw-   0        0        0      192 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.coveragerc
--rw-rw-rw-   0        0        0      373 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.235581 pyauxlib-0.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.326579 pyauxlib-0.0.1/.github/workflows/
--rw-rw-rw-   0        0        0     2012 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.github/workflows/github-actions.yml
--rw-rw-rw-   0        0        0      714 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      241 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/.readthedocs.yml
--rw-rw-rw-   0        0        0       79 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0       94 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2403 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1538 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1818 2023-06-05 01:35:10.500581 pyauxlib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2253 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.336584 pyauxlib-0.0.1/ci/
--rw-rw-rw-   0        0        0     2950 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/bootstrap.py
--rw-rw-rw-   0        0        0       78 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.239581 pyauxlib-0.0.1/ci/templates/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.239581 pyauxlib-0.0.1/ci/templates/.github/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.341581 pyauxlib-0.0.1/ci/templates/.github/workflows/
--rw-rw-rw-   0        0        0     2195 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/ci/templates/.github/workflows/github-actions.yml
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.380580 pyauxlib-0.0.1/docs/
--rw-rw-rw-   0        0        0       29 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/authors.rst
--rw-rw-rw-   0        0        0       31 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     1193 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/contributing.rst
--rw-rw-rw-   0        0        0      265 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/index.rst
--rw-rw-rw-   0        0        0       95 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/installation.rst
--rw-rw-rw-   0        0        0       28 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.388582 pyauxlib-0.0.1/docs/reference/
--rw-rw-rw-   0        0        0       67 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/reference/index.rst
--rw-rw-rw-   0        0        0      111 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/reference/pyauxlib.rst
--rw-rw-rw-   0        0        0       31 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/requirements.txt
--rw-rw-rw-   0        0        0      120 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/spelling_wordlist.txt
--rw-rw-rw-   0        0        0       75 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/docs/usage.rst
--rw-rw-rw-   0        0        0     1262 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-06-05 01:35:10.503582 pyauxlib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2161 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.244581 pyauxlib-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.392580 pyauxlib-0.0.1/src/pyauxlib/
--rw-rw-rw-   0        0        0      153 2023-06-02 09:40:03.000000 pyauxlib-0.0.1/src/pyauxlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.422582 pyauxlib-0.0.1/src/pyauxlib/callables/
--rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/callables/__init__.py
--rw-rw-rw-   0        0        0     3128 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/callables/callables.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.428580 pyauxlib-0.0.1/src/pyauxlib/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/decorators/__init__.py
--rw-rw-rw-   0        0        0      349 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/decorators/timing.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.448581 pyauxlib-0.0.1/src/pyauxlib/experimental/
--rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/__init__.py
--rw-rw-rw-   0        0        0     4595 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/decorator.py
--rw-rw-rw-   0        0        0     1035 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/get_caller_path.py
--rw-rw-rw-   0        0        0      694 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/kwargs.py
--rw-rw-rw-   0        0        0     1333 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/experimental/lists.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.465580 pyauxlib-0.0.1/src/pyauxlib/io/
--rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/__init__.py
--rw-rw-rw-   0        0        0     5364 2023-06-02 09:44:05.000000 pyauxlib-0.0.1/src/pyauxlib/io/filesfolders.py
--rw-rw-rw-   0        0        0      443 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/utils.py
--rw-rw-rw-   0        0        0     1854 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/io/yamlio.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.491580 pyauxlib-0.0.1/src/pyauxlib/utils/
--rw-rw-rw-   0        0        0        0 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/deprecations.py
--rw-rw-rw-   0        0        0     1464 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/dictionaries.py
--rw-rw-rw-   0        0        0     2559 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/encoding.py
--rw-rw-rw-   0        0        0     3897 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/logger.py
--rw-rw-rw-   0        0        0     5422 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/src/pyauxlib/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.415581 pyauxlib-0.0.1/src/pyauxlib.egg-info/
--rw-rw-rw-   0        0        0     1818 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1476 2023-06-05 01:35:10.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 01:34:54.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 01:35:09.000000 pyauxlib-0.0.1/src/pyauxlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 01:35:10.496580 pyauxlib-0.0.1/tests/
--rw-rw-rw-   0        0        0      598 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/tests/test_pyauxlib.py
--rw-rw-rw-   0        0        0     1476 2023-06-01 03:17:52.000000 pyauxlib-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/reference/pyauxlib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.138184 pyauxlib-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.142184 pyauxlib-0.0.2/src/pyauxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/callables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/callables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/callables/callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/decorators/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/get_caller_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/experimental/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/filesfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/io/yamlio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/src/pyauxlib/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/src/pyauxlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:59:27.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 03:59:28.000000 pyauxlib-0.0.2/src/pyauxlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:28.146184 pyauxlib-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/tests/test_pyauxlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-30 03:59:18.000000 pyauxlib-0.0.2/tox.ini
```

### Comparing `pyauxlib-0.0.1/.bumpversion.cfg` & `pyauxlib-0.0.2/.bumpversion.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[bumpversion]
-current_version = 0.0.1
-commit = True
-tag = True
-
-[bumpversion:file:setup.py]
-search = version="{current_version}"
-replace = version="{new_version}"
-
-[bumpversion:file (badge):README.rst]
-search = /v{current_version}.svg
-replace = /v{new_version}.svg
-
-[bumpversion:file (link):README.rst]
-search = /v{current_version}...main
-replace = /v{new_version}...main
-
-[bumpversion:file:docs/conf.py]
-search = version = release = "{current_version}"
-replace = version = release = "{new_version}"
-
-[bumpversion:file:src/pyauxlib/__init__.py]
-search = __version__ = "{current_version}"
-replace = __version__ = "{new_version}"
-
-[bumpversion:file:.cookiecutterrc]
-search = version: {current_version}
-replace = version: {new_version}
+[bumpversion]
+current_version = 0.0.2
+commit = True
+tag = True
+
+[bumpversion:file:setup.py]
+search = version="{current_version}"
+replace = version="{new_version}"
+
+[bumpversion:file (badge):README.rst]
+search = /v{current_version}.svg
+replace = /v{new_version}.svg
+
+[bumpversion:file (link):README.rst]
+search = /v{current_version}...main
+replace = /v{new_version}...main
+
+[bumpversion:file:docs/conf.py]
+search = version = release = "{current_version}"
+replace = version = release = "{new_version}"
+
+[bumpversion:file:src/pyauxlib/__init__.py]
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
+
+[bumpversion:file:.cookiecutterrc]
+search = version: {current_version}
+replace = version: {new_version}
```

### Comparing `pyauxlib-0.0.1/.cookiecutterrc` & `pyauxlib-0.0.2/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://pyauxlib.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "sphinx-rtd-theme"
     test_matrix_separate_coverage: "no"
-    version: 0.0.1
+    version: 0.0.2
     version_manager: "bump2version"
     website: "https://github.com/psolsfer"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `pyauxlib-0.0.1/.pre-commit-config.yaml` & `pyauxlib-0.0.2/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# To install the git pre-commit hooks run:
-#   pre-commit install --install-hooks
-# To update the versions:
-#   pre-commit autoupdate
-exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
-# Note the order is intentional to avoid multiple passes of the hooks
-repos:
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
-    hooks:
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix, --show-fixes]
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
-    hooks:
-      - id: trailing-whitespace
-      - id: end-of-file-fixer
-      - id: debug-statements
+# To install the git pre-commit hooks run:
+#   pre-commit install --install-hooks
+# To update the versions:
+#   pre-commit autoupdate
+exclude: '^(\.tox|ci/templates|\.bumpversion\.cfg)(/|$)'
+# Note the order is intentional to avoid multiple passes of the hooks
+repos:
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.270
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix, --show-fixes]
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: trailing-whitespace
+      - id: end-of-file-fixer
+      - id: debug-statements
```

### Comparing `pyauxlib-0.0.1/CONTRIBUTING.rst` & `pyauxlib-0.0.2/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every
-little bit helps, and credit will always be given.
-
-Bug reports
-===========
-
-When `reporting a bug <https://github.com/psolsfer/pyauxlib/issues>`_ please include:
-
-    * Your operating system name and version.
-    * Any details about your local setup that might be helpful in troubleshooting.
-    * Detailed steps to reproduce the bug.
-
-Documentation improvements
-==========================
-
-PyAuxLib could always use more documentation, whether as part of the
-official PyAuxLib docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Feature requests and feedback
-=============================
-
-The best way to send feedback is to file an issue at https://github.com/psolsfer/pyauxlib/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that code contributions are welcome :)
-
-Development
-===========
-
-To set up `pyauxlib` for local development:
-
-1. Fork `pyauxlib <https://github.com/psolsfer/pyauxlib>`_
-   (look for the "Fork" button).
-2. Clone your fork locally::
-
-    git clone git@github.com:YOURGITHUBNAME/pyauxlib.git
-
-3. Create a branch for local development::
-
-    git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-4. When you're done making changes run all the checks and docs builder with one command::
-
-    tox
-
-5. Commit your changes and push your branch to GitHub::
-
-    git add .
-    git commit -m "Your detailed description of your changes."
-    git push origin name-of-your-bugfix-or-feature
-
-6. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-If you need some code review or feedback while you're developing the code just make the pull request.
-
-For merging, you should:
-
-1. Include passing tests (run ``tox``).
-2. Update documentation when there's new API, functionality etc.
-3. Add a note to ``CHANGELOG.rst`` about the changes.
-4. Add yourself to ``AUTHORS.rst``.
-
-Tips
-----
-
-To run a subset of tests::
-
-    tox -e envname -- pytest -k test_myfeature
-
-To run all the test environments in *parallel*::
-
-    tox -p auto
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every
+little bit helps, and credit will always be given.
+
+Bug reports
+===========
+
+When `reporting a bug <https://github.com/psolsfer/pyauxlib/issues>`_ please include:
+
+    * Your operating system name and version.
+    * Any details about your local setup that might be helpful in troubleshooting.
+    * Detailed steps to reproduce the bug.
+
+Documentation improvements
+==========================
+
+PyAuxLib could always use more documentation, whether as part of the
+official PyAuxLib docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Feature requests and feedback
+=============================
+
+The best way to send feedback is to file an issue at https://github.com/psolsfer/pyauxlib/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that code contributions are welcome :)
+
+Development
+===========
+
+To set up `pyauxlib` for local development:
+
+1. Fork `pyauxlib <https://github.com/psolsfer/pyauxlib>`_
+   (look for the "Fork" button).
+2. Clone your fork locally::
+
+    git clone git@github.com:YOURGITHUBNAME/pyauxlib.git
+
+3. Create a branch for local development::
+
+    git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+4. When you're done making changes run all the checks and docs builder with one command::
+
+    tox
+
+5. Commit your changes and push your branch to GitHub::
+
+    git add .
+    git commit -m "Your detailed description of your changes."
+    git push origin name-of-your-bugfix-or-feature
+
+6. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+If you need some code review or feedback while you're developing the code just make the pull request.
+
+For merging, you should:
+
+1. Include passing tests (run ``tox``).
+2. Update documentation when there's new API, functionality etc.
+3. Add a note to ``CHANGELOG.rst`` about the changes.
+4. Add yourself to ``AUTHORS.rst``.
+
+Tips
+----
+
+To run a subset of tests::
+
+    tox -e envname -- pytest -k test_myfeature
+
+To run all the test environments in *parallel*::
+
+    tox -p auto
```

### Comparing `pyauxlib-0.0.1/LICENSE` & `pyauxlib-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Pablo Solís Fernández. All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-    2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-    3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Pablo Solís Fernández. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+    2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+    3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pyauxlib-0.0.1/README.rst` & `pyauxlib-0.0.2/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-========
-Overview
-========
-
-.. start-badges
-
-.. list-table::
-    :stub-columns: 1
-
-    * - docs
-      - |docs|
-    * - tests
-      - | |github-actions|
-    * - package
-      - | |version| |wheel| |supported-versions| |supported-implementations|
-        | |commits-since|
-.. |docs| image:: https://readthedocs.org/projects/pyauxlib/badge/?style=flat
-    :target: https://pyauxlib.readthedocs.io/
-    :alt: Documentation Status
-
-.. |github-actions| image:: https://github.com/psolsfer/pyauxlib/actions/workflows/github-actions.yml/badge.svg
-    :alt: GitHub Actions Build Status
-    :target: https://github.com/psolsfer/pyauxlib/actions
-
-.. |version| image:: https://img.shields.io/pypi/v/pyauxlib.svg
-    :alt: PyPI Package latest release
-    :target: https://pypi.org/project/pyauxlib
-
-.. |wheel| image:: https://img.shields.io/pypi/wheel/pyauxlib.svg
-    :alt: PyPI Wheel
-    :target: https://pypi.org/project/pyauxlib
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pyauxlib.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/pyauxlib
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyauxlib.svg
-    :alt: Supported implementations
-    :target: https://pypi.org/project/pyauxlib
-
-.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.1.svg
-    :alt: Commits since latest release
-    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.1...main
-
-
-
-.. end-badges
-
-Auxiliary library for python.
-
-* Free software: BSD 3-Clause License
-
-Installation
-============
-
-::
-
-    pip install pyauxlib
-
-You can also install the in-development version with::
-
-    pip install https://github.com/psolsfer/pyauxlib/archive/main.zip
-
-
-Documentation
-=============
-
-
-https://pyauxlib.readthedocs.io/
-
-
-Development
-===========
-
-To run all the tests run::
-
-    tox
-
-Note, to combine the coverage data from all the tox environments run:
-
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
-
-    - - Windows
-      - ::
-
-            set PYTEST_ADDOPTS=--cov-append
-            tox
-
-    - - Other
-      - ::
-
-            PYTEST_ADDOPTS=--cov-append tox
+========
+Overview
+========
+
+.. start-badges
+
+.. list-table::
+    :stub-columns: 1
+
+    * - docs
+      - |docs|
+    * - tests
+      - | |github-actions|
+    * - package
+      - | |version| |wheel| |supported-versions| |supported-implementations|
+        | |commits-since|
+.. |docs| image:: https://readthedocs.org/projects/pyauxlib/badge/?style=flat
+    :target: https://pyauxlib.readthedocs.io/
+    :alt: Documentation Status
+
+.. |github-actions| image:: https://github.com/psolsfer/pyauxlib/actions/workflows/github-actions.yml/badge.svg
+    :alt: GitHub Actions Build Status
+    :target: https://github.com/psolsfer/pyauxlib/actions
+
+.. |version| image:: https://img.shields.io/pypi/v/pyauxlib.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/pyauxlib
+
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pyauxlib.svg
+    :alt: PyPI Wheel
+    :target: https://pypi.org/project/pyauxlib
+
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pyauxlib.svg
+    :alt: Supported versions
+    :target: https://pypi.org/project/pyauxlib
+
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pyauxlib.svg
+    :alt: Supported implementations
+    :target: https://pypi.org/project/pyauxlib
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/psolsfer/pyauxlib/v0.0.2.svg
+    :alt: Commits since latest release
+    :target: https://github.com/psolsfer/pyauxlib/compare/v0.0.2...main
+
+
+
+.. end-badges
+
+Auxiliary library for python.
+
+* Free software: BSD 3-Clause License
+
+Installation
+============
+
+::
+
+    pip install pyauxlib
+
+You can also install the in-development version with::
+
+    pip install https://github.com/psolsfer/pyauxlib/archive/main.zip
+
+
+Documentation
+=============
+
+
+https://pyauxlib.readthedocs.io/
+
+
+Development
+===========
+
+To run all the tests run::
+
+    tox
+
+Note, to combine the coverage data from all the tox environments run:
+
+.. list-table::
+    :widths: 10 90
+    :stub-columns: 1
+
+    - - Windows
+      - ::
+
+            set PYTEST_ADDOPTS=--cov-append
+            tox
+
+    - - Other
+      - ::
+
+            PYTEST_ADDOPTS=--cov-append tox
```

### Comparing `pyauxlib-0.0.1/ci/bootstrap.py` & `pyauxlib-0.0.2/ci/bootstrap.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-#!/usr/bin/env python
-import os
-import pathlib
-import subprocess
-import sys
-
-base_path: pathlib.Path = pathlib.Path(__file__).resolve().parent.parent
-templates_path = base_path / "ci" / "templates"
-
-
-def check_call(args):
-    print("+", *args)
-    subprocess.check_call(args)
-
-
-def exec_in_env():
-    env_path = base_path / ".tox" / "bootstrap"
-    if sys.platform == "win32":
-        bin_path = env_path / "Scripts"
-    else:
-        bin_path = env_path / "bin"
-    if not env_path.exists():
-        import subprocess
-
-        print(f"Making bootstrap env in: {env_path} ...")
-        try:
-            check_call([sys.executable, "-m", "venv", env_path])
-        except subprocess.CalledProcessError:
-            try:
-                check_call([sys.executable, "-m", "virtualenv", env_path])
-            except subprocess.CalledProcessError:
-                check_call(["virtualenv", env_path])
-        print("Installing `jinja2` into bootstrap environment...")
-        check_call([bin_path / "pip", "install", "jinja2", "tox"])
-    python_executable = bin_path / "python"
-    if not python_executable.exists():
-        python_executable = python_executable.with_suffix(".exe")
-
-    print(f"Re-executing with: {python_executable}")
-    print("+ exec", python_executable, __file__, "--no-env")
-    os.execv(python_executable, [python_executable, __file__, "--no-env"])
-
-
-def main():
-    import jinja2
-
-    print(f"Project path: {base_path}")
-
-    jinja = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(str(templates_path)),
-        trim_blocks=True,
-        lstrip_blocks=True,
-        keep_trailing_newline=True,
-    )
-    tox_environments = [
-        line.strip()
-        # 'tox' need not be installed globally, but must be importable
-        # by the Python that is running this script.
-        # This uses sys.executable the same way that the call in
-        # cookiecutter-pylibrary/hooks/post_gen_project.py
-        # invokes this bootstrap.py itself.
-        for line in subprocess.check_output([sys.executable, "-m", "tox", "--listenvs"], universal_newlines=True).splitlines()
-    ]
-    tox_environments = [line for line in tox_environments if line.startswith("py")]
-    for template in templates_path.rglob("*"):
-        if template.is_file():
-            template_path = template.relative_to(templates_path).as_posix()
-            destination = base_path / template_path
-            destination.parent.mkdir(parents=True, exist_ok=True)
-            destination.write_text(jinja.get_template(template_path).render(tox_environments=tox_environments))
-            print(f"Wrote {template_path}")
-    print("DONE.")
-
-
-if __name__ == "__main__":
-    args = sys.argv[1:]
-    if args == ["--no-env"]:
-        main()
-    elif not args:
-        exec_in_env()
-    else:
-        print(f"Unexpected arguments: {args}", file=sys.stderr)
-        sys.exit(1)
+#!/usr/bin/env python
+import os
+import pathlib
+import subprocess
+import sys
+
+base_path: pathlib.Path = pathlib.Path(__file__).resolve().parent.parent
+templates_path = base_path / "ci" / "templates"
+
+
+def check_call(args):
+    print("+", *args)
+    subprocess.check_call(args)
+
+
+def exec_in_env():
+    env_path = base_path / ".tox" / "bootstrap"
+    if sys.platform == "win32":
+        bin_path = env_path / "Scripts"
+    else:
+        bin_path = env_path / "bin"
+    if not env_path.exists():
+        import subprocess
+
+        print(f"Making bootstrap env in: {env_path} ...")
+        try:
+            check_call([sys.executable, "-m", "venv", env_path])
+        except subprocess.CalledProcessError:
+            try:
+                check_call([sys.executable, "-m", "virtualenv", env_path])
+            except subprocess.CalledProcessError:
+                check_call(["virtualenv", env_path])
+        print("Installing `jinja2` into bootstrap environment...")
+        check_call([bin_path / "pip", "install", "jinja2", "tox"])
+    python_executable = bin_path / "python"
+    if not python_executable.exists():
+        python_executable = python_executable.with_suffix(".exe")
+
+    print(f"Re-executing with: {python_executable}")
+    print("+ exec", python_executable, __file__, "--no-env")
+    os.execv(python_executable, [python_executable, __file__, "--no-env"])
+
+
+def main():
+    import jinja2
+
+    print(f"Project path: {base_path}")
+
+    jinja = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(str(templates_path)),
+        trim_blocks=True,
+        lstrip_blocks=True,
+        keep_trailing_newline=True,
+    )
+    tox_environments = [
+        line.strip()
+        # 'tox' need not be installed globally, but must be importable
+        # by the Python that is running this script.
+        # This uses sys.executable the same way that the call in
+        # cookiecutter-pylibrary/hooks/post_gen_project.py
+        # invokes this bootstrap.py itself.
+        for line in subprocess.check_output([sys.executable, "-m", "tox", "--listenvs"], universal_newlines=True).splitlines()
+    ]
+    tox_environments = [line for line in tox_environments if line.startswith("py")]
+    for template in templates_path.rglob("*"):
+        if template.is_file():
+            template_path = template.relative_to(templates_path).as_posix()
+            destination = base_path / template_path
+            destination.parent.mkdir(parents=True, exist_ok=True)
+            destination.write_text(jinja.get_template(template_path).render(tox_environments=tox_environments))
+            print(f"Wrote {template_path}")
+    print("DONE.")
+
+
+if __name__ == "__main__":
+    args = sys.argv[1:]
+    if args == ["--no-env"]:
+        main()
+    elif not args:
+        exec_in_env()
+    else:
+        print(f"Unexpected arguments: {args}", file=sys.stderr)
+        sys.exit(1)
```

### Comparing `pyauxlib-0.0.1/ci/templates/.github/workflows/github-actions.yml` & `pyauxlib-0.0.2/ci/templates/.github/workflows/github-actions.yml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-name: build
-on: [push, pull_request]
-jobs:
-  test:
-    name: {{ '${{ matrix.name }}' }}
-    runs-on: {{ '${{ matrix.os }}' }}
-    timeout-minutes: 30
-    strategy:
-      fail-fast: false
-      matrix:
-        include:
-          - name: 'check'
-            python: '3.11'
-            toxpython: 'python3.11'
-            tox_env: 'check'
-            os: 'ubuntu-latest'
-          - name: 'docs'
-            python: '3.11'
-            toxpython: 'python3.11'
-            tox_env: 'docs'
-            os: 'ubuntu-latest'
-{% for env in tox_environments %}
-{% set prefix = env.split('-')[0] -%}
-{% if prefix.startswith('pypy') %}
-{% set python %}pypy-{{ prefix[4] }}.{{ prefix[5] }}{% endset %}
-{% set cpython %}pp{{ prefix[4:5] }}{% endset %}
-{% set toxpython %}pypy{{ prefix[4] }}.{{ prefix[5] }}{% endset %}
-{% else %}
-{% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
-{% set cpython %}cp{{ prefix[2:] }}{% endset %}
-{% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
-{% endif %}
-{% for os, python_arch in [
-    ['ubuntu', 'x64'],
-    ['windows', 'x64'],
-] %}
-          - name: '{{ env }} ({{ os }})'
-            python: '{{ python }}'
-            toxpython: '{{ toxpython }}'
-            python_arch: '{{ python_arch }}'
-            tox_env: '{{ env }}'
-            os: '{{ os }}-latest'
-{% endfor %}
-{% endfor %}
-    steps:
-    - uses: actions/checkout@v3
-      with:
-        fetch-depth: 0
-    - uses: actions/setup-python@v4
-      with:
-        python-version: {{ '${{ matrix.python }}' }}
-        architecture: {{ '${{ matrix.python_arch }}' }}
-    - name: install dependencies
-      run: |
-        python -mpip install --progress-bar=off -r ci/requirements.txt
-        virtualenv --version
-        pip --version
-        tox --version
-        pip list --format=freeze
-    - name: test
-      env:
-        TOXPYTHON: '{{ '${{ matrix.toxpython }}' }}'
-      run: >
-        tox -e {{ '${{ matrix.tox_env }}' }} -v
-  finish:
-    needs: test
-    if: {{ '${{ always() }}' }}
-    runs-on: ubuntu-latest
-    steps:
-    - uses: coverallsapp/github-action@v2
-      with:
-        parallel-finished: true
+name: build
+on: [push, pull_request]
+jobs:
+  test:
+    name: {{ '${{ matrix.name }}' }}
+    runs-on: {{ '${{ matrix.os }}' }}
+    timeout-minutes: 30
+    strategy:
+      fail-fast: false
+      matrix:
+        include:
+          - name: 'check'
+            python: '3.11'
+            toxpython: 'python3.11'
+            tox_env: 'check'
+            os: 'ubuntu-latest'
+          - name: 'docs'
+            python: '3.11'
+            toxpython: 'python3.11'
+            tox_env: 'docs'
+            os: 'ubuntu-latest'
+{% for env in tox_environments %}
+{% set prefix = env.split('-')[0] -%}
+{% if prefix.startswith('pypy') %}
+{% set python %}pypy-{{ prefix[4] }}.{{ prefix[5] }}{% endset %}
+{% set cpython %}pp{{ prefix[4:5] }}{% endset %}
+{% set toxpython %}pypy{{ prefix[4] }}.{{ prefix[5] }}{% endset %}
+{% else %}
+{% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
+{% set cpython %}cp{{ prefix[2:] }}{% endset %}
+{% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
+{% endif %}
+{% for os, python_arch in [
+    ['ubuntu', 'x64'],
+    ['windows', 'x64'],
+] %}
+          - name: '{{ env }} ({{ os }})'
+            python: '{{ python }}'
+            toxpython: '{{ toxpython }}'
+            python_arch: '{{ python_arch }}'
+            tox_env: '{{ env }}'
+            os: '{{ os }}-latest'
+{% endfor %}
+{% endfor %}
+    steps:
+    - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+    - uses: actions/setup-python@v4
+      with:
+        python-version: {{ '${{ matrix.python }}' }}
+        architecture: {{ '${{ matrix.python_arch }}' }}
+    - name: install dependencies
+      run: |
+        python -mpip install --progress-bar=off -r ci/requirements.txt
+        virtualenv --version
+        pip --version
+        tox --version
+        pip list --format=freeze
+    - name: test
+      env:
+        TOXPYTHON: '{{ '${{ matrix.toxpython }}' }}'
+      run: >
+        tox -e {{ '${{ matrix.tox_env }}' }} -v
+  finish:
+    needs: test
+    if: {{ '${{ always() }}' }}
+    runs-on: ubuntu-latest
+    steps:
+    - uses: coverallsapp/github-action@v2
+      with:
+        parallel-finished: true
```

### Comparing `pyauxlib-0.0.1/docs/conf.py` & `pyauxlib-0.0.2/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import os
-
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.coverage",
-    "sphinx.ext.doctest",
-    "sphinx.ext.extlinks",
-    "sphinx.ext.ifconfig",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
-    "sphinx.ext.viewcode",
-]
-source_suffix = ".rst"
-master_doc = "index"
-project = "PyAuxLib"
-year = "2023"
-author = "Pablo Solís Fernández"
-copyright = f"{year}, {author}"
-version = release = "0.0.1"
-
-pygments_style = "trac"
-templates_path = ["."]
-extlinks = {
-    "issue": ("https://github.com/psolsfer/pyauxlib/issues/%s", "#"),
-    "pr": ("https://github.com/psolsfer/pyauxlib/pull/%s", "PR #"),
-}
-# on_rtd is whether we are on readthedocs.org
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
-
-if not on_rtd:  # only set the theme if we are building docs locally
-    html_theme = "sphinx_rtd_theme"
-
-html_use_smartypants = True
-html_last_updated_fmt = "%b %d, %Y"
-html_split_index = False
-html_sidebars = {
-    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
-}
-html_short_title = f"{project}-{version}"
-
-napoleon_use_ivar = True
-napoleon_use_rtype = False
-napoleon_use_param = False
+import os
+
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+]
+source_suffix = ".rst"
+master_doc = "index"
+project = "PyAuxLib"
+year = "2023"
+author = "Pablo Solís Fernández"
+copyright = f"{year}, {author}"
+version = release = "0.0.2"
+
+pygments_style = "trac"
+templates_path = ["."]
+extlinks = {
+    "issue": ("https://github.com/psolsfer/pyauxlib/issues/%s", "#"),
+    "pr": ("https://github.com/psolsfer/pyauxlib/pull/%s", "PR #"),
+}
+# on_rtd is whether we are on readthedocs.org
+on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+
+if not on_rtd:  # only set the theme if we are building docs locally
+    html_theme = "sphinx_rtd_theme"
+
+html_use_smartypants = True
+html_last_updated_fmt = "%b %d, %Y"
+html_split_index = False
+html_sidebars = {
+    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
+}
+html_short_title = f"{project}-{version}"
+
+napoleon_use_ivar = True
+napoleon_use_rtype = False
+napoleon_use_param = False
```

### Comparing `pyauxlib-0.0.1/pyproject.toml` & `pyauxlib-0.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-[build-system]
-requires = [
-    "setuptools>=30.3.0",
-    "wheel",
-]
-
-[tool.ruff.per-file-ignores]
-"ci/*" = ["S"]
-
-[tool.ruff]
-extend-exclude = ["static", "ci/templates"]
-ignore = [
-    "RUF001", # ruff-specific rules ambiguous-unicode-character-string
-    "S101", # flake8-bandit assert
-    "S308", # flake8-bandit suspicious-mark-safe-usage
-    "E501", # pycodestyle line-too-long
-]
-line-length = 140
-select = [
-    "B", # flake8-bugbear
-    "C4", # flake8-comprehensions
-    "DTZ", # flake8-datetimez
-    "E", # pycodestyle errors
-    "EXE", # flake8-executable
-    "F", # pyflakes
-    "I", # isort
-    "INT", # flake8-gettext
-    "PIE", # flake8-pie
-    "PLC", # pylint convention
-    "PLE", # pylint errors
-    "PT", # flake8-pytest-style
-    "PTH", # flake8-use-pathlib
-    "Q", # flake8-quotes
-    "RSE", # flake8-raise
-    "RUF", # ruff-specific rules
-    "S", # flake8-bandit
-    "UP", # pyupgrade
-    "W", # pycodestyle warnings
-]
-src = ["src", "tests"]
-target-version = "py310"
-
-[tool.ruff.flake8-pytest-style]
-fixture-parentheses = false
-mark-parentheses = false
-
-[tool.ruff.isort]
-forced-separate = ["conftest"]
-force-single-line = true
-
-[tool.black]
-line-length = 140
-target-version = ["py310"]
+[build-system]
+requires = [
+    "setuptools>=30.3.0",
+    "wheel",
+]
+
+[tool.ruff.per-file-ignores]
+"ci/*" = ["S"]
+
+[tool.ruff]
+extend-exclude = ["static", "ci/templates"]
+ignore = [
+    "RUF001", # ruff-specific rules ambiguous-unicode-character-string
+    "S101", # flake8-bandit assert
+    "S308", # flake8-bandit suspicious-mark-safe-usage
+    "E501", # pycodestyle line-too-long
+]
+line-length = 140
+select = [
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "DTZ", # flake8-datetimez
+    "E", # pycodestyle errors
+    "EXE", # flake8-executable
+    "F", # pyflakes
+    "I", # isort
+    "INT", # flake8-gettext
+    "PIE", # flake8-pie
+    "PLC", # pylint convention
+    "PLE", # pylint errors
+    "PT", # flake8-pytest-style
+    "PTH", # flake8-use-pathlib
+    "Q", # flake8-quotes
+    "RSE", # flake8-raise
+    "RUF", # ruff-specific rules
+    "S", # flake8-bandit
+    "UP", # pyupgrade
+    "W", # pycodestyle warnings
+]
+src = ["src", "tests"]
+target-version = "py310"
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
+
+[tool.ruff.isort]
+forced-separate = ["conftest"]
+force-single-line = true
+
+[tool.black]
+line-length = 140
+target-version = ["py310"]
```

### Comparing `pyauxlib-0.0.1/pytest.ini` & `pyauxlib-0.0.2/pytest.ini`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[pytest]
-# If a pytest section is found in one of the possible config files
-# (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
-# so if you add a pytest config section elsewhere,
-# you will need to delete this section from setup.cfg.
-norecursedirs =
-    migrations
-
-python_files =
-    test_*.py
-    *_test.py
-    tests.py
-addopts =
-    -ra
-    --strict-markers
-    --doctest-modules
-    --doctest-glob=\*.rst
-    --tb=short
-testpaths =
-    tests
-
-# Idea from: https://til.simonwillison.net/pytest/treat-warnings-as-errors
-filterwarnings =
-    error
-# You can add exclusions, some examples:
-#    ignore:'pyauxlib' defines default_app_config:PendingDeprecationWarning::
-#    ignore:The {{% if:::
-#    ignore:Coverage disabled via --no-cov switch!
+[pytest]
+# If a pytest section is found in one of the possible config files
+# (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
+# so if you add a pytest config section elsewhere,
+# you will need to delete this section from setup.cfg.
+norecursedirs =
+    migrations
+
+python_files =
+    test_*.py
+    *_test.py
+    tests.py
+addopts =
+    -ra
+    --strict-markers
+    --doctest-modules
+    --doctest-glob=\*.rst
+    --tb=short
+testpaths =
+    tests
+
+# Idea from: https://til.simonwillison.net/pytest/treat-warnings-as-errors
+filterwarnings =
+    error
+# You can add exclusions, some examples:
+#    ignore:'pyauxlib' defines default_app_config:PendingDeprecationWarning::
+#    ignore:The {{% if:::
+#    ignore:Coverage disabled via --no-cov switch!
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/callables/callables.py` & `pyauxlib-0.0.2/src/pyauxlib/callables/callables.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import inspect
-import sys
-from collections.abc import Callable
-
-
-def call_with_arguments(*args: dict, callable_object: Callable) -> Callable:
-    """Check if the required arguments of a callable object are included in the
-    passed arguments, and returns the callable_object(arguments)
-
-    Parameters
-    ----------
-    *args : dict
-        variable number of dictionaries with arguments to be passed to the callable.
-        In case of duplicate entries, the last values from last dictionaries overwrite
-        those of the first ones.
-    callable_object : Callable
-        callable object (function, class)
-
-    Returns
-    -------
-    Callable
-        the callable object with the passed arguments
-
-    Raises
-    ------
-    TypeError
-        required argument for the callable object is absent in arguments
-    """
-
-    if callable(callable_object):
-        # Check the parameters of callable_object
-        params = inspect.signature(callable_object).parameters
-    else:
-        # TODO: handle the fact that the object passed is not callable...
-        sys.exit(1)
-
-    argskwargs = _get_argskwargs(callable_object)
-
-    # Merge all the dictionaries in *args into a single one
-    # Values from last dictionaries in *args will overwrite existing keys in the previous
-    arguments = {key: val for d in args for key, val in d.items()}
-
-    # TODO: do anything with the arguments passed but not in the function???
-    # Just pass them as **kwargs or raise a warning??"""
-    # If pass them as *args/**kwargs, then need to see if the callable accept them,
-    # in the 'params_spec' of get _get_argskwargs (varargs, varkw, as seen in
-    # https://docs.python.org/3/library/inspect.html#inspect.getfullargspec
-    {k: v for (k, v) in arguments.items() if k not in params.keys()}
-
-    kwargs = {}
-
-    for arg_name, v in params.items():
-        # Required argument (doesn't have a default value in callable_object)
-        # *args and **kwargs are not required
-        required_argument = (v.default == inspect.Parameter.empty) if arg_name not in argskwargs else False
-
-        arg_value = arguments.get(arg_name)
-
-        if required_argument:
-            if arg_name in arguments.keys():
-                kwargs[arg_name] = arguments[arg_name]
-            else:
-                raise TypeError(f"Argument '{arg_name}' is missing")
-        elif arg_name in arguments.keys():
-            # ??? Returns the default value if 'None' in arguments. Ok?
-            kwargs[arg_name] = arg_value if arg_value is not None else v.default
-
-    return callable_object(**kwargs)  # FIXME Some Callables don't accept kwargs (e.g. math.floor)
-
-
-def _get_argskwargs(callable: Callable) -> list[str | None]:
-    """Returns a list with the args and kwargs of a callable
-
-    Parameters
-    ----------
-    callable : Callable
-        object to check for args and kwargs
-
-    Returns
-    -------
-    list[str]
-        list of args and kwargs
-    """
-
-    params_spec = inspect.getfullargspec(callable)
-
-    return [params_spec.varargs, params_spec.varkw]
+import inspect
+import sys
+from collections.abc import Callable
+
+
+def call_with_arguments(*args: dict, callable_object: Callable) -> Callable:
+    """Check if the required arguments of a callable object are included in the
+    passed arguments, and returns the callable_object(arguments)
+
+    Parameters
+    ----------
+    *args : dict
+        variable number of dictionaries with arguments to be passed to the callable.
+        In case of duplicate entries, the last values from last dictionaries overwrite
+        those of the first ones.
+    callable_object : Callable
+        callable object (function, class)
+
+    Returns
+    -------
+    Callable
+        the callable object with the passed arguments
+
+    Raises
+    ------
+    TypeError
+        required argument for the callable object is absent in arguments
+    """
+
+    if callable(callable_object):
+        # Check the parameters of callable_object
+        params = inspect.signature(callable_object).parameters
+    else:
+        # TODO: handle the fact that the object passed is not callable...
+        sys.exit(1)
+
+    argskwargs = _get_argskwargs(callable_object)
+
+    # Merge all the dictionaries in *args into a single one
+    # Values from last dictionaries in *args will overwrite existing keys in the previous
+    arguments = {key: val for d in args for key, val in d.items()}
+
+    # TODO: do anything with the arguments passed but not in the function???
+    # Just pass them as **kwargs or raise a warning??"""
+    # If pass them as *args/**kwargs, then need to see if the callable accept them,
+    # in the 'params_spec' of get _get_argskwargs (varargs, varkw, as seen in
+    # https://docs.python.org/3/library/inspect.html#inspect.getfullargspec
+    {k: v for (k, v) in arguments.items() if k not in params.keys()}
+
+    kwargs = {}
+
+    for arg_name, v in params.items():
+        # Required argument (doesn't have a default value in callable_object)
+        # *args and **kwargs are not required
+        required_argument = (v.default == inspect.Parameter.empty) if arg_name not in argskwargs else False
+
+        arg_value = arguments.get(arg_name)
+
+        if required_argument:
+            if arg_name in arguments.keys():
+                kwargs[arg_name] = arguments[arg_name]
+            else:
+                raise TypeError(f"Argument '{arg_name}' is missing")
+        elif arg_name in arguments.keys():
+            # ??? Returns the default value if 'None' in arguments. Ok?
+            kwargs[arg_name] = arg_value if arg_value is not None else v.default
+
+    return callable_object(**kwargs)  # FIXME Some Callables don't accept kwargs (e.g. math.floor)
+
+
+def _get_argskwargs(callable: Callable) -> list[str | None]:
+    """Returns a list with the args and kwargs of a callable
+
+    Parameters
+    ----------
+    callable : Callable
+        object to check for args and kwargs
+
+    Returns
+    -------
+    list[str]
+        list of args and kwargs
+    """
+
+    params_spec = inspect.getfullargspec(callable)
+
+    return [params_spec.varargs, params_spec.varkw]
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/experimental/get_caller_path.py` & `pyauxlib-0.0.2/src/pyauxlib/experimental/get_caller_path.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from inspect import currentframe
-from inspect import getframeinfo
-from pathlib import Path
-from types import FrameType
-
-
-def get_caller_path() -> Path | None:
-    # FIXME: Does this work as intended? Is it useful?
-    """Gets the path of the caller script.
-    The 'caller' here is the caller of the script that called this one.
-
-    Returns
-    -------
-    Path | None
-        Path of the caller script (None if there is no caller)
-    """
-    # Gets the path of the calling script (must be the "main")
-
-    # NOTE: 'f:back' twice
-    # The 1st is for the script calling this one, the 2nd is for the script calling the
-    # script that called this... which might be a NoneType
-
-    caller_1 = currentframe().f_back
-    caller_2 = caller_1.f_back
-
-    if not isinstance(caller_1, FrameType):
-        # No caller
-        # TODO: raise some exception, warning???
-        return None
-
-    caller = caller_2 if isinstance(caller_2, FrameType) else caller_1
-
-    return Path(getframeinfo(caller).filename)
+from inspect import currentframe
+from inspect import getframeinfo
+from pathlib import Path
+from types import FrameType
+
+
+def get_caller_path() -> Path | None:
+    # FIXME: Does this work as intended? Is it useful?
+    """Gets the path of the caller script.
+    The 'caller' here is the caller of the script that called this one.
+
+    Returns
+    -------
+    Path | None
+        Path of the caller script (None if there is no caller)
+    """
+    # Gets the path of the calling script (must be the "main")
+
+    # NOTE: 'f:back' twice
+    # The 1st is for the script calling this one, the 2nd is for the script calling the
+    # script that called this... which might be a NoneType
+
+    caller_1 = currentframe().f_back
+    caller_2 = caller_1.f_back
+
+    if not isinstance(caller_1, FrameType):
+        # No caller
+        # TODO: raise some exception, warning???
+        return None
+
+    caller = caller_2 if isinstance(caller_2, FrameType) else caller_1
+
+    return Path(getframeinfo(caller).filename)
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/experimental/lists.py` & `pyauxlib-0.0.2/src/pyauxlib/experimental/lists.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from pyauxlib.experimental.decorator import experimental
-
-
-@experimental
-def list_elements_to_numeric(lst: list) -> list:
-    """Converts to numeric values all the possible elements of a list.
-    First try to convert to int, and then to float. Elements that cannot be converted
-    are left untouched.
-
-    Parameters
-    ----------
-    lst : list
-        original list
-
-    Returns
-    -------
-    list
-        list with all possible elements converted to numeric
-    """
-    new_list = []
-    for ele in lst:
-        new_list.append(is_number(ele))
-
-    return new_list
-
-
-@experimental
-def is_number(ele):
-    """Returns an object converted to int. If it cannot be converted to int, it will
-    try to convert to float.
-
-    Parameters
-    ----------
-    ele : _type_
-        object
-
-    Returns
-    -------
-    int(ele) | is_float(ele)
-    """
-    try:
-        return int(ele)
-    except ValueError:
-        return is_float(ele)
-
-
-@experimental
-def is_float(ele):
-    """Returns an object converted to float, or the original object if it cannot be
-    converted
-
-    Parameters
-    ----------
-    ele : _type_
-        original object
-
-    Returns
-    -------
-    float(ele) | ele
-    """
-    try:
-        return float(ele)
-    except ValueError:
-        return ele
+from pyauxlib.experimental.decorator import experimental
+
+
+@experimental
+def list_elements_to_numeric(lst: list) -> list:
+    """Converts to numeric values all the possible elements of a list.
+    First try to convert to int, and then to float. Elements that cannot be converted
+    are left untouched.
+
+    Parameters
+    ----------
+    lst : list
+        original list
+
+    Returns
+    -------
+    list
+        list with all possible elements converted to numeric
+    """
+    new_list = []
+    for ele in lst:
+        new_list.append(is_number(ele))
+
+    return new_list
+
+
+@experimental
+def is_number(ele):
+    """Returns an object converted to int. If it cannot be converted to int, it will
+    try to convert to float.
+
+    Parameters
+    ----------
+    ele : _type_
+        object
+
+    Returns
+    -------
+    int(ele) | is_float(ele)
+    """
+    try:
+        return int(ele)
+    except ValueError:
+        return is_float(ele)
+
+
+@experimental
+def is_float(ele):
+    """Returns an object converted to float, or the original object if it cannot be
+    converted
+
+    Parameters
+    ----------
+    ele : _type_
+        original object
+
+    Returns
+    -------
+    float(ele) | ele
+    """
+    try:
+        return float(ele)
+    except ValueError:
+        return ele
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/io/yamlio.py` & `pyauxlib-0.0.2/src/pyauxlib/io/yamlio.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import logging
-import re
-from functools import partial
-from pathlib import Path
-
-import yaml
-from yaml.parser import ParserError
-
-logger = logging.getLogger(__name__)
-
-
-def _loader_scientific_notation():
-    """Returns a yaml loader that can parse numbers in scientific notation as numbers
-    instead of string. This is because library 'pyyaml' uses YAML 1.1 spec instead of
-    YAML 1.2 spec. See:
-    https://github.com/yaml/pyyaml/issues/173
-    https://stackoverflow.com/a/30462009
-    """
-    loader = yaml.FullLoader
-    loader.add_implicit_resolver(
-        "tag:yaml.org,2002:float",
-        re.compile(
-            """^(?:
-     [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
-    |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
-    |\\.[0-9_]+(?:[eE][-+][0-9]+)?
-    |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
-    |[-+]?\\.(?:inf|Inf|INF)
-    |\\.(?:nan|NaN|NAN))$""",
-            re.X,
-        ),
-        list("-+0123456789."),
-    )
-    return loader
-
-
-def load_yaml(file: Path, safe_load: bool = False) -> dict:
-    """Loads a yaml file and returns it as a dictionary.
-    If file is not found, returns an empty dictionary.
-
-    Parameters
-    ----------
-    file : Path
-        file
-    safe_load : bool
-        use safe load for the yaml
-
-    Returns
-    -------
-    dict
-        dictionary with the the yaml contents
-    """
-
-    load = yaml.safe_load if safe_load else partial(yaml.load, Loader=_loader_scientific_notation())
-
-    try:
-        with Path.open(file) as f:
-            conf = load(f)
-            if conf is None:
-                return {}
-    except ParserError:
-        logger.warning("Error loading the file '%s'", file)
-        raise
-    except FileNotFoundError:
-        logger.warning("File '%s' was not found", file)
-        raise
-
-    return conf
+import logging
+import re
+from functools import partial
+from pathlib import Path
+
+import yaml
+from yaml.parser import ParserError
+
+logger = logging.getLogger(__name__)
+
+
+def _loader_scientific_notation():
+    """Returns a yaml loader that can parse numbers in scientific notation as numbers
+    instead of string. This is because library 'pyyaml' uses YAML 1.1 spec instead of
+    YAML 1.2 spec. See:
+    https://github.com/yaml/pyyaml/issues/173
+    https://stackoverflow.com/a/30462009
+    """
+    loader = yaml.FullLoader
+    loader.add_implicit_resolver(
+        "tag:yaml.org,2002:float",
+        re.compile(
+            """^(?:
+     [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
+    |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
+    |\\.[0-9_]+(?:[eE][-+][0-9]+)?
+    |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
+    |[-+]?\\.(?:inf|Inf|INF)
+    |\\.(?:nan|NaN|NAN))$""",
+            re.X,
+        ),
+        list("-+0123456789."),
+    )
+    return loader
+
+
+def load_yaml(file: Path, safe_load: bool = False) -> dict:
+    """Loads a yaml file and returns it as a dictionary.
+    If file is not found, returns an empty dictionary.
+
+    Parameters
+    ----------
+    file : Path
+        file
+    safe_load : bool
+        use safe load for the yaml
+
+    Returns
+    -------
+    dict
+        dictionary with the the yaml contents
+    """
+
+    load = yaml.safe_load if safe_load else partial(yaml.load, Loader=_loader_scientific_notation())
+
+    try:
+        with Path.open(file) as f:
+            conf = load(f)
+            if conf is None:
+                return {}
+    except ParserError:
+        logger.warning("Error loading the file '%s'", file)
+        raise
+    except FileNotFoundError:
+        logger.warning("File '%s' was not found", file)
+        raise
+
+    return conf
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/utils/deprecations.py` & `pyauxlib-0.0.2/src/pyauxlib/utils/deprecations.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import warnings
-
-
-def warn_deprecated_argument(
-    method: str = "",
-    argument: str = "",
-    version: str = "",
-    additional_msg: str = "",
-    category=DeprecationWarning,
-    stacklevel=2,
-):
-    # Warns of a deprecated argument.
-    # To be called from within the method, when the deprecated argument is being used
-    # method : method name
-    # argument: argument to be deprecated
-    # version: in which will be removed
-    # additional_msg: e.g. "Use 'other_arg' instead"
-    # TODO: PROBABLY it can be improved quite a lot...
-    # TODO: Is it possible to convert it in a decorator?
-
-    if not any([method, argument, version]):
-        msg = "Used argument from method"
-    if method:
-        method = f"from method '{method}' "
-    if argument:
-        argument = f"'{argument}' "
-    if version:
-        version = f" in version {version}"
-    if additional_msg:
-        additional_msg = f". {additional_msg}."
-    msg = f"Argument {argument}{method}is being deprecated{version}{additional_msg}"
-    warnings.warn(msg, category=category, stacklevel=stacklevel)
+import warnings
+
+
+def warn_deprecated_argument(
+    method: str = "",
+    argument: str = "",
+    version: str = "",
+    additional_msg: str = "",
+    category=DeprecationWarning,
+    stacklevel=2,
+):
+    # Warns of a deprecated argument.
+    # To be called from within the method, when the deprecated argument is being used
+    # method : method name
+    # argument: argument to be deprecated
+    # version: in which will be removed
+    # additional_msg: e.g. "Use 'other_arg' instead"
+    # TODO: PROBABLY it can be improved quite a lot...
+    # TODO: Is it possible to convert it in a decorator?
+
+    if not any([method, argument, version]):
+        msg = "Used argument from method"
+    if method:
+        method = f"from method '{method}' "
+    if argument:
+        argument = f"'{argument}' "
+    if version:
+        version = f" in version {version}"
+    if additional_msg:
+        additional_msg = f". {additional_msg}."
+    msg = f"Argument {argument}{method}is being deprecated{version}{additional_msg}"
+    warnings.warn(msg, category=category, stacklevel=stacklevel)
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/utils/dictionaries.py` & `pyauxlib-0.0.2/src/pyauxlib/utils/dictionaries.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-def remove_keys(dictionary: dict, remove: list) -> dict:
-    """Removes the keys from a dictionary specified in the list `remove`.
-
-    If an element from `remove` is not a key in `dict`, then it will ignore (won't raise
-    any error)
-
-    Parameters
-    ----------
-    dictionary : dict
-        Original dictionary
-    remove : list
-        List with the keys to be removed from `dictionary`
-
-    Returns
-    -------
-    dict
-        Dictionary with the specified keys removed.
-    """
-
-    new_dict = dictionary.copy()
-    for k in remove:
-        new_dict.pop(k, None)
-
-    return new_dict
-
-
-def is_empty_or_none(dictionary: dict) -> bool:
-    """Returns if a dictionary is empty, or if all the values are `None`.
-
-    .. note::
-        A value of '0' is not considered empty.
-
-    Examples
-    --------
-    >>>nested_dict = {'a': {'b': None, 'c': {}}}
-    >>>print(is_empty_or_none(nested_dict))  # Output: True
-
-    >>>nested_dict = {'a': {'b': None, 'c': {'d': None}}}
-    >>>print(is_empty_or_none(nested_dict))  # Output: True
-
-    >>>nested_dict = {'a': {'b': 0, 'c': {'d': None}}}
-    >>>print(is_empty_or_none(nested_dict))  # Output: False
-    """
-    if not dictionary:
-        return True
-
-    for v in dictionary.values():
-        if isinstance(v, dict):
-            if not is_empty_or_none(v):
-                return False
-        elif v is not None:
-            return False
-
-    return True
+def remove_keys(dictionary: dict, remove: list) -> dict:
+    """Removes the keys from a dictionary specified in the list `remove`.
+
+    If an element from `remove` is not a key in `dict`, then it will ignore (won't raise
+    any error)
+
+    Parameters
+    ----------
+    dictionary : dict
+        Original dictionary
+    remove : list
+        List with the keys to be removed from `dictionary`
+
+    Returns
+    -------
+    dict
+        Dictionary with the specified keys removed.
+    """
+
+    new_dict = dictionary.copy()
+    for k in remove:
+        new_dict.pop(k, None)
+
+    return new_dict
+
+
+def is_empty_or_none(dictionary: dict) -> bool:
+    """Returns if a dictionary is empty, or if all the values are `None`.
+
+    .. note::
+        A value of '0' is not considered empty.
+
+    Examples
+    --------
+    >>>nested_dict = {'a': {'b': None, 'c': {}}}
+    >>>print(is_empty_or_none(nested_dict))  # Output: True
+
+    >>>nested_dict = {'a': {'b': None, 'c': {'d': None}}}
+    >>>print(is_empty_or_none(nested_dict))  # Output: True
+
+    >>>nested_dict = {'a': {'b': 0, 'c': {'d': None}}}
+    >>>print(is_empty_or_none(nested_dict))  # Output: False
+    """
+    if not dictionary:
+        return True
+
+    for v in dictionary.values():
+        if isinstance(v, dict):
+            if not is_empty_or_none(v):
+                return False
+        elif v is not None:
+            return False
+
+    return True
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/utils/encoding.py` & `pyauxlib-0.0.2/src/pyauxlib/utils/encoding.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import logging
-from codecs import BOM_UTF8
-from codecs import BOM_UTF16
-from codecs import BOM_UTF16_BE
-from codecs import BOM_UTF16_LE
-from codecs import BOM_UTF32
-from codecs import BOM_UTF32_BE
-from codecs import BOM_UTF32_LE
-from pathlib import Path
-
-try:
-    import chardet
-except ImportError:
-    chardet = None
-
-logger = logging.getLogger(__name__)
-
-
-def detect_encoding(file: str | Path) -> str | None:
-    """Detects the encoding of a file by reading the first bytes
-
-    Parameters
-    ----------
-    file : str | Path
-        file to be checked
-
-    Returns
-    -------
-    encoding : str | None
-        encoding of the file (None if file is not found)
-    """
-
-    codecs = {
-        BOM_UTF8: "utf_8_sig",
-        BOM_UTF16: "utf_16",
-        BOM_UTF16_BE: "utf_16_be",
-        BOM_UTF16_LE: "utf_16_le",
-        BOM_UTF32: "utf_32",
-        BOM_UTF32_BE: "utf_32_be",
-        BOM_UTF32_LE: "utf_32_le",
-    }
-
-    try:
-        with Path.open(file, "rb") as f:
-            # Reads the first 5 bytes
-            beginning = f.read(5)
-
-            if beginning[0:2] in codecs:
-                encoding = codecs[beginning[0:2]]
-            elif beginning[0:3] in codecs:
-                encoding = codecs[beginning[0:3]]
-            elif beginning[0:4] in codecs:
-                encoding = codecs[beginning[0:4]]
-            elif beginning[0:5] in codecs:
-                encoding = codecs[beginning[0:5]]
-            else:
-                encoding = "utf-8"
-            return encoding
-    except FileNotFoundError as err:
-        # TODO: how to use the logger in a module???
-        print(f"Error loading file: {file}")
-        print(err)
-        return None
-
-
-def detect_encoding_chardet(file: str | Path) -> str | None:
-    """Detects the encoding of the file using the chardet library. This library uses
-    heuristics to make an educated guess about the encoding of a file. However, this
-    method is not always accurate and may be slow for large files.
-    Use in cases where `detect_encoding` fails."""
-    try:
-        with Path.open(file, "rb") as f:
-            raw_data = f.read()
-            result = chardet.detect(raw_data)
-            encoding = result["encoding"]
-            return encoding
-    except AttributeError:
-        logger.warning("Install package 'chardet' for additional encoding detection.")
-        return None
-    except FileNotFoundError as err:
-        print(f"Error loading file: {file}")
-        print(err)
-        return None
+import logging
+from codecs import BOM_UTF8
+from codecs import BOM_UTF16
+from codecs import BOM_UTF16_BE
+from codecs import BOM_UTF16_LE
+from codecs import BOM_UTF32
+from codecs import BOM_UTF32_BE
+from codecs import BOM_UTF32_LE
+from pathlib import Path
+
+try:
+    import chardet
+except ImportError:
+    chardet = None
+
+logger = logging.getLogger(__name__)
+
+
+def detect_encoding(file: str | Path) -> str | None:
+    """Detects the encoding of a file by reading the first bytes
+
+    Parameters
+    ----------
+    file : str | Path
+        file to be checked
+
+    Returns
+    -------
+    encoding : str | None
+        encoding of the file (None if file is not found)
+    """
+
+    codecs = {
+        BOM_UTF8: "utf_8_sig",
+        BOM_UTF16: "utf_16",
+        BOM_UTF16_BE: "utf_16_be",
+        BOM_UTF16_LE: "utf_16_le",
+        BOM_UTF32: "utf_32",
+        BOM_UTF32_BE: "utf_32_be",
+        BOM_UTF32_LE: "utf_32_le",
+    }
+
+    try:
+        with Path.open(file, "rb") as f:
+            # Reads the first 5 bytes
+            beginning = f.read(5)
+
+            if beginning[0:2] in codecs:
+                encoding = codecs[beginning[0:2]]
+            elif beginning[0:3] in codecs:
+                encoding = codecs[beginning[0:3]]
+            elif beginning[0:4] in codecs:
+                encoding = codecs[beginning[0:4]]
+            elif beginning[0:5] in codecs:
+                encoding = codecs[beginning[0:5]]
+            else:
+                encoding = "utf-8"
+            return encoding
+    except FileNotFoundError as err:
+        # TODO: how to use the logger in a module???
+        print(f"Error loading file: {file}")
+        print(err)
+        return None
+
+
+def detect_encoding_chardet(file: str | Path) -> str | None:
+    """Detects the encoding of the file using the chardet library. This library uses
+    heuristics to make an educated guess about the encoding of a file. However, this
+    method is not always accurate and may be slow for large files.
+    Use in cases where `detect_encoding` fails."""
+    try:
+        with Path.open(file, "rb") as f:
+            raw_data = f.read()
+            result = chardet.detect(raw_data)
+            encoding = result["encoding"]
+            return encoding
+    except AttributeError:
+        logger.warning("Install package 'chardet' for additional encoding detection.")
+        return None
+    except FileNotFoundError as err:
+        print(f"Error loading file: {file}")
+        print(err)
+        return None
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/utils/logger.py` & `pyauxlib-0.0.2/src/pyauxlib/utils/logger.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import logging
-import logging.handlers
-from pathlib import Path
-
-
-def _set_level(level: int | str | None, default_level: int | str = "INFO") -> int:
-    """Returns a correct level value.
-
-    Parameters
-    ----------
-    level : int | str | None
-        level of the logger, by "INFO"
-        Any of the levers of logging can be passed as a string:
-        ['CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']
-        Note that lower case letters can also be used
-    default_level : int | str, optional
-        default level in case that `level` is incorrect, by default "INFO"
-
-    Returns
-    -------
-    The level as an int
-    """
-
-    if level is None:
-        return _set_level(default_level)
-
-    if isinstance(level, str):
-        level: int = logging.getLevelName(level.upper())
-    elif not isinstance(level, int):
-        level = logging.INFO
-
-    return level
-
-
-def init_logger(
-    name: str,
-    level: int | str = "INFO",
-    level_console: int | str | None = None,
-    level_file: int | str | None = None,
-    output_file: Path | None = None,
-    file_size: int = 0,
-    propagate: bool = False,
-    output_console: bool = True,
-    output_format: str = "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-) -> logging.Logger:
-    """Initializes the logger
-
-    Parameters
-    ----------
-    name : str
-        name of the logger
-    level : int | str, optional
-        level of the logger, by default "INFO"
-        Any of the levers of logging can be passed as a string:
-        ['CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']
-        Note that lower case letters can also be used
-    level_console : int | str | None, optional
-        level of the console logger, by default None
-    level_file : int | str | None, optional
-        level of the file logger, by default None
-    output_file : Path, optional
-        file to output the log, by default None
-    file_size : int, optional
-        maximum size of the output file in bytes, by default 0 (=unlimited size)
-    propagate : bool, optional
-        the log messages are passed or not to the parent logger, by default False
-    output_console : bool, optional
-        output the log to the console, by default True
-    output_format : str, optional
-        format of the output
-
-    Returns
-    -------
-    logging.Logger
-        logger
-    """
-
-    # FIXME Need some way to handle if the passed level string is not correct
-    level = _set_level(level)
-
-    level_console = _set_level(level_console, default_level=level)
-    level_file = _set_level(level_file, default_level=level)
-
-    level = min([level, level_console, level_file])
-
-    formatter = logging.Formatter(output_format)
-
-    handler_list: list[logging.Handler] = []
-    if output_file:
-        file_handler = logging.handlers.RotatingFileHandler(filename=output_file, maxBytes=file_size, backupCount=5)
-        file_handler.setLevel(level_file)
-        file_handler.setFormatter(formatter)
-        handler_list.append(file_handler)
-
-    if output_console:
-        console_handler = logging.StreamHandler()
-        console_handler.setLevel(level_console)
-        console_handler.setFormatter(formatter)
-        handler_list.append(console_handler)
-
-    logger = logging.getLogger(name)
-
-    # ??? Do I need to set the basicConfig for the root logger?
-    # Check if the parent is the root logger
-    # if logger.parent == logging.getLogger():
-    #     logging.basicConfig(
-    #         level=level,
-    #         # format=output_format,
-    #         handlers=handler_list,
-    #     )
-
-    # logger = logging.getLogger(name)
-
-    logger.setLevel(level=level)
-    logger.propagate = propagate
-    for handler in handler_list:
-        logger.addHandler(handler)
-    return logger
+import logging
+import logging.handlers
+from pathlib import Path
+
+
+def _set_level(level: int | str | None, default_level: int | str = "INFO") -> int:
+    """Returns a correct level value.
+
+    Parameters
+    ----------
+    level : int | str | None
+        level of the logger, by "INFO"
+        Any of the levers of logging can be passed as a string:
+        ['CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']
+        Note that lower case letters can also be used
+    default_level : int | str, optional
+        default level in case that `level` is incorrect, by default "INFO"
+
+    Returns
+    -------
+    The level as an int
+    """
+
+    if level is None:
+        return _set_level(default_level)
+
+    if isinstance(level, str):
+        level: int = logging.getLevelName(level.upper())
+    elif not isinstance(level, int):
+        level = logging.INFO
+
+    return level
+
+
+def init_logger(
+    name: str,
+    level: int | str = "INFO",
+    level_console: int | str | None = None,
+    level_file: int | str | None = None,
+    output_file: Path | None = None,
+    file_size: int = 0,
+    propagate: bool = False,
+    output_console: bool = True,
+    output_format: str = "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+) -> logging.Logger:
+    """Initializes the logger
+
+    Parameters
+    ----------
+    name : str
+        name of the logger
+    level : int | str, optional
+        level of the logger, by default "INFO"
+        Any of the levers of logging can be passed as a string:
+        ['CRITICAL', 'FATAL', 'ERROR', 'WARN', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']
+        Note that lower case letters can also be used
+    level_console : int | str | None, optional
+        level of the console logger, by default None
+    level_file : int | str | None, optional
+        level of the file logger, by default None
+    output_file : Path, optional
+        file to output the log, by default None
+    file_size : int, optional
+        maximum size of the output file in bytes, by default 0 (=unlimited size)
+    propagate : bool, optional
+        the log messages are passed or not to the parent logger, by default False
+    output_console : bool, optional
+        output the log to the console, by default True
+    output_format : str, optional
+        format of the output
+
+    Returns
+    -------
+    logging.Logger
+        logger
+    """
+
+    # FIXME Need some way to handle if the passed level string is not correct
+    level = _set_level(level)
+
+    level_console = _set_level(level_console, default_level=level)
+    level_file = _set_level(level_file, default_level=level)
+
+    level = min([level, level_console, level_file])
+
+    formatter = logging.Formatter(output_format)
+
+    handler_list: list[logging.Handler] = []
+    if output_file:
+        file_handler = logging.handlers.RotatingFileHandler(filename=output_file, maxBytes=file_size, backupCount=5)
+        file_handler.setLevel(level_file)
+        file_handler.setFormatter(formatter)
+        handler_list.append(file_handler)
+
+    if output_console:
+        console_handler = logging.StreamHandler()
+        console_handler.setLevel(level_console)
+        console_handler.setFormatter(formatter)
+        handler_list.append(console_handler)
+
+    logger = logging.getLogger(name)
+
+    # ??? Do I need to set the basicConfig for the root logger?
+    # Check if the parent is the root logger
+    # if logger.parent == logging.getLogger():
+    #     logging.basicConfig(
+    #         level=level,
+    #         # format=output_format,
+    #         handlers=handler_list,
+    #     )
+
+    # logger = logging.getLogger(name)
+
+    logger.setLevel(level=level)
+    logger.propagate = propagate
+    for handler in handler_list:
+        logger.addHandler(handler)
+    return logger
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib/utils/timer.py` & `pyauxlib-0.0.2/src/pyauxlib/utils/timer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import csv
-import logging
-import time
-import warnings
-from pathlib import Path
-
-
-class Timer:
-    """Timer class to measure execution times.
-
-    The timer can be managed manually, calling the start, stop,... methods.
-    It can also be used as a context manager:
-    ```python
-    with Timer(file) as t: # This will automaticall start the timer
-        # code here
-        t.add_timestamp("#1")
-        # more code
-    # The timer will automatically be stopped when exiting the context manager
-    ```
-
-    Parameters
-    ----------
-    filename : str | Path | None
-        The name or path of the file to save the timestamps.
-    time_func : callable, optional
-        The time function to use. It can be time.time, time.perf_counter or
-        time.process_time. By default time.time.
-    logger : logging.Logger, optional
-        The logger to use for logging warnings. By default None.
-
-    Attributes
-    ----------
-    filename : str | Path | None
-        The name of the file to save the timestamps. By default None.
-    start_time : float or None
-        The start time of the timer.
-    stop_time : float or None
-        The stop time of the timer.
-    timestamps : list of float
-        The list of timestamps added during the timer execution.
-    texts : list of str
-        The list of texts associated with each timestamp.
-    """
-
-    def __init__(
-        self,
-        filename: str | Path | None = None,
-        time_func=time.time,
-        logger: logging.Logger | None = None,
-    ):
-        self.filename = filename
-        self.time_func = time_func
-        self.logger = warnings.warn if logger is None else logger.warning
-        self.where_output = None if logger is None else logger.info
-        self.reset()
-
-    def __enter__(self):
-        """Start a new timer as a context manager"""
-        self.start()
-        return self
-
-    def __exit__(self, *exc_info):
-        """Stop the context manager timer"""
-        self.stop()
-
-    def start(self):
-        """Starts the timer."""
-        if self.stop_time is not None:
-            self.logger("Timer has not been resetted.")
-            return
-        self.start_time = self.time_func()
-
-    def stop(self) -> float:
-        """Stops the timer and returns the ellapsed time. It also saves the timestamps
-        to a file, when provided."""
-        if self.start_time is None:
-            self.logger("Timer has not been started.")
-            return 0
-
-        self.stop_time = self.time_func()
-        self.texts.append("stop")
-        self.save()
-
-        ellapsed_time = self.stop_time - self.start_time
-
-        if self.where_output is not None:
-            self.where_output(f"Ellapsed time: {ellapsed_time} s")
-
-        return ellapsed_time
-
-    def add_timestamp(self, text=""):
-        """Adds a timestamp with an associated text.
-
-        Parameters
-        ----------
-        text : str, optional
-            The text associated with the timestamp. By default "".
-        """
-        if self.start_time is None:
-            self.logger("Timer has not been started.")
-            return
-        if self.stop_time is not None:
-            self.logger("Timer is stopped.")
-            return
-
-        self.timestamps.append(self.time_func())
-        self.texts.append(text)
-
-    def save(self):
-        """Saves the timestamps and their associated texts to a file."""
-        if self.start_time is None:
-            self.logger("Timer has not been started.")
-            return
-        if self.stop_time is None:
-            self.logger("Timer has not been stopped yet.")
-            return
-        if self.filename is None:
-            return
-
-        with Path.open(self.filename, "w", newline="") as csvfile:
-            writer = csv.writer(csvfile)
-            header = ["Comment", "Timestamp", "Time", "Elapsed Time", "Total Time"]
-            writer.writerow(header)
-
-            formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.start_time))
-            row = [self.texts[0], self.start_time, formatted_time, 0, 0]
-            writer.writerow(row)
-            prev_time = self.start_time
-            for i, timestamp in enumerate(self.timestamps):
-                elapsed_time = timestamp - prev_time
-                total_time = timestamp - self.start_time
-                formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(timestamp))
-                row = [
-                    self.texts[i + 1],
-                    timestamp,
-                    formatted_time,
-                    elapsed_time,
-                    total_time,
-                ]
-                writer.writerow(row)
-                prev_time = timestamp
-            elapsed_time = self.stop_time - prev_time
-            total_time = self.stop_time - self.start_time
-            formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.stop_time))
-            row = [
-                self.texts[-1],
-                self.stop_time,
-                formatted_time,
-                elapsed_time,
-                total_time,
-            ]
-            writer.writerow(row)
-
-    def reset(self):
-        """Resets the timer."""
-        self.start_time = None
-        self.stop_time = None
-        self.timestamps = []
-        self.texts = ["start"]
+import csv
+import logging
+import time
+import warnings
+from pathlib import Path
+
+
+class Timer:
+    """Timer class to measure execution times.
+
+    The timer can be managed manually, calling the start, stop,... methods.
+    It can also be used as a context manager:
+    ```python
+    with Timer(file) as t: # This will automaticall start the timer
+        # code here
+        t.add_timestamp("#1")
+        # more code
+    # The timer will automatically be stopped when exiting the context manager
+    ```
+
+    Parameters
+    ----------
+    filename : str | Path | None
+        The name or path of the file to save the timestamps.
+    time_func : callable, optional
+        The time function to use. It can be time.time, time.perf_counter or
+        time.process_time. By default time.time.
+    logger : logging.Logger, optional
+        The logger to use for logging warnings. By default None.
+
+    Attributes
+    ----------
+    filename : str | Path | None
+        The name of the file to save the timestamps. By default None.
+    start_time : float or None
+        The start time of the timer.
+    stop_time : float or None
+        The stop time of the timer.
+    timestamps : list of float
+        The list of timestamps added during the timer execution.
+    texts : list of str
+        The list of texts associated with each timestamp.
+    """
+
+    def __init__(
+        self,
+        filename: str | Path | None = None,
+        time_func=time.time,
+        logger: logging.Logger | None = None,
+    ):
+        self.filename = filename
+        self.time_func = time_func
+        self.logger = warnings.warn if logger is None else logger.warning
+        self.where_output = None if logger is None else logger.info
+        self.reset()
+
+    def __enter__(self):
+        """Start a new timer as a context manager"""
+        self.start()
+        return self
+
+    def __exit__(self, *exc_info):
+        """Stop the context manager timer"""
+        self.stop()
+
+    def start(self):
+        """Starts the timer."""
+        if self.stop_time is not None:
+            self.logger("Timer has not been resetted.")
+            return
+        self.start_time = self.time_func()
+
+    def stop(self) -> float:
+        """Stops the timer and returns the ellapsed time. It also saves the timestamps
+        to a file, when provided."""
+        if self.start_time is None:
+            self.logger("Timer has not been started.")
+            return 0
+
+        self.stop_time = self.time_func()
+        self.texts.append("stop")
+        self.save()
+
+        ellapsed_time = self.stop_time - self.start_time
+
+        if self.where_output is not None:
+            self.where_output(f"Ellapsed time: {ellapsed_time} s")
+
+        return ellapsed_time
+
+    def add_timestamp(self, text=""):
+        """Adds a timestamp with an associated text.
+
+        Parameters
+        ----------
+        text : str, optional
+            The text associated with the timestamp. By default "".
+        """
+        if self.start_time is None:
+            self.logger("Timer has not been started.")
+            return
+        if self.stop_time is not None:
+            self.logger("Timer is stopped.")
+            return
+
+        self.timestamps.append(self.time_func())
+        self.texts.append(text)
+
+    def save(self):
+        """Saves the timestamps and their associated texts to a file."""
+        if self.start_time is None:
+            self.logger("Timer has not been started.")
+            return
+        if self.stop_time is None:
+            self.logger("Timer has not been stopped yet.")
+            return
+        if self.filename is None:
+            return
+
+        with Path.open(self.filename, "w", newline="") as csvfile:
+            writer = csv.writer(csvfile)
+            header = ["Comment", "Timestamp", "Time", "Elapsed Time", "Total Time"]
+            writer.writerow(header)
+
+            formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.start_time))
+            row = [self.texts[0], self.start_time, formatted_time, 0, 0]
+            writer.writerow(row)
+            prev_time = self.start_time
+            for i, timestamp in enumerate(self.timestamps):
+                elapsed_time = timestamp - prev_time
+                total_time = timestamp - self.start_time
+                formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(timestamp))
+                row = [
+                    self.texts[i + 1],
+                    timestamp,
+                    formatted_time,
+                    elapsed_time,
+                    total_time,
+                ]
+                writer.writerow(row)
+                prev_time = timestamp
+            elapsed_time = self.stop_time - prev_time
+            total_time = self.stop_time - self.start_time
+            formatted_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.stop_time))
+            row = [
+                self.texts[-1],
+                self.stop_time,
+                formatted_time,
+                elapsed_time,
+                total_time,
+            ]
+            writer.writerow(row)
+
+    def reset(self):
+        """Resets the timer."""
+        self.start_time = None
+        self.stop_time = None
+        self.timestamps = []
+        self.texts = ["start"]
```

### Comparing `pyauxlib-0.0.1/src/pyauxlib.egg-info/SOURCES.txt` & `pyauxlib-0.0.2/src/pyauxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyauxlib-0.0.1/tox.ini` & `pyauxlib-0.0.2/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,88 @@
 00000000: 5b74 6573 7465 6e76 3a62 6f6f 7473 7472  [testenv:bootstr
-00000010: 6170 5d0d 0a64 6570 7320 3d0d 0a20 2020  ap]..deps =..   
-00000020: 206a 696e 6a61 320d 0a20 2020 2074 6f78   jinja2..    tox
-00000030: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
-00000040: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
-00000050: 3d0d 0a20 2020 2070 7974 686f 6e20 6369  =..    python ci
-00000060: 2f62 6f6f 7473 7472 6170 2e70 7920 2d2d  /bootstrap.py --
-00000070: 6e6f 2d65 6e76 0d0a 7061 7373 656e 7620  no-env..passenv 
-00000080: 3d0d 0a20 2020 202a 0d0a 0d0a 3b20 6120  =..    *....; a 
-00000090: 6765 6e65 7261 7469 7665 2074 6f78 2063  generative tox c
-000000a0: 6f6e 6669 6775 7261 7469 6f6e 2c20 7365  onfiguration, se
-000000b0: 653a 2068 7474 7073 3a2f 2f74 6f78 2e77  e: https://tox.w
-000000c0: 696b 692f 656e 2f6c 6174 6573 742f 7573  iki/en/latest/us
-000000d0: 6572 5f67 7569 6465 2e68 746d 6c23 6765  er_guide.html#ge
-000000e0: 6e65 7261 7469 7665 2d65 6e76 6972 6f6e  nerative-environ
-000000f0: 6d65 6e74 730d 0a5b 746f 785d 0d0a 656e  ments..[tox]..en
-00000100: 766c 6973 7420 3d0d 0a20 2020 2063 6c65  vlist =..    cle
-00000110: 616e 2c0d 0a20 2020 2063 6865 636b 2c0d  an,..    check,.
-00000120: 0a20 2020 2064 6f63 732c 0d0a 2020 2020  .    docs,..    
-00000130: 7b70 7933 3130 2c70 7933 3131 7d2c 0d0a  {py310,py311},..
-00000140: 2020 2020 7265 706f 7274 0d0a 6967 6e6f      report..igno
-00000150: 7265 5f62 6173 6570 7974 686f 6e5f 636f  re_basepython_co
-00000160: 6e66 6c69 6374 203d 2074 7275 650d 0a0d  nflict = true...
-00000170: 0a5b 7465 7374 656e 765d 0d0a 6261 7365  .[testenv]..base
-00000180: 7079 7468 6f6e 203d 0d0a 2020 2020 7079  python =..    py
-00000190: 3331 303a 207b 656e 763a 544f 5850 5954  310: {env:TOXPYT
-000001a0: 484f 4e3a 7079 7468 6f6e 332e 3130 7d0d  HON:python3.10}.
-000001b0: 0a20 2020 2070 7933 3131 3a20 7b65 6e76  .    py311: {env
-000001c0: 3a54 4f58 5059 5448 4f4e 3a70 7974 686f  :TOXPYTHON:pytho
-000001d0: 6e33 2e31 317d 0d0a 2020 2020 7b62 6f6f  n3.11}..    {boo
-000001e0: 7473 7472 6170 2c63 6c65 616e 2c63 6865  tstrap,clean,che
-000001f0: 636b 2c72 6570 6f72 742c 646f 6373 7d3a  ck,report,docs}:
-00000200: 207b 656e 763a 544f 5850 5954 484f 4e3a   {env:TOXPYTHON:
-00000210: 7079 7468 6f6e 337d 0d0a 7365 7465 6e76  python3}..setenv
-00000220: 203d 0d0a 2020 2020 5059 5448 4f4e 5041   =..    PYTHONPA
-00000230: 5448 3d7b 746f 7869 6e69 6469 727d 2f74  TH={toxinidir}/t
-00000240: 6573 7473 0d0a 2020 2020 5059 5448 4f4e  ests..    PYTHON
-00000250: 554e 4255 4646 4552 4544 3d79 6573 0d0a  UNBUFFERED=yes..
-00000260: 7061 7373 656e 7620 3d0d 0a20 2020 202a  passenv =..    *
-00000270: 0d0a 7573 6564 6576 656c 6f70 203d 2066  ..usedevelop = f
-00000280: 616c 7365 0d0a 6465 7073 203d 0d0a 2020  alse..deps =..  
-00000290: 2020 7079 7465 7374 0d0a 2020 2020 7079    pytest..    py
-000002a0: 7465 7374 2d63 6f76 0d0a 636f 6d6d 616e  test-cov..comman
-000002b0: 6473 203d 0d0a 2020 2020 7b70 6f73 6172  ds =..    {posar
-000002c0: 6773 3a70 7974 6573 7420 2d2d 636f 7620  gs:pytest --cov 
-000002d0: 2d2d 636f 762d 7265 706f 7274 3d74 6572  --cov-report=ter
-000002e0: 6d2d 6d69 7373 696e 6720 2d2d 636f 762d  m-missing --cov-
-000002f0: 7265 706f 7274 3d78 6d6c 202d 7676 2074  report=xml -vv t
-00000300: 6573 7473 7d0d 0a0d 0a5b 7465 7374 656e  ests}....[testen
-00000310: 763a 6368 6563 6b5d 0d0a 6465 7073 203d  v:check]..deps =
-00000320: 0d0a 2020 2020 646f 6375 7469 6c73 0d0a  ..    docutils..
-00000330: 2020 2020 6368 6563 6b2d 6d61 6e69 6665      check-manife
-00000340: 7374 0d0a 2020 2020 7072 652d 636f 6d6d  st..    pre-comm
-00000350: 6974 0d0a 2020 2020 7265 6164 6d65 2d72  it..    readme-r
-00000360: 656e 6465 7265 720d 0a20 2020 2070 7967  enderer..    pyg
-00000370: 6d65 6e74 730d 0a20 2020 2069 736f 7274  ments..    isort
-00000380: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
-00000390: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
-000003a0: 3d0d 0a20 2020 2070 7974 686f 6e20 7365  =..    python se
-000003b0: 7475 702e 7079 2063 6865 636b 202d 2d73  tup.py check --s
-000003c0: 7472 6963 7420 2d2d 6d65 7461 6461 7461  trict --metadata
-000003d0: 202d 2d72 6573 7472 7563 7475 7265 6474   --restructuredt
-000003e0: 6578 740d 0a20 2020 2063 6865 636b 2d6d  ext..    check-m
-000003f0: 616e 6966 6573 7420 2e0d 0a20 2020 2070  anifest ...    p
-00000400: 7265 2d63 6f6d 6d69 7420 7275 6e20 2d2d  re-commit run --
-00000410: 616c 6c2d 6669 6c65 7320 2d2d 7368 6f77  all-files --show
-00000420: 2d64 6966 662d 6f6e 2d66 6169 6c75 7265  -diff-on-failure
-00000430: 0d0a 0d0a 5b74 6573 7465 6e76 3a64 6f63  ....[testenv:doc
-00000440: 735d 0d0a 7573 6564 6576 656c 6f70 203d  s]..usedevelop =
-00000450: 2074 7275 650d 0a64 6570 7320 3d0d 0a20   true..deps =.. 
-00000460: 2020 202d 727b 746f 7869 6e69 6469 727d     -r{toxinidir}
-00000470: 2f64 6f63 732f 7265 7175 6972 656d 656e  /docs/requiremen
-00000480: 7473 2e74 7874 0d0a 636f 6d6d 616e 6473  ts.txt..commands
-00000490: 203d 0d0a 2020 2020 7370 6869 6e78 2d62   =..    sphinx-b
-000004a0: 7569 6c64 207b 706f 7361 7267 733a 2d45  uild {posargs:-E
-000004b0: 7d20 2d62 2068 746d 6c20 646f 6373 2064  } -b html docs d
-000004c0: 6973 742f 646f 6373 0d0a 2020 2020 7370  ist/docs..    sp
-000004d0: 6869 6e78 2d62 7569 6c64 202d 6220 6c69  hinx-build -b li
-000004e0: 6e6b 6368 6563 6b20 646f 6373 2064 6973  nkcheck docs dis
-000004f0: 742f 646f 6373 0d0a 0d0a 5b74 6573 7465  t/docs....[teste
-00000500: 6e76 3a72 6570 6f72 745d 0d0a 6465 7073  nv:report]..deps
-00000510: 203d 0d0a 2020 2020 636f 7665 7261 6765   =..    coverage
-00000520: 0d0a 736b 6970 5f69 6e73 7461 6c6c 203d  ..skip_install =
-00000530: 2074 7275 650d 0a63 6f6d 6d61 6e64 7320   true..commands 
-00000540: 3d0d 0a20 2020 2063 6f76 6572 6167 6520  =..    coverage 
-00000550: 7265 706f 7274 0d0a 2020 2020 636f 7665  report..    cove
-00000560: 7261 6765 2068 746d 6c0d 0a0d 0a5b 7465  rage html....[te
-00000570: 7374 656e 763a 636c 6561 6e5d 0d0a 636f  stenv:clean]..co
-00000580: 6d6d 616e 6473 203d 2063 6f76 6572 6167  mmands = coverag
-00000590: 6520 6572 6173 650d 0a73 6b69 705f 696e  e erase..skip_in
-000005a0: 7374 616c 6c20 3d20 7472 7565 0d0a 6465  stall = true..de
-000005b0: 7073 203d 0d0a 2020 2020 636f 7665 7261  ps =..    covera
-000005c0: 6765 0d0a                                ge..
+00000010: 6170 5d0a 6465 7073 203d 0a20 2020 206a  ap].deps =.    j
+00000020: 696e 6a61 320a 2020 2020 746f 780a 736b  inja2.    tox.sk
+00000030: 6970 5f69 6e73 7461 6c6c 203d 2074 7275  ip_install = tru
+00000040: 650a 636f 6d6d 616e 6473 203d 0a20 2020  e.commands =.   
+00000050: 2070 7974 686f 6e20 6369 2f62 6f6f 7473   python ci/boots
+00000060: 7472 6170 2e70 7920 2d2d 6e6f 2d65 6e76  trap.py --no-env
+00000070: 0a70 6173 7365 6e76 203d 0a20 2020 202a  .passenv =.    *
+00000080: 0a0a 3b20 6120 6765 6e65 7261 7469 7665  ..; a generative
+00000090: 2074 6f78 2063 6f6e 6669 6775 7261 7469   tox configurati
+000000a0: 6f6e 2c20 7365 653a 2068 7474 7073 3a2f  on, see: https:/
+000000b0: 2f74 6f78 2e77 696b 692f 656e 2f6c 6174  /tox.wiki/en/lat
+000000c0: 6573 742f 7573 6572 5f67 7569 6465 2e68  est/user_guide.h
+000000d0: 746d 6c23 6765 6e65 7261 7469 7665 2d65  tml#generative-e
+000000e0: 6e76 6972 6f6e 6d65 6e74 730a 5b74 6f78  nvironments.[tox
+000000f0: 5d0a 656e 766c 6973 7420 3d0a 2020 2020  ].envlist =.    
+00000100: 636c 6561 6e2c 0a20 2020 2063 6865 636b  clean,.    check
+00000110: 2c0a 2020 2020 646f 6373 2c0a 2020 2020  ,.    docs,.    
+00000120: 7b70 7933 3130 2c70 7933 3131 7d2c 0a20  {py310,py311},. 
+00000130: 2020 2072 6570 6f72 740a 6967 6e6f 7265     report.ignore
+00000140: 5f62 6173 6570 7974 686f 6e5f 636f 6e66  _basepython_conf
+00000150: 6c69 6374 203d 2074 7275 650a 0a5b 7465  lict = true..[te
+00000160: 7374 656e 765d 0a62 6173 6570 7974 686f  stenv].basepytho
+00000170: 6e20 3d0a 2020 2020 7079 3331 303a 207b  n =.    py310: {
+00000180: 656e 763a 544f 5850 5954 484f 4e3a 7079  env:TOXPYTHON:py
+00000190: 7468 6f6e 332e 3130 7d0a 2020 2020 7079  thon3.10}.    py
+000001a0: 3331 313a 207b 656e 763a 544f 5850 5954  311: {env:TOXPYT
+000001b0: 484f 4e3a 7079 7468 6f6e 332e 3131 7d0a  HON:python3.11}.
+000001c0: 2020 2020 7b62 6f6f 7473 7472 6170 2c63      {bootstrap,c
+000001d0: 6c65 616e 2c63 6865 636b 2c72 6570 6f72  lean,check,repor
+000001e0: 742c 646f 6373 7d3a 207b 656e 763a 544f  t,docs}: {env:TO
+000001f0: 5850 5954 484f 4e3a 7079 7468 6f6e 337d  XPYTHON:python3}
+00000200: 0a73 6574 656e 7620 3d0a 2020 2020 5059  .setenv =.    PY
+00000210: 5448 4f4e 5041 5448 3d7b 746f 7869 6e69  THONPATH={toxini
+00000220: 6469 727d 2f74 6573 7473 0a20 2020 2050  dir}/tests.    P
+00000230: 5954 484f 4e55 4e42 5546 4645 5245 443d  YTHONUNBUFFERED=
+00000240: 7965 730a 7061 7373 656e 7620 3d0a 2020  yes.passenv =.  
+00000250: 2020 2a0a 7573 6564 6576 656c 6f70 203d    *.usedevelop =
+00000260: 2066 616c 7365 0a64 6570 7320 3d0a 2020   false.deps =.  
+00000270: 2020 7079 7465 7374 0a20 2020 2070 7974    pytest.    pyt
+00000280: 6573 742d 636f 760a 636f 6d6d 616e 6473  est-cov.commands
+00000290: 203d 0a20 2020 207b 706f 7361 7267 733a   =.    {posargs:
+000002a0: 7079 7465 7374 202d 2d63 6f76 202d 2d63  pytest --cov --c
+000002b0: 6f76 2d72 6570 6f72 743d 7465 726d 2d6d  ov-report=term-m
+000002c0: 6973 7369 6e67 202d 2d63 6f76 2d72 6570  issing --cov-rep
+000002d0: 6f72 743d 786d 6c20 2d76 7620 7465 7374  ort=xml -vv test
+000002e0: 737d 0a0a 5b74 6573 7465 6e76 3a63 6865  s}..[testenv:che
+000002f0: 636b 5d0a 6465 7073 203d 0a20 2020 2064  ck].deps =.    d
+00000300: 6f63 7574 696c 730a 2020 2020 6368 6563  ocutils.    chec
+00000310: 6b2d 6d61 6e69 6665 7374 0a20 2020 2070  k-manifest.    p
+00000320: 7265 2d63 6f6d 6d69 740a 2020 2020 7265  re-commit.    re
+00000330: 6164 6d65 2d72 656e 6465 7265 720a 2020  adme-renderer.  
+00000340: 2020 7079 676d 656e 7473 0a20 2020 2069    pygments.    i
+00000350: 736f 7274 0a73 6b69 705f 696e 7374 616c  sort.skip_instal
+00000360: 6c20 3d20 7472 7565 0a63 6f6d 6d61 6e64  l = true.command
+00000370: 7320 3d0a 2020 2020 7079 7468 6f6e 2073  s =.    python s
+00000380: 6574 7570 2e70 7920 6368 6563 6b20 2d2d  etup.py check --
+00000390: 7374 7269 6374 202d 2d6d 6574 6164 6174  strict --metadat
+000003a0: 6120 2d2d 7265 7374 7275 6374 7572 6564  a --restructured
+000003b0: 7465 7874 0a20 2020 2063 6865 636b 2d6d  text.    check-m
+000003c0: 616e 6966 6573 7420 2e0a 2020 2020 7072  anifest ..    pr
+000003d0: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
+000003e0: 6c6c 2d66 696c 6573 202d 2d73 686f 772d  ll-files --show-
+000003f0: 6469 6666 2d6f 6e2d 6661 696c 7572 650a  diff-on-failure.
+00000400: 0a5b 7465 7374 656e 763a 646f 6373 5d0a  .[testenv:docs].
+00000410: 7573 6564 6576 656c 6f70 203d 2074 7275  usedevelop = tru
+00000420: 650a 6465 7073 203d 0a20 2020 202d 727b  e.deps =.    -r{
+00000430: 746f 7869 6e69 6469 727d 2f64 6f63 732f  toxinidir}/docs/
+00000440: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
+00000450: 0a63 6f6d 6d61 6e64 7320 3d0a 2020 2020  .commands =.    
+00000460: 7370 6869 6e78 2d62 7569 6c64 207b 706f  sphinx-build {po
+00000470: 7361 7267 733a 2d45 7d20 2d62 2068 746d  sargs:-E} -b htm
+00000480: 6c20 646f 6373 2064 6973 742f 646f 6373  l docs dist/docs
+00000490: 0a20 2020 2073 7068 696e 782d 6275 696c  .    sphinx-buil
+000004a0: 6420 2d62 206c 696e 6b63 6865 636b 2064  d -b linkcheck d
+000004b0: 6f63 7320 6469 7374 2f64 6f63 730a 0a5b  ocs dist/docs..[
+000004c0: 7465 7374 656e 763a 7265 706f 7274 5d0a  testenv:report].
+000004d0: 6465 7073 203d 0a20 2020 2063 6f76 6572  deps =.    cover
+000004e0: 6167 650a 736b 6970 5f69 6e73 7461 6c6c  age.skip_install
+000004f0: 203d 2074 7275 650a 636f 6d6d 616e 6473   = true.commands
+00000500: 203d 0a20 2020 2063 6f76 6572 6167 6520   =.    coverage 
+00000510: 7265 706f 7274 0a20 2020 2063 6f76 6572  report.    cover
+00000520: 6167 6520 6874 6d6c 0a0a 5b74 6573 7465  age html..[teste
+00000530: 6e76 3a63 6c65 616e 5d0a 636f 6d6d 616e  nv:clean].comman
+00000540: 6473 203d 2063 6f76 6572 6167 6520 6572  ds = coverage er
+00000550: 6173 650a 736b 6970 5f69 6e73 7461 6c6c  ase.skip_install
+00000560: 203d 2074 7275 650a 6465 7073 203d 0a20   = true.deps =. 
+00000570: 2020 2063 6f76 6572 6167 650a               coverage.
```

