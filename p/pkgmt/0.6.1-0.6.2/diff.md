# Comparing `tmp/pkgmt-0.6.1.tar.gz` & `tmp/pkgmt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.6.1.tar", last modified: Fri Jun  9 17:42:12 2023, max compression
+gzip compressed data, was "pkgmt-0.6.2.tar", last modified: Fri Jun 30 15:32:14 2023, max compression
```

## Comparing `pkgmt-0.6.1.tar` & `pkgmt-0.6.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-09 17:41:55.000000 pkgmt-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-09 17:41:55.000000 pkgmt-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 17:41:55.000000 pkgmt-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 17:42:12.486443 pkgmt-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 17:41:55.000000 pkgmt-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 17:41:55.000000 pkgmt-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:42:12.486443 pkgmt-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-09 17:41:55.000000 pkgmt-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.482443 pkgmt-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.482443 pkgmt-0.6.1/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/template/src/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/src/package_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/fail_if_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/fail_if_not_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioner/abstractversioner.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioner/versionernonsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 17:41:55.000000 pkgmt-0.6.1/src/pkgmt/versioner/versionersetup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:42:12.486443 pkgmt-0.6.1/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 17:42:12.000000 pkgmt-0.6.1/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-06-30 15:31:57.000000 pkgmt-0.6.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 15:31:57.000000 pkgmt-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 15:31:57.000000 pkgmt-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 15:32:14.946761 pkgmt-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 15:31:57.000000 pkgmt-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 15:31:57.000000 pkgmt-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 15:32:14.946761 pkgmt-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-30 15:31:57.000000 pkgmt-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/src/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/src/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/fail_if_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/fail_if_not_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.946761 pkgmt-0.6.2/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/abstractversioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/versionernonsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-30 15:31:57.000000 pkgmt-0.6.2/src/pkgmt/versioner/versionersetup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:32:14.942762 pkgmt-0.6.2/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 15:32:14.000000 pkgmt-0.6.2/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.6.1/CHANGELOG.md` & `pkgmt-0.6.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## 0.6.2 (2023-06-30)
+
+* [Feature] Added file path to `pkgmt lint` ([#56](https://github.com/ploomber/pkgmt/issues/56))
+* [Feature] Clearer error when missing `pyproject.toml`
+* [Feature] Added `--exclude` option to pkgmt `lint` and pkgmt `format` ([#55](https://github.com/ploomber/pkgmt/issues/55))
+
 ## 0.6.1 (2023-06-09)
 
 * [Feature] Adds `python -m pkgmt.fail_if_not_modified` to test if certain paths in the repository have been modified
 
 ## 0.6.0 (2023-06-05)
 
 * [API Change] Support for `pkgmt new` when argument contains `_` or `-`
```

### Comparing `pkgmt-0.6.1/LICENSE` & `pkgmt-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/README.md` & `pkgmt-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/setup.py` & `pkgmt-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,17 @@
     author=None,
     author_email=None,
     url=None,
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     include_package_data=True,
-    classifiers=[],
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+    ],
     keywords=[],
     install_requires=REQUIRES,
     extras_require={
         "dev": DEV + CHECK,
         "all": ALL,
         "check": CHECK,
     },
```

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/.github/pull_request_template.md` & `pkgmt-0.6.2/src/pkgmt/assets/template/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.6.2/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.6.2/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/pyproject.toml` & `pkgmt-0.6.2/src/pkgmt/assets/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/setup.py` & `pkgmt-0.6.2/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.6.2/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/assets/template/tests/conftest.py` & `pkgmt-0.6.2/src/pkgmt/assets/template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/changelog.py` & `pkgmt-0.6.2/src/pkgmt/changelog.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/cli.py` & `pkgmt-0.6.2/src/pkgmt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,19 +158,35 @@
     try:
         dev.doc(Context(), clean=clean)
     except UnexpectedExit as e:
         raise SystemExit(f"Error running: {e.result.command}") from e
 
 
 @cli.command()
-def format():
+@click.option(
+    "-e",
+    "--exclude",
+    multiple=True,
+    default=[],
+    help="Exclude multiple files or dir from the build. Can also pass regex."
+    "Eg: -e tmp -e tmp/a.py -e tmp|src",
+)
+def format(exclude):
     """Run black on .py files and notebooks (.ipynb, .md)"""
-    formatting.format()
+    formatting.format(exclude)
 
 
 @cli.command()
-def lint():
+@click.argument("files", nargs=-1)
+@click.option(
+    "-e",
+    "--exclude",
+    multiple=True,
+    default=[],
+    help="Exclude multiple files or dir from the build" "Eg: -e tmp -e tmp/a.py",
+)
+def lint(files, exclude):
     """Lint .py files and notebooks (.ipynb, .md) with flake8"""
-    returncode = hook_._lint()
+    returncode = hook_._lint(files=files, exclude=exclude)
 
     if returncode:
         raise SystemExit("Error linting")
```

### Comparing `pkgmt-0.6.1/src/pkgmt/config.py` & `pkgmt-0.6.2/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/dependencies.py` & `pkgmt-0.6.2/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/deprecation.py` & `pkgmt-0.6.2/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/dev.py` & `pkgmt-0.6.2/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/fail_if_modified.py` & `pkgmt-0.6.2/src/pkgmt/fail_if_modified.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         "-b", "--base-branch", default="main", help="Base branch to compare against"
     )
     parser.add_argument(
         "-e",
         "--exclude-path",
         default=["doc"],
         nargs="+",
-        help="Path to exclude from git diff."
-        "Can be used multiple times eg: -e p1 -e p2",
+        help="Path to exclude from git diff." "Can be used multiple times eg: -e p1 p2",
     )
     parser.add_argument("--debug", action="store_true", help="Print debug info")
 
     args = parser.parse_args()
     returncode = check_modified(args.base_branch, args.exclude_path, debug=args.debug)
     sys.exit(returncode)
```

### Comparing `pkgmt-0.6.1/src/pkgmt/fail_if_not_modified.py` & `pkgmt-0.6.2/src/pkgmt/fail_if_not_modified.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     parser.add_argument(
         "-i",
         "--include-path",
         default=["CHANGELOG.md"],
         nargs="+",
         help="Path to include in git diff. "
         "Will fail if anyone of the path is not modified."
-        "Can be used multiple times eg: -i p1 -i p2",
+        "Can be used multiple times eg: -i p1 p2",
     )
     parser.add_argument("--debug", action="store_true", help="Print debug info")
 
     args = parser.parse_args()
     returncode = check_modified(args.base_branch, args.include_path, debug=args.debug)
     sys.exit(returncode)
```

### Comparing `pkgmt-0.6.1/src/pkgmt/formatting.py` & `pkgmt-0.6.2/src/pkgmt/formatting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 from pathlib import Path
 import sys
 import subprocess
+import click
 
 try:
     import jupytext
 except ModuleNotFoundError:
     jupytext = None
 
 
 try:
     import nbqa
 except ModuleNotFoundError:
     nbqa = None
+from shlex import quote
 
 
 def find_root():
     current = Path().resolve()
 
     while not (current / "pyproject.toml").exists():
         if current == current.parent:
-            sys.exit("Could not find project root.")
+            sys.exit(
+                (
+                    "Could not find project root."
+                    "Please add a pyproject.toml file in the root folder."
+                )
+            )
 
         current = current.parent
 
     return str(current)
 
 
-def format():
+def format(exclude):
     current = find_root()
 
-    print("Running: black .")
-    res = subprocess.run(["black", "."], cwd=current)
+    exclude_str = "|".join(exclude)
+
+    cmd = ["black", ".", "--extend-exclude", exclude_str]
+    click.echo("Running command:" + " ".join(map(quote, cmd)))
+    res = subprocess.run(cmd, cwd=current)
 
     error = False
 
     if res.returncode:
         error = True
 
     if not nbqa:
-        print(
+        click.echo(
             "nbqa is missing, black won't run on notebooks. "
             "Fix it with: pip install nbqa"
         )
 
     if not jupytext:
-        print(
+        click.echo(
             "jupytext is missing, black won't run on notebooks. "
             "Fix it with: pip install jupytext"
         )
 
     if nbqa and jupytext:
-        print("Running: nbqa black .")
-        res_nb = subprocess.run(["nbqa", "black", "."], cwd=current)
+        cmd = ["nbqa", "black", ".", "--extend-exclude", exclude_str]
+        click.echo("Running command:" + " ".join(map(quote, cmd)))
+        res_nb = subprocess.run(cmd, cwd=current)
 
         if res_nb.returncode:
             error = True
 
     if error:
-        print()
+        click.echo()
         sys.exit("***black returned errors.***")
 
-    print("Finished formatting with black!")
+    click.echo("Finished formatting with black!")
```

### Comparing `pkgmt-0.6.1/src/pkgmt/github.py` & `pkgmt-0.6.2/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/hook.py` & `pkgmt-0.6.2/src/pkgmt/hook.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,66 +18,83 @@
 
 
 def find_root():
     current = Path().resolve()
 
     while not (current / "pyproject.toml").exists():
         if current == current.parent:
-            sys.exit("Could not find project root.")
+            sys.exit(
+                (
+                    "Could not find project root."
+                    "Please add a pyproject.toml file in the root folder."
+                )
+            )
 
         current = current.parent
 
     return str(current)
 
 
 class Runner:
     def __init__(self, cwd) -> None:
         self._cwd = cwd
         self._errors = []
 
     def run(self, cmd, fix):
         cmd_ = " ".join(cmd)
         header = "=" * 20
-        print(f"{header} Running: {cmd_} {header}")
+        click.echo(f"{header} Running: {cmd_} {header}")
         res = subprocess.run(cmd, cwd=self._cwd)
 
         if res.returncode:
             self._errors.append((cmd_, fix))
 
     def check(self):
         if self._errors:
             for cmd, fix in self._errors:
-                print(f"The following command failed: {cmd}\\nTo fix it: {fix}")
+                click.echo(f"The following command failed: {cmd}\\nTo fix it: {fix}")
 
             return 1
         else:
-            print("All checks passed!")
+            click.echo("All checks passed!")
             return 0
 
 
-def _lint():
+def _lint(files=None, exclude=None):
+    if len(files) == 0:
+        files = ["."]
+    else:
+        files = list(files)
+
+    exclude_str_flake8 = ",".join(exclude)
+    exclude_str_black = "|".join(exclude)
+
+    cmd_black = ["black", "--check"] + files + ["--extend-exclude", exclude_str_black]
+    cmd_flake8 = ["flake8"] + files + ["--extend-exclude", exclude_str_flake8]
     runner = Runner(find_root())
-    runner.run(["flake8"], fix="Run: pkgmt format")
-    runner.run(["black", "--check", "."], fix="Run: pkgmt format")
+    runner.run(cmd_flake8, fix="Run: pkgmt format")
+    runner.run(cmd_black, fix="Run: pkgmt format")
 
     if not nbqa:
-        print(
+        click.echo(
             "nbqa is missing, flake8 won't run on notebooks. "
             "Fix it with: pip install nbqa"
         )
 
     if not jupytext:
-        print(
+        click.echo(
             "jupytext is missing, flake8 won't run on notebooks. "
             "Fix it with: pip install jupytext"
         )
 
     if nbqa and jupytext:
+        cmd = ["nbqa", "flake8"] + files + ["--extend-exclude", exclude_str_flake8]
         runner.run(
-            ["nbqa", "flake8", "."], fix="Install nbqa jupytext and run: pkgmt format"
+            cmd,
+            fix="Install nbqa jupytext and run: pkgmt format",
         )
 
     return runner.check()
 
 
 pre_push_hook = """\
 #!/usr/bin/env python3
```

### Comparing `pkgmt-0.6.1/src/pkgmt/links.py` & `pkgmt-0.6.2/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/new.py` & `pkgmt-0.6.2/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/test.py` & `pkgmt-0.6.2/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/versioneer.py` & `pkgmt-0.6.2/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/versioner/abstractversioner.py` & `pkgmt-0.6.2/src/pkgmt/versioner/abstractversioner.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,12 +184,15 @@
             start_new = f"{start_current}\n\n{new_header}"
             replace_in_file(self.path_to_changelog, start_current, start_new)
         else:
             print("No CHANGELOG.{rst,md} found, skipping changelog editing...")
 
     @abc.abstractmethod
     def find_package(self):
+        """Must return the package name and the path to the package root"""
         pass
 
     @abc.abstractmethod
     def version_file(self):
+        """Must return a path to the version file, relative to the package root (as
+        returned by find_package)"""
         pass
```

### Comparing `pkgmt-0.6.1/src/pkgmt/versioner/util.py` & `pkgmt-0.6.2/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt/versioner/versionernonsetup.py` & `pkgmt-0.6.2/src/pkgmt/versioner/versionernonsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class VersionerNonSetup(AbstractVersioner):
     def __init__(self, version_package, project_root="."):
         self.version_package = version_package
         super().__init__(project_root)
 
     def find_package(self):
-        for path, dirs, files in os.walk(self.project_root):
+        for path, dirs, _ in os.walk(self.project_root):
             if self.version_package in dirs:
                 PACKAGE = Path(path, self.version_package)
 
         package_name = self.version_package
         return package_name, PACKAGE
 
     def version_file(self):
```

### Comparing `pkgmt-0.6.1/src/pkgmt/versioner/versionersetup.py` & `pkgmt-0.6.2/src/pkgmt/versioner/versionersetup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.6.1/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.6.2/src/pkgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

