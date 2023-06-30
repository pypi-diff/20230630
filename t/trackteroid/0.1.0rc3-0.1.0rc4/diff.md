# Comparing `tmp/trackteroid-0.1.0rc3.tar.gz` & `tmp/trackteroid-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackteroid-0.1.0rc3.tar", last modified: Mon Jun 26 09:05:37 2023, max compression
+gzip compressed data, was "trackteroid-0.1.0rc4.tar", last modified: Fri Jun 30 12:16:16 2023, max compression
```

## Comparing `trackteroid-0.1.0rc3.tar` & `trackteroid-0.1.0rc4.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.337818 trackteroid-0.1.0rc3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.337818 trackteroid-0.1.0rc3/.graphics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.graphics/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.graphics/svg/logo_black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.graphics/svg/logo_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/_static/logo_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/collections/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/emptycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/entitycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections.md
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/query/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query.md
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/session.md
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.341818 trackteroid-0.1.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/src/trackteroid/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72524 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/entities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/relationships_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/schematypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/criteria.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/stubs/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/src/trackteroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/tests/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.graphics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.graphics/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.graphics/svg/logo_black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.graphics/svg/logo_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/_static/logo_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/emptycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/entitycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26744 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/entity.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/session.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/src/trackteroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71990 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/relationships_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/schematypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/criteria.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/stubs/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/src/trackteroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/tests/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/tox.ini
```

### Comparing `trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--bug-report.md` & `trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--bug-report.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--feature-request.md` & `trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--feature-request.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/.github/workflows/python-publish.yml` & `trackteroid-0.1.0rc4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/.graphics/svg/logo_black.svg` & `trackteroid-0.1.0rc4/.graphics/svg/logo_black.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/.graphics/svg/logo_white.svg` & `trackteroid-0.1.0rc4/.graphics/svg/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/.readthedocs.yaml` & `trackteroid-0.1.0rc4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/LICENSE` & `trackteroid-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/Makefile` & `trackteroid-0.1.0rc4/doc/sphinx_source/Makefile`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/_static/favicon.ico` & `trackteroid-0.1.0rc4/doc/sphinx_source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/_static/logo_white.svg` & `trackteroid-0.1.0rc4/doc/sphinx_source/_static/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/collections/emptycollection.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/collections/emptycollection.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/collections/overview.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/collections/overview.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/conf.py` & `trackteroid-0.1.0rc4/doc/sphinx_source/conf.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/configuration.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/configuration.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/installation.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/installation.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/make.bat` & `trackteroid-0.1.0rc4/doc/sphinx_source/make.bat`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/query/examples.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/query/examples.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/doc/sphinx_source/query/overview.md` & `trackteroid-0.1.0rc4/doc/sphinx_source/query/overview.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/pyproject.toml` & `trackteroid-0.1.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/__init__.py` & `trackteroid-0.1.0rc4/src/trackteroid/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/configuration.py` & `trackteroid-0.1.0rc4/src/trackteroid/configuration.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/constants.py` & `trackteroid-0.1.0rc4/src/trackteroid/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__VERSION__ = "0.1.0rc3"
+__VERSION__ = "0.1.0rc4"
```

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/__init__.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/base.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 equal = equal and getattr(self, slot) == getattr(other, slot)
         return equal
 
     def __getattr__(self, item):
         current_depth = self.depth
         collection_copy = copy(self)
         # in case we use methods like .values() or .from_entities() etc
-        # we need to take care to not increment the depth, as it doesn represent
+        # we need to take care to not increment the depth, as it doesn't represent
         # an attribute/relation access
         if item in [_ for _ in dir(EntityCollection) if not re.match(r"__\w+__|children", _)]:
             collection_copy.depth = current_depth
         return collection_copy
 
     def __getitem__(self, item):
         # TEST: Maybe we should return somthing else when accessing POD
@@ -413,24 +413,39 @@
                         else:
                             values.append(_)
                     if not entities and not values and not entity_type:
                         entity_type = Entity.from_entity_type(
                             name=self._get_attribute_compatibility_types(item).types[0].__name__
                         )
                 elif value.__class__.__name__ == "KeyValueMappedCollectionProxy":
-                    values.append(dict(entity.ftrack_entity["metadata"].items()))
+                    values.append(dict(entity.ftrack_entity[item].items()))
 
                 # wrap ftrack entity
                 elif hasattr(value, "entity_type"):
                     entities.append(Entity.from_entity_type(str(value.entity_type), ftrack_entity=value))
                 else:
                     values.append(value)
 
             if entities:
-                return self.from_entities(entities, source=(item, self))
+                # wrap into lambdas so this will be only requested when needed
+                _to_typedcontext = lambda: getattr(importlib.import_module("..entities", __name__), "TypedContext")
+                _to_component = lambda: getattr(importlib.import_module("..entities", __name__), "Component")
+                _to_original = lambda: lambda collection: collection
+
+                coerce_attributes = {
+                    "parent": _to_typedcontext,
+                    "children": _to_typedcontext,
+                    "ancestors": _to_typedcontext,
+                    "descendants": _to_typedcontext,
+                    "components": _to_component
+                }
+                coercion_type = coerce_attributes.get(item, _to_original)()
+
+                return coercion_type(self.from_entities(entities, source=(item, self)))
+
             elif entity_type:
                 return EmptyCollection(_type=entity_type, source=self, session=self._session)
             return values
 
         elif item == "get":
             return self._get_relatives
 
@@ -635,61 +650,27 @@
 
         Args:
             entity_type (Entity): a given entity class that must be a subclass of the type of the current collection
 
         Returns:
             EntityCollection[entity_type] or EmptyCollection[entity_type]
         """
-        if not issubclass(entity_type, ForwardDeclaration):
-            # this can only work if the given entity type is a subclass of our currently
-            # used collection type, like TypedContext -> AssetBuild|Shot|Sequence... or Component -> FileComponent
-            # TODO: re-think the necessity of checking for the actual base type
-            #  Enforcing a type coercion before filtering via entity type makes the code more clear, but is
-            #  not strictly needed for correct filtering.
-            assert issubclass(entity_type, self.entity_type)
-        else:
+        if issubclass(entity_type, ForwardDeclaration):
             entity_type = getattr(importlib.import_module("..entities", __name__), entity_type.__name__)
 
         matched_types = self.filter(lambda x: list(x.values())[0].ftrack_entity.entity_type == entity_type.__name__)
         return self.from_entities(
             [
                 Entity.from_entity_type(entity_type.__name__, ftrack_entity=_.ftrack_entity) for _ in
                 matched_types.values() or []  # fall back to empty list in case we already have an EmptyCollection
             ],
             type_override=entity_type,
             source=getattr(matched_types, "source", None)
         )
 
-    @property
-    def children(self):
-        """ get all children
-
-        Returns:
-            EntityCollection[TypedContext]
-        """
-        # TODO: deal with this when it becomes a problem ;)
-        #  Other entities like Context or Group have children too. When we need to
-        #  access those we have to implement the functionality properly here.
-        # if not isinstance(self._entity, TypedContext):
-        #     getattr(self, "children")
-
-        default_projections = ["children.{}".format(_) for _ in self._entity.projections]
-        self._simple_children_fetch("children.object_type.name", *default_projections)
-
-        children_entities = []
-
-        for entity in self.values():
-            if entity["children"]:
-                for child in entity["children"]:
-                    children_entities.append(
-                        Entity.from_entity_type("TypedContext", ftrack_entity=child)
-                    )
-
-        return self.from_entities(children_entities, source=self)
-
     def query_children(self, projections=None, session=None):
         """Queries and returns the children of the collection. Only supported for
         entities that have a "children" relation
 
         Args:
             projections (`list` of `str`): Projections to fetch from the children
             session (Session): Optional session to use.
@@ -1011,15 +992,15 @@
             startvalue = predicate(startvalue, entitycollection)
         return startvalue
 
     def map(self, predicate):
         """ Returns a list of results that is obtained by running the predicate
         with each Entity as it's argument and returning the result.
         """
-        return map(predicate, self)
+        return list(map(predicate, self))
 
     def group_and_map(self, group_predicate, map_predicate):
         """ Runs a group_by first and then runs map on all the Collection in
         the resulting dictionary values.
         """
         groups = self.group(group_predicate)
 
@@ -1695,19 +1676,25 @@
             source_collection = args[0]
 
             if source_collection:
                 _cls = source_collection.entity_type
             else:
                 _cls = source_collection.entity_type.__class__
 
-            assert issubclass(_cls, cls), \
-                "Can't coerce `{source}` to `{target}`, because `{source}` is not a subtype of `{target}`.".format(
-                    source=_cls.__name__,
-                    target=cls.__name__,
-                )
+            _ACCEPT_CASES = {
+                "TypedContext": ["Project"]
+            }
+            bypass_exception = _cls.__name__ in _ACCEPT_CASES.get(cls.__name__, [])
+
+            if not bypass_exception:
+                assert issubclass(_cls, cls), \
+                    "Can't coerce `{source}` to `{target}`, because `{source}` is not a subtype of `{target}`.".format(
+                        source=_cls.__name__,
+                        target=cls.__name__,
+                    )
 
             _source = getattr(source_collection, "source", None)
 
             target_collection = source_collection.from_entities(
                 source_collection.values() or [],
                 type_override=cls,
                 source=_source
```

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.pyi` & `trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/entities.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/entities.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/entities.pyi` & `trackteroid-0.1.0rc4/src/trackteroid/entities/entities.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/relationships_parser.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/relationships_parser.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/entities/schematypes.py` & `trackteroid-0.1.0rc4/src/trackteroid/entities/schematypes.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/query/__init__.py` & `trackteroid-0.1.0rc4/src/trackteroid/query/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/query/criteria.py` & `trackteroid-0.1.0rc4/src/trackteroid/query/criteria.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/query/criteria.pyi` & `trackteroid-0.1.0rc4/src/trackteroid/query/criteria.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/query/query.py` & `trackteroid-0.1.0rc4/src/trackteroid/query/query.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/query/utils.py` & `trackteroid-0.1.0rc4/src/trackteroid/query/utils.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/session.py` & `trackteroid-0.1.0rc4/src/trackteroid/session.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/stubs/__init__.py` & `trackteroid-0.1.0rc4/src/trackteroid/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid/stubs/stubs.py` & `trackteroid-0.1.0rc4/src/trackteroid/stubs/stubs.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc3/src/trackteroid.egg-info/SOURCES.txt` & `trackteroid-0.1.0rc4/src/trackteroid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .graphics/svg/logo_black.svg
 .graphics/svg/logo_white.svg
 doc/requirements.txt
 doc/sphinx_source/Makefile
 doc/sphinx_source/collections.md
 doc/sphinx_source/conf.py
 doc/sphinx_source/configuration.md
+doc/sphinx_source/entity.md
 doc/sphinx_source/index.md
 doc/sphinx_source/installation.md
 doc/sphinx_source/make.bat
 doc/sphinx_source/query.md
 doc/sphinx_source/quickstart.md
 doc/sphinx_source/session.md
 doc/sphinx_source/_static/favicon.ico
```

