# Comparing `tmp/ebdtable2graph-0.1.8.tar.gz` & `tmp/ebdtable2graph-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebdtable2graph-0.1.8.tar", last modified: Thu Mar 23 08:30:15 2023, max compression
+gzip compressed data, was "ebdtable2graph-0.1.9.tar", last modified: Mon Mar 27 06:49:30 2023, max compression
```

## Comparing `ebdtable2graph-0.1.8.tar` & `ebdtable2graph-0.1.9.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.436143 ebdtable2graph-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.436143 ebdtable2graph-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-23 08:30:15.444142 ebdtable2graph-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/dev_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-coverage.in
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-coverage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-formatting.in
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-formatting.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-linting.in
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-linting.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-tests.in
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-type_check.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/dev_requirements/requirements-type_check.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/mwe_e0003.svg
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-23 08:30:15.444142 ebdtable2graph-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.436143 ebdtable2graph-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/src/ebdtable2graph/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/add_watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/graph_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/graphviz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/hochfrequenz-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/src/ebdtable2graph/models/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/models/ebd_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/models/ebd_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/src/ebdtable2graph/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 08:30:15.000000 ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:15.440142 ebdtable2graph-0.1.8/unittests/output/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003.dot
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003.puml
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003.puml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003_with_watermark.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0003_without_watermark.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0015.dot
--rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0015.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0015.puml
--rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0015.puml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0025.dot
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0025.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0025.puml
--rw-r--r--   0 runner    (1001) docker     (123)    16441 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0025.puml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0401.dot
--rw-r--r--   0 runner    (1001) docker     (123)    37183 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/output/E_0401.dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/test_ebd_table_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-03-23 08:30:07.000000 ebdtable2graph-0.1.8/unittests/test_table_to_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.688725 ebdtable2graph-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-27 06:49:30.688725 ebdtable2graph-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/dev_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-coverage.in
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-formatting.in
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-linting.in
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-linting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-type_check.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/mwe_e0003.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-27 06:49:30.688725 ebdtable2graph-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.680725 ebdtable2graph-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/src/ebdtable2graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/add_watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/graph_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/hochfrequenz-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/src/ebdtable2graph/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/models/ebd_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/models/ebd_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/src/ebdtable2graph/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 06:49:30.000000 ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.684725 ebdtable2graph-0.1.9/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:49:30.688725 ebdtable2graph-0.1.9/unittests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003.puml
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003.puml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003_with_background.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003_with_watermark.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003_with_watermark_background_is_False.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003_with_watermark_background_is_True.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0003_without_watermark.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0015.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    26366 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0015.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0015.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0015.puml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0025.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    13927 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0025.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0025.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    16441 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0025.puml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0401.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/output/E_0401.dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/test_ebd_table_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-03-27 06:49:24.000000 ebdtable2graph-0.1.9/unittests/test_table_to_graph.py
```

### Comparing `ebdtable2graph-0.1.8/.github/dependabot.yml` & `ebdtable2graph-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/coverage.yml` & `ebdtable2graph-0.1.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/formatting.yml` & `ebdtable2graph-0.1.9/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/packaging_test.yml` & `ebdtable2graph-0.1.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/python-publish.yml` & `ebdtable2graph-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/pythonlint.yml` & `ebdtable2graph-0.1.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.github/workflows/unittests.yml` & `ebdtable2graph-0.1.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.gitignore` & `ebdtable2graph-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/.pre-commit-config.yaml` & `ebdtable2graph-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/PKG-INFO` & `ebdtable2graph-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebdtable2graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Converts (already scraped) Entscheidungsbaumdiagramm tables to real graphs
 Home-page: https://github.com/Hochfrequenz/ebd_table_to_graph
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/ebd_table_to_graph
 Project-URL: Code, https://github.com/Hochfrequenz/ebd_table_to_graph
```

### Comparing `ebdtable2graph-0.1.8/README.md` & `ebdtable2graph-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/dev_requirements/requirements-linting.txt` & `ebdtable2graph-0.1.9/dev_requirements/requirements-linting.txt`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/mwe_e0003.svg` & `ebdtable2graph-0.1.9/mwe_e0003.svg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/requirements.txt` & `ebdtable2graph-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/setup.cfg` & `ebdtable2graph-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/graph_conversion.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/graph_conversion.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/graph_utils.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/graph_utils.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/graphviz.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/graphviz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains logic to convert EbdGraph data to dot code (Graphviz) and further to parse this code to SVG images.
 """
 from typing import List
 
 import requests
 
+from ebdtable2graph.add_watermark import add_background as add_background_function
 from ebdtable2graph.add_watermark import add_watermark as add_watermark_function
 from ebdtable2graph.graph_utils import _mark_last_common_ancestors
 from ebdtable2graph.models import (
     DecisionNode,
     EbdGraph,
     EbdGraphEdge,
     EndNode,
@@ -61,15 +62,15 @@
         f'<B>{ebd_graph.graph.nodes[node]["node"].result_code}</B><BR align="center"/>'
         f'<FONT point-size="12">'
         f'<U>Hinweis:</U><BR align="left"/>{_format_label(ebd_graph.graph.nodes[node]["node"].note)}<BR align="left"/>'
         f"</FONT>"
     )
     return (
         f'{indent}"{node}" '
-        f'[margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<{formatted_label}>];'
+        f'[margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<{formatted_label}>];'
     )
 
 
 def _convert_decision_node_to_dot(ebd_graph: EbdGraph, node: str, indent: str) -> str:
     """
     Convert a DecisionNode to dot code
     """
@@ -172,29 +173,31 @@
     assert "1" in nx_graph["Start"], "Start node must be connected to decision node '1'."
     dot_code += _convert_nodes_to_dot(ebd_graph, ADD_INDENT) + "\n\n"
     dot_code += "\n".join(_convert_edges_to_dot(ebd_graph, ADD_INDENT)) + "\n"
     dot_code += '\n    bgcolor="transparent";\n'
     return dot_code + "}"
 
 
-def convert_dot_to_svg_kroki(dot_code: str, add_watermark: bool = True) -> str:
+def convert_dot_to_svg_kroki(dot_code: str, add_watermark: bool = True, add_background: bool = True) -> str:
     """
     Converts dot code to svg (code) and returns the result as string. It uses kroki.io.
-    Then add the HF watermark to the svg code
+    Optionally add the HF watermark to the svg code, controlled by the argument 'add_watermark'
+    Optionally add a background with the color 'HF white', controlled by the argument 'add_background'
+    If 'add_background' is False, the background is transparent.
     """
     url = "https://kroki.io"
     answer = requests.post(
         url,
         json={"diagram_source": dot_code, "diagram_type": "graphviz", "output_format": "svg"},
         timeout=5,
     )
     if answer.status_code != 200:
         raise ValueError(
             f"Error while converting dot to svg: {answer.status_code}: {requests.codes[answer.status_code]}. "
             f"{answer.text}"
         )
+    svg_out = answer.text
     if add_watermark:
-        svg_code_without_watermark = answer.text
-        svg_out = add_watermark_function(svg_code_without_watermark.encode()).decode("utf-8")
-    else:
-        svg_out = answer.text
+        svg_out = add_watermark_function(svg_out)
+    if add_background:
+        svg_out = add_background_function(svg_out)
     return svg_out
```

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/hochfrequenz-logo.svg` & `ebdtable2graph-0.1.9/src/ebdtable2graph/hochfrequenz-logo.svg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/models/ebd_graph.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/models/ebd_graph.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/models/ebd_table.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/models/ebd_table.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph/plantuml.py` & `ebdtable2graph-0.1.9/src/ebdtable2graph/plantuml.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/PKG-INFO` & `ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebdtable2graph
-Version: 0.1.8
+Version: 0.1.9
 Summary: Converts (already scraped) Entscheidungsbaumdiagramm tables to real graphs
 Home-page: https://github.com/Hochfrequenz/ebd_table_to_graph
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/ebd_table_to_graph
 Project-URL: Code, https://github.com/Hochfrequenz/ebd_table_to_graph
```

### Comparing `ebdtable2graph-0.1.8/src/ebdtable2graph.egg-info/SOURCES.txt` & `ebdtable2graph-0.1.9/src/ebdtable2graph.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 unittests/examples.py
 unittests/test_ebd_table_models.py
 unittests/test_table_to_graph.py
 unittests/output/E_0003.dot
 unittests/output/E_0003.dot.svg
 unittests/output/E_0003.puml
 unittests/output/E_0003.puml.svg
+unittests/output/E_0003_with_background.dot.svg
 unittests/output/E_0003_with_watermark.dot.svg
+unittests/output/E_0003_with_watermark_background_is_False.dot.svg
+unittests/output/E_0003_with_watermark_background_is_True.dot.svg
 unittests/output/E_0003_without_watermark.dot.svg
 unittests/output/E_0015.dot
 unittests/output/E_0015.dot.svg
 unittests/output/E_0015.puml
 unittests/output/E_0015.puml.svg
 unittests/output/E_0025.dot
 unittests/output/E_0025.dot.svg
```

### Comparing `ebdtable2graph-0.1.8/tox.ini` & `ebdtable2graph-0.1.9/tox.ini`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/examples.py` & `ebdtable2graph-0.1.9/unittests/examples.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003.dot` & `ebdtable2graph-0.1.9/unittests/output/E_0025.dot`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 digraph D {
     labelloc="t";
-    label=<<B><FONT POINT-SIZE="18">7.39 AD: Bestellung der Aggregationsebene der Bilanzkreissummenzeitreihe auf Ebene der Regelzone</FONT></B><BR/><BR/><B><FONT POINT-SIZE="16">7.39.1 E_0003_Bestellung der Aggregationsebene RZ prüfen</FONT></B><BR/><BR/><BR/><BR/>>;
-    "Start" [margin="0.2,0.12", shape=box, style=filled, fillcolor="#7a8da1", label=<<B>E_0003</B><BR align="center"/><FONT point-size="12"><B><U>Prüfende Rolle:</U> ÜNB</B></FONT><BR align="center"/>>];
-    "1" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>1: </B>Erfolgt der Eingang der Bestellung fristgerecht?<BR align="left"/>>];
-    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Fristüberschreitung<BR align="left"/></FONT>>];
-    "2" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>2: </B>Erfolgt die Bestellung zum Monatsersten 00:00 Uhr?<BR align="left"/>>];
-    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Gewählter Zeitpunkt nicht zulässig<BR align="left"/></FONT>>];
+    label=<<B><FONT POINT-SIZE="18">7.41 AD: Übermittlung Prüfmitteilung für die Bilanzkreissummenzeitreihe vom BKV an BIKO und ÜNB</FONT></B><BR/><BR/><B><FONT POINT-SIZE="16">7.41.2 E_0025_Prüfmitteilung prüfen</FONT></B><BR/><BR/><BR/><BR/>>;
+    "Start" [margin="0.2,0.12", shape=box, style=filled, fillcolor="#7a8da1", label=<<B>E_0025</B><BR align="center"/><FONT point-size="12"><B><U>Prüfende Rolle:</U> BIKO</B></FONT><BR align="center"/>>];
+    "1" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>1: </B>Erfolgt der Eingang der Prüfmitteilung nach Ablauf der Clearingfrist für die KBKA?<BR align="left"/>>];
+    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Fristüberschreitung<BR align="left"/></FONT>>];
+    "2" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>2: </B>Befindet sich der MaBiS-ZP auf der Aggregationsebene RZ?<BR align="left"/>>];
+    "3" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>3: </B>Hat der BKV für den BK dieses MaBiS-ZP in diesem Bilanzie-<BR align="left"/>rungsmonat die Aggregationsebene RZ abbestellt?<BR align="left"/>>];
     "Ende" [margin="0.2,0.12", shape=box, style=filled, fillcolor="#7a8da1", label="Ende"];
+    "4" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>4: </B>Hat der BKV dem BIKO für diesen Bilanzierungsmonat bereits<BR align="left"/>mitgeteilt, dass die weiteren Prüfungen auf Ebene des BG<BR align="left"/>stattfinden müssen?<BR align="left"/>>];
+    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Falsche Aggregationsebene BG<BR align="left"/></FONT>>];
+    "5" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>5: </B>Hat der BKV dem BIKO für diesen Bilanzierungsmonat bereits<BR align="left"/>mitgeteilt, dass die weiteren Prüfungen auf Ebene des BG<BR align="left"/>stattfinden müssen?<BR align="left"/>>];
+    "A03" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A03</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Falsche Aggregationsebene RZ<BR align="left"/></FONT>>];
 
     "Start" -> "1";
-    "1" -> "A01" [label="Nein"];
-    "1" -> "2" [label="Ja"];
-    "2" -> "A02" [label="Nein"];
-    "2" -> "Ende" [label="Ja"];
+    "1" -> "A01" [label="Ja"];
+    "1" -> "2" [label="Nein"];
+    "2" -> "3" [label="Nein"];
+    "2" -> "5" [label="Ja"];
+    "3" -> "4" [label="Nein"];
+    "3" -> "Ende" [label="Ja"];
+    "4" -> "A02" [label="Nein"];
+    "4" -> "Ende" [label="Ja"];
+    "5" -> "A03" [label="Ja"];
+    "5" -> "Ende" [label="Nein"];
 
     bgcolor="transparent";
 }
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0003_with_watermark.dot.svg`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 00001240: 3233 392e 3537 2034 3034 2e35 2c2d 3234  239.57 404.5,-24
 00001250: 392e 3537 2034 3131 2e35 2c2d 3234 392e  9.57 411.5,-249.
 00001260: 3537 222f 3e0a 3c2f 673e 0a3c 212d 2d20  57"/>.</g>.<!-- 
 00001270: 4130 3120 2d2d 3e0a 3c67 2069 643d 226e  A01 -->.<g id="n
 00001280: 6f64 6533 2220 636c 6173 733d 226e 6f64  ode3" class="nod
 00001290: 6522 3e0a 3c74 6974 6c65 3e41 3031 3c2f  e">.<title>A01</
 000012a0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-000012b0: 6669 6c6c 3d22 2363 6361 3961 6222 2073  fill="#cca9ab" s
+000012b0: 6669 6c6c 3d22 2363 6662 3938 3622 2073  fill="#cfb986" s
 000012c0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
 000012d0: 696e 7473 3d22 3339 302e 352c 2d31 3531  ints="390.5,-151
 000012e0: 2032 3435 2e35 2c2d 3135 3120 3234 352e   245.5,-151 245.
 000012f0: 352c 2d31 3031 2033 3930 2e35 2c2d 3130  5,-101 390.5,-10
 00001300: 3120 3339 302e 352c 2d31 3531 222f 3e0a  1 390.5,-151"/>.
 00001310: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
 00001320: 723d 2273 7461 7274 2220 783d 2233 3032  r="start" x="302
@@ -416,15 +416,15 @@
 000019f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
 00001a00: 653d 2231 342e 3030 223e 4a61 3c2f 7465  e="14.00">Ja</te
 00001a10: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 4130  xt>.</g>.<!-- A0
 00001a20: 3220 2d2d 3e0a 3c67 2069 643d 226e 6f64  2 -->.<g id="nod
 00001a30: 6535 2220 636c 6173 733d 226e 6f64 6522  e5" class="node"
 00001a40: 3e0a 3c74 6974 6c65 3e41 3032 3c2f 7469  >.<title>A02</ti
 00001a50: 746c 653e 0a3c 706f 6c79 676f 6e20 6669  tle>.<polygon fi
-00001a60: 6c6c 3d22 2363 6361 3961 6222 2073 7472  ll="#cca9ab" str
+00001a60: 6c6c 3d22 2363 6662 3938 3622 2073 7472  ll="#cfb986" str
 00001a70: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
 00001a80: 7473 3d22 3635 362e 352c 2d35 3020 3432  ts="656.5,-50 42
 00001a90: 312e 352c 2d35 3020 3432 312e 352c 3020  1.5,-50 421.5,0 
 00001aa0: 3635 362e 352c 3020 3635 362e 352c 2d35  656.5,0 656.5,-5
 00001ab0: 3022 2f3e 0a3c 7465 7874 2074 6578 742d  0"/>.<text text-
 00001ac0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
 00001ad0: 3d22 3532 332e 3522 2079 3d22 2d33 332e  ="523.5" y="-33.
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003.puml` & `ebdtable2graph-0.1.9/unittests/output/E_0003.puml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003.puml.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0003.puml.svg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003_with_watermark.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0003_with_watermark_background_is_False.dot.svg`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 00001240: 3233 392e 3537 2034 3034 2e35 2c2d 3234  239.57 404.5,-24
 00001250: 392e 3537 2034 3131 2e35 2c2d 3234 392e  9.57 411.5,-249.
 00001260: 3537 222f 3e0a 3c2f 673e 0a3c 212d 2d20  57"/>.</g>.<!-- 
 00001270: 4130 3120 2d2d 3e0a 3c67 2069 643d 226e  A01 -->.<g id="n
 00001280: 6f64 6533 2220 636c 6173 733d 226e 6f64  ode3" class="nod
 00001290: 6522 3e0a 3c74 6974 6c65 3e41 3031 3c2f  e">.<title>A01</
 000012a0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-000012b0: 6669 6c6c 3d22 2363 6361 3961 6222 2073  fill="#cca9ab" s
+000012b0: 6669 6c6c 3d22 2363 6662 3938 3622 2073  fill="#cfb986" s
 000012c0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
 000012d0: 696e 7473 3d22 3339 302e 352c 2d31 3531  ints="390.5,-151
 000012e0: 2032 3435 2e35 2c2d 3135 3120 3234 352e   245.5,-151 245.
 000012f0: 352c 2d31 3031 2033 3930 2e35 2c2d 3130  5,-101 390.5,-10
 00001300: 3120 3339 302e 352c 2d31 3531 222f 3e0a  1 390.5,-151"/>.
 00001310: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
 00001320: 723d 2273 7461 7274 2220 783d 2233 3032  r="start" x="302
@@ -416,15 +416,15 @@
 000019f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
 00001a00: 653d 2231 342e 3030 223e 4a61 3c2f 7465  e="14.00">Ja</te
 00001a10: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 4130  xt>.</g>.<!-- A0
 00001a20: 3220 2d2d 3e0a 3c67 2069 643d 226e 6f64  2 -->.<g id="nod
 00001a30: 6535 2220 636c 6173 733d 226e 6f64 6522  e5" class="node"
 00001a40: 3e0a 3c74 6974 6c65 3e41 3032 3c2f 7469  >.<title>A02</ti
 00001a50: 746c 653e 0a3c 706f 6c79 676f 6e20 6669  tle>.<polygon fi
-00001a60: 6c6c 3d22 2363 6361 3961 6222 2073 7472  ll="#cca9ab" str
+00001a60: 6c6c 3d22 2363 6662 3938 3622 2073 7472  ll="#cfb986" str
 00001a70: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
 00001a80: 7473 3d22 3635 362e 352c 2d35 3020 3432  ts="656.5,-50 42
 00001a90: 312e 352c 2d35 3020 3432 312e 352c 3020  1.5,-50 421.5,0 
 00001aa0: 3635 362e 352c 3020 3635 362e 352c 2d35  656.5,0 656.5,-5
 00001ab0: 3022 2f3e 0a3c 7465 7874 2074 6578 742d  0"/>.<text text-
 00001ac0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
 00001ad0: 3d22 3532 332e 3522 2079 3d22 2d33 332e  ="523.5" y="-33.
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0003_without_watermark.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0003_without_watermark.dot.svg`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 00000920: 2034 3038 2c2d 3233 392e 3537 2034 3034   408,-239.57 404
 00000930: 2e35 2c2d 3234 392e 3537 2034 3131 2e35  .5,-249.57 411.5
 00000940: 2c2d 3234 392e 3537 222f 3e0a 3c2f 673e  ,-249.57"/>.</g>
 00000950: 0a3c 212d 2d20 4130 3120 2d2d 3e0a 3c67  .<!-- A01 -->.<g
 00000960: 2069 643d 226e 6f64 6533 2220 636c 6173   id="node3" clas
 00000970: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
 00000980: 3e41 3031 3c2f 7469 746c 653e 0a3c 706f  >A01</title>.<po
-00000990: 6c79 676f 6e20 6669 6c6c 3d22 2363 6361  lygon fill="#cca
-000009a0: 3961 6222 2073 7472 6f6b 653d 2262 6c61  9ab" stroke="bla
+00000990: 6c79 676f 6e20 6669 6c6c 3d22 2363 6662  lygon fill="#cfb
+000009a0: 3938 3622 2073 7472 6f6b 653d 2262 6c61  986" stroke="bla
 000009b0: 636b 2220 706f 696e 7473 3d22 3339 302e  ck" points="390.
 000009c0: 352c 2d31 3531 2032 3435 2e35 2c2d 3135  5,-151 245.5,-15
 000009d0: 3120 3234 352e 352c 2d31 3031 2033 3930  1 245.5,-101 390
 000009e0: 2e35 2c2d 3130 3120 3339 302e 352c 2d31  .5,-101 390.5,-1
 000009f0: 3531 222f 3e0a 3c74 6578 7420 7465 7874  51"/>.<text text
 00000a00: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
 00000a10: 783d 2233 3032 2e35 2220 793d 222d 3133  x="302.5" y="-13
@@ -271,15 +271,15 @@
 000010e0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
 000010f0: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
 00001100: 673e 0a3c 212d 2d20 4130 3220 2d2d 3e0a  g>.<!-- A02 -->.
 00001110: 3c67 2069 643d 226e 6f64 6535 2220 636c  <g id="node5" cl
 00001120: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
 00001130: 6c65 3e41 3032 3c2f 7469 746c 653e 0a3c  le>A02</title>.<
 00001140: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
-00001150: 6361 3961 6222 2073 7472 6f6b 653d 2262  ca9ab" stroke="b
+00001150: 6662 3938 3622 2073 7472 6f6b 653d 2262  fb986" stroke="b
 00001160: 6c61 636b 2220 706f 696e 7473 3d22 3635  lack" points="65
 00001170: 362e 352c 2d35 3020 3432 312e 352c 2d35  6.5,-50 421.5,-5
 00001180: 3020 3432 312e 352c 3020 3635 362e 352c  0 421.5,0 656.5,
 00001190: 3020 3635 362e 352c 2d35 3022 2f3e 0a3c  0 656.5,-50"/>.<
 000011a0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
 000011b0: 3d22 7374 6172 7422 2078 3d22 3532 332e  ="start" x="523.
 000011c0: 3522 2079 3d22 2d33 332e 3822 2066 6f6e  5" y="-33.8" fon
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0015.dot` & `ebdtable2graph-0.1.9/unittests/output/E_0015.dot`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 digraph D {
     labelloc="t";
     label=<<B><FONT POINT-SIZE="18">7.17 AD: Aktivierung eines MaBiS-ZP für Bilanzierungsgebietssummenzeitreihen vom ÜNB an BIKO und NB</FONT></B><BR/><BR/><B><FONT POINT-SIZE="16">7.17.1 E_0015_MaBiS-ZP Aktivierung prüfen</FONT></B><BR/><BR/><BR/><BR/>>;
     "Start" [margin="0.2,0.12", shape=box, style=filled, fillcolor="#7a8da1", label=<<B>E_0015</B><BR align="center"/><FONT point-size="12"><B><U>Prüfende Rolle:</U> BIKO</B></FONT><BR align="center"/>>];
     "1" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>1: </B>Erfolgt die Aktivierung nach Ablauf der Clearingfrist für die KBKA?<BR align="left"/>>];
-    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Fristüberschreitung<BR align="left"/></FONT>>];
+    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Fristüberschreitung<BR align="left"/></FONT>>];
     "2" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>2: </B>Erfolgt die Aktivierung zum Monatsersten 00:00 Uhr?<BR align="left"/>>];
-    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Gewählter Zeitpunkt nicht zulässig<BR align="left"/></FONT>>];
+    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Gewählter Zeitpunkt nicht zulässig<BR align="left"/></FONT>>];
     "3" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>3: </B>Ist die richtige Regelzone angegeben<BR align="left"/>>];
-    "A03" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A03</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Regelzone falsch<BR align="left"/></FONT>>];
+    "A03" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A03</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Regelzone falsch<BR align="left"/></FONT>>];
     "4" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>4: </B>Ist das Bilanzierungsgebiet zum Aktivierungsbeginn in der Regelzone des BIKO gültig?<BR align="left"/>>];
-    "A04" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A04</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Bilanzierungsgebiet nicht gültig<BR align="left"/></FONT>>];
+    "A04" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A04</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Bilanzierungsgebiet nicht gültig<BR align="left"/></FONT>>];
     "5" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>5: </B>Ist der ÜNB zum Aktivierungsbeginn für das Bilanzierungsgebiet zuständig?<BR align="left"/>>];
-    "A05" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A05</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Keine Berechtigung<BR align="left"/></FONT>>];
+    "A05" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A05</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Keine Berechtigung<BR align="left"/></FONT>>];
     "6" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>6: </B>Existiert bereits ein abweichendes Tupel unter der ID des MaBiS-ZP?<BR align="left"/>>];
-    "A06" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A06</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Abweichender MaBiS-ZP bereits vorhanden<BR align="left"/></FONT>>];
+    "A06" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A06</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Abweichender MaBiS-ZP bereits vorhanden<BR align="left"/></FONT>>];
     "7" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>7: </B>Existiert bereits für das genannte Tupel aus Aggregations-verantwortlicher, Bilanzierungsgebiet, Spannungsebene und ZRT eine abweichende ID des MaBiS-ZP?<BR align="left"/>>];
-    "A07" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A07</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Abweichende ID zum MaBiS-ZP bereits vorhanden<BR align="left"/></FONT>>];
+    "A07" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A07</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>Abweichende ID zum MaBiS-ZP bereits vorhanden<BR align="left"/></FONT>>];
     "8" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>8: </B>Ist der ÜNB zur Aktivierung des ZRT berechtigt?<BR align="left"/>>];
-    "A08" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A08</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>ZRT Aktivierung nicht berechtigt<BR align="left"/></FONT>>];
+    "A08" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A08</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>ZRT Aktivierung nicht berechtigt<BR align="left"/></FONT>>];
     "9" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>9: </B>Passt die OBIS-Kennzahl zum ZRT?<BR align="left"/>>];
-    "A09" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A09</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>OBIS nicht passend<BR align="left"/></FONT>>];
+    "A09" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A09</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>OBIS nicht passend<BR align="left"/></FONT>>];
     "10" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>10: </B>Ist der MaBiS-ZP zum Zeitpunkt der Aktivierung bereits aktiviert?<BR align="left"/>>];
-    "A10" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A10</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>MaBiS-ZP bereits aktiviert<BR align="left"/></FONT>>];
-    "A11" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A11</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Aktivierung durchgeführt<BR align="left"/></FONT>>];
+    "A10" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A10</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster Ablehnung<BR align="left"/>MaBiS-ZP bereits aktiviert<BR align="left"/></FONT>>];
+    "A11" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A11</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Aktivierung durchgeführt<BR align="left"/></FONT>>];
 
     "Start" -> "1";
     "1" -> "A01" [label="Ja"];
     "1" -> "2" [label="Nein"];
     "2" -> "A02" [label="Nein"];
     "2" -> "3" [label="Ja"];
     "3" -> "A03" [label="Nein"];
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0015.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0015.dot.svg`

 * *Files 2% similar despite different names*

```diff
@@ -9,1627 +9,1640 @@
 00000080: 3939 392f 786c 696e 6b22 2076 6572 7369  999/xlink" versi
 00000090: 6f6e 3d22 312e 3122 2077 6964 7468 3d22  on="1.1" width="
 000000a0: 3432 3537 2e33 3333 3333 3333 3333 3333  4257.33333333333
 000000b0: 3370 7822 2076 6965 7742 6f78 3d22 3020  3px" viewBox="0 
 000000c0: 3020 3432 3537 2e33 3333 3333 3333 3333  0 4257.333333333
 000000d0: 3333 3320 3138 3034 2e30 2220 6865 6967  333 1804.0" heig
 000000e0: 6874 3d22 3138 3034 2e30 7078 223e 0a20  ht="1804.0px">. 
-000000f0: 203c 673e 0a20 2020 203c 6720 7472 616e   <g>.    <g tran
-00000100: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00000110: 2831 3430 372e 3630 3139 3234 3637 3435  (1407.6019246745
-00000120: 3531 342c 2031 3830 2e33 3939 3939 3939  514, 180.3999999
-00000130: 3939 3939 3939 3529 2073 6361 6c65 2831  9999995) scale(1
-00000140: 2031 2920 7472 616e 736c 6174 6528 302c   1) translate(0,
-00000150: 2030 2920 7363 616c 6528 382e 3135 3837   0) scale(8.1587
-00000160: 3938 3939 3232 3235 3531 3220 382e 3135  98992225512 8.15
-00000170: 3837 3938 3939 3232 3235 3531 3229 2022  8798992225512) "
-00000180: 3e3c 736f 6469 706f 6469 3a6e 616d 6564  ><sodipodi:named
-00000190: 7669 6577 2078 6d6c 6e73 3a73 6f64 6970  view xmlns:sodip
-000001a0: 6f64 693d 2268 7474 703a 2f2f 736f 6469  odi="http://sodi
-000001b0: 706f 6469 2e73 6f75 7263 6566 6f72 6765  podi.sourceforge
-000001c0: 2e6e 6574 2f44 5444 2f73 6f64 6970 6f64  .net/DTD/sodipod
-000001d0: 692d 302e 6474 6422 2078 6d6c 6e73 3a69  i-0.dtd" xmlns:i
-000001e0: 6e6b 7363 6170 653d 2268 7474 703a 2f2f  nkscape="http://
-000001f0: 7777 772e 696e 6b73 6361 7065 2e6f 7267  www.inkscape.org
-00000200: 2f6e 616d 6573 7061 6365 732f 696e 6b73  /namespaces/inks
-00000210: 6361 7065 2220 6964 3d22 6e61 6d65 6476  cape" id="namedv
-00000220: 6965 7737 2220 7061 6765 636f 6c6f 723d  iew7" pagecolor=
-00000230: 2223 6666 6666 6666 2220 626f 7264 6572  "#ffffff" border
-00000240: 636f 6c6f 723d 2223 3939 3939 3939 2220  color="#999999" 
-00000250: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
-00000260: 2220 696e 6b73 6361 7065 3a70 6167 6573  " inkscape:pages
-00000270: 6861 646f 773d 2230 2220 696e 6b73 6361  hadow="0" inksca
-00000280: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
-00000290: 3022 2069 6e6b 7363 6170 653a 7061 6765  0" inkscape:page
-000002a0: 6368 6563 6b65 7262 6f61 7264 3d22 3022  checkerboard="0"
-000002b0: 2069 6e6b 7363 6170 653a 646f 6375 6d65   inkscape:docume
-000002c0: 6e74 2d75 6e69 7473 3d22 6d6d 2220 7368  nt-units="mm" sh
-000002d0: 6f77 6772 6964 3d22 6661 6c73 6522 2066  owgrid="false" f
-000002e0: 6974 2d6d 6172 6769 6e2d 746f 703d 2230  it-margin-top="0
-000002f0: 2220 6669 742d 6d61 7267 696e 2d6c 6566  " fit-margin-lef
-00000300: 743d 2230 2220 6669 742d 6d61 7267 696e  t="0" fit-margin
-00000310: 2d72 6967 6874 3d22 3022 2066 6974 2d6d  -right="0" fit-m
-00000320: 6172 6769 6e2d 626f 7474 6f6d 3d22 3022  argin-bottom="0"
-00000330: 2069 6e6b 7363 6170 653a 7a6f 6f6d 3d22   inkscape:zoom="
-00000340: 302e 3634 3035 3233 3239 2220 696e 6b73  0.64052329" inks
-00000350: 6361 7065 3a63 783d 2231 3330 2e33 3632  cape:cx="130.362
-00000360: 3136 2220 696e 6b73 6361 7065 3a63 793d  16" inkscape:cy=
-00000370: 2234 3132 2e31 3633 2220 696e 6b73 6361  "412.163" inksca
-00000380: 7065 3a77 696e 646f 772d 7769 6474 683d  pe:window-width=
-00000390: 2231 3531 3222 2069 6e6b 7363 6170 653a  "1512" inkscape:
-000003a0: 7769 6e64 6f77 2d68 6569 6768 743d 2239  window-height="9
-000003b0: 3136 2220 696e 6b73 6361 7065 3a77 696e  16" inkscape:win
-000003c0: 646f 772d 783d 2233 3834 3022 2069 6e6b  dow-x="3840" ink
-000003d0: 7363 6170 653a 7769 6e64 6f77 2d79 3d22  scape:window-y="
-000003e0: 3133 3622 2069 6e6b 7363 6170 653a 7769  136" inkscape:wi
-000003f0: 6e64 6f77 2d6d 6178 696d 697a 6564 3d22  ndow-maximized="
-00000400: 3022 2069 6e6b 7363 6170 653a 6375 7272  0" inkscape:curr
-00000410: 656e 742d 6c61 7965 723d 226c 6179 6572  ent-layer="layer
-00000420: 3122 2f3e 0a20 203c 6465 6673 2069 643d  1"/>.  <defs id=
-00000430: 2264 6566 7332 223e 0a20 2020 203c 636c  "defs2">.    <cl
-00000440: 6970 5061 7468 2063 6c69 7050 6174 6855  ipPath clipPathU
-00000450: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00000460: 6e55 7365 2220 6964 3d22 636c 6970 5061  nUse" id="clipPa
-00000470: 7468 3233 223e 0a20 2020 2020 203c 7061  th23">.      <pa
-00000480: 7468 2064 3d22 4d20 302c 3536 382e 3135  th d="M 0,568.15
-00000490: 3620 4820 3537 392e 3233 3620 5620 3020  6 H 579.236 V 0 
-000004a0: 4820 3020 5a22 2069 643d 2270 6174 6832  H 0 Z" id="path2
-000004b0: 3122 2f3e 0a20 2020 203c 2f63 6c69 7050  1"/>.    </clipP
-000004c0: 6174 683e 0a20 203c 2f64 6566 733e 0a20  ath>.  </defs>. 
-000004d0: 203c 6720 786d 6c6e 733a 696e 6b73 6361   <g xmlns:inksca
-000004e0: 7065 3d22 6874 7470 3a2f 2f77 7777 2e69  pe="http://www.i
-000004f0: 6e6b 7363 6170 652e 6f72 672f 6e61 6d65  nkscape.org/name
-00000500: 7370 6163 6573 2f69 6e6b 7363 6170 6522  spaces/inkscape"
-00000510: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
-00000520: 224c 6179 6572 2031 2220 696e 6b73 6361  "Layer 1" inksca
-00000530: 7065 3a67 726f 7570 6d6f 6465 3d22 6c61  pe:groupmode="la
-00000540: 7965 7222 2069 643d 226c 6179 6572 3122  yer" id="layer1"
-00000550: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00000560: 736c 6174 6528 2d31 362e 3534 3139 3337  slate(-16.541937
-00000570: 2c2d 3535 2e33 3035 3236 3729 223e 0a20  ,-55.305267)">. 
-00000580: 2020 203c 6720 6964 3d22 6731 3922 2063     <g id="g19" c
-00000590: 6c69 702d 7061 7468 3d22 7572 6c28 2363  lip-path="url(#c
-000005a0: 6c69 7050 6174 6832 3329 2220 7472 616e  lipPath23)" tran
-000005b0: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
-000005c0: 3335 3237 3737 3737 2c30 2c30 2c2d 302e  35277777,0,0,-0.
-000005d0: 3335 3237 3737 3737 2c30 2e30 3130 3137  35277777,0.01017
-000005e0: 3032 332c 3234 332e 3733 3637 3529 2220  023,243.73675)" 
-000005f0: 7374 796c 653d 226f 7061 6369 7479 3a30  style="opacity:0
-00000600: 2e32 223e 0a20 2020 2020 203c 6720 6964  .2">.      <g id
-00000610: 3d22 6732 3522 2074 7261 6e73 666f 726d  ="g25" transform
-00000620: 3d22 7472 616e 736c 6174 6528 3132 322e  ="translate(122.
-00000630: 3434 342c 3332 2e37 3139 3529 223e 0a20  444,32.7195)">. 
-00000640: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
-00000650: 6d20 302c 3020 6820 2d35 362e 3130 3420  m 0,0 h -56.104 
-00000660: 6320 2d31 312c 3020 2d31 392e 3839 382c  c -11,0 -19.898,
-00000670: 392e 3132 3320 2d31 392e 3436 332c 3230  9.123 -19.463,20
-00000680: 2e31 3135 2031 302e 3539 342c 3236 372e  .115 10.594,267.
-00000690: 3139 3120 3233 312e 3237 372c 3438 312e  191 231.277,481.
-000006a0: 3330 3220 3530 312e 3032 392c 3438 312e  302 501.029,481.
-000006b0: 3330 3220 7620 2d35 362e 3032 2063 2030  302 v -56.02 c 0
-000006c0: 2c2d 3130 2e39 3820 2d38 2e36 3838 2c2d  ,-10.98 -8.688,-
-000006d0: 3139 2e38 3932 202d 3139 2e36 3538 2c2d  19.892 -19.658,-
-000006e0: 3230 2e33 3933 2043 2031 3830 2e32 392c  20.393 C 180.29,
-000006f0: 3431 342e 3639 3720 302c 3232 382e 3030  414.697 0,228.00
-00000700: 3520 302c 3022 2073 7479 6c65 3d22 6669  5 0,0" style="fi
-00000710: 6c6c 3a23 3665 6164 3833 3b66 696c 6c2d  ll:#6ead83;fill-
-00000720: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
-00000730: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
-00000740: 6b65 3a6e 6f6e 6522 2069 643d 2270 6174  ke:none" id="pat
-00000750: 6832 3722 2f3e 0a20 2020 2020 203c 2f67  h27"/>.      </g
-00000760: 3e0a 2020 2020 2020 3c67 2069 643d 2267  >.      <g id="g
-00000770: 3239 2220 7472 616e 7366 6f72 6d3d 2274  29" transform="t
-00000780: 7261 6e73 6c61 7465 2832 3733 2e37 3832  ranslate(273.782
-00000790: 382c 3332 2e37 3139 3529 223e 0a20 2020  8,32.7195)">.   
-000007a0: 2020 2020 203c 7061 7468 2064 3d22 6d20       <path d="m 
-000007b0: 302c 3020 6820 2d35 352e 3932 3620 6320  0,0 h -55.926 c 
-000007c0: 2d31 312e 3232 382c 3020 2d32 302e 3039  -11.228,0 -20.09
-000007d0: 312c 392e 3438 3220 2d31 392e 3433 352c  1,9.482 -19.435,
-000007e0: 3230 2e36 3920 3130 2e37 3434 2c31 3833  20.69 10.744,183
-000007f0: 2e34 3339 2031 3633 2e33 3839 2c33 3239  .439 163.389,329
-00000800: 2e33 3838 2033 3439 2e34 3835 2c33 3239  .388 349.485,329
-00000810: 2e33 3838 2076 202d 3536 2e32 3633 2063  .388 v -56.263 c
-00000820: 2030 2c2d 3130 2e37 3039 202d 382e 3237   0,-10.709 -8.27
-00000830: 332c 2d31 392e 3631 3720 2d31 382e 3935  3,-19.617 -18.95
-00000840: 372c 2d32 302e 3335 2043 2031 3132 2e38  7,-20.35 C 112.8
-00000850: 3139 2c32 3633 2e36 3936 2030 2c31 3434  19,263.696 0,144
-00000860: 2e37 3734 2030 2c30 2220 7374 796c 653d  .774 0,0" style=
-00000870: 2266 696c 6c3a 2336 6561 6438 333b 6669  "fill:#6ead83;fi
-00000880: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
-00000890: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
-000008a0: 7472 6f6b 653a 6e6f 6e65 2220 6964 3d22  troke:none" id="
-000008b0: 7061 7468 3331 222f 3e0a 2020 2020 2020  path31"/>.      
-000008c0: 3c2f 673e 0a20 2020 2020 203c 6720 6964  </g>.      <g id
-000008d0: 3d22 6733 3322 2074 7261 6e73 666f 726d  ="g33" transform
-000008e0: 3d22 7472 616e 736c 6174 6528 3432 352e  ="translate(425.
-000008f0: 3736 3637 2c33 322e 3731 3935 2922 3e0a  7667,32.7195)">.
-00000900: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-00000910: 226d 2030 2c30 2068 202d 3535 2e34 3435  "m 0,0 h -55.445
-00000920: 2063 202d 3131 2e36 3533 2c30 202d 3230   c -11.653,0 -20
-00000930: 2e36 3034 2c31 302e 3137 202d 3139 2e33  .604,10.17 -19.3
-00000940: 3334 2c32 312e 3735 3320 3130 2e38 3636  34,21.753 10.866
-00000950: 2c39 392e 3033 3220 3935 2e30 3331 2c31  ,99.032 95.031,1
-00000960: 3736 2e33 3431 2031 3936 2e39 3139 2c31  76.341 196.919,1
-00000970: 3736 2e33 3431 2076 202d 3537 2e30 3131  76.341 v -57.011
-00000980: 2063 2030 2c2d 3130 2e30 3436 202d 372e   c 0,-10.046 -7.
-00000990: 3238 332c 2d31 382e 3735 3520 2d31 372e  283,-18.755 -17.
-000009a0: 3232 392c 2d32 302e 3136 3520 4320 3435  229,-20.165 C 45
-000009b0: 2e36 3838 2c31 3132 2e35 3232 2030 2c36  .688,112.522 0,6
-000009c0: 312e 3439 3720 302c 3022 2073 7479 6c65  1.497 0,0" style
-000009d0: 3d22 6669 6c6c 3a23 3665 6164 3833 3b66  ="fill:#6ead83;f
-000009e0: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
-000009f0: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-00000a00: 7374 726f 6b65 3a6e 6f6e 6522 2069 643d  stroke:none" id=
-00000a10: 2270 6174 6833 3522 2f3e 0a20 2020 2020  "path35"/>.     
-00000a20: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a20   </g>.    </g>. 
-00000a30: 203c 2f67 3e0a 3c2f 673e 0a20 2020 203c   </g>.</g>.    <
-00000a40: 7376 6720 7769 6474 683d 2233 3139 3370  svg width="3193p
-00000a50: 7422 2068 6569 6768 743d 2231 3335 3370  t" height="1353p
-00000a60: 7422 2076 6965 7742 6f78 3d22 302e 3030  t" viewBox="0.00
-00000a70: 2030 2e30 3020 3331 3932 2e35 3020 3133   0.00 3192.50 13
-00000a80: 3533 2e30 3022 3e0a 3c67 2069 643d 2267  53.00">.<g id="g
-00000a90: 7261 7068 3022 2063 6c61 7373 3d22 6772  raph0" class="gr
-00000aa0: 6170 6822 2074 7261 6e73 666f 726d 3d22  aph" transform="
-00000ab0: 7363 616c 6528 3120 3129 2072 6f74 6174  scale(1 1) rotat
-00000ac0: 6528 3029 2074 7261 6e73 6c61 7465 2834  e(0) translate(4
-00000ad0: 2031 3334 3929 223e 0a3c 7469 746c 653e   1349)">.<title>
-00000ae0: 443c 2f74 6974 6c65 3e0a 3c74 6578 7420  D</title>.<text 
-00000af0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00000b00: 7274 2220 783d 2231 3034 352e 3735 2220  rt" x="1045.75" 
-00000b10: 793d 222d 3133 3237 2e36 2220 666f 6e74  y="-1327.6" font
-00000b20: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00000b30: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-00000b40: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-00000b50: 7a65 3d22 3138 2e30 3022 3e37 2e31 3720  ze="18.00">7.17 
-00000b60: 4144 3a20 416b 7469 7669 6572 756e 6720  AD: Aktivierung 
-00000b70: 6569 6e65 7320 4d61 4269 532d 5a50 2066  eines MaBiS-ZP f
-00000b80: 2623 3235 323b 7220 4269 6c61 6e7a 6965  &#252;r Bilanzie
-00000b90: 7275 6e67 7367 6562 6965 7473 7375 6d6d  rungsgebietssumm
-00000ba0: 656e 7a65 6974 7265 6968 656e 2076 6f6d  enzeitreihen vom
-00000bb0: 2026 2332 3230 3b4e 4220 616e 2042 494b   &#220;NB an BIK
-00000bc0: 4f20 756e 6420 4e42 3c2f 7465 7874 3e0a  O und NB</text>.
-00000bd0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00000be0: 723d 2273 7461 7274 2220 783d 2231 3339  r="start" x="139
-00000bf0: 302e 3735 2220 793d 222d 3132 3937 2e32  0.75" y="-1297.2
-00000c00: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00000c10: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00000c20: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
-00000c30: 6f6e 742d 7369 7a65 3d22 3136 2e30 3022  ont-size="16.00"
-00000c40: 3e37 2e31 372e 3120 455f 3030 3135 5f4d  >7.17.1 E_0015_M
-00000c50: 6142 6953 2d5a 5020 416b 7469 7669 6572  aBiS-ZP Aktivier
-00000c60: 756e 6720 7072 2623 3235 323b 6665 6e3c  ung pr&#252;fen<
-00000c70: 2f74 6578 743e 0a3c 212d 2d20 5374 6172  /text>.<!-- Star
-00000c80: 7420 2d2d 3e0a 3c67 2069 643d 226e 6f64  t -->.<g id="nod
-00000c90: 6531 2220 636c 6173 733d 226e 6f64 6522  e1" class="node"
-00000ca0: 3e0a 3c74 6974 6c65 3e53 7461 7274 3c2f  >.<title>Start</
-00000cb0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-00000cc0: 6669 6c6c 3d22 2337 6138 6461 3122 2073  fill="#7a8da1" s
-00000cd0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00000ce0: 696e 7473 3d22 3335 322c 2d31 3234 3720  ints="352,-1247 
-00000cf0: 3137 372c 2d31 3234 3720 3137 372c 2d31  177,-1247 177,-1
-00000d00: 3230 3320 3335 322c 2d31 3230 3320 3335  203 352,-1203 35
-00000d10: 322c 2d31 3234 3722 2f3e 0a3c 7465 7874  2,-1247"/>.<text
-00000d20: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00000d30: 6172 7422 2078 3d22 3233 3622 2079 3d22  art" x="236" y="
-00000d40: 2d31 3232 372e 3822 2066 6f6e 742d 6661  -1227.8" font-fa
-00000d50: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00000d60: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-00000d70: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-00000d80: 2231 342e 3030 223e 455f 3030 3135 3c2f  "14.00">E_0015</
-00000d90: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00000da0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00000db0: 783d 2231 3931 2220 793d 222d 3132 3135  x="191" y="-1215
-00000dc0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
-00000dd0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00000de0: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-00000df0: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
-00000e00: 3d22 756e 6465 726c 696e 6522 2066 6f6e  ="underline" fon
-00000e10: 742d 7369 7a65 3d22 3132 2e30 3022 3e50  t-size="12.00">P
-00000e20: 7226 2332 3532 3b66 656e 6465 2052 6f6c  r&#252;fende Rol
-00000e30: 6c65 3a3c 2f74 6578 743e 0a3c 7465 7874  le:</text>.<text
-00000e40: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00000e50: 6172 7422 2078 3d22 3239 3722 2079 3d22  art" x="297" y="
-00000e60: 2d31 3231 352e 3422 2066 6f6e 742d 6661  -1215.4" font-fa
-00000e70: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00000e80: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-00000e90: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-00000ea0: 2231 322e 3030 223e 2042 494b 4f3c 2f74  "12.00"> BIKO</t
-00000eb0: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2031  ext>.</g>.<!-- 1
-00000ec0: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
-00000ed0: 3222 2063 6c61 7373 3d22 6e6f 6465 223e  2" class="node">
-00000ee0: 0a3c 7469 746c 653e 313c 2f74 6974 6c65  .<title>1</title
-00000ef0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
-00000f00: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
-00000f10: 6c61 636b 2220 643d 224d 3531 372c 2d31  lack" d="M517,-1
-00000f20: 3136 3643 3531 372c 2d31 3136 3620 3132  166C517,-1166 12
-00000f30: 2c2d 3131 3636 2031 322c 2d31 3136 3620  ,-1166 12,-1166 
-00000f40: 362c 2d31 3136 3620 302c 2d31 3136 3020  6,-1166 0,-1160 
-00000f50: 302c 2d31 3135 3420 302c 2d31 3135 3420  0,-1154 0,-1154 
-00000f60: 302c 2d31 3134 3220 302c 2d31 3134 3220  0,-1142 0,-1142 
-00000f70: 302c 2d31 3133 3620 362c 2d31 3133 3020  0,-1136 6,-1130 
-00000f80: 3132 2c2d 3131 3330 2031 322c 2d31 3133  12,-1130 12,-113
-00000f90: 3020 3531 372c 2d31 3133 3020 3531 372c  0 517,-1130 517,
-00000fa0: 2d31 3133 3020 3532 332c 2d31 3133 3020  -1130 523,-1130 
-00000fb0: 3532 392c 2d31 3133 3620 3532 392c 2d31  529,-1136 529,-1
-00000fc0: 3134 3220 3532 392c 2d31 3134 3220 3532  142 529,-1142 52
-00000fd0: 392c 2d31 3135 3420 3532 392c 2d31 3135  9,-1154 529,-115
-00000fe0: 3420 3532 392c 2d31 3136 3020 3532 332c  4 529,-1160 523,
-00000ff0: 2d31 3136 3620 3531 372c 2d31 3136 3622  -1166 517,-1166"
-00001000: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
-00001010: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00001020: 3134 2220 793d 222d 3131 3435 2e33 2220  14" y="-1145.3" 
-00001030: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00001040: 6573 2c73 6572 6966 2220 666f 6e74 2d77  es,serif" font-w
-00001050: 6569 6768 743d 2262 6f6c 6422 2066 6f6e  eight="bold" fon
-00001060: 742d 7369 7a65 3d22 3134 2e30 3022 3e31  t-size="14.00">1
-00001070: 3a20 3c2f 7465 7874 3e0a 3c74 6578 7420  : </text>.<text 
-00001080: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00001090: 7274 2220 783d 2233 3422 2079 3d22 2d31  rt" x="34" y="-1
-000010a0: 3134 352e 3322 2066 6f6e 742d 6661 6d69  145.3" font-fami
-000010b0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-000010c0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-000010d0: 3022 3e45 7266 6f6c 6774 2064 6965 2041  0">Erfolgt die A
-000010e0: 6b74 6976 6965 7275 6e67 206e 6163 6820  ktivierung nach 
-000010f0: 4162 6c61 7566 2064 6572 2043 6c65 6172  Ablauf der Clear
-00001100: 696e 6766 7269 7374 2066 2623 3235 323b  ingfrist f&#252;
-00001110: 7220 6469 6520 4b42 4b41 3f3c 2f74 6578  r die KBKA?</tex
-00001120: 743e 0a3c 2f67 3e0a 3c21 2d2d 2053 7461  t>.</g>.<!-- Sta
-00001130: 7274 2623 3435 3b26 6774 3b31 202d 2d3e  rt&#45;&gt;1 -->
-00001140: 0a3c 6720 6964 3d22 6564 6765 3122 2063  .<g id="edge1" c
-00001150: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00001160: 746c 653e 5374 6172 742d 2667 743b 313c  tle>Start-&gt;1<
-00001170: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00001180: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00001190: 3d22 626c 6163 6b22 2064 3d22 4d32 3634  ="black" d="M264
-000011a0: 2e35 2c2d 3132 3032 2e37 3143 3236 342e  .5,-1202.71C264.
-000011b0: 352c 2d31 3139 342e 3832 2032 3634 2e35  5,-1194.82 264.5
-000011c0: 2c2d 3131 3835 2e37 3520 3236 342e 352c  ,-1185.75 264.5,
-000011d0: 2d31 3137 372e 3333 222f 3e0a 3c70 6f6c  -1177.33"/>.<pol
-000011e0: 7967 6f6e 2066 696c 6c3d 2262 6c61 636b  ygon fill="black
-000011f0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00001200: 2070 6f69 6e74 733d 2232 3638 2c2d 3131   points="268,-11
-00001210: 3737 2e35 3720 3236 342e 352c 2d31 3136  77.57 264.5,-116
-00001220: 372e 3537 2032 3631 2c2d 3131 3737 2e35  7.57 261,-1177.5
-00001230: 3720 3236 382c 2d31 3137 372e 3537 222f  7 268,-1177.57"/
-00001240: 3e0a 3c2f 673e 0a3c 212d 2d20 4130 3120  >.</g>.<!-- A01 
-00001250: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6533  -->.<g id="node3
-00001260: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
-00001270: 3c74 6974 6c65 3e41 3031 3c2f 7469 746c  <title>A01</titl
-00001280: 653e 0a3c 706f 6c79 676f 6e20 6669 6c6c  e>.<polygon fill
-00001290: 3d22 2363 6361 3961 6222 2073 7472 6f6b  ="#cca9ab" strok
-000012a0: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-000012b0: 3d22 3331 392c 2d31 3037 3920 3137 342c  ="319,-1079 174,
-000012c0: 2d31 3037 3920 3137 342c 2d31 3031 3720  -1079 174,-1017 
-000012d0: 3331 392c 2d31 3031 3720 3331 392c 2d31  319,-1017 319,-1
-000012e0: 3037 3922 2f3e 0a3c 7465 7874 2074 6578  079"/>.<text tex
-000012f0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00001300: 2078 3d22 3233 3122 2079 3d22 2d31 3036   x="231" y="-106
-00001310: 322e 3822 2066 6f6e 742d 6661 6d69 6c79  2.8" font-family
-00001320: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00001330: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
-00001340: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00001350: 3030 223e 4130 313c 2f74 6578 743e 0a3c  00">A01</text>.<
-00001360: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00001370: 3d22 7374 6172 7422 2078 3d22 3138 3622  ="start" x="186"
-00001380: 2079 3d22 2d31 3035 302e 3422 2066 6f6e   y="-1050.4" fon
-00001390: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000013a0: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
-000013b0: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
-000013c0: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
-000013d0: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
-000013e0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-000013f0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00001400: 3d22 3138 3622 2079 3d22 2d31 3033 382e  ="186" y="-1038.
-00001410: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-00001420: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00001430: 742d 7369 7a65 3d22 3132 2e30 3022 3e43  t-size="12.00">C
-00001440: 6c75 7374 6572 2041 626c 6568 6e75 6e67  luster Ablehnung
-00001450: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00001460: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00001470: 2220 783d 2231 3836 2220 793d 222d 3130  " x="186" y="-10
-00001480: 3236 2e34 2220 666f 6e74 2d66 616d 696c  26.4" font-famil
-00001490: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-000014a0: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-000014b0: 223e 4672 6973 7426 2332 3532 3b62 6572  ">Frist&#252;ber
-000014c0: 7363 6872 6569 7475 6e67 3c2f 7465 7874  schreitung</text
-000014d0: 3e0a 3c2f 673e 0a3c 212d 2d20 3126 2334  >.</g>.<!-- 1&#4
-000014e0: 353b 2667 743b 4130 3120 2d2d 3e0a 3c67  5;&gt;A01 -->.<g
-000014f0: 2069 643d 2265 6467 6532 2220 636c 6173   id="edge2" clas
-00001500: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-00001510: 3e31 2d26 6774 3b41 3031 3c2f 7469 746c  >1-&gt;A01</titl
-00001520: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
-00001530: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
-00001540: 636b 2220 643d 224d 3236 312e 3336 2c2d  ck" d="M261.36,-
-00001550: 3131 3239 2e39 3343 3235 392e 3337 2c2d  1129.93C259.37,-
-00001560: 3131 3139 2e30 3520 3235 362e 3638 2c2d  1119.05 256.68,-
-00001570: 3131 3034 2e34 3420 3235 342e 3135 2c2d  1104.44 254.15,-
-00001580: 3130 3930 2e36 3422 2f3e 0a3c 706f 6c79  1090.64"/>.<poly
-00001590: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-000015a0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-000015b0: 706f 696e 7473 3d22 3235 372e 3539 2c2d  points="257.59,-
-000015c0: 3130 3930 2e30 3220 3235 322e 3334 2c2d  1090.02 252.34,-
-000015d0: 3130 3830 2e38 3220 3235 302e 3731 2c2d  1080.82 250.71,-
-000015e0: 3130 3931 2e32 3820 3235 372e 3539 2c2d  1091.28 257.59,-
-000015f0: 3130 3930 2e30 3222 2f3e 0a3c 7465 7874  1090.02"/>.<text
-00001600: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00001610: 6464 6c65 2220 783d 2232 3635 2e35 2220  ddle" x="265.5" 
-00001620: 793d 222d 3131 3030 2e38 2220 666f 6e74  y="-1100.8" font
-00001630: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00001640: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00001650: 2231 342e 3030 223e 4a61 3c2f 7465 7874  "14.00">Ja</text
-00001660: 3e0a 3c2f 673e 0a3c 212d 2d20 3220 2d2d  >.</g>.<!-- 2 --
-00001670: 3e0a 3c67 2069 643d 226e 6f64 6534 2220  >.<g id="node4" 
-00001680: 636c 6173 733d 226e 6f64 6522 3e0a 3c74  class="node">.<t
-00001690: 6974 6c65 3e32 3c2f 7469 746c 653e 0a3c  itle>2</title>.<
-000016a0: 7061 7468 2066 696c 6c3d 2223 3761 6162  path fill="#7aab
-000016b0: 3861 2220 7374 726f 6b65 3d22 626c 6163  8a" stroke="blac
-000016c0: 6b22 2064 3d22 4d37 3631 2e35 2c2d 3130  k" d="M761.5,-10
-000016d0: 3636 4337 3631 2e35 2c2d 3130 3636 2033  66C761.5,-1066 3
-000016e0: 3439 2e35 2c2d 3130 3636 2033 3439 2e35  49.5,-1066 349.5
-000016f0: 2c2d 3130 3636 2033 3433 2e35 2c2d 3130  ,-1066 343.5,-10
-00001700: 3636 2033 3337 2e35 2c2d 3130 3630 2033  66 337.5,-1060 3
-00001710: 3337 2e35 2c2d 3130 3534 2033 3337 2e35  37.5,-1054 337.5
-00001720: 2c2d 3130 3534 2033 3337 2e35 2c2d 3130  ,-1054 337.5,-10
-00001730: 3432 2033 3337 2e35 2c2d 3130 3432 2033  42 337.5,-1042 3
-00001740: 3337 2e35 2c2d 3130 3336 2033 3433 2e35  37.5,-1036 343.5
-00001750: 2c2d 3130 3330 2033 3439 2e35 2c2d 3130  ,-1030 349.5,-10
-00001760: 3330 2033 3439 2e35 2c2d 3130 3330 2037  30 349.5,-1030 7
-00001770: 3631 2e35 2c2d 3130 3330 2037 3631 2e35  61.5,-1030 761.5
-00001780: 2c2d 3130 3330 2037 3637 2e35 2c2d 3130  ,-1030 767.5,-10
-00001790: 3330 2037 3733 2e35 2c2d 3130 3336 2037  30 773.5,-1036 7
-000017a0: 3733 2e35 2c2d 3130 3432 2037 3733 2e35  73.5,-1042 773.5
-000017b0: 2c2d 3130 3432 2037 3733 2e35 2c2d 3130  ,-1042 773.5,-10
-000017c0: 3534 2037 3733 2e35 2c2d 3130 3534 2037  54 773.5,-1054 7
-000017d0: 3733 2e35 2c2d 3130 3630 2037 3637 2e35  73.5,-1060 767.5
-000017e0: 2c2d 3130 3636 2037 3631 2e35 2c2d 3130  ,-1066 761.5,-10
-000017f0: 3636 222f 3e0a 3c74 6578 7420 7465 7874  66"/>.<text text
-00001800: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00001810: 783d 2233 3531 2e35 2220 793d 222d 3130  x="351.5" y="-10
-00001820: 3435 2e33 2220 666f 6e74 2d66 616d 696c  45.3" font-famil
-00001830: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00001840: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
-00001850: 6422 2066 6f6e 742d 7369 7a65 3d22 3134  d" font-size="14
-00001860: 2e30 3022 3e32 3a20 3c2f 7465 7874 3e0a  .00">2: </text>.
-00001870: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00001880: 723d 2273 7461 7274 2220 783d 2233 3731  r="start" x="371
-00001890: 2e35 2220 793d 222d 3130 3435 2e33 2220  .5" y="-1045.3" 
-000018a0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000018b0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-000018c0: 697a 653d 2231 342e 3030 223e 4572 666f  ize="14.00">Erfo
-000018d0: 6c67 7420 6469 6520 416b 7469 7669 6572  lgt die Aktivier
-000018e0: 756e 6720 7a75 6d20 4d6f 6e61 7473 6572  ung zum Monatser
-000018f0: 7374 656e 2030 303a 3030 2055 6872 3f3c  sten 00:00 Uhr?<
-00001900: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
-00001910: 2031 2623 3435 3b26 6774 3b32 202d 2d3e   1&#45;&gt;2 -->
-00001920: 0a3c 6720 6964 3d22 6564 6765 3322 2063  .<g id="edge3" c
-00001930: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00001940: 746c 653e 312d 2667 743b 323c 2f74 6974  tle>1-&gt;2</tit
-00001950: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-00001960: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00001970: 6163 6b22 2064 3d22 4d33 3136 2e31 392c  ack" d="M316.19,
-00001980: 2d31 3132 392e 3539 4333 3635 2e35 392c  -1129.59C365.59,
-00001990: 2d31 3131 322e 3936 2034 3430 2e31 352c  -1112.96 440.15,
-000019a0: 2d31 3038 372e 3835 2034 3932 2e39 2c2d  -1087.85 492.9,-
-000019b0: 3130 3730 2e30 3822 2f3e 0a3c 706f 6c79  1070.08"/>.<poly
-000019c0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-000019d0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-000019e0: 706f 696e 7473 3d22 3439 342e 3031 2c2d  points="494.01,-
-000019f0: 3130 3733 2e34 2035 3032 2e33 372c 2d31  1073.4 502.37,-1
-00001a00: 3036 362e 3839 2034 3931 2e37 372c 2d31  066.89 491.77,-1
-00001a10: 3036 362e 3737 2034 3934 2e30 312c 2d31  066.77 494.01,-1
-00001a20: 3037 332e 3422 2f3e 0a3c 7465 7874 2074  073.4"/>.<text t
-00001a30: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00001a40: 6c65 2220 783d 2234 3237 2e35 2220 793d  le" x="427.5" y=
-00001a50: 222d 3131 3030 2e38 2220 666f 6e74 2d66  "-1100.8" font-f
-00001a60: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00001a70: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00001a80: 342e 3030 223e 4e65 696e 3c2f 7465 7874  4.00">Nein</text
-00001a90: 3e0a 3c2f 673e 0a3c 212d 2d20 4130 3220  >.</g>.<!-- A02 
-00001aa0: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6535  -->.<g id="node5
-00001ab0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
-00001ac0: 3c74 6974 6c65 3e41 3032 3c2f 7469 746c  <title>A02</titl
-00001ad0: 653e 0a3c 706f 6c79 676f 6e20 6669 6c6c  e>.<polygon fill
-00001ae0: 3d22 2363 6361 3961 6222 2073 7472 6f6b  ="#cca9ab" strok
-00001af0: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-00001b00: 3d22 3538 352c 2d39 3636 2033 3530 2c2d  ="585,-966 350,-
-00001b10: 3936 3620 3335 302c 2d39 3034 2035 3835  966 350,-904 585
-00001b20: 2c2d 3930 3420 3538 352c 2d39 3636 222f  ,-904 585,-966"/
-00001b30: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00001b40: 686f 723d 2273 7461 7274 2220 783d 2234  hor="start" x="4
-00001b50: 3532 2220 793d 222d 3934 392e 3822 2066  52" y="-949.8" f
-00001b60: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001b70: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00001b80: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00001b90: 2d73 697a 653d 2231 342e 3030 223e 4130  -size="14.00">A0
-00001ba0: 323c 2f74 6578 743e 0a3c 7465 7874 2074  2</text>.<text t
-00001bb0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00001bc0: 7422 2078 3d22 3336 3222 2079 3d22 2d39  t" x="362" y="-9
-00001bd0: 3337 2e34 2220 666f 6e74 2d66 616d 696c  37.4" font-famil
-00001be0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00001bf0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00001c00: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
-00001c10: 2d73 697a 653d 2231 322e 3030 223e 4869  -size="12.00">Hi
-00001c20: 6e77 6569 733a 3c2f 7465 7874 3e0a 3c74  nweis:</text>.<t
-00001c30: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00001c40: 2273 7461 7274 2220 783d 2233 3632 2220  "start" x="362" 
-00001c50: 793d 222d 3932 352e 3422 2066 6f6e 742d  y="-925.4" font-
-00001c60: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00001c70: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00001c80: 3132 2e30 3022 3e43 6c75 7374 6572 2041  12.00">Cluster A
-00001c90: 626c 6568 6e75 6e67 3c2f 7465 7874 3e0a  blehnung</text>.
-00001ca0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00001cb0: 723d 2273 7461 7274 2220 783d 2233 3632  r="start" x="362
-00001cc0: 2220 793d 222d 3931 332e 3422 2066 6f6e  " y="-913.4" fon
-00001cd0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00001ce0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00001cf0: 3d22 3132 2e30 3022 3e47 6577 2623 3232  ="12.00">Gew&#22
-00001d00: 383b 686c 7465 7220 5a65 6974 7075 6e6b  8;hlter Zeitpunk
-00001d10: 7420 6e69 6368 7420 7a75 6c26 2332 3238  t nicht zul&#228
-00001d20: 3b73 7369 673c 2f74 6578 743e 0a3c 2f67  ;ssig</text>.</g
-00001d30: 3e0a 3c21 2d2d 2032 2623 3435 3b26 6774  >.<!-- 2&#45;&gt
-00001d40: 3b41 3032 202d 2d3e 0a3c 6720 6964 3d22  ;A02 -->.<g id="
-00001d50: 6564 6765 3422 2063 6c61 7373 3d22 6564  edge4" class="ed
-00001d60: 6765 223e 0a3c 7469 746c 653e 322d 2667  ge">.<title>2-&g
-00001d70: 743b 4130 323c 2f74 6974 6c65 3e0a 3c70  t;A02</title>.<p
-00001d80: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
-00001d90: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
-00001da0: 3d22 4d35 3431 2e37 352c 2d31 3032 392e  ="M541.75,-1029.
-00001db0: 3636 4335 3330 2e32 2c2d 3130 3135 2e30  66C530.2,-1015.0
-00001dc0: 3920 3531 332e 3236 2c2d 3939 332e 3732  9 513.26,-993.72
-00001dd0: 2034 3938 2e34 382c 2d39 3735 2e30 3822   498.48,-975.08"
-00001de0: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
-00001df0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00001e00: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00001e10: 3530 312e 3333 2c2d 3937 332e 3033 2034  501.33,-973.03 4
-00001e20: 3932 2e33 372c 2d39 3637 2e33 3720 3439  92.37,-967.37 49
-00001e30: 352e 3834 2c2d 3937 372e 3338 2035 3031  5.84,-977.38 501
-00001e40: 2e33 332c 2d39 3733 2e30 3322 2f3e 0a3c  .33,-973.03"/>.<
-00001e50: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00001e60: 3d22 6d69 6464 6c65 2220 783d 2235 3334  ="middle" x="534
-00001e70: 2e35 2220 793d 222d 3938 372e 3822 2066  .5" y="-987.8" f
-00001e80: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001e90: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00001ea0: 7a65 3d22 3134 2e30 3022 3e4e 6569 6e3c  ze="14.00">Nein<
-00001eb0: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
-00001ec0: 2033 202d 2d3e 0a3c 6720 6964 3d22 6e6f   3 -->.<g id="no
-00001ed0: 6465 3622 2063 6c61 7373 3d22 6e6f 6465  de6" class="node
-00001ee0: 223e 0a3c 7469 746c 653e 333c 2f74 6974  ">.<title>3</tit
-00001ef0: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-00001f00: 2337 6161 6238 6122 2073 7472 6f6b 653d  #7aab8a" stroke=
-00001f10: 2262 6c61 636b 2220 643d 224d 3930 352e  "black" d="M905.
-00001f20: 352c 2d39 3533 4339 3035 2e35 2c2d 3935  5,-953C905.5,-95
-00001f30: 3320 3631 352e 352c 2d39 3533 2036 3135  3 615.5,-953 615
-00001f40: 2e35 2c2d 3935 3320 3630 392e 352c 2d39  .5,-953 609.5,-9
-00001f50: 3533 2036 3033 2e35 2c2d 3934 3720 3630  53 603.5,-947 60
-00001f60: 332e 352c 2d39 3431 2036 3033 2e35 2c2d  3.5,-941 603.5,-
-00001f70: 3934 3120 3630 332e 352c 2d39 3239 2036  941 603.5,-929 6
-00001f80: 3033 2e35 2c2d 3932 3920 3630 332e 352c  03.5,-929 603.5,
-00001f90: 2d39 3233 2036 3039 2e35 2c2d 3931 3720  -923 609.5,-917 
-00001fa0: 3631 352e 352c 2d39 3137 2036 3135 2e35  615.5,-917 615.5
-00001fb0: 2c2d 3931 3720 3930 352e 352c 2d39 3137  ,-917 905.5,-917
-00001fc0: 2039 3035 2e35 2c2d 3931 3720 3931 312e   905.5,-917 911.
-00001fd0: 352c 2d39 3137 2039 3137 2e35 2c2d 3932  5,-917 917.5,-92
-00001fe0: 3320 3931 372e 352c 2d39 3239 2039 3137  3 917.5,-929 917
-00001ff0: 2e35 2c2d 3932 3920 3931 372e 352c 2d39  .5,-929 917.5,-9
-00002000: 3431 2039 3137 2e35 2c2d 3934 3120 3931  41 917.5,-941 91
-00002010: 372e 352c 2d39 3437 2039 3131 2e35 2c2d  7.5,-947 911.5,-
-00002020: 3935 3320 3930 352e 352c 2d39 3533 222f  953 905.5,-953"/
-00002030: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00002040: 686f 723d 2273 7461 7274 2220 783d 2236  hor="start" x="6
-00002050: 3137 2e35 2220 793d 222d 3933 322e 3322  17.5" y="-932.3"
-00002060: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00002070: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00002080: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
-00002090: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000020a0: 333a 203c 2f74 6578 743e 0a3c 7465 7874  3: </text>.<text
-000020b0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-000020c0: 6172 7422 2078 3d22 3633 372e 3522 2079  art" x="637.5" y
-000020d0: 3d22 2d39 3332 2e33 2220 666f 6e74 2d66  ="-932.3" font-f
-000020e0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-000020f0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00002100: 342e 3030 223e 4973 7420 6469 6520 7269  4.00">Ist die ri
-00002110: 6368 7469 6765 2052 6567 656c 7a6f 6e65  chtige Regelzone
-00002120: 2061 6e67 6567 6562 656e 3c2f 7465 7874   angegeben</text
-00002130: 3e0a 3c2f 673e 0a3c 212d 2d20 3226 2334  >.</g>.<!-- 2&#4
-00002140: 353b 2667 743b 3320 2d2d 3e0a 3c67 2069  5;&gt;3 -->.<g i
-00002150: 643d 2265 6467 6535 2220 636c 6173 733d  d="edge5" class=
-00002160: 2265 6467 6522 3e0a 3c74 6974 6c65 3e32  "edge">.<title>2
-00002170: 2d26 6774 3b33 3c2f 7469 746c 653e 0a3c  -&gt;3</title>.<
-00002180: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
-00002190: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-000021a0: 643d 224d 3538 372e 3533 2c2d 3130 3239  d="M587.53,-1029
-000021b0: 2e36 3643 3632 322e 3738 2c2d 3130 3130  .66C622.78,-1010
-000021c0: 2e35 3720 3637 392e 3538 2c2d 3937 392e  .57 679.58,-979.
-000021d0: 3831 2037 3138 2e34 312c 2d39 3538 2e37  81 718.41,-958.7
-000021e0: 3922 2f3e 0a3c 706f 6c79 676f 6e20 6669  9"/>.<polygon fi
-000021f0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-00002200: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-00002210: 3d22 3731 392e 392c 2d39 3631 2e39 3620  ="719.9,-961.96 
-00002220: 3732 372e 3033 2c2d 3935 342e 3133 2037  727.03,-954.13 7
-00002230: 3136 2e35 362c 2d39 3535 2e38 3120 3731  16.56,-955.81 71
-00002240: 392e 392c 2d39 3631 2e39 3622 2f3e 0a3c  9.9,-961.96"/>.<
-00002250: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00002260: 3d22 6d69 6464 6c65 2220 783d 2236 3737  ="middle" x="677
-00002270: 2e35 2220 793d 222d 3938 372e 3822 2066  .5" y="-987.8" f
-00002280: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00002290: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-000022a0: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
-000022b0: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
-000022c0: 3033 202d 2d3e 0a3c 6720 6964 3d22 6e6f  03 -->.<g id="no
-000022d0: 6465 3722 2063 6c61 7373 3d22 6e6f 6465  de7" class="node
-000022e0: 223e 0a3c 7469 746c 653e 4130 333c 2f74  ">.<title>A03</t
-000022f0: 6974 6c65 3e0a 3c70 6f6c 7967 6f6e 2066  itle>.<polygon f
-00002300: 696c 6c3d 2223 6363 6139 6162 2220 7374  ill="#cca9ab" st
-00002310: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00002320: 6e74 733d 2237 3039 2e35 2c2d 3835 3320  nts="709.5,-853 
-00002330: 3537 332e 352c 2d38 3533 2035 3733 2e35  573.5,-853 573.5
-00002340: 2c2d 3739 3120 3730 392e 352c 2d37 3931  ,-791 709.5,-791
-00002350: 2037 3039 2e35 2c2d 3835 3322 2f3e 0a3c   709.5,-853"/>.<
-00002360: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00002370: 3d22 7374 6172 7422 2078 3d22 3632 3622  ="start" x="626"
-00002380: 2079 3d22 2d38 3336 2e38 2220 666f 6e74   y="-836.8" font
-00002390: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-000023a0: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-000023b0: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-000023c0: 7a65 3d22 3134 2e30 3022 3e41 3033 3c2f  ze="14.00">A03</
-000023d0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-000023e0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-000023f0: 783d 2235 3835 2e35 2220 793d 222d 3832  x="585.5" y="-82
-00002400: 342e 3422 2066 6f6e 742d 6661 6d69 6c79  4.4" font-family
-00002410: 3d22 5469 6d65 732c 7365 7269 6622 2074  ="Times,serif" t
-00002420: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
-00002430: 756e 6465 726c 696e 6522 2066 6f6e 742d  underline" font-
-00002440: 7369 7a65 3d22 3132 2e30 3022 3e48 696e  size="12.00">Hin
-00002450: 7765 6973 3a3c 2f74 6578 743e 0a3c 7465  weis:</text>.<te
-00002460: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00002470: 7374 6172 7422 2078 3d22 3538 352e 3522  start" x="585.5"
-00002480: 2079 3d22 2d38 3132 2e34 2220 666f 6e74   y="-812.4" font
-00002490: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-000024a0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-000024b0: 2231 322e 3030 223e 436c 7573 7465 7220  "12.00">Cluster 
-000024c0: 4162 6c65 686e 756e 673c 2f74 6578 743e  Ablehnung</text>
-000024d0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-000024e0: 6f72 3d22 7374 6172 7422 2078 3d22 3538  or="start" x="58
-000024f0: 352e 3522 2079 3d22 2d38 3030 2e34 2220  5.5" y="-800.4" 
-00002500: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00002510: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00002520: 697a 653d 2231 322e 3030 223e 5265 6765  ize="12.00">Rege
-00002530: 6c7a 6f6e 6520 6661 6c73 6368 3c2f 7465  lzone falsch</te
-00002540: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3326  xt>.</g>.<!-- 3&
-00002550: 2334 353b 2667 743b 4130 3320 2d2d 3e0a  #45;&gt;A03 -->.
-00002560: 3c67 2069 643d 2265 6467 6536 2220 636c  <g id="edge6" cl
-00002570: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
-00002580: 6c65 3e33 2d26 6774 3b41 3033 3c2f 7469  le>3-&gt;A03</ti
-00002590: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
-000025a0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
-000025b0: 6c61 636b 2220 643d 224d 3734 312e 3931  lack" d="M741.91
-000025c0: 2c2d 3931 362e 3636 4337 3235 2e39 332c  ,-916.66C725.93,
-000025d0: 2d39 3031 2e37 3620 3730 322e 3334 2c2d  -901.76 702.34,-
-000025e0: 3837 392e 3735 2036 3832 2e30 342c 2d38  879.75 682.04,-8
-000025f0: 3630 2e38 3122 2f3e 0a3c 706f 6c79 676f  60.81"/>.<polygo
-00002600: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
-00002610: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00002620: 696e 7473 3d22 3638 342e 3637 2c2d 3835  ints="684.67,-85
-00002630: 382e 3438 2036 3734 2e39 372c 2d38 3534  8.48 674.97,-854
-00002640: 2e32 3220 3637 392e 3839 2c2d 3836 332e  .22 679.89,-863.
-00002650: 3620 3638 342e 3637 2c2d 3835 382e 3438  6 684.67,-858.48
-00002660: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00002670: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
-00002680: 3d22 3732 352e 3522 2079 3d22 2d38 3734  ="725.5" y="-874
-00002690: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-000026a0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000026b0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000026c0: 4e65 696e 3c2f 7465 7874 3e0a 3c2f 673e  Nein</text>.</g>
-000026d0: 0a3c 212d 2d20 3420 2d2d 3e0a 3c67 2069  .<!-- 4 -->.<g i
-000026e0: 643d 226e 6f64 6538 2220 636c 6173 733d  d="node8" class=
-000026f0: 226e 6f64 6522 3e0a 3c74 6974 6c65 3e34  "node">.<title>4
-00002700: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
-00002710: 696c 6c3d 2223 3761 6162 3861 2220 7374  ill="#7aab8a" st
-00002720: 726f 6b65 3d22 626c 6163 6b22 2064 3d22  roke="black" d="
-00002730: 4d31 3338 372e 352c 2d38 3430 4331 3338  M1387.5,-840C138
-00002740: 372e 352c 2d38 3430 2037 3339 2e35 2c2d  7.5,-840 739.5,-
-00002750: 3834 3020 3733 392e 352c 2d38 3430 2037  840 739.5,-840 7
-00002760: 3333 2e35 2c2d 3834 3020 3732 372e 352c  33.5,-840 727.5,
-00002770: 2d38 3334 2037 3237 2e35 2c2d 3832 3820  -834 727.5,-828 
-00002780: 3732 372e 352c 2d38 3238 2037 3237 2e35  727.5,-828 727.5
-00002790: 2c2d 3831 3620 3732 372e 352c 2d38 3136  ,-816 727.5,-816
-000027a0: 2037 3237 2e35 2c2d 3831 3020 3733 332e   727.5,-810 733.
-000027b0: 352c 2d38 3034 2037 3339 2e35 2c2d 3830  5,-804 739.5,-80
-000027c0: 3420 3733 392e 352c 2d38 3034 2031 3338  4 739.5,-804 138
-000027d0: 372e 352c 2d38 3034 2031 3338 372e 352c  7.5,-804 1387.5,
-000027e0: 2d38 3034 2031 3339 332e 352c 2d38 3034  -804 1393.5,-804
-000027f0: 2031 3339 392e 352c 2d38 3130 2031 3339   1399.5,-810 139
-00002800: 392e 352c 2d38 3136 2031 3339 392e 352c  9.5,-816 1399.5,
-00002810: 2d38 3136 2031 3339 392e 352c 2d38 3238  -816 1399.5,-828
-00002820: 2031 3339 392e 352c 2d38 3238 2031 3339   1399.5,-828 139
-00002830: 392e 352c 2d38 3334 2031 3339 332e 352c  9.5,-834 1393.5,
-00002840: 2d38 3430 2031 3338 372e 352c 2d38 3430  -840 1387.5,-840
-00002850: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00002860: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00002870: 2237 3431 2e35 2220 793d 222d 3831 392e  "741.5" y="-819.
-00002880: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
-00002890: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-000028a0: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
-000028b0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-000028c0: 223e 343a 203c 2f74 6578 743e 0a3c 7465  ">4: </text>.<te
-000028d0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-000028e0: 7374 6172 7422 2078 3d22 3736 312e 3522  start" x="761.5"
-000028f0: 2079 3d22 2d38 3139 2e33 2220 666f 6e74   y="-819.3" font
-00002900: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00002910: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00002920: 2231 342e 3030 223e 4973 7420 6461 7320  "14.00">Ist das 
-00002930: 4269 6c61 6e7a 6965 7275 6e67 7367 6562  Bilanzierungsgeb
-00002940: 6965 7420 7a75 6d20 416b 7469 7669 6572  iet zum Aktivier
-00002950: 756e 6773 6265 6769 6e6e 2069 6e20 6465  ungsbeginn in de
-00002960: 7220 5265 6765 6c7a 6f6e 6520 6465 7320  r Regelzone des 
-00002970: 4249 4b4f 2067 2623 3235 323b 6c74 6967  BIKO g&#252;ltig
-00002980: 3f3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  ?</text>.</g>.<!
-00002990: 2d2d 2033 2623 3435 3b26 6774 3b34 202d  -- 3&#45;&gt;4 -
-000029a0: 2d3e 0a3c 6720 6964 3d22 6564 6765 3722  ->.<g id="edge7"
-000029b0: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
-000029c0: 7469 746c 653e 332d 2667 743b 343c 2f74  title>3-&gt;4</t
-000029d0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-000029e0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-000029f0: 626c 6163 6b22 2064 3d22 4d38 3038 2e31  black" d="M808.1
-00002a00: 382c 2d39 3136 2e35 3343 3836 312e 3537  8,-916.53C861.57
-00002a10: 2c2d 3839 362e 3938 2039 3438 2e31 2c2d  ,-896.98 948.1,-
-00002a20: 3836 352e 3237 2031 3030 352e 342c 2d38  865.27 1005.4,-8
-00002a30: 3434 2e32 3822 2f3e 0a3c 706f 6c79 676f  44.28"/>.<polygo
-00002a40: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
-00002a50: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00002a60: 696e 7473 3d22 3130 3036 2e34 392c 2d38  ints="1006.49,-8
-00002a70: 3437 2e36 3120 3130 3134 2e36 382c 2d38  47.61 1014.68,-8
-00002a80: 3430 2e38 3820 3130 3034 2e30 392c 2d38  40.88 1004.09,-8
-00002a90: 3431 2e30 3420 3130 3036 2e34 392c 2d38  41.04 1006.49,-8
-00002aa0: 3437 2e36 3122 2f3e 0a3c 7465 7874 2074  47.61"/>.<text t
-00002ab0: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00002ac0: 6c65 2220 783d 2239 3337 2e35 2220 793d  le" x="937.5" y=
-00002ad0: 222d 3837 342e 3822 2066 6f6e 742d 6661  "-874.8" font-fa
-00002ae0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00002af0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
-00002b00: 2e30 3022 3e4a 613c 2f74 6578 743e 0a3c  .00">Ja</text>.<
-00002b10: 2f67 3e0a 3c21 2d2d 2041 3034 202d 2d3e  /g>.<!-- A04 -->
-00002b20: 0a3c 6720 6964 3d22 6e6f 6465 3922 2063  .<g id="node9" c
-00002b30: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00002b40: 746c 653e 4130 343c 2f74 6974 6c65 3e0a  tle>A04</title>.
-00002b50: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2223  <polygon fill="#
-00002b60: 6363 6139 6162 2220 7374 726f 6b65 3d22  cca9ab" stroke="
-00002b70: 626c 6163 6b22 2070 6f69 6e74 733d 2231  black" points="1
-00002b80: 3035 312e 352c 2d37 3430 2038 3335 2e35  051.5,-740 835.5
-00002b90: 2c2d 3734 3020 3833 352e 352c 2d36 3738  ,-740 835.5,-678
-00002ba0: 2031 3035 312e 352c 2d36 3738 2031 3035   1051.5,-678 105
-00002bb0: 312e 352c 2d37 3430 222f 3e0a 3c74 6578  1.5,-740"/>.<tex
-00002bc0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00002bd0: 7461 7274 2220 783d 2239 3238 2220 793d  tart" x="928" y=
-00002be0: 222d 3732 332e 3822 2066 6f6e 742d 6661  "-723.8" font-fa
-00002bf0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00002c00: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-00002c10: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-00002c20: 2231 342e 3030 223e 4130 343c 2f74 6578  "14.00">A04</tex
-00002c30: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00002c40: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00002c50: 3834 372e 3522 2079 3d22 2d37 3131 2e34  847.5" y="-711.4
-00002c60: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00002c70: 696d 6573 2c73 6572 6966 2220 7465 7874  imes,serif" text
-00002c80: 2d64 6563 6f72 6174 696f 6e3d 2275 6e64  -decoration="und
-00002c90: 6572 6c69 6e65 2220 666f 6e74 2d73 697a  erline" font-siz
-00002ca0: 653d 2231 322e 3030 223e 4869 6e77 6569  e="12.00">Hinwei
-00002cb0: 733a 3c2f 7465 7874 3e0a 3c74 6578 7420  s:</text>.<text 
-00002cc0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00002cd0: 7274 2220 783d 2238 3437 2e35 2220 793d  rt" x="847.5" y=
-00002ce0: 222d 3639 392e 3422 2066 6f6e 742d 6661  "-699.4" font-fa
-00002cf0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00002d00: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
-00002d10: 2e30 3022 3e43 6c75 7374 6572 2041 626c  .00">Cluster Abl
-00002d20: 6568 6e75 6e67 3c2f 7465 7874 3e0a 3c74  ehnung</text>.<t
-00002d30: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00002d40: 2273 7461 7274 2220 783d 2238 3437 2e35  "start" x="847.5
-00002d50: 2220 793d 222d 3638 372e 3422 2066 6f6e  " y="-687.4" fon
-00002d60: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00002d70: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00002d80: 3d22 3132 2e30 3022 3e42 696c 616e 7a69  ="12.00">Bilanzi
-00002d90: 6572 756e 6773 6765 6269 6574 206e 6963  erungsgebiet nic
-00002da0: 6874 2067 2623 3235 323b 6c74 6967 3c2f  ht g&#252;ltig</
-00002db0: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00002dc0: 3426 2334 353b 2667 743b 4130 3420 2d2d  4&#45;&gt;A04 --
-00002dd0: 3e0a 3c67 2069 643d 2265 6467 6538 2220  >.<g id="edge8" 
-00002de0: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
-00002df0: 6974 6c65 3e34 2d26 6774 3b41 3034 3c2f  itle>4-&gt;A04</
-00002e00: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
-00002e10: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
-00002e20: 2262 6c61 636b 2220 643d 224d 3130 3434  "black" d="M1044
-00002e30: 2e37 352c 2d38 3033 2e36 3643 3130 3238  .75,-803.66C1028
-00002e40: 2e36 342c 2d37 3838 2e37 3620 3130 3034  .64,-788.76 1004
-00002e50: 2e38 352c 2d37 3636 2e37 3520 3938 342e  .85,-766.75 984.
-00002e60: 3338 2c2d 3734 372e 3831 222f 3e0a 3c70  38,-747.81"/>.<p
-00002e70: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00002e80: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-00002e90: 6b22 2070 6f69 6e74 733d 2239 3836 2e39  k" points="986.9
-00002ea0: 362c 2d37 3435 2e34 3320 3937 372e 3234  6,-745.43 977.24
-00002eb0: 2c2d 3734 312e 3231 2039 3832 2e32 312c  ,-741.21 982.21,
-00002ec0: 2d37 3530 2e35 3720 3938 362e 3936 2c2d  -750.57 986.96,-
-00002ed0: 3734 352e 3433 222f 3e0a 3c74 6578 7420  745.43"/>.<text 
-00002ee0: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
-00002ef0: 646c 6522 2078 3d22 3130 3238 2e35 2220  dle" x="1028.5" 
-00002f00: 793d 222d 3736 312e 3822 2066 6f6e 742d  y="-761.8" font-
-00002f10: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00002f20: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00002f30: 3134 2e30 3022 3e4e 6569 6e3c 2f74 6578  14.00">Nein</tex
-00002f40: 743e 0a3c 2f67 3e0a 3c21 2d2d 2035 202d  t>.</g>.<!-- 5 -
-00002f50: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3130  ->.<g id="node10
-00002f60: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
-00002f70: 3c74 6974 6c65 3e35 3c2f 7469 746c 653e  <title>5</title>
-00002f80: 0a3c 7061 7468 2066 696c 6c3d 2223 3761  .<path fill="#7a
-00002f90: 6162 3861 2220 7374 726f 6b65 3d22 626c  ab8a" stroke="bl
-00002fa0: 6163 6b22 2064 3d22 4d31 3635 352e 352c  ack" d="M1655.5,
-00002fb0: 2d37 3237 4331 3635 352e 352c 2d37 3237  -727C1655.5,-727
-00002fc0: 2031 3038 312e 352c 2d37 3237 2031 3038   1081.5,-727 108
-00002fd0: 312e 352c 2d37 3237 2031 3037 352e 352c  1.5,-727 1075.5,
-00002fe0: 2d37 3237 2031 3036 392e 352c 2d37 3231  -727 1069.5,-721
-00002ff0: 2031 3036 392e 352c 2d37 3135 2031 3036   1069.5,-715 106
-00003000: 392e 352c 2d37 3135 2031 3036 392e 352c  9.5,-715 1069.5,
-00003010: 2d37 3033 2031 3036 392e 352c 2d37 3033  -703 1069.5,-703
-00003020: 2031 3036 392e 352c 2d36 3937 2031 3037   1069.5,-697 107
-00003030: 352e 352c 2d36 3931 2031 3038 312e 352c  5.5,-691 1081.5,
-00003040: 2d36 3931 2031 3038 312e 352c 2d36 3931  -691 1081.5,-691
-00003050: 2031 3635 352e 352c 2d36 3931 2031 3635   1655.5,-691 165
-00003060: 352e 352c 2d36 3931 2031 3636 312e 352c  5.5,-691 1661.5,
-00003070: 2d36 3931 2031 3636 372e 352c 2d36 3937  -691 1667.5,-697
-00003080: 2031 3636 372e 352c 2d37 3033 2031 3636   1667.5,-703 166
-00003090: 372e 352c 2d37 3033 2031 3636 372e 352c  7.5,-703 1667.5,
-000030a0: 2d37 3135 2031 3636 372e 352c 2d37 3135  -715 1667.5,-715
-000030b0: 2031 3636 372e 352c 2d37 3231 2031 3636   1667.5,-721 166
-000030c0: 312e 352c 2d37 3237 2031 3635 352e 352c  1.5,-727 1655.5,
-000030d0: 2d37 3237 222f 3e0a 3c74 6578 7420 7465  -727"/>.<text te
-000030e0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-000030f0: 2220 783d 2231 3038 332e 3522 2079 3d22  " x="1083.5" y="
-00003100: 2d37 3036 2e33 2220 666f 6e74 2d66 616d  -706.3" font-fam
-00003110: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00003120: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
-00003130: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
-00003140: 3134 2e30 3022 3e35 3a20 3c2f 7465 7874  14.00">5: </text
-00003150: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00003160: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00003170: 3130 332e 3522 2079 3d22 2d37 3036 2e33  103.5" y="-706.3
-00003180: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00003190: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-000031a0: 2d73 697a 653d 2231 342e 3030 223e 4973  -size="14.00">Is
-000031b0: 7420 6465 7220 2623 3232 303b 4e42 207a  t der &#220;NB z
-000031c0: 756d 2041 6b74 6976 6965 7275 6e67 7362  um Aktivierungsb
-000031d0: 6567 696e 6e20 6626 2332 3532 3b72 2064  eginn f&#252;r d
-000031e0: 6173 2042 696c 616e 7a69 6572 756e 6773  as Bilanzierungs
-000031f0: 6765 6269 6574 207a 7573 7426 2332 3238  gebiet zust&#228
-00003200: 3b6e 6469 673f 3c2f 7465 7874 3e0a 3c2f  ;ndig?</text>.</
-00003210: 673e 0a3c 212d 2d20 3426 2334 353b 2667  g>.<!-- 4&#45;&g
-00003220: 743b 3520 2d2d 3e0a 3c67 2069 643d 2265  t;5 -->.<g id="e
-00003230: 6467 6539 2220 636c 6173 733d 2265 6467  dge9" class="edg
-00003240: 6522 3e0a 3c74 6974 6c65 3e34 2d26 6774  e">.<title>4-&gt
-00003250: 3b35 3c2f 7469 746c 653e 0a3c 7061 7468  ;5</title>.<path
-00003260: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
-00003270: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00003280: 3131 3131 2e34 392c 2d38 3033 2e35 3343  1111.49,-803.53C
-00003290: 3131 3635 2e31 352c 2d37 3834 2031 3235  1165.15,-784 125
-000032a0: 322e 3038 2c2d 3735 322e 3337 2031 3330  2.08,-752.37 130
-000032b0: 392e 3737 2c2d 3733 312e 3338 222f 3e0a  9.77,-731.38"/>.
-000032c0: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
-000032d0: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
-000032e0: 6163 6b22 2070 6f69 6e74 733d 2231 3331  ack" points="131
-000032f0: 302e 3931 2c2d 3733 342e 3638 2031 3331  0.91,-734.68 131
-00003300: 392e 3131 2c2d 3732 372e 3937 2031 3330  9.11,-727.97 130
-00003310: 382e 3532 2c2d 3732 382e 3120 3133 3130  8.52,-728.1 1310
-00003320: 2e39 312c 2d37 3334 2e36 3822 2f3e 0a3c  .91,-734.68"/>.<
-00003330: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00003340: 3d22 6d69 6464 6c65 2220 783d 2231 3234  ="middle" x="124
-00003350: 312e 3522 2079 3d22 2d37 3631 2e38 2220  1.5" y="-761.8" 
-00003360: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00003370: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00003380: 697a 653d 2231 342e 3030 223e 4a61 3c2f  ize="14.00">Ja</
-00003390: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-000033a0: 4130 3520 2d2d 3e0a 3c67 2069 643d 226e  A05 -->.<g id="n
-000033b0: 6f64 6531 3122 2063 6c61 7373 3d22 6e6f  ode11" class="no
-000033c0: 6465 223e 0a3c 7469 746c 653e 4130 353c  de">.<title>A05<
-000033d0: 2f74 6974 6c65 3e0a 3c70 6f6c 7967 6f6e  /title>.<polygon
-000033e0: 2066 696c 6c3d 2223 6363 6139 6162 2220   fill="#cca9ab" 
-000033f0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
-00003400: 6f69 6e74 733d 2231 3333 352c 2d36 3237  oints="1335,-627
-00003410: 2031 3139 322c 2d36 3237 2031 3139 322c   1192,-627 1192,
-00003420: 2d35 3635 2031 3333 352c 2d35 3635 2031  -565 1335,-565 1
-00003430: 3333 352c 2d36 3237 222f 3e0a 3c74 6578  335,-627"/>.<tex
-00003440: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00003450: 7461 7274 2220 783d 2231 3234 3822 2079  tart" x="1248" y
-00003460: 3d22 2d36 3130 2e38 2220 666f 6e74 2d66  ="-610.8" font-f
-00003470: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00003480: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
-00003490: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
-000034a0: 3d22 3134 2e30 3022 3e41 3035 3c2f 7465  ="14.00">A05</te
-000034b0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-000034c0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-000034d0: 2231 3230 3422 2079 3d22 2d35 3938 2e34  "1204" y="-598.4
-000034e0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-000034f0: 696d 6573 2c73 6572 6966 2220 7465 7874  imes,serif" text
-00003500: 2d64 6563 6f72 6174 696f 6e3d 2275 6e64  -decoration="und
-00003510: 6572 6c69 6e65 2220 666f 6e74 2d73 697a  erline" font-siz
-00003520: 653d 2231 322e 3030 223e 4869 6e77 6569  e="12.00">Hinwei
-00003530: 733a 3c2f 7465 7874 3e0a 3c74 6578 7420  s:</text>.<text 
-00003540: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00003550: 7274 2220 783d 2231 3230 3422 2079 3d22  rt" x="1204" y="
-00003560: 2d35 3836 2e34 2220 666f 6e74 2d66 616d  -586.4" font-fam
-00003570: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00003580: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
-00003590: 3030 223e 436c 7573 7465 7220 4162 6c65  00">Cluster Able
-000035a0: 686e 756e 673c 2f74 6578 743e 0a3c 7465  hnung</text>.<te
-000035b0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-000035c0: 7374 6172 7422 2078 3d22 3132 3034 2220  start" x="1204" 
-000035d0: 793d 222d 3537 342e 3422 2066 6f6e 742d  y="-574.4" font-
-000035e0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-000035f0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00003600: 3132 2e30 3022 3e4b 6569 6e65 2042 6572  12.00">Keine Ber
-00003610: 6563 6874 6967 756e 673c 2f74 6578 743e  echtigung</text>
-00003620: 0a3c 2f67 3e0a 3c21 2d2d 2035 2623 3435  .</g>.<!-- 5&#45
-00003630: 3b26 6774 3b41 3035 202d 2d3e 0a3c 6720  ;&gt;A05 -->.<g 
-00003640: 6964 3d22 6564 6765 3130 2220 636c 6173  id="edge10" clas
-00003650: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-00003660: 3e35 2d26 6774 3b41 3035 3c2f 7469 746c  >5-&gt;A05</titl
-00003670: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
-00003680: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
-00003690: 636b 2220 643d 224d 3133 3532 2e30 392c  ck" d="M1352.09,
-000036a0: 2d36 3930 2e36 3643 3133 3338 2e31 332c  -690.66C1338.13,
-000036b0: 2d36 3735 2e38 3920 3133 3137 2e35 352c  -675.89 1317.55,
-000036c0: 2d36 3534 2e31 3420 3132 3939 2e37 352c  -654.14 1299.75,
-000036d0: 2d36 3335 2e33 3222 2f3e 0a3c 706f 6c79  -635.32"/>.<poly
-000036e0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-000036f0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00003700: 706f 696e 7473 3d22 3133 3032 2e35 312c  points="1302.51,
-00003710: 2d36 3333 2e31 3420 3132 3933 2e30 392c  -633.14 1293.09,
-00003720: 2d36 3238 2e32 3820 3132 3937 2e34 322c  -628.28 1297.42,
-00003730: 2d36 3337 2e39 3520 3133 3032 2e35 312c  -637.95 1302.51,
-00003740: 2d36 3333 2e31 3422 2f3e 0a3c 7465 7874  -633.14"/>.<text
-00003750: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00003760: 6464 6c65 2220 783d 2231 3333 392e 3522  ddle" x="1339.5"
-00003770: 2079 3d22 2d36 3438 2e38 2220 666f 6e74   y="-648.8" font
-00003780: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00003790: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-000037a0: 2231 342e 3030 223e 4e65 696e 3c2f 7465  "14.00">Nein</te
-000037b0: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3620  xt>.</g>.<!-- 6 
-000037c0: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6531  -->.<g id="node1
-000037d0: 3222 2063 6c61 7373 3d22 6e6f 6465 223e  2" class="node">
-000037e0: 0a3c 7469 746c 653e 363c 2f74 6974 6c65  .<title>6</title
-000037f0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
-00003800: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
-00003810: 6c61 636b 2220 643d 224d 3138 3838 2c2d  lack" d="M1888,-
-00003820: 3631 3443 3138 3838 2c2d 3631 3420 3133  614C1888,-614 13
-00003830: 3635 2c2d 3631 3420 3133 3635 2c2d 3631  65,-614 1365,-61
-00003840: 3420 3133 3539 2c2d 3631 3420 3133 3533  4 1359,-614 1353
-00003850: 2c2d 3630 3820 3133 3533 2c2d 3630 3220  ,-608 1353,-602 
-00003860: 3133 3533 2c2d 3630 3220 3133 3533 2c2d  1353,-602 1353,-
-00003870: 3539 3020 3133 3533 2c2d 3539 3020 3133  590 1353,-590 13
-00003880: 3533 2c2d 3538 3420 3133 3539 2c2d 3537  53,-584 1359,-57
-00003890: 3820 3133 3635 2c2d 3537 3820 3133 3635  8 1365,-578 1365
-000038a0: 2c2d 3537 3820 3138 3838 2c2d 3537 3820  ,-578 1888,-578 
-000038b0: 3138 3838 2c2d 3537 3820 3138 3934 2c2d  1888,-578 1894,-
-000038c0: 3537 3820 3139 3030 2c2d 3538 3420 3139  578 1900,-584 19
-000038d0: 3030 2c2d 3539 3020 3139 3030 2c2d 3539  00,-590 1900,-59
-000038e0: 3020 3139 3030 2c2d 3630 3220 3139 3030  0 1900,-602 1900
-000038f0: 2c2d 3630 3220 3139 3030 2c2d 3630 3820  ,-602 1900,-608 
-00003900: 3138 3934 2c2d 3631 3420 3138 3838 2c2d  1894,-614 1888,-
-00003910: 3631 3422 2f3e 0a3c 7465 7874 2074 6578  614"/>.<text tex
-00003920: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00003930: 2078 3d22 3133 3637 2220 793d 222d 3539   x="1367" y="-59
-00003940: 332e 3322 2066 6f6e 742d 6661 6d69 6c79  3.3" font-family
-00003950: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00003960: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
-00003970: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00003980: 3030 223e 363a 203c 2f74 6578 743e 0a3c  00">6: </text>.<
-00003990: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-000039a0: 3d22 7374 6172 7422 2078 3d22 3133 3837  ="start" x="1387
-000039b0: 2220 793d 222d 3539 332e 3322 2066 6f6e  " y="-593.3" fon
-000039c0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000039d0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000039e0: 3d22 3134 2e30 3022 3e45 7869 7374 6965  ="14.00">Existie
-000039f0: 7274 2062 6572 6569 7473 2065 696e 2061  rt bereits ein a
-00003a00: 6277 6569 6368 656e 6465 7320 5475 7065  bweichendes Tupe
-00003a10: 6c20 756e 7465 7220 6465 7220 4944 2064  l unter der ID d
-00003a20: 6573 204d 6142 6953 2d5a 503f 3c2f 7465  es MaBiS-ZP?</te
-00003a30: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3526  xt>.</g>.<!-- 5&
-00003a40: 2334 353b 2667 743b 3620 2d2d 3e0a 3c67  #45;&gt;6 -->.<g
-00003a50: 2069 643d 2265 6467 6531 3122 2063 6c61   id="edge11" cla
-00003a60: 7373 3d22 6564 6765 223e 0a3c 7469 746c  ss="edge">.<titl
-00003a70: 653e 352d 2667 743b 363c 2f74 6974 6c65  e>5-&gt;6</title
-00003a80: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00003a90: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00003aa0: 6b22 2064 3d22 4d31 3430 392e 312c 2d36  k" d="M1409.1,-6
-00003ab0: 3930 2e35 3343 3134 3534 2e31 382c 2d36  90.53C1454.18,-6
-00003ac0: 3731 2e31 3420 3135 3237 2e30 322c 2d36  71.14 1527.02,-6
-00003ad0: 3339 2e38 2031 3537 352e 3831 2c2d 3631  39.8 1575.81,-61
-00003ae0: 382e 3831 222f 3e0a 3c70 6f6c 7967 6f6e  8.81"/>.<polygon
-00003af0: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-00003b00: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00003b10: 6e74 733d 2231 3537 362e 3935 2c2d 3632  nts="1576.95,-62
-00003b20: 322e 3133 2031 3538 342e 3735 2c2d 3631  2.13 1584.75,-61
-00003b30: 342e 3936 2031 3537 342e 3138 2c2d 3631  4.96 1574.18,-61
-00003b40: 352e 3720 3135 3736 2e39 352c 2d36 3232  5.7 1576.95,-622
-00003b50: 2e31 3322 2f3e 0a3c 7465 7874 2074 6578  .13"/>.<text tex
-00003b60: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-00003b70: 2220 783d 2231 3532 302e 3522 2079 3d22  " x="1520.5" y="
-00003b80: 2d36 3438 2e38 2220 666f 6e74 2d66 616d  -648.8" font-fam
-00003b90: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00003ba0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00003bb0: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
-00003bc0: 673e 0a3c 212d 2d20 4130 3620 2d2d 3e0a  g>.<!-- A06 -->.
-00003bd0: 3c67 2069 643d 226e 6f64 6531 3322 2063  <g id="node13" c
-00003be0: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00003bf0: 746c 653e 4130 363c 2f74 6974 6c65 3e0a  tle>A06</title>.
-00003c00: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2223  <polygon fill="#
-00003c10: 6363 6139 6162 2220 7374 726f 6b65 3d22  cca9ab" stroke="
-00003c20: 626c 6163 6b22 2070 6f69 6e74 733d 2231  black" points="1
-00003c30: 3537 312c 2d35 3134 2031 3238 322c 2d35  571,-514 1282,-5
-00003c40: 3134 2031 3238 322c 2d34 3532 2031 3537  14 1282,-452 157
-00003c50: 312c 2d34 3532 2031 3537 312c 2d35 3134  1,-452 1571,-514
-00003c60: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00003c70: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00003c80: 2231 3431 3122 2079 3d22 2d34 3937 2e38  "1411" y="-497.8
-00003c90: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00003ca0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00003cb0: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
-00003cc0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00003cd0: 3e41 3036 3c2f 7465 7874 3e0a 3c74 6578  >A06</text>.<tex
-00003ce0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00003cf0: 7461 7274 2220 783d 2231 3239 3422 2079  tart" x="1294" y
-00003d00: 3d22 2d34 3835 2e34 2220 666f 6e74 2d66  ="-485.4" font-f
-00003d10: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00003d20: 6966 2220 7465 7874 2d64 6563 6f72 6174  if" text-decorat
-00003d30: 696f 6e3d 2275 6e64 6572 6c69 6e65 2220  ion="underline" 
-00003d40: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00003d50: 223e 4869 6e77 6569 733a 3c2f 7465 7874  ">Hinweis:</text
-00003d60: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00003d70: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00003d80: 3239 3422 2079 3d22 2d34 3733 2e34 2220  294" y="-473.4" 
-00003d90: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00003da0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00003db0: 697a 653d 2231 322e 3030 223e 436c 7573  ize="12.00">Clus
-00003dc0: 7465 7220 4162 6c65 686e 756e 673c 2f74  ter Ablehnung</t
-00003dd0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00003de0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00003df0: 3d22 3132 3934 2220 793d 222d 3436 312e  ="1294" y="-461.
-00003e00: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-00003e10: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00003e20: 742d 7369 7a65 3d22 3132 2e30 3022 3e41  t-size="12.00">A
-00003e30: 6277 6569 6368 656e 6465 7220 4d61 4269  bweichender MaBi
-00003e40: 532d 5a50 2062 6572 6569 7473 2076 6f72  S-ZP bereits vor
-00003e50: 6861 6e64 656e 3c2f 7465 7874 3e0a 3c2f  handen</text>.</
-00003e60: 673e 0a3c 212d 2d20 3626 2334 353b 2667  g>.<!-- 6&#45;&g
-00003e70: 743b 4130 3620 2d2d 3e0a 3c67 2069 643d  t;A06 -->.<g id=
-00003e80: 2265 6467 6531 3222 2063 6c61 7373 3d22  "edge12" class="
-00003e90: 6564 6765 223e 0a3c 7469 746c 653e 362d  edge">.<title>6-
-00003ea0: 2667 743b 4130 363c 2f74 6974 6c65 3e0a  &gt;A06</title>.
-00003eb0: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00003ec0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00003ed0: 2064 3d22 4d31 3539 352e 3235 2c2d 3537   d="M1595.25,-57
-00003ee0: 372e 3636 4331 3536 372e 3433 2c2d 3536  7.66C1567.43,-56
-00003ef0: 322e 3232 2031 3532 352e 3836 2c2d 3533  2.22 1525.86,-53
-00003f00: 392e 3134 2031 3439 302e 3934 2c2d 3531  9.14 1490.94,-51
-00003f10: 392e 3736 222f 3e0a 3c70 6f6c 7967 6f6e  9.76"/>.<polygon
-00003f20: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-00003f30: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00003f40: 6e74 733d 2231 3439 332e 3035 2c2d 3531  nts="1493.05,-51
-00003f50: 362e 3933 2031 3438 322e 3631 2c2d 3531  6.93 1482.61,-51
-00003f60: 352e 3134 2031 3438 392e 3635 2c2d 3532  5.14 1489.65,-52
-00003f70: 332e 3035 2031 3439 332e 3035 2c2d 3531  3.05 1493.05,-51
-00003f80: 362e 3933 222f 3e0a 3c74 6578 7420 7465  6.93"/>.<text te
-00003f90: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
-00003fa0: 6522 2078 3d22 3135 3435 2e35 2220 793d  e" x="1545.5" y=
-00003fb0: 222d 3533 352e 3822 2066 6f6e 742d 6661  "-535.8" font-fa
-00003fc0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00003fd0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
-00003fe0: 2e30 3022 3e4a 613c 2f74 6578 743e 0a3c  .00">Ja</text>.<
-00003ff0: 2f67 3e0a 3c21 2d2d 2037 202d 2d3e 0a3c  /g>.<!-- 7 -->.<
-00004000: 6720 6964 3d22 6e6f 6465 3134 2220 636c  g id="node14" cl
-00004010: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
-00004020: 6c65 3e37 3c2f 7469 746c 653e 0a3c 7061  le>7</title>.<pa
-00004030: 7468 2066 696c 6c3d 2223 3761 6162 3861  th fill="#7aab8a
-00004040: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00004050: 2064 3d22 4d32 3737 392e 352c 2d35 3031   d="M2779.5,-501
-00004060: 4332 3737 392e 352c 2d35 3031 2031 3630  C2779.5,-501 160
-00004070: 312e 352c 2d35 3031 2031 3630 312e 352c  1.5,-501 1601.5,
-00004080: 2d35 3031 2031 3539 352e 352c 2d35 3031  -501 1595.5,-501
-00004090: 2031 3538 392e 352c 2d34 3935 2031 3538   1589.5,-495 158
-000040a0: 392e 352c 2d34 3839 2031 3538 392e 352c  9.5,-489 1589.5,
-000040b0: 2d34 3839 2031 3538 392e 352c 2d34 3737  -489 1589.5,-477
-000040c0: 2031 3538 392e 352c 2d34 3737 2031 3538   1589.5,-477 158
-000040d0: 392e 352c 2d34 3731 2031 3539 352e 352c  9.5,-471 1595.5,
-000040e0: 2d34 3635 2031 3630 312e 352c 2d34 3635  -465 1601.5,-465
-000040f0: 2031 3630 312e 352c 2d34 3635 2032 3737   1601.5,-465 277
-00004100: 392e 352c 2d34 3635 2032 3737 392e 352c  9.5,-465 2779.5,
-00004110: 2d34 3635 2032 3738 352e 352c 2d34 3635  -465 2785.5,-465
-00004120: 2032 3739 312e 352c 2d34 3731 2032 3739   2791.5,-471 279
-00004130: 312e 352c 2d34 3737 2032 3739 312e 352c  1.5,-477 2791.5,
-00004140: 2d34 3737 2032 3739 312e 352c 2d34 3839  -477 2791.5,-489
-00004150: 2032 3739 312e 352c 2d34 3839 2032 3739   2791.5,-489 279
-00004160: 312e 352c 2d34 3935 2032 3738 352e 352c  1.5,-495 2785.5,
-00004170: 2d35 3031 2032 3737 392e 352c 2d35 3031  -501 2779.5,-501
-00004180: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00004190: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-000041a0: 2231 3630 332e 3522 2079 3d22 2d34 3830  "1603.5" y="-480
-000041b0: 2e33 2220 666f 6e74 2d66 616d 696c 793d  .3" font-family=
-000041c0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000041d0: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-000041e0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-000041f0: 3022 3e37 3a20 3c2f 7465 7874 3e0a 3c74  0">7: </text>.<t
-00004200: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004210: 2273 7461 7274 2220 783d 2231 3632 332e  "start" x="1623.
-00004220: 3522 2079 3d22 2d34 3830 2e33 2220 666f  5" y="-480.3" fo
-00004230: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00004240: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00004250: 653d 2231 342e 3030 223e 4578 6973 7469  e="14.00">Existi
-00004260: 6572 7420 6265 7265 6974 7320 6626 2332  ert bereits f&#2
-00004270: 3532 3b72 2064 6173 2067 656e 616e 6e74  52;r das genannt
-00004280: 6520 5475 7065 6c20 6175 7320 4167 6772  e Tupel aus Aggr
-00004290: 6567 6174 696f 6e73 2d76 6572 616e 7477  egations-verantw
-000042a0: 6f72 746c 6963 6865 722c 2042 696c 616e  ortlicher, Bilan
-000042b0: 7a69 6572 756e 6773 6765 6269 6574 2c20  zierungsgebiet, 
-000042c0: 5370 616e 6e75 6e67 7365 6265 6e65 2075  Spannungsebene u
-000042d0: 6e64 205a 5254 2065 696e 6520 6162 7765  nd ZRT eine abwe
-000042e0: 6963 6865 6e64 6520 4944 2064 6573 204d  ichende ID des M
-000042f0: 6142 6953 2d5a 503f 3c2f 7465 7874 3e0a  aBiS-ZP?</text>.
-00004300: 3c2f 673e 0a3c 212d 2d20 3626 2334 353b  </g>.<!-- 6&#45;
-00004310: 2667 743b 3720 2d2d 3e0a 3c67 2069 643d  &gt;7 -->.<g id=
-00004320: 2265 6467 6531 3322 2063 6c61 7373 3d22  "edge13" class="
-00004330: 6564 6765 223e 0a3c 7469 746c 653e 362d  edge">.<title>6-
-00004340: 2667 743b 373c 2f74 6974 6c65 3e0a 3c70  &gt;7</title>.<p
-00004350: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
-00004360: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
-00004370: 3d22 4d31 3731 352e 3235 2c2d 3537 372e  ="M1715.25,-577.
-00004380: 3533 4331 3831 372e 3236 2c2d 3535 372e  53C1817.26,-557.
-00004390: 3436 2031 3938 342e 332c 2d35 3234 2e35  46 1984.3,-524.5
-000043a0: 3820 3230 3930 2e37 342c 2d35 3033 2e36  8 2090.74,-503.6
-000043b0: 3322 2f3e 0a3c 706f 6c79 676f 6e20 6669  3"/>.<polygon fi
-000043c0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-000043d0: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-000043e0: 3d22 3230 3931 2e31 392c 2d35 3037 2e31  ="2091.19,-507.1
-000043f0: 3120 3231 3030 2e33 322c 2d35 3031 2e37  1 2100.32,-501.7
-00004400: 3520 3230 3839 2e38 332c 2d35 3030 2e32  5 2089.83,-500.2
-00004410: 3420 3230 3931 2e31 392c 2d35 3037 2e31  4 2091.19,-507.1
-00004420: 3122 2f3e 0a3c 7465 7874 2074 6578 742d  1"/>.<text text-
-00004430: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
-00004440: 783d 2231 3935 392e 3522 2079 3d22 2d35  x="1959.5" y="-5
-00004450: 3335 2e38 2220 666f 6e74 2d66 616d 696c  35.8" font-famil
-00004460: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00004470: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00004480: 223e 4e65 696e 3c2f 7465 7874 3e0a 3c2f  ">Nein</text>.</
-00004490: 673e 0a3c 212d 2d20 4130 3720 2d2d 3e0a  g>.<!-- A07 -->.
-000044a0: 3c67 2069 643d 226e 6f64 6531 3522 2063  <g id="node15" c
-000044b0: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-000044c0: 746c 653e 4130 373c 2f74 6974 6c65 3e0a  tle>A07</title>.
-000044d0: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2223  <polygon fill="#
-000044e0: 6363 6139 6162 2220 7374 726f 6b65 3d22  cca9ab" stroke="
-000044f0: 626c 6163 6b22 2070 6f69 6e74 733d 2232  black" points="2
-00004500: 3235 302e 352c 2d34 3031 2031 3932 302e  250.5,-401 1920.
-00004510: 352c 2d34 3031 2031 3932 302e 352c 2d33  5,-401 1920.5,-3
-00004520: 3339 2032 3235 302e 352c 2d33 3339 2032  39 2250.5,-339 2
-00004530: 3235 302e 352c 2d34 3031 222f 3e0a 3c74  250.5,-401"/>.<t
-00004540: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004550: 2273 7461 7274 2220 783d 2232 3037 3022  "start" x="2070"
-00004560: 2079 3d22 2d33 3834 2e38 2220 666f 6e74   y="-384.8" font
-00004570: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00004580: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-00004590: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-000045a0: 7a65 3d22 3134 2e30 3022 3e41 3037 3c2f  ze="14.00">A07</
-000045b0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-000045c0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-000045d0: 783d 2231 3933 322e 3522 2079 3d22 2d33  x="1932.5" y="-3
-000045e0: 3732 2e34 2220 666f 6e74 2d66 616d 696c  72.4" font-famil
-000045f0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00004600: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00004610: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
-00004620: 2d73 697a 653d 2231 322e 3030 223e 4869  -size="12.00">Hi
-00004630: 6e77 6569 733a 3c2f 7465 7874 3e0a 3c74  nweis:</text>.<t
-00004640: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004650: 2273 7461 7274 2220 783d 2231 3933 322e  "start" x="1932.
-00004660: 3522 2079 3d22 2d33 3630 2e34 2220 666f  5" y="-360.4" fo
-00004670: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00004680: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00004690: 653d 2231 322e 3030 223e 436c 7573 7465  e="12.00">Cluste
-000046a0: 7220 4162 6c65 686e 756e 673c 2f74 6578  r Ablehnung</tex
-000046b0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-000046c0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-000046d0: 3139 3332 2e35 2220 793d 222d 3334 382e  1932.5" y="-348.
-000046e0: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-000046f0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00004700: 742d 7369 7a65 3d22 3132 2e30 3022 3e41  t-size="12.00">A
-00004710: 6277 6569 6368 656e 6465 2049 4420 7a75  bweichende ID zu
-00004720: 6d20 4d61 4269 532d 5a50 2062 6572 6569  m MaBiS-ZP berei
-00004730: 7473 2076 6f72 6861 6e64 656e 3c2f 7465  ts vorhanden</te
-00004740: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3726  xt>.</g>.<!-- 7&
-00004750: 2334 353b 2667 743b 4130 3720 2d2d 3e0a  #45;&gt;A07 -->.
-00004760: 3c67 2069 643d 2265 6467 6531 3422 2063  <g id="edge14" c
-00004770: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00004780: 746c 653e 372d 2667 743b 4130 373c 2f74  tle>7-&gt;A07</t
-00004790: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-000047a0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-000047b0: 626c 6163 6b22 2064 3d22 4d32 3137 342e  black" d="M2174.
-000047c0: 3039 2c2d 3436 342e 3636 4332 3136 302e  09,-464.66C2160.
-000047d0: 3133 2c2d 3434 392e 3839 2032 3133 392e  13,-449.89 2139.
-000047e0: 3535 2c2d 3432 382e 3134 2032 3132 312e  55,-428.14 2121.
-000047f0: 3735 2c2d 3430 392e 3332 222f 3e0a 3c70  75,-409.32"/>.<p
-00004800: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00004810: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-00004820: 6b22 2070 6f69 6e74 733d 2232 3132 342e  k" points="2124.
-00004830: 3531 2c2d 3430 372e 3134 2032 3131 352e  51,-407.14 2115.
-00004840: 3039 2c2d 3430 322e 3238 2032 3131 392e  09,-402.28 2119.
-00004850: 3432 2c2d 3431 312e 3935 2032 3132 342e  42,-411.95 2124.
-00004860: 3531 2c2d 3430 372e 3134 222f 3e0a 3c74  51,-407.14"/>.<t
-00004870: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004880: 226d 6964 646c 6522 2078 3d22 3231 3531  "middle" x="2151
-00004890: 2e35 2220 793d 222d 3432 322e 3822 2066  .5" y="-422.8" f
-000048a0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-000048b0: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-000048c0: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
-000048d0: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2038  ext>.</g>.<!-- 8
-000048e0: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
-000048f0: 3136 2220 636c 6173 733d 226e 6f64 6522  16" class="node"
-00004900: 3e0a 3c74 6974 6c65 3e38 3c2f 7469 746c  >.<title>8</titl
-00004910: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
-00004920: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
-00004930: 626c 6163 6b22 2064 3d22 4d32 3635 362e  black" d="M2656.
-00004940: 352c 2d33 3838 4332 3635 362e 352c 2d33  5,-388C2656.5,-3
-00004950: 3838 2032 3238 302e 352c 2d33 3838 2032  88 2280.5,-388 2
-00004960: 3238 302e 352c 2d33 3838 2032 3237 342e  280.5,-388 2274.
-00004970: 352c 2d33 3838 2032 3236 382e 352c 2d33  5,-388 2268.5,-3
-00004980: 3832 2032 3236 382e 352c 2d33 3736 2032  82 2268.5,-376 2
-00004990: 3236 382e 352c 2d33 3736 2032 3236 382e  268.5,-376 2268.
-000049a0: 352c 2d33 3634 2032 3236 382e 352c 2d33  5,-364 2268.5,-3
-000049b0: 3634 2032 3236 382e 352c 2d33 3538 2032  64 2268.5,-358 2
-000049c0: 3237 342e 352c 2d33 3532 2032 3238 302e  274.5,-352 2280.
-000049d0: 352c 2d33 3532 2032 3238 302e 352c 2d33  5,-352 2280.5,-3
-000049e0: 3532 2032 3635 362e 352c 2d33 3532 2032  52 2656.5,-352 2
-000049f0: 3635 362e 352c 2d33 3532 2032 3636 322e  656.5,-352 2662.
-00004a00: 352c 2d33 3532 2032 3636 382e 352c 2d33  5,-352 2668.5,-3
-00004a10: 3538 2032 3636 382e 352c 2d33 3634 2032  58 2668.5,-364 2
-00004a20: 3636 382e 352c 2d33 3634 2032 3636 382e  668.5,-364 2668.
-00004a30: 352c 2d33 3736 2032 3636 382e 352c 2d33  5,-376 2668.5,-3
-00004a40: 3736 2032 3636 382e 352c 2d33 3832 2032  76 2668.5,-382 2
-00004a50: 3636 322e 352c 2d33 3838 2032 3635 362e  662.5,-388 2656.
-00004a60: 352c 2d33 3838 222f 3e0a 3c74 6578 7420  5,-388"/>.<text 
-00004a70: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00004a80: 7274 2220 783d 2232 3238 322e 3522 2079  rt" x="2282.5" y
-00004a90: 3d22 2d33 3637 2e33 2220 666f 6e74 2d66  ="-367.3" font-f
-00004aa0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00004ab0: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
-00004ac0: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
-00004ad0: 3d22 3134 2e30 3022 3e38 3a20 3c2f 7465  ="14.00">8: </te
-00004ae0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00004af0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00004b00: 2232 3330 322e 3522 2079 3d22 2d33 3637  "2302.5" y="-367
-00004b10: 2e33 2220 666f 6e74 2d66 616d 696c 793d  .3" font-family=
-00004b20: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00004b30: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-00004b40: 4973 7420 6465 7220 2623 3232 303b 4e42  Ist der &#220;NB
-00004b50: 207a 7572 2041 6b74 6976 6965 7275 6e67   zur Aktivierung
-00004b60: 2064 6573 205a 5254 2062 6572 6563 6874   des ZRT berecht
-00004b70: 6967 743f 3c2f 7465 7874 3e0a 3c2f 673e  igt?</text>.</g>
-00004b80: 0a3c 212d 2d20 3726 2334 353b 2667 743b  .<!-- 7&#45;&gt;
-00004b90: 3820 2d2d 3e0a 3c67 2069 643d 2265 6467  8 -->.<g id="edg
-00004ba0: 6531 3522 2063 6c61 7373 3d22 6564 6765  e15" class="edge
-00004bb0: 223e 0a3c 7469 746c 653e 372d 2667 743b  ">.<title>7-&gt;
-00004bc0: 383c 2f74 6974 6c65 3e0a 3c70 6174 6820  8</title>.<path 
-00004bd0: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
-00004be0: 6b65 3d22 626c 6163 6b22 2064 3d22 4d32  ke="black" d="M2
-00004bf0: 3233 342e 3234 2c2d 3436 342e 3533 4332  234.24,-464.53C2
-00004c00: 3238 332e 3032 2c2d 3434 352e 3036 2032  283.02,-445.06 2
-00004c10: 3336 312e 3936 2c2d 3431 332e 3534 2032  361.96,-413.54 2
-00004c20: 3431 342e 3534 2c2d 3339 322e 3535 222f  414.54,-392.55"/
-00004c30: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
-00004c40: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
-00004c50: 626c 6163 6b22 2070 6f69 6e74 733d 2232  black" points="2
-00004c60: 3431 352e 3632 2c2d 3339 352e 3838 2032  415.62,-395.88 2
-00004c70: 3432 332e 3631 2c2d 3338 382e 3933 2032  423.61,-388.93 2
-00004c80: 3431 332e 3032 2c2d 3338 392e 3338 2032  413.02,-389.38 2
-00004c90: 3431 352e 3632 2c2d 3339 352e 3838 222f  415.62,-395.88"/
-00004ca0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00004cb0: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
-00004cc0: 3233 3633 2e35 2220 793d 222d 3432 322e  2363.5" y="-422.
-00004cd0: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00004ce0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00004cf0: 742d 7369 7a65 3d22 3134 2e30 3022 3e4e  t-size="14.00">N
-00004d00: 6569 6e3c 2f74 6578 743e 0a3c 2f67 3e0a  ein</text>.</g>.
-00004d10: 3c21 2d2d 2041 3038 202d 2d3e 0a3c 6720  <!-- A08 -->.<g 
-00004d20: 6964 3d22 6e6f 6465 3137 2220 636c 6173  id="node17" clas
-00004d30: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
-00004d40: 3e41 3038 3c2f 7469 746c 653e 0a3c 706f  >A08</title>.<po
-00004d50: 6c79 676f 6e20 6669 6c6c 3d22 2363 6361  lygon fill="#cca
-00004d60: 3961 6222 2073 7472 6f6b 653d 2262 6c61  9ab" stroke="bla
-00004d70: 636b 2220 706f 696e 7473 3d22 3234 3936  ck" points="2496
-00004d80: 2c2d 3238 3820 3232 3733 2c2d 3238 3820  ,-288 2273,-288 
-00004d90: 3232 3733 2c2d 3232 3620 3234 3936 2c2d  2273,-226 2496,-
-00004da0: 3232 3620 3234 3936 2c2d 3238 3822 2f3e  226 2496,-288"/>
-00004db0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00004dc0: 6f72 3d22 7374 6172 7422 2078 3d22 3233  or="start" x="23
-00004dd0: 3639 2220 793d 222d 3237 312e 3822 2066  69" y="-271.8" f
-00004de0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00004df0: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00004e00: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00004e10: 2d73 697a 653d 2231 342e 3030 223e 4130  -size="14.00">A0
-00004e20: 383c 2f74 6578 743e 0a3c 7465 7874 2074  8</text>.<text t
-00004e30: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00004e40: 7422 2078 3d22 3232 3835 2220 793d 222d  t" x="2285" y="-
-00004e50: 3235 392e 3422 2066 6f6e 742d 6661 6d69  259.4" font-fami
-00004e60: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00004e70: 2074 6578 742d 6465 636f 7261 7469 6f6e   text-decoration
-00004e80: 3d22 756e 6465 726c 696e 6522 2066 6f6e  ="underline" fon
-00004e90: 742d 7369 7a65 3d22 3132 2e30 3022 3e48  t-size="12.00">H
-00004ea0: 696e 7765 6973 3a3c 2f74 6578 743e 0a3c  inweis:</text>.<
-00004eb0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00004ec0: 3d22 7374 6172 7422 2078 3d22 3232 3835  ="start" x="2285
-00004ed0: 2220 793d 222d 3234 372e 3422 2066 6f6e  " y="-247.4" fon
-00004ee0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00004ef0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00004f00: 3d22 3132 2e30 3022 3e43 6c75 7374 6572  ="12.00">Cluster
-00004f10: 2041 626c 6568 6e75 6e67 3c2f 7465 7874   Ablehnung</text
-00004f20: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00004f30: 686f 723d 2273 7461 7274 2220 783d 2232  hor="start" x="2
-00004f40: 3238 3522 2079 3d22 2d32 3335 2e34 2220  285" y="-235.4" 
-00004f50: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00004f60: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00004f70: 697a 653d 2231 322e 3030 223e 5a52 5420  ize="12.00">ZRT 
-00004f80: 416b 7469 7669 6572 756e 6720 6e69 6368  Aktivierung nich
-00004f90: 7420 6265 7265 6368 7469 6774 3c2f 7465  t berechtigt</te
-00004fa0: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3826  xt>.</g>.<!-- 8&
-00004fb0: 2334 353b 2667 743b 4130 3820 2d2d 3e0a  #45;&gt;A08 -->.
-00004fc0: 3c67 2069 643d 2265 6467 6531 3622 2063  <g id="edge16" c
-00004fd0: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00004fe0: 746c 653e 382d 2667 743b 4130 383c 2f74  tle>8-&gt;A08</t
-00004ff0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00005000: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-00005010: 626c 6163 6b22 2064 3d22 4d32 3435 352e  black" d="M2455.
-00005020: 3338 2c2d 3335 312e 3636 4332 3434 342e  38,-351.66C2444.
-00005030: 342c 2d33 3337 2e31 3620 3234 3238 2e33  4,-337.16 2428.3
-00005040: 332c 2d33 3135 2e39 3220 3234 3134 2e32  3,-315.92 2414.2
-00005050: 372c 2d32 3937 2e33 3322 2f3e 0a3c 706f  7,-297.33"/>.<po
-00005060: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
-00005070: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
-00005080: 2220 706f 696e 7473 3d22 3234 3137 2e30  " points="2417.0
-00005090: 382c 2d32 3935 2e32 3520 3234 3038 2e32  8,-295.25 2408.2
-000050a0: 362c 2d32 3839 2e33 3920 3234 3131 2e35  6,-289.39 2411.5
-000050b0: 2c2d 3239 392e 3438 2032 3431 372e 3038  ,-299.48 2417.08
-000050c0: 2c2d 3239 352e 3235 222f 3e0a 3c74 6578  ,-295.25"/>.<tex
-000050d0: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
-000050e0: 6964 646c 6522 2078 3d22 3234 3439 2e35  iddle" x="2449.5
-000050f0: 2220 793d 222d 3330 392e 3822 2066 6f6e  " y="-309.8" fon
-00005100: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00005110: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00005120: 3d22 3134 2e30 3022 3e4e 6569 6e3c 2f74  ="14.00">Nein</t
-00005130: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2039  ext>.</g>.<!-- 9
-00005140: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
-00005150: 3138 2220 636c 6173 733d 226e 6f64 6522  18" class="node"
-00005160: 3e0a 3c74 6974 6c65 3e39 3c2f 7469 746c  >.<title>9</titl
-00005170: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
-00005180: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
-00005190: 626c 6163 6b22 2064 3d22 4d32 3830 322e  black" d="M2802.
-000051a0: 352c 2d32 3735 4332 3830 322e 352c 2d32  5,-275C2802.5,-2
-000051b0: 3735 2032 3532 362e 352c 2d32 3735 2032  75 2526.5,-275 2
-000051c0: 3532 362e 352c 2d32 3735 2032 3532 302e  526.5,-275 2520.
-000051d0: 352c 2d32 3735 2032 3531 342e 352c 2d32  5,-275 2514.5,-2
-000051e0: 3639 2032 3531 342e 352c 2d32 3633 2032  69 2514.5,-263 2
-000051f0: 3531 342e 352c 2d32 3633 2032 3531 342e  514.5,-263 2514.
-00005200: 352c 2d32 3531 2032 3531 342e 352c 2d32  5,-251 2514.5,-2
-00005210: 3531 2032 3531 342e 352c 2d32 3435 2032  51 2514.5,-245 2
-00005220: 3532 302e 352c 2d32 3339 2032 3532 362e  520.5,-239 2526.
-00005230: 352c 2d32 3339 2032 3532 362e 352c 2d32  5,-239 2526.5,-2
-00005240: 3339 2032 3830 322e 352c 2d32 3339 2032  39 2802.5,-239 2
-00005250: 3830 322e 352c 2d32 3339 2032 3830 382e  802.5,-239 2808.
-00005260: 352c 2d32 3339 2032 3831 342e 352c 2d32  5,-239 2814.5,-2
-00005270: 3435 2032 3831 342e 352c 2d32 3531 2032  45 2814.5,-251 2
-00005280: 3831 342e 352c 2d32 3531 2032 3831 342e  814.5,-251 2814.
-00005290: 352c 2d32 3633 2032 3831 342e 352c 2d32  5,-263 2814.5,-2
-000052a0: 3633 2032 3831 342e 352c 2d32 3639 2032  63 2814.5,-269 2
-000052b0: 3830 382e 352c 2d32 3735 2032 3830 322e  808.5,-275 2802.
-000052c0: 352c 2d32 3735 222f 3e0a 3c74 6578 7420  5,-275"/>.<text 
-000052d0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-000052e0: 7274 2220 783d 2232 3532 382e 3522 2079  rt" x="2528.5" y
-000052f0: 3d22 2d32 3534 2e33 2220 666f 6e74 2d66  ="-254.3" font-f
-00005300: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00005310: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
-00005320: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
-00005330: 3d22 3134 2e30 3022 3e39 3a20 3c2f 7465  ="14.00">9: </te
-00005340: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00005350: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00005360: 2232 3534 382e 3522 2079 3d22 2d32 3534  "2548.5" y="-254
-00005370: 2e33 2220 666f 6e74 2d66 616d 696c 793d  .3" font-family=
-00005380: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00005390: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000053a0: 5061 7373 7420 6469 6520 4f42 4953 2d4b  Passt die OBIS-K
-000053b0: 656e 6e7a 6168 6c20 7a75 6d20 5a52 543f  ennzahl zum ZRT?
-000053c0: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-000053d0: 2d20 3826 2334 353b 2667 743b 3920 2d2d  - 8&#45;&gt;9 --
-000053e0: 3e0a 3c67 2069 643d 2265 6467 6531 3722  >.<g id="edge17"
-000053f0: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
-00005400: 7469 746c 653e 382d 2667 743b 393c 2f74  title>8-&gt;9</t
-00005410: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00005420: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-00005430: 626c 6163 6b22 2064 3d22 4d32 3439 392e  black" d="M2499.
-00005440: 3132 2c2d 3335 312e 3636 4332 3533 322e  12,-351.66C2532.
-00005450: 3638 2c2d 3333 322e 3635 2032 3538 362e  68,-332.65 2586.
-00005460: 3637 2c2d 3330 322e 3038 2032 3632 332e  67,-302.08 2623.
-00005470: 3738 2c2d 3238 312e 3036 222f 3e0a 3c70  78,-281.06"/>.<p
-00005480: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00005490: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-000054a0: 6b22 2070 6f69 6e74 733d 2232 3632 352e  k" points="2625.
-000054b0: 3437 2c2d 3238 342e 3132 2032 3633 322e  47,-284.12 2632.
-000054c0: 3435 2c2d 3237 362e 3135 2032 3632 322e  45,-276.15 2622.
-000054d0: 3032 2c2d 3237 382e 3033 2032 3632 352e  02,-278.03 2625.
-000054e0: 3437 2c2d 3238 342e 3132 222f 3e0a 3c74  47,-284.12"/>.<t
-000054f0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00005500: 226d 6964 646c 6522 2078 3d22 3235 3835  "middle" x="2585
-00005510: 2e35 2220 793d 222d 3330 392e 3822 2066  .5" y="-309.8" f
-00005520: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00005530: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00005540: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
-00005550: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
-00005560: 3039 202d 2d3e 0a3c 6720 6964 3d22 6e6f  09 -->.<g id="no
-00005570: 6465 3139 2220 636c 6173 733d 226e 6f64  de19" class="nod
-00005580: 6522 3e0a 3c74 6974 6c65 3e41 3039 3c2f  e">.<title>A09</
-00005590: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-000055a0: 6669 6c6c 3d22 2363 6361 3961 6222 2073  fill="#cca9ab" s
-000055b0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-000055c0: 696e 7473 3d22 3236 3332 2e35 2c2d 3137  ints="2632.5,-17
-000055d0: 3520 3234 3930 2e35 2c2d 3137 3520 3234  5 2490.5,-175 24
-000055e0: 3930 2e35 2c2d 3131 3320 3236 3332 2e35  90.5,-113 2632.5
-000055f0: 2c2d 3131 3320 3236 3332 2e35 2c2d 3137  ,-113 2632.5,-17
-00005600: 3522 2f3e 0a3c 7465 7874 2074 6578 742d  5"/>.<text text-
-00005610: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00005620: 3d22 3235 3436 2220 793d 222d 3135 382e  ="2546" y="-158.
-00005630: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00005640: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00005650: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
-00005660: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00005670: 223e 4130 393c 2f74 6578 743e 0a3c 7465  ">A09</text>.<te
-00005680: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00005690: 7374 6172 7422 2078 3d22 3235 3032 2e35  start" x="2502.5
-000056a0: 2220 793d 222d 3134 362e 3422 2066 6f6e  " y="-146.4" fon
-000056b0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000056c0: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
-000056d0: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
-000056e0: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
-000056f0: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
-00005700: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00005710: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00005720: 3d22 3235 3032 2e35 2220 793d 222d 3133  ="2502.5" y="-13
-00005730: 342e 3422 2066 6f6e 742d 6661 6d69 6c79  4.4" font-family
-00005740: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00005750: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
-00005760: 3e43 6c75 7374 6572 2041 626c 6568 6e75  >Cluster Ablehnu
-00005770: 6e67 3c2f 7465 7874 3e0a 3c74 6578 7420  ng</text>.<text 
-00005780: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00005790: 7274 2220 783d 2232 3530 322e 3522 2079  rt" x="2502.5" y
-000057a0: 3d22 2d31 3232 2e34 2220 666f 6e74 2d66  ="-122.4" font-f
-000057b0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-000057c0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-000057d0: 322e 3030 223e 4f42 4953 206e 6963 6874  2.00">OBIS nicht
-000057e0: 2070 6173 7365 6e64 3c2f 7465 7874 3e0a   passend</text>.
-000057f0: 3c2f 673e 0a3c 212d 2d20 3926 2334 353b  </g>.<!-- 9&#45;
-00005800: 2667 743b 4130 3920 2d2d 3e0a 3c67 2069  &gt;A09 -->.<g i
-00005810: 643d 2265 6467 6531 3822 2063 6c61 7373  d="edge18" class
-00005820: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
-00005830: 392d 2667 743b 4130 393c 2f74 6974 6c65  9-&gt;A09</title
-00005840: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00005850: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00005860: 6b22 2064 3d22 4d32 3634 382e 3431 2c2d  k" d="M2648.41,-
-00005870: 3233 382e 3636 4332 3633 342e 3737 2c2d  238.66C2634.77,-
-00005880: 3232 332e 3936 2032 3631 342e 372c 2d32  223.96 2614.7,-2
-00005890: 3032 2e33 3420 3235 3937 2e32 392c 2d31  02.34 2597.29,-1
-000058a0: 3833 2e35 3722 2f3e 0a3c 706f 6c79 676f  83.57"/>.<polygo
-000058b0: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
-000058c0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-000058d0: 696e 7473 3d22 3235 3939 2e39 312c 2d31  ints="2599.91,-1
-000058e0: 3831 2e32 3420 3235 3930 2e35 342c 2d31  81.24 2590.54,-1
-000058f0: 3736 2e32 3920 3235 3934 2e37 382c 2d31  76.29 2594.78,-1
-00005900: 3836 2e30 3120 3235 3939 2e39 312c 2d31  86.01 2599.91,-1
-00005910: 3831 2e32 3422 2f3e 0a3c 7465 7874 2074  81.24"/>.<text t
-00005920: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00005930: 6c65 2220 783d 2232 3633 362e 3522 2079  le" x="2636.5" y
-00005940: 3d22 2d31 3936 2e38 2220 666f 6e74 2d66  ="-196.8" font-f
-00005950: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00005960: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00005970: 342e 3030 223e 4e65 696e 3c2f 7465 7874  4.00">Nein</text
-00005980: 3e0a 3c2f 673e 0a3c 212d 2d20 3130 202d  >.</g>.<!-- 10 -
-00005990: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3230  ->.<g id="node20
-000059a0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
-000059b0: 3c74 6974 6c65 3e31 303c 2f74 6974 6c65  <title>10</title
-000059c0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
-000059d0: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
-000059e0: 6c61 636b 2220 643d 224d 3331 3732 2e35  lack" d="M3172.5
-000059f0: 2c2d 3136 3243 3331 3732 2e35 2c2d 3136  ,-162C3172.5,-16
-00005a00: 3220 3236 3632 2e35 2c2d 3136 3220 3236  2 2662.5,-162 26
-00005a10: 3632 2e35 2c2d 3136 3220 3236 3536 2e35  62.5,-162 2656.5
-00005a20: 2c2d 3136 3220 3236 3530 2e35 2c2d 3135  ,-162 2650.5,-15
-00005a30: 3620 3236 3530 2e35 2c2d 3135 3020 3236  6 2650.5,-150 26
-00005a40: 3530 2e35 2c2d 3135 3020 3236 3530 2e35  50.5,-150 2650.5
-00005a50: 2c2d 3133 3820 3236 3530 2e35 2c2d 3133  ,-138 2650.5,-13
-00005a60: 3820 3236 3530 2e35 2c2d 3133 3220 3236  8 2650.5,-132 26
-00005a70: 3536 2e35 2c2d 3132 3620 3236 3632 2e35  56.5,-126 2662.5
-00005a80: 2c2d 3132 3620 3236 3632 2e35 2c2d 3132  ,-126 2662.5,-12
-00005a90: 3620 3331 3732 2e35 2c2d 3132 3620 3331  6 3172.5,-126 31
-00005aa0: 3732 2e35 2c2d 3132 3620 3331 3738 2e35  72.5,-126 3178.5
-00005ab0: 2c2d 3132 3620 3331 3834 2e35 2c2d 3133  ,-126 3184.5,-13
-00005ac0: 3220 3331 3834 2e35 2c2d 3133 3820 3331  2 3184.5,-138 31
-00005ad0: 3834 2e35 2c2d 3133 3820 3331 3834 2e35  84.5,-138 3184.5
-00005ae0: 2c2d 3135 3020 3331 3834 2e35 2c2d 3135  ,-150 3184.5,-15
-00005af0: 3020 3331 3834 2e35 2c2d 3135 3620 3331  0 3184.5,-156 31
-00005b00: 3738 2e35 2c2d 3136 3220 3331 3732 2e35  78.5,-162 3172.5
-00005b10: 2c2d 3136 3222 2f3e 0a3c 7465 7874 2074  ,-162"/>.<text t
-00005b20: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00005b30: 7422 2078 3d22 3236 3634 2e35 2220 793d  t" x="2664.5" y=
-00005b40: 222d 3134 312e 3322 2066 6f6e 742d 6661  "-141.3" font-fa
-00005b50: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00005b60: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-00005b70: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-00005b80: 2231 342e 3030 223e 3130 3a20 3c2f 7465  "14.00">10: </te
-00005b90: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00005ba0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00005bb0: 2232 3639 342e 3522 2079 3d22 2d31 3431  "2694.5" y="-141
-00005bc0: 2e33 2220 666f 6e74 2d66 616d 696c 793d  .3" font-family=
-00005bd0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00005be0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-00005bf0: 4973 7420 6465 7220 4d61 4269 532d 5a50  Ist der MaBiS-ZP
-00005c00: 207a 756d 205a 6569 7470 756e 6b74 2064   zum Zeitpunkt d
-00005c10: 6572 2041 6b74 6976 6965 7275 6e67 2062  er Aktivierung b
-00005c20: 6572 6569 7473 2061 6b74 6976 6965 7274  ereits aktiviert
-00005c30: 3f3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  ?</text>.</g>.<!
-00005c40: 2d2d 2039 2623 3435 3b26 6774 3b31 3020  -- 9&#45;&gt;10 
-00005c50: 2d2d 3e0a 3c67 2069 643d 2265 6467 6531  -->.<g id="edge1
-00005c60: 3922 2063 6c61 7373 3d22 6564 6765 223e  9" class="edge">
-00005c70: 0a3c 7469 746c 653e 392d 2667 743b 3130  .<title>9-&gt;10
-00005c80: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
-00005c90: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
-00005ca0: 653d 2262 6c61 636b 2220 643d 224d 3237  e="black" d="M27
-00005cb0: 3034 2e33 312c 2d32 3338 2e35 3343 3237  04.31,-238.53C27
-00005cc0: 3438 2e34 332c 2d32 3139 2e31 3820 3238  48.43,-219.18 28
-00005cd0: 3139 2e36 342c 2d31 3837 2e39 3320 3238  19.64,-187.93 28
-00005ce0: 3637 2e34 392c 2d31 3636 2e39 3422 2f3e  67.49,-166.94"/>
-00005cf0: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
-00005d00: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
-00005d10: 6c61 636b 2220 706f 696e 7473 3d22 3238  lack" points="28
-00005d20: 3638 2e37 392c 2d31 3730 2e31 3920 3238  68.79,-170.19 28
-00005d30: 3736 2e35 342c 2d31 3632 2e39 3720 3238  76.54,-162.97 28
-00005d40: 3635 2e39 372c 2d31 3633 2e37 3820 3238  65.97,-163.78 28
-00005d50: 3638 2e37 392c 2d31 3730 2e31 3922 2f3e  68.79,-170.19"/>
-00005d60: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00005d70: 6f72 3d22 6d69 6464 6c65 2220 783d 2232  or="middle" x="2
-00005d80: 3831 332e 3522 2079 3d22 2d31 3936 2e38  813.5" y="-196.8
-00005d90: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00005da0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00005db0: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
-00005dc0: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00005dd0: 2d20 4131 3020 2d2d 3e0a 3c67 2069 643d  - A10 -->.<g id=
-00005de0: 226e 6f64 6532 3122 2063 6c61 7373 3d22  "node21" class="
-00005df0: 6e6f 6465 223e 0a3c 7469 746c 653e 4131  node">.<title>A1
-00005e00: 303c 2f74 6974 6c65 3e0a 3c70 6f6c 7967  0</title>.<polyg
-00005e10: 6f6e 2066 696c 6c3d 2223 6363 6139 6162  on fill="#cca9ab
-00005e20: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00005e30: 2070 6f69 6e74 733d 2232 3931 302e 352c   points="2910.5,
-00005e40: 2d36 3220 3237 3234 2e35 2c2d 3632 2032  -62 2724.5,-62 2
-00005e50: 3732 342e 352c 3020 3239 3130 2e35 2c30  724.5,0 2910.5,0
-00005e60: 2032 3931 302e 352c 2d36 3222 2f3e 0a3c   2910.5,-62"/>.<
-00005e70: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00005e80: 3d22 7374 6172 7422 2078 3d22 3238 3032  ="start" x="2802
-00005e90: 2220 793d 222d 3435 2e38 2220 666f 6e74  " y="-45.8" font
-00005ea0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00005eb0: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-00005ec0: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-00005ed0: 7a65 3d22 3134 2e30 3022 3e41 3130 3c2f  ze="14.00">A10</
-00005ee0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00005ef0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00005f00: 783d 2232 3733 362e 3522 2079 3d22 2d33  x="2736.5" y="-3
-00005f10: 332e 3422 2066 6f6e 742d 6661 6d69 6c79  3.4" font-family
-00005f20: 3d22 5469 6d65 732c 7365 7269 6622 2074  ="Times,serif" t
-00005f30: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
-00005f40: 756e 6465 726c 696e 6522 2066 6f6e 742d  underline" font-
-00005f50: 7369 7a65 3d22 3132 2e30 3022 3e48 696e  size="12.00">Hin
-00005f60: 7765 6973 3a3c 2f74 6578 743e 0a3c 7465  weis:</text>.<te
-00005f70: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00005f80: 7374 6172 7422 2078 3d22 3237 3336 2e35  start" x="2736.5
-00005f90: 2220 793d 222d 3231 2e34 2220 666f 6e74  " y="-21.4" font
-00005fa0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00005fb0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00005fc0: 2231 322e 3030 223e 436c 7573 7465 7220  "12.00">Cluster 
-00005fd0: 4162 6c65 686e 756e 673c 2f74 6578 743e  Ablehnung</text>
-00005fe0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00005ff0: 6f72 3d22 7374 6172 7422 2078 3d22 3237  or="start" x="27
-00006000: 3336 2e35 2220 793d 222d 392e 3422 2066  36.5" y="-9.4" f
-00006010: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00006020: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00006030: 7a65 3d22 3132 2e30 3022 3e4d 6142 6953  ze="12.00">MaBiS
-00006040: 2d5a 5020 6265 7265 6974 7320 616b 7469  -ZP bereits akti
-00006050: 7669 6572 743c 2f74 6578 743e 0a3c 2f67  viert</text>.</g
-00006060: 3e0a 3c21 2d2d 2031 3026 2334 353b 2667  >.<!-- 10&#45;&g
-00006070: 743b 4131 3020 2d2d 3e0a 3c67 2069 643d  t;A10 -->.<g id=
-00006080: 2265 6467 6532 3022 2063 6c61 7373 3d22  "edge20" class="
-00006090: 6564 6765 223e 0a3c 7469 746c 653e 3130  edge">.<title>10
-000060a0: 2d26 6774 3b41 3130 3c2f 7469 746c 653e  -&gt;A10</title>
-000060b0: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
-000060c0: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-000060d0: 2220 643d 224d 3239 3031 2e38 382c 2d31  " d="M2901.88,-1
-000060e0: 3235 2e36 3643 3238 3838 2e36 332c 2d31  25.66C2888.63,-1
-000060f0: 3130 2e39 3620 3238 3639 2e31 352c 2d38  10.96 2869.15,-8
-00006100: 392e 3334 2032 3835 322e 3235 2c2d 3730  9.34 2852.25,-70
-00006110: 2e35 3722 2f3e 0a3c 706f 6c79 676f 6e20  .57"/>.<polygon 
-00006120: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00006130: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
-00006140: 7473 3d22 3238 3535 2c2d 3638 2e34 2032  ts="2855,-68.4 2
-00006150: 3834 352e 3731 2c2d 3633 2e33 3120 3238  845.71,-63.31 28
-00006160: 3439 2e38 2c2d 3733 2e30 3820 3238 3535  49.8,-73.08 2855
-00006170: 2c2d 3638 2e34 222f 3e0a 3c74 6578 7420  ,-68.4"/>.<text 
-00006180: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
-00006190: 646c 6522 2078 3d22 3238 3830 2e35 2220  dle" x="2880.5" 
-000061a0: 793d 222d 3833 2e38 2220 666f 6e74 2d66  y="-83.8" font-f
-000061b0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-000061c0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-000061d0: 342e 3030 223e 4a61 3c2f 7465 7874 3e0a  4.00">Ja</text>.
-000061e0: 3c2f 673e 0a3c 212d 2d20 4131 3120 2d2d  </g>.<!-- A11 --
-000061f0: 3e0a 3c67 2069 643d 226e 6f64 6532 3222  >.<g id="node22"
-00006200: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
-00006210: 7469 746c 653e 4131 313c 2f74 6974 6c65  title>A11</title
-00006220: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
-00006230: 2223 6363 6139 6162 2220 7374 726f 6b65  "#cca9ab" stroke
-00006240: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
-00006250: 2233 3130 362e 352c 2d36 3220 3239 3238  "3106.5,-62 2928
-00006260: 2e35 2c2d 3632 2032 3932 382e 352c 3020  .5,-62 2928.5,0 
-00006270: 3331 3036 2e35 2c30 2033 3130 362e 352c  3106.5,0 3106.5,
-00006280: 2d36 3222 2f3e 0a3c 7465 7874 2074 6578  -62"/>.<text tex
-00006290: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-000062a0: 2078 3d22 3330 3032 2220 793d 222d 3435   x="3002" y="-45
-000062b0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-000062c0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000062d0: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-000062e0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-000062f0: 3022 3e41 3131 3c2f 7465 7874 3e0a 3c74  0">A11</text>.<t
-00006300: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00006310: 2273 7461 7274 2220 783d 2232 3934 302e  "start" x="2940.
-00006320: 3522 2079 3d22 2d33 332e 3422 2066 6f6e  5" y="-33.4" fon
-00006330: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00006340: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
-00006350: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
-00006360: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
-00006370: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
-00006380: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00006390: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-000063a0: 3d22 3239 3430 2e35 2220 793d 222d 3231  ="2940.5" y="-21
-000063b0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
-000063c0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000063d0: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
-000063e0: 436c 7573 7465 723a 205a 7573 7469 6d6d  Cluster: Zustimm
-000063f0: 756e 673c 2f74 6578 743e 0a3c 7465 7874  ung</text>.<text
-00006400: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00006410: 6172 7422 2078 3d22 3239 3430 2e35 2220  art" x="2940.5" 
-00006420: 793d 222d 392e 3422 2066 6f6e 742d 6661  y="-9.4" font-fa
-00006430: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00006440: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
-00006450: 2e30 3022 3e41 6b74 6976 6965 7275 6e67  .00">Aktivierung
-00006460: 2064 7572 6368 6765 6626 2332 3532 3b68   durchgef&#252;h
-00006470: 7274 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  rt</text>.</g>.<
-00006480: 212d 2d20 3130 2623 3435 3b26 6774 3b41  !-- 10&#45;&gt;A
-00006490: 3131 202d 2d3e 0a3c 6720 6964 3d22 6564  11 -->.<g id="ed
-000064a0: 6765 3231 2220 636c 6173 733d 2265 6467  ge21" class="edg
-000064b0: 6522 3e0a 3c74 6974 6c65 3e31 302d 2667  e">.<title>10-&g
-000064c0: 743b 4131 313c 2f74 6974 6c65 3e0a 3c70  t;A11</title>.<p
-000064d0: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
-000064e0: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
-000064f0: 3d22 4d32 3933 332e 3132 2c2d 3132 352e  ="M2933.12,-125.
-00006500: 3636 4332 3934 362e 3337 2c2d 3131 302e  66C2946.37,-110.
-00006510: 3936 2032 3936 352e 3835 2c2d 3839 2e33  96 2965.85,-89.3
-00006520: 3420 3239 3832 2e37 352c 2d37 302e 3537  4 2982.75,-70.57
-00006530: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
-00006540: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-00006550: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
-00006560: 2232 3938 352e 322c 2d37 332e 3038 2032  "2985.2,-73.08 2
-00006570: 3938 392e 3239 2c2d 3633 2e33 3120 3239  989.29,-63.31 29
-00006580: 3830 2c2d 3638 2e34 2032 3938 352e 322c  80,-68.4 2985.2,
-00006590: 2d37 332e 3038 222f 3e0a 3c74 6578 7420  -73.08"/>.<text 
-000065a0: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
-000065b0: 646c 6522 2078 3d22 3239 3930 2e35 2220  dle" x="2990.5" 
-000065c0: 793d 222d 3833 2e38 2220 666f 6e74 2d66  y="-83.8" font-f
-000065d0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-000065e0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-000065f0: 342e 3030 223e 4e65 696e 3c2f 7465 7874  4.00">Nein</text
-00006600: 3e0a 3c2f 673e 0a3c 2f67 3e0a 3c2f 7376  >.</g>.</g>.</sv
-00006610: 673e 0a20 203c 2f67 3e0a 3c2f 7376 673e  g>.  </g>.</svg>
-00006620: 0a                                       .
+000000f0: 203c 673e 0a20 2020 203c 7376 6720 7665   <g>.    <svg ve
+00000100: 7273 696f 6e3d 2231 2e31 2220 7769 6474  rsion="1.1" widt
+00000110: 683d 2234 3235 372e 3333 3333 3333 3333  h="4257.33333333
+00000120: 3333 3333 7078 2220 7669 6577 426f 783d  3333px" viewBox=
+00000130: 2230 2030 2034 3235 372e 3333 3333 3333  "0 0 4257.333333
+00000140: 3333 3333 3333 2031 3830 342e 3022 2068  333333 1804.0" h
+00000150: 6569 6768 743d 2231 3830 342e 3070 7822  eight="1804.0px"
+00000160: 3e0a 2020 3c70 6f6c 7967 6f6e 2066 696c  >.  <polygon fil
+00000170: 6c3d 2223 6633 6631 6636 2220 706f 696e  l="#f3f1f6" poin
+00000180: 7473 3d22 302c 3020 3432 3537 2e33 3333  ts="0,0 4257.333
+00000190: 3333 3333 3333 3333 332c 3020 3432 3537  333333333,0 4257
+000001a0: 2e33 3333 3333 3333 3333 3333 332c 3138  .333333333333,18
+000001b0: 3034 2e30 2030 2c31 3830 342e 3022 2f3e  04.0 0,1804.0"/>
+000001c0: 3c67 3e0a 2020 2020 3c67 2074 7261 6e73  <g>.    <g trans
+000001d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+000001e0: 3134 3037 2e36 3031 3932 3436 3734 3535  1407.60192467455
+000001f0: 3134 2c20 3138 302e 3339 3939 3939 3939  14, 180.39999999
+00000200: 3939 3939 3935 2920 7363 616c 6528 3120  999995) scale(1 
+00000210: 3129 2074 7261 6e73 6c61 7465 2830 2c20  1) translate(0, 
+00000220: 3029 2073 6361 6c65 2838 2e31 3538 3739  0) scale(8.15879
+00000230: 3839 3932 3232 3535 3132 2038 2e31 3538  8992225512 8.158
+00000240: 3739 3839 3932 3232 3535 3132 2920 223e  798992225512) ">
+00000250: 3c73 6f64 6970 6f64 693a 6e61 6d65 6476  <sodipodi:namedv
+00000260: 6965 7720 786d 6c6e 733a 736f 6469 706f  iew xmlns:sodipo
+00000270: 6469 3d22 6874 7470 3a2f 2f73 6f64 6970  di="http://sodip
+00000280: 6f64 692e 736f 7572 6365 666f 7267 652e  odi.sourceforge.
+00000290: 6e65 742f 4454 442f 736f 6469 706f 6469  net/DTD/sodipodi
+000002a0: 2d30 2e64 7464 2220 786d 6c6e 733a 696e  -0.dtd" xmlns:in
+000002b0: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
+000002c0: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
+000002d0: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
+000002e0: 6170 6522 2069 643d 226e 616d 6564 7669  ape" id="namedvi
+000002f0: 6577 3722 2070 6167 6563 6f6c 6f72 3d22  ew7" pagecolor="
+00000300: 2366 6666 6666 6622 2062 6f72 6465 7263  #ffffff" borderc
+00000310: 6f6c 6f72 3d22 2339 3939 3939 3922 2062  olor="#999999" b
+00000320: 6f72 6465 726f 7061 6369 7479 3d22 3122  orderopacity="1"
+00000330: 2069 6e6b 7363 6170 653a 7061 6765 7368   inkscape:pagesh
+00000340: 6164 6f77 3d22 3022 2069 6e6b 7363 6170  adow="0" inkscap
+00000350: 653a 7061 6765 6f70 6163 6974 793d 2230  e:pageopacity="0
+00000360: 2220 696e 6b73 6361 7065 3a70 6167 6563  " inkscape:pagec
+00000370: 6865 636b 6572 626f 6172 643d 2230 2220  heckerboard="0" 
+00000380: 696e 6b73 6361 7065 3a64 6f63 756d 656e  inkscape:documen
+00000390: 742d 756e 6974 733d 226d 6d22 2073 686f  t-units="mm" sho
+000003a0: 7767 7269 643d 2266 616c 7365 2220 6669  wgrid="false" fi
+000003b0: 742d 6d61 7267 696e 2d74 6f70 3d22 3022  t-margin-top="0"
+000003c0: 2066 6974 2d6d 6172 6769 6e2d 6c65 6674   fit-margin-left
+000003d0: 3d22 3022 2066 6974 2d6d 6172 6769 6e2d  ="0" fit-margin-
+000003e0: 7269 6768 743d 2230 2220 6669 742d 6d61  right="0" fit-ma
+000003f0: 7267 696e 2d62 6f74 746f 6d3d 2230 2220  rgin-bottom="0" 
+00000400: 696e 6b73 6361 7065 3a7a 6f6f 6d3d 2230  inkscape:zoom="0
+00000410: 2e36 3430 3532 3332 3922 2069 6e6b 7363  .64052329" inksc
+00000420: 6170 653a 6378 3d22 3133 302e 3336 3231  ape:cx="130.3621
+00000430: 3622 2069 6e6b 7363 6170 653a 6379 3d22  6" inkscape:cy="
+00000440: 3431 322e 3136 3322 2069 6e6b 7363 6170  412.163" inkscap
+00000450: 653a 7769 6e64 6f77 2d77 6964 7468 3d22  e:window-width="
+00000460: 3135 3132 2220 696e 6b73 6361 7065 3a77  1512" inkscape:w
+00000470: 696e 646f 772d 6865 6967 6874 3d22 3931  indow-height="91
+00000480: 3622 2069 6e6b 7363 6170 653a 7769 6e64  6" inkscape:wind
+00000490: 6f77 2d78 3d22 3338 3430 2220 696e 6b73  ow-x="3840" inks
+000004a0: 6361 7065 3a77 696e 646f 772d 793d 2231  cape:window-y="1
+000004b0: 3336 2220 696e 6b73 6361 7065 3a77 696e  36" inkscape:win
+000004c0: 646f 772d 6d61 7869 6d69 7a65 643d 2230  dow-maximized="0
+000004d0: 2220 696e 6b73 6361 7065 3a63 7572 7265  " inkscape:curre
+000004e0: 6e74 2d6c 6179 6572 3d22 6c61 7965 7231  nt-layer="layer1
+000004f0: 222f 3e0a 2020 3c64 6566 7320 6964 3d22  "/>.  <defs id="
+00000500: 6465 6673 3222 3e0a 2020 2020 3c63 6c69  defs2">.    <cli
+00000510: 7050 6174 6820 636c 6970 5061 7468 556e  pPath clipPathUn
+00000520: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+00000530: 5573 6522 2069 643d 2263 6c69 7050 6174  Use" id="clipPat
+00000540: 6832 3322 3e0a 2020 2020 2020 3c70 6174  h23">.      <pat
+00000550: 6820 643d 224d 2030 2c35 3638 2e31 3536  h d="M 0,568.156
+00000560: 2048 2035 3739 2e32 3336 2056 2030 2048   H 579.236 V 0 H
+00000570: 2030 205a 2220 6964 3d22 7061 7468 3231   0 Z" id="path21
+00000580: 222f 3e0a 2020 2020 3c2f 636c 6970 5061  "/>.    </clipPa
+00000590: 7468 3e0a 2020 3c2f 6465 6673 3e0a 2020  th>.  </defs>.  
+000005a0: 3c67 2078 6d6c 6e73 3a69 6e6b 7363 6170  <g xmlns:inkscap
+000005b0: 653d 2268 7474 703a 2f2f 7777 772e 696e  e="http://www.in
+000005c0: 6b73 6361 7065 2e6f 7267 2f6e 616d 6573  kscape.org/names
+000005d0: 7061 6365 732f 696e 6b73 6361 7065 2220  paces/inkscape" 
+000005e0: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+000005f0: 4c61 7965 7220 3122 2069 6e6b 7363 6170  Layer 1" inkscap
+00000600: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
+00000610: 6572 2220 6964 3d22 6c61 7965 7231 2220  er" id="layer1" 
+00000620: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00000630: 6c61 7465 282d 3136 2e35 3431 3933 372c  late(-16.541937,
+00000640: 2d35 352e 3330 3532 3637 2922 3e0a 2020  -55.305267)">.  
+00000650: 2020 3c67 2069 643d 2267 3139 2220 636c    <g id="g19" cl
+00000660: 6970 2d70 6174 683d 2275 726c 2823 636c  ip-path="url(#cl
+00000670: 6970 5061 7468 3233 2922 2074 7261 6e73  ipPath23)" trans
+00000680: 666f 726d 3d22 6d61 7472 6978 2830 2e33  form="matrix(0.3
+00000690: 3532 3737 3737 372c 302c 302c 2d30 2e33  5277777,0,0,-0.3
+000006a0: 3532 3737 3737 372c 302e 3031 3031 3730  5277777,0.010170
+000006b0: 3233 2c32 3433 2e37 3336 3735 2922 2073  23,243.73675)" s
+000006c0: 7479 6c65 3d22 6f70 6163 6974 793a 302e  tyle="opacity:0.
+000006d0: 3222 3e0a 2020 2020 2020 3c67 2069 643d  2">.      <g id=
+000006e0: 2267 3235 2220 7472 616e 7366 6f72 6d3d  "g25" transform=
+000006f0: 2274 7261 6e73 6c61 7465 2831 3232 2e34  "translate(122.4
+00000700: 3434 2c33 322e 3731 3935 2922 3e0a 2020  44,32.7195)">.  
+00000710: 2020 2020 2020 3c70 6174 6820 643d 226d        <path d="m
+00000720: 2030 2c30 2068 202d 3536 2e31 3034 2063   0,0 h -56.104 c
+00000730: 202d 3131 2c30 202d 3139 2e38 3938 2c39   -11,0 -19.898,9
+00000740: 2e31 3233 202d 3139 2e34 3633 2c32 302e  .123 -19.463,20.
+00000750: 3131 3520 3130 2e35 3934 2c32 3637 2e31  115 10.594,267.1
+00000760: 3931 2032 3331 2e32 3737 2c34 3831 2e33  91 231.277,481.3
+00000770: 3032 2035 3031 2e30 3239 2c34 3831 2e33  02 501.029,481.3
+00000780: 3032 2076 202d 3536 2e30 3220 6320 302c  02 v -56.02 c 0,
+00000790: 2d31 302e 3938 202d 382e 3638 382c 2d31  -10.98 -8.688,-1
+000007a0: 392e 3839 3220 2d31 392e 3635 382c 2d32  9.892 -19.658,-2
+000007b0: 302e 3339 3320 4320 3138 302e 3239 2c34  0.393 C 180.29,4
+000007c0: 3134 2e36 3937 2030 2c32 3238 2e30 3035  14.697 0,228.005
+000007d0: 2030 2c30 2220 7374 796c 653d 2266 696c   0,0" style="fil
+000007e0: 6c3a 2336 6561 6438 333b 6669 6c6c 2d6f  l:#6ead83;fill-o
+000007f0: 7061 6369 7479 3a31 3b66 696c 6c2d 7275  pacity:1;fill-ru
+00000800: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
+00000810: 653a 6e6f 6e65 2220 6964 3d22 7061 7468  e:none" id="path
+00000820: 3237 222f 3e0a 2020 2020 2020 3c2f 673e  27"/>.      </g>
+00000830: 0a20 2020 2020 203c 6720 6964 3d22 6732  .      <g id="g2
+00000840: 3922 2074 7261 6e73 666f 726d 3d22 7472  9" transform="tr
+00000850: 616e 736c 6174 6528 3237 332e 3738 3238  anslate(273.7828
+00000860: 2c33 322e 3731 3935 2922 3e0a 2020 2020  ,32.7195)">.    
+00000870: 2020 2020 3c70 6174 6820 643d 226d 2030      <path d="m 0
+00000880: 2c30 2068 202d 3535 2e39 3236 2063 202d  ,0 h -55.926 c -
+00000890: 3131 2e32 3238 2c30 202d 3230 2e30 3931  11.228,0 -20.091
+000008a0: 2c39 2e34 3832 202d 3139 2e34 3335 2c32  ,9.482 -19.435,2
+000008b0: 302e 3639 2031 302e 3734 342c 3138 332e  0.69 10.744,183.
+000008c0: 3433 3920 3136 332e 3338 392c 3332 392e  439 163.389,329.
+000008d0: 3338 3820 3334 392e 3438 352c 3332 392e  388 349.485,329.
+000008e0: 3338 3820 7620 2d35 362e 3236 3320 6320  388 v -56.263 c 
+000008f0: 302c 2d31 302e 3730 3920 2d38 2e32 3733  0,-10.709 -8.273
+00000900: 2c2d 3139 2e36 3137 202d 3138 2e39 3537  ,-19.617 -18.957
+00000910: 2c2d 3230 2e33 3520 4320 3131 322e 3831  ,-20.35 C 112.81
+00000920: 392c 3236 332e 3639 3620 302c 3134 342e  9,263.696 0,144.
+00000930: 3737 3420 302c 3022 2073 7479 6c65 3d22  774 0,0" style="
+00000940: 6669 6c6c 3a23 3665 6164 3833 3b66 696c  fill:#6ead83;fil
+00000950: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
+00000960: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
+00000970: 726f 6b65 3a6e 6f6e 6522 2069 643d 2270  roke:none" id="p
+00000980: 6174 6833 3122 2f3e 0a20 2020 2020 203c  ath31"/>.      <
+00000990: 2f67 3e0a 2020 2020 2020 3c67 2069 643d  /g>.      <g id=
+000009a0: 2267 3333 2220 7472 616e 7366 6f72 6d3d  "g33" transform=
+000009b0: 2274 7261 6e73 6c61 7465 2834 3235 2e37  "translate(425.7
+000009c0: 3636 372c 3332 2e37 3139 3529 223e 0a20  667,32.7195)">. 
+000009d0: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
+000009e0: 6d20 302c 3020 6820 2d35 352e 3434 3520  m 0,0 h -55.445 
+000009f0: 6320 2d31 312e 3635 332c 3020 2d32 302e  c -11.653,0 -20.
+00000a00: 3630 342c 3130 2e31 3720 2d31 392e 3333  604,10.17 -19.33
+00000a10: 342c 3231 2e37 3533 2031 302e 3836 362c  4,21.753 10.866,
+00000a20: 3939 2e30 3332 2039 352e 3033 312c 3137  99.032 95.031,17
+00000a30: 362e 3334 3120 3139 362e 3931 392c 3137  6.341 196.919,17
+00000a40: 362e 3334 3120 7620 2d35 372e 3031 3120  6.341 v -57.011 
+00000a50: 6320 302c 2d31 302e 3034 3620 2d37 2e32  c 0,-10.046 -7.2
+00000a60: 3833 2c2d 3138 2e37 3535 202d 3137 2e32  83,-18.755 -17.2
+00000a70: 3239 2c2d 3230 2e31 3635 2043 2034 352e  29,-20.165 C 45.
+00000a80: 3638 382c 3131 322e 3532 3220 302c 3631  688,112.522 0,61
+00000a90: 2e34 3937 2030 2c30 2220 7374 796c 653d  .497 0,0" style=
+00000aa0: 2266 696c 6c3a 2336 6561 6438 333b 6669  "fill:#6ead83;fi
+00000ab0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00000ac0: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+00000ad0: 7472 6f6b 653a 6e6f 6e65 2220 6964 3d22  troke:none" id="
+00000ae0: 7061 7468 3335 222f 3e0a 2020 2020 2020  path35"/>.      
+00000af0: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
+00000b00: 3c2f 673e 0a3c 2f67 3e0a 2020 2020 3c73  </g>.</g>.    <s
+00000b10: 7667 2077 6964 7468 3d22 3331 3933 7074  vg width="3193pt
+00000b20: 2220 6865 6967 6874 3d22 3133 3533 7074  " height="1353pt
+00000b30: 2220 7669 6577 426f 783d 2230 2e30 3020  " viewBox="0.00 
+00000b40: 302e 3030 2033 3139 322e 3530 2031 3335  0.00 3192.50 135
+00000b50: 332e 3030 223e 0a3c 6720 6964 3d22 6772  3.00">.<g id="gr
+00000b60: 6170 6830 2220 636c 6173 733d 2267 7261  aph0" class="gra
+00000b70: 7068 2220 7472 616e 7366 6f72 6d3d 2273  ph" transform="s
+00000b80: 6361 6c65 2831 2031 2920 726f 7461 7465  cale(1 1) rotate
+00000b90: 2830 2920 7472 616e 736c 6174 6528 3420  (0) translate(4 
+00000ba0: 3133 3439 2922 3e0a 3c74 6974 6c65 3e44  1349)">.<title>D
+00000bb0: 3c2f 7469 746c 653e 0a3c 7465 7874 2074  </title>.<text t
+00000bc0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00000bd0: 7422 2078 3d22 3130 3435 2e37 3522 2079  t" x="1045.75" y
+00000be0: 3d22 2d31 3332 372e 3622 2066 6f6e 742d  ="-1327.6" font-
+00000bf0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00000c00: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+00000c10: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+00000c20: 653d 2231 382e 3030 223e 372e 3137 2041  e="18.00">7.17 A
+00000c30: 443a 2041 6b74 6976 6965 7275 6e67 2065  D: Aktivierung e
+00000c40: 696e 6573 204d 6142 6953 2d5a 5020 6626  ines MaBiS-ZP f&
+00000c50: 2332 3532 3b72 2042 696c 616e 7a69 6572  #252;r Bilanzier
+00000c60: 756e 6773 6765 6269 6574 7373 756d 6d65  ungsgebietssumme
+00000c70: 6e7a 6569 7472 6569 6865 6e20 766f 6d20  nzeitreihen vom 
+00000c80: 2623 3232 303b 4e42 2061 6e20 4249 4b4f  &#220;NB an BIKO
+00000c90: 2075 6e64 204e 423c 2f74 6578 743e 0a3c   und NB</text>.<
+00000ca0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00000cb0: 3d22 7374 6172 7422 2078 3d22 3133 3930  ="start" x="1390
+00000cc0: 2e37 3522 2079 3d22 2d31 3239 372e 3222  .75" y="-1297.2"
+00000cd0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00000ce0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00000cf0: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
+00000d00: 6e74 2d73 697a 653d 2231 362e 3030 223e  nt-size="16.00">
+00000d10: 372e 3137 2e31 2045 5f30 3031 355f 4d61  7.17.1 E_0015_Ma
+00000d20: 4269 532d 5a50 2041 6b74 6976 6965 7275  BiS-ZP Aktivieru
+00000d30: 6e67 2070 7226 2332 3532 3b66 656e 3c2f  ng pr&#252;fen</
+00000d40: 7465 7874 3e0a 3c21 2d2d 2053 7461 7274  text>.<!-- Start
+00000d50: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
+00000d60: 3122 2063 6c61 7373 3d22 6e6f 6465 223e  1" class="node">
+00000d70: 0a3c 7469 746c 653e 5374 6172 743c 2f74  .<title>Start</t
+00000d80: 6974 6c65 3e0a 3c70 6f6c 7967 6f6e 2066  itle>.<polygon f
+00000d90: 696c 6c3d 2223 3761 3864 6131 2220 7374  ill="#7a8da1" st
+00000da0: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+00000db0: 6e74 733d 2233 3532 2c2d 3132 3437 2031  nts="352,-1247 1
+00000dc0: 3737 2c2d 3132 3437 2031 3737 2c2d 3132  77,-1247 177,-12
+00000dd0: 3033 2033 3532 2c2d 3132 3033 2033 3532  03 352,-1203 352
+00000de0: 2c2d 3132 3437 222f 3e0a 3c74 6578 7420  ,-1247"/>.<text 
+00000df0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00000e00: 7274 2220 783d 2232 3336 2220 793d 222d  rt" x="236" y="-
+00000e10: 3132 3237 2e38 2220 666f 6e74 2d66 616d  1227.8" font-fam
+00000e20: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00000e30: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00000e40: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+00000e50: 3134 2e30 3022 3e45 5f30 3031 353c 2f74  14.00">E_0015</t
+00000e60: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00000e70: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00000e80: 3d22 3139 3122 2079 3d22 2d31 3231 352e  ="191" y="-1215.
+00000e90: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00000ea0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00000eb0: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+00000ec0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
+00000ed0: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
+00000ee0: 2d73 697a 653d 2231 322e 3030 223e 5072  -size="12.00">Pr
+00000ef0: 2623 3235 323b 6665 6e64 6520 526f 6c6c  &#252;fende Roll
+00000f00: 653a 3c2f 7465 7874 3e0a 3c74 6578 7420  e:</text>.<text 
+00000f10: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00000f20: 7274 2220 783d 2232 3937 2220 793d 222d  rt" x="297" y="-
+00000f30: 3132 3135 2e34 2220 666f 6e74 2d66 616d  1215.4" font-fam
+00000f40: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00000f50: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00000f60: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+00000f70: 3132 2e30 3022 3e20 4249 4b4f 3c2f 7465  12.00"> BIKO</te
+00000f80: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3120  xt>.</g>.<!-- 1 
+00000f90: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6532  -->.<g id="node2
+00000fa0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
+00000fb0: 3c74 6974 6c65 3e31 3c2f 7469 746c 653e  <title>1</title>
+00000fc0: 0a3c 7061 7468 2066 696c 6c3d 2223 3761  .<path fill="#7a
+00000fd0: 6162 3861 2220 7374 726f 6b65 3d22 626c  ab8a" stroke="bl
+00000fe0: 6163 6b22 2064 3d22 4d35 3137 2c2d 3131  ack" d="M517,-11
+00000ff0: 3636 4335 3137 2c2d 3131 3636 2031 322c  66C517,-1166 12,
+00001000: 2d31 3136 3620 3132 2c2d 3131 3636 2036  -1166 12,-1166 6
+00001010: 2c2d 3131 3636 2030 2c2d 3131 3630 2030  ,-1166 0,-1160 0
+00001020: 2c2d 3131 3534 2030 2c2d 3131 3534 2030  ,-1154 0,-1154 0
+00001030: 2c2d 3131 3432 2030 2c2d 3131 3432 2030  ,-1142 0,-1142 0
+00001040: 2c2d 3131 3336 2036 2c2d 3131 3330 2031  ,-1136 6,-1130 1
+00001050: 322c 2d31 3133 3020 3132 2c2d 3131 3330  2,-1130 12,-1130
+00001060: 2035 3137 2c2d 3131 3330 2035 3137 2c2d   517,-1130 517,-
+00001070: 3131 3330 2035 3233 2c2d 3131 3330 2035  1130 523,-1130 5
+00001080: 3239 2c2d 3131 3336 2035 3239 2c2d 3131  29,-1136 529,-11
+00001090: 3432 2035 3239 2c2d 3131 3432 2035 3239  42 529,-1142 529
+000010a0: 2c2d 3131 3534 2035 3239 2c2d 3131 3534  ,-1154 529,-1154
+000010b0: 2035 3239 2c2d 3131 3630 2035 3233 2c2d   529,-1160 523,-
+000010c0: 3131 3636 2035 3137 2c2d 3131 3636 222f  1166 517,-1166"/
+000010d0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+000010e0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+000010f0: 3422 2079 3d22 2d31 3134 352e 3322 2066  4" y="-1145.3" f
+00001100: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00001110: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
+00001120: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
+00001130: 2d73 697a 653d 2231 342e 3030 223e 313a  -size="14.00">1:
+00001140: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
+00001150: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00001160: 7422 2078 3d22 3334 2220 793d 222d 3131  t" x="34" y="-11
+00001170: 3435 2e33 2220 666f 6e74 2d66 616d 696c  45.3" font-famil
+00001180: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00001190: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+000011a0: 223e 4572 666f 6c67 7420 6469 6520 416b  ">Erfolgt die Ak
+000011b0: 7469 7669 6572 756e 6720 6e61 6368 2041  tivierung nach A
+000011c0: 626c 6175 6620 6465 7220 436c 6561 7269  blauf der Cleari
+000011d0: 6e67 6672 6973 7420 6626 2332 3532 3b72  ngfrist f&#252;r
+000011e0: 2064 6965 204b 424b 413f 3c2f 7465 7874   die KBKA?</text
+000011f0: 3e0a 3c2f 673e 0a3c 212d 2d20 5374 6172  >.</g>.<!-- Star
+00001200: 7426 2334 353b 2667 743b 3120 2d2d 3e0a  t&#45;&gt;1 -->.
+00001210: 3c67 2069 643d 2265 6467 6531 2220 636c  <g id="edge1" cl
+00001220: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00001230: 6c65 3e53 7461 7274 2d26 6774 3b31 3c2f  le>Start-&gt;1</
+00001240: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+00001250: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00001260: 2262 6c61 636b 2220 643d 224d 3236 342e  "black" d="M264.
+00001270: 352c 2d31 3230 322e 3731 4332 3634 2e35  5,-1202.71C264.5
+00001280: 2c2d 3131 3934 2e38 3220 3236 342e 352c  ,-1194.82 264.5,
+00001290: 2d31 3138 352e 3735 2032 3634 2e35 2c2d  -1185.75 264.5,-
+000012a0: 3131 3737 2e33 3322 2f3e 0a3c 706f 6c79  1177.33"/>.<poly
+000012b0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
+000012c0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+000012d0: 706f 696e 7473 3d22 3236 382c 2d31 3137  points="268,-117
+000012e0: 372e 3537 2032 3634 2e35 2c2d 3131 3637  7.57 264.5,-1167
+000012f0: 2e35 3720 3236 312c 2d31 3137 372e 3537  .57 261,-1177.57
+00001300: 2032 3638 2c2d 3131 3737 2e35 3722 2f3e   268,-1177.57"/>
+00001310: 0a3c 2f67 3e0a 3c21 2d2d 2041 3031 202d  .</g>.<!-- A01 -
+00001320: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3322  ->.<g id="node3"
+00001330: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
+00001340: 7469 746c 653e 4130 313c 2f74 6974 6c65  title>A01</title
+00001350: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+00001360: 2223 6366 6239 3836 2220 7374 726f 6b65  "#cfb986" stroke
+00001370: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+00001380: 2233 3139 2c2d 3130 3739 2031 3734 2c2d  "319,-1079 174,-
+00001390: 3130 3739 2031 3734 2c2d 3130 3137 2033  1079 174,-1017 3
+000013a0: 3139 2c2d 3130 3137 2033 3139 2c2d 3130  19,-1017 319,-10
+000013b0: 3739 222f 3e0a 3c74 6578 7420 7465 7874  79"/>.<text text
+000013c0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+000013d0: 783d 2232 3331 2220 793d 222d 3130 3632  x="231" y="-1062
+000013e0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+000013f0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00001400: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
+00001410: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00001420: 3022 3e41 3031 3c2f 7465 7874 3e0a 3c74  0">A01</text>.<t
+00001430: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00001440: 2273 7461 7274 2220 783d 2231 3836 2220  "start" x="186" 
+00001450: 793d 222d 3130 3530 2e34 2220 666f 6e74  y="-1050.4" font
+00001460: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00001470: 6572 6966 2220 7465 7874 2d64 6563 6f72  erif" text-decor
+00001480: 6174 696f 6e3d 2275 6e64 6572 6c69 6e65  ation="underline
+00001490: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+000014a0: 3030 223e 4869 6e77 6569 733a 3c2f 7465  00">Hinweis:</te
+000014b0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+000014c0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+000014d0: 2231 3836 2220 793d 222d 3130 3338 2e34  "186" y="-1038.4
+000014e0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+000014f0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00001500: 2d73 697a 653d 2231 322e 3030 223e 436c  -size="12.00">Cl
+00001510: 7573 7465 7220 4162 6c65 686e 756e 673c  uster Ablehnung<
+00001520: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00001530: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00001540: 2078 3d22 3138 3622 2079 3d22 2d31 3032   x="186" y="-102
+00001550: 362e 3422 2066 6f6e 742d 6661 6d69 6c79  6.4" font-family
+00001560: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00001570: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00001580: 3e46 7269 7374 2623 3235 323b 6265 7273  >Frist&#252;bers
+00001590: 6368 7265 6974 756e 673c 2f74 6578 743e  chreitung</text>
+000015a0: 0a3c 2f67 3e0a 3c21 2d2d 2031 2623 3435  .</g>.<!-- 1&#45
+000015b0: 3b26 6774 3b41 3031 202d 2d3e 0a3c 6720  ;&gt;A01 -->.<g 
+000015c0: 6964 3d22 6564 6765 3222 2063 6c61 7373  id="edge2" class
+000015d0: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
+000015e0: 312d 2667 743b 4130 313c 2f74 6974 6c65  1-&gt;A01</title
+000015f0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
+00001600: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00001610: 6b22 2064 3d22 4d32 3631 2e33 362c 2d31  k" d="M261.36,-1
+00001620: 3132 392e 3933 4332 3539 2e33 372c 2d31  129.93C259.37,-1
+00001630: 3131 392e 3035 2032 3536 2e36 382c 2d31  119.05 256.68,-1
+00001640: 3130 342e 3434 2032 3534 2e31 352c 2d31  104.44 254.15,-1
+00001650: 3039 302e 3634 222f 3e0a 3c70 6f6c 7967  090.64"/>.<polyg
+00001660: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00001670: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00001680: 6f69 6e74 733d 2232 3537 2e35 392c 2d31  oints="257.59,-1
+00001690: 3039 302e 3032 2032 3532 2e33 342c 2d31  090.02 252.34,-1
+000016a0: 3038 302e 3832 2032 3530 2e37 312c 2d31  080.82 250.71,-1
+000016b0: 3039 312e 3238 2032 3537 2e35 392c 2d31  091.28 257.59,-1
+000016c0: 3039 302e 3032 222f 3e0a 3c74 6578 7420  090.02"/>.<text 
+000016d0: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
+000016e0: 646c 6522 2078 3d22 3236 352e 3522 2079  dle" x="265.5" y
+000016f0: 3d22 2d31 3130 302e 3822 2066 6f6e 742d  ="-1100.8" font-
+00001700: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00001710: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00001720: 3134 2e30 3022 3e4a 613c 2f74 6578 743e  14.00">Ja</text>
+00001730: 0a3c 2f67 3e0a 3c21 2d2d 2032 202d 2d3e  .</g>.<!-- 2 -->
+00001740: 0a3c 6720 6964 3d22 6e6f 6465 3422 2063  .<g id="node4" c
+00001750: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
+00001760: 746c 653e 323c 2f74 6974 6c65 3e0a 3c70  tle>2</title>.<p
+00001770: 6174 6820 6669 6c6c 3d22 2337 6161 6238  ath fill="#7aab8
+00001780: 6122 2073 7472 6f6b 653d 2262 6c61 636b  a" stroke="black
+00001790: 2220 643d 224d 3736 312e 352c 2d31 3036  " d="M761.5,-106
+000017a0: 3643 3736 312e 352c 2d31 3036 3620 3334  6C761.5,-1066 34
+000017b0: 392e 352c 2d31 3036 3620 3334 392e 352c  9.5,-1066 349.5,
+000017c0: 2d31 3036 3620 3334 332e 352c 2d31 3036  -1066 343.5,-106
+000017d0: 3620 3333 372e 352c 2d31 3036 3020 3333  6 337.5,-1060 33
+000017e0: 372e 352c 2d31 3035 3420 3333 372e 352c  7.5,-1054 337.5,
+000017f0: 2d31 3035 3420 3333 372e 352c 2d31 3034  -1054 337.5,-104
+00001800: 3220 3333 372e 352c 2d31 3034 3220 3333  2 337.5,-1042 33
+00001810: 372e 352c 2d31 3033 3620 3334 332e 352c  7.5,-1036 343.5,
+00001820: 2d31 3033 3020 3334 392e 352c 2d31 3033  -1030 349.5,-103
+00001830: 3020 3334 392e 352c 2d31 3033 3020 3736  0 349.5,-1030 76
+00001840: 312e 352c 2d31 3033 3020 3736 312e 352c  1.5,-1030 761.5,
+00001850: 2d31 3033 3020 3736 372e 352c 2d31 3033  -1030 767.5,-103
+00001860: 3020 3737 332e 352c 2d31 3033 3620 3737  0 773.5,-1036 77
+00001870: 332e 352c 2d31 3034 3220 3737 332e 352c  3.5,-1042 773.5,
+00001880: 2d31 3034 3220 3737 332e 352c 2d31 3035  -1042 773.5,-105
+00001890: 3420 3737 332e 352c 2d31 3035 3420 3737  4 773.5,-1054 77
+000018a0: 332e 352c 2d31 3036 3020 3736 372e 352c  3.5,-1060 767.5,
+000018b0: 2d31 3036 3620 3736 312e 352c 2d31 3036  -1066 761.5,-106
+000018c0: 3622 2f3e 0a3c 7465 7874 2074 6578 742d  6"/>.<text text-
+000018d0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000018e0: 3d22 3335 312e 3522 2079 3d22 2d31 3034  ="351.5" y="-104
+000018f0: 352e 3322 2066 6f6e 742d 6661 6d69 6c79  5.3" font-family
+00001900: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00001910: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
+00001920: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00001930: 3030 223e 323a 203c 2f74 6578 743e 0a3c  00">2: </text>.<
+00001940: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00001950: 3d22 7374 6172 7422 2078 3d22 3337 312e  ="start" x="371.
+00001960: 3522 2079 3d22 2d31 3034 352e 3322 2066  5" y="-1045.3" f
+00001970: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00001980: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00001990: 7a65 3d22 3134 2e30 3022 3e45 7266 6f6c  ze="14.00">Erfol
+000019a0: 6774 2064 6965 2041 6b74 6976 6965 7275  gt die Aktivieru
+000019b0: 6e67 207a 756d 204d 6f6e 6174 7365 7273  ng zum Monatsers
+000019c0: 7465 6e20 3030 3a30 3020 5568 723f 3c2f  ten 00:00 Uhr?</
+000019d0: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
+000019e0: 3126 2334 353b 2667 743b 3220 2d2d 3e0a  1&#45;&gt;2 -->.
+000019f0: 3c67 2069 643d 2265 6467 6533 2220 636c  <g id="edge3" cl
+00001a00: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00001a10: 6c65 3e31 2d26 6774 3b32 3c2f 7469 746c  le>1-&gt;2</titl
+00001a20: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
+00001a30: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+00001a40: 636b 2220 643d 224d 3331 362e 3139 2c2d  ck" d="M316.19,-
+00001a50: 3131 3239 2e35 3943 3336 352e 3539 2c2d  1129.59C365.59,-
+00001a60: 3131 3132 2e39 3620 3434 302e 3135 2c2d  1112.96 440.15,-
+00001a70: 3130 3837 2e38 3520 3439 322e 392c 2d31  1087.85 492.9,-1
+00001a80: 3037 302e 3038 222f 3e0a 3c70 6f6c 7967  070.08"/>.<polyg
+00001a90: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00001aa0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00001ab0: 6f69 6e74 733d 2234 3934 2e30 312c 2d31  oints="494.01,-1
+00001ac0: 3037 332e 3420 3530 322e 3337 2c2d 3130  073.4 502.37,-10
+00001ad0: 3636 2e38 3920 3439 312e 3737 2c2d 3130  66.89 491.77,-10
+00001ae0: 3636 2e37 3720 3439 342e 3031 2c2d 3130  66.77 494.01,-10
+00001af0: 3733 2e34 222f 3e0a 3c74 6578 7420 7465  73.4"/>.<text te
+00001b00: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00001b10: 6522 2078 3d22 3432 372e 3522 2079 3d22  e" x="427.5" y="
+00001b20: 2d31 3130 302e 3822 2066 6f6e 742d 6661  -1100.8" font-fa
+00001b30: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00001b40: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+00001b50: 2e30 3022 3e4e 6569 6e3c 2f74 6578 743e  .00">Nein</text>
+00001b60: 0a3c 2f67 3e0a 3c21 2d2d 2041 3032 202d  .</g>.<!-- A02 -
+00001b70: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3522  ->.<g id="node5"
+00001b80: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
+00001b90: 7469 746c 653e 4130 323c 2f74 6974 6c65  title>A02</title
+00001ba0: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+00001bb0: 2223 6366 6239 3836 2220 7374 726f 6b65  "#cfb986" stroke
+00001bc0: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+00001bd0: 2235 3835 2c2d 3936 3620 3335 302c 2d39  "585,-966 350,-9
+00001be0: 3636 2033 3530 2c2d 3930 3420 3538 352c  66 350,-904 585,
+00001bf0: 2d39 3034 2035 3835 2c2d 3936 3622 2f3e  -904 585,-966"/>
+00001c00: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00001c10: 6f72 3d22 7374 6172 7422 2078 3d22 3435  or="start" x="45
+00001c20: 3222 2079 3d22 2d39 3439 2e38 2220 666f  2" y="-949.8" fo
+00001c30: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00001c40: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+00001c50: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
+00001c60: 7369 7a65 3d22 3134 2e30 3022 3e41 3032  size="14.00">A02
+00001c70: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+00001c80: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00001c90: 2220 783d 2233 3632 2220 793d 222d 3933  " x="362" y="-93
+00001ca0: 372e 3422 2066 6f6e 742d 6661 6d69 6c79  7.4" font-family
+00001cb0: 3d22 5469 6d65 732c 7365 7269 6622 2074  ="Times,serif" t
+00001cc0: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
+00001cd0: 756e 6465 726c 696e 6522 2066 6f6e 742d  underline" font-
+00001ce0: 7369 7a65 3d22 3132 2e30 3022 3e48 696e  size="12.00">Hin
+00001cf0: 7765 6973 3a3c 2f74 6578 743e 0a3c 7465  weis:</text>.<te
+00001d00: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00001d10: 7374 6172 7422 2078 3d22 3336 3222 2079  start" x="362" y
+00001d20: 3d22 2d39 3235 2e34 2220 666f 6e74 2d66  ="-925.4" font-f
+00001d30: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00001d40: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00001d50: 322e 3030 223e 436c 7573 7465 7220 4162  2.00">Cluster Ab
+00001d60: 6c65 686e 756e 673c 2f74 6578 743e 0a3c  lehnung</text>.<
+00001d70: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00001d80: 3d22 7374 6172 7422 2078 3d22 3336 3222  ="start" x="362"
+00001d90: 2079 3d22 2d39 3133 2e34 2220 666f 6e74   y="-913.4" font
+00001da0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00001db0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00001dc0: 2231 322e 3030 223e 4765 7726 2332 3238  "12.00">Gew&#228
+00001dd0: 3b68 6c74 6572 205a 6569 7470 756e 6b74  ;hlter Zeitpunkt
+00001de0: 206e 6963 6874 207a 756c 2623 3232 383b   nicht zul&#228;
+00001df0: 7373 6967 3c2f 7465 7874 3e0a 3c2f 673e  ssig</text>.</g>
+00001e00: 0a3c 212d 2d20 3226 2334 353b 2667 743b  .<!-- 2&#45;&gt;
+00001e10: 4130 3220 2d2d 3e0a 3c67 2069 643d 2265  A02 -->.<g id="e
+00001e20: 6467 6534 2220 636c 6173 733d 2265 6467  dge4" class="edg
+00001e30: 6522 3e0a 3c74 6974 6c65 3e32 2d26 6774  e">.<title>2-&gt
+00001e40: 3b41 3032 3c2f 7469 746c 653e 0a3c 7061  ;A02</title>.<pa
+00001e50: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
+00001e60: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
+00001e70: 224d 3534 312e 3735 2c2d 3130 3239 2e36  "M541.75,-1029.6
+00001e80: 3643 3533 302e 322c 2d31 3031 352e 3039  6C530.2,-1015.09
+00001e90: 2035 3133 2e32 362c 2d39 3933 2e37 3220   513.26,-993.72 
+00001ea0: 3439 382e 3438 2c2d 3937 352e 3038 222f  498.48,-975.08"/
+00001eb0: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+00001ec0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+00001ed0: 626c 6163 6b22 2070 6f69 6e74 733d 2235  black" points="5
+00001ee0: 3031 2e33 332c 2d39 3733 2e30 3320 3439  01.33,-973.03 49
+00001ef0: 322e 3337 2c2d 3936 372e 3337 2034 3935  2.37,-967.37 495
+00001f00: 2e38 342c 2d39 3737 2e33 3820 3530 312e  .84,-977.38 501.
+00001f10: 3333 2c2d 3937 332e 3033 222f 3e0a 3c74  33,-973.03"/>.<t
+00001f20: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00001f30: 226d 6964 646c 6522 2078 3d22 3533 342e  "middle" x="534.
+00001f40: 3522 2079 3d22 2d39 3837 2e38 2220 666f  5" y="-987.8" fo
+00001f50: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00001f60: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00001f70: 653d 2231 342e 3030 223e 4e65 696e 3c2f  e="14.00">Nein</
+00001f80: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
+00001f90: 3320 2d2d 3e0a 3c67 2069 643d 226e 6f64  3 -->.<g id="nod
+00001fa0: 6536 2220 636c 6173 733d 226e 6f64 6522  e6" class="node"
+00001fb0: 3e0a 3c74 6974 6c65 3e33 3c2f 7469 746c  >.<title>3</titl
+00001fc0: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
+00001fd0: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
+00001fe0: 626c 6163 6b22 2064 3d22 4d39 3035 2e35  black" d="M905.5
+00001ff0: 2c2d 3935 3343 3930 352e 352c 2d39 3533  ,-953C905.5,-953
+00002000: 2036 3135 2e35 2c2d 3935 3320 3631 352e   615.5,-953 615.
+00002010: 352c 2d39 3533 2036 3039 2e35 2c2d 3935  5,-953 609.5,-95
+00002020: 3320 3630 332e 352c 2d39 3437 2036 3033  3 603.5,-947 603
+00002030: 2e35 2c2d 3934 3120 3630 332e 352c 2d39  .5,-941 603.5,-9
+00002040: 3431 2036 3033 2e35 2c2d 3932 3920 3630  41 603.5,-929 60
+00002050: 332e 352c 2d39 3239 2036 3033 2e35 2c2d  3.5,-929 603.5,-
+00002060: 3932 3320 3630 392e 352c 2d39 3137 2036  923 609.5,-917 6
+00002070: 3135 2e35 2c2d 3931 3720 3631 352e 352c  15.5,-917 615.5,
+00002080: 2d39 3137 2039 3035 2e35 2c2d 3931 3720  -917 905.5,-917 
+00002090: 3930 352e 352c 2d39 3137 2039 3131 2e35  905.5,-917 911.5
+000020a0: 2c2d 3931 3720 3931 372e 352c 2d39 3233  ,-917 917.5,-923
+000020b0: 2039 3137 2e35 2c2d 3932 3920 3931 372e   917.5,-929 917.
+000020c0: 352c 2d39 3239 2039 3137 2e35 2c2d 3934  5,-929 917.5,-94
+000020d0: 3120 3931 372e 352c 2d39 3431 2039 3137  1 917.5,-941 917
+000020e0: 2e35 2c2d 3934 3720 3931 312e 352c 2d39  .5,-947 911.5,-9
+000020f0: 3533 2039 3035 2e35 2c2d 3935 3322 2f3e  53 905.5,-953"/>
+00002100: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00002110: 6f72 3d22 7374 6172 7422 2078 3d22 3631  or="start" x="61
+00002120: 372e 3522 2079 3d22 2d39 3332 2e33 2220  7.5" y="-932.3" 
+00002130: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00002140: 6573 2c73 6572 6966 2220 666f 6e74 2d77  es,serif" font-w
+00002150: 6569 6768 743d 2262 6f6c 6422 2066 6f6e  eight="bold" fon
+00002160: 742d 7369 7a65 3d22 3134 2e30 3022 3e33  t-size="14.00">3
+00002170: 3a20 3c2f 7465 7874 3e0a 3c74 6578 7420  : </text>.<text 
+00002180: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00002190: 7274 2220 783d 2236 3337 2e35 2220 793d  rt" x="637.5" y=
+000021a0: 222d 3933 322e 3322 2066 6f6e 742d 6661  "-932.3" font-fa
+000021b0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+000021c0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+000021d0: 2e30 3022 3e49 7374 2064 6965 2072 6963  .00">Ist die ric
+000021e0: 6874 6967 6520 5265 6765 6c7a 6f6e 6520  htige Regelzone 
+000021f0: 616e 6765 6765 6265 6e3c 2f74 6578 743e  angegeben</text>
+00002200: 0a3c 2f67 3e0a 3c21 2d2d 2032 2623 3435  .</g>.<!-- 2&#45
+00002210: 3b26 6774 3b33 202d 2d3e 0a3c 6720 6964  ;&gt;3 -->.<g id
+00002220: 3d22 6564 6765 3522 2063 6c61 7373 3d22  ="edge5" class="
+00002230: 6564 6765 223e 0a3c 7469 746c 653e 322d  edge">.<title>2-
+00002240: 2667 743b 333c 2f74 6974 6c65 3e0a 3c70  &gt;3</title>.<p
+00002250: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
+00002260: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
+00002270: 3d22 4d35 3837 2e35 332c 2d31 3032 392e  ="M587.53,-1029.
+00002280: 3636 4336 3232 2e37 382c 2d31 3031 302e  66C622.78,-1010.
+00002290: 3537 2036 3739 2e35 382c 2d39 3739 2e38  57 679.58,-979.8
+000022a0: 3120 3731 382e 3431 2c2d 3935 382e 3739  1 718.41,-958.79
+000022b0: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
+000022c0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+000022d0: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+000022e0: 2237 3139 2e39 2c2d 3936 312e 3936 2037  "719.9,-961.96 7
+000022f0: 3237 2e30 332c 2d39 3534 2e31 3320 3731  27.03,-954.13 71
+00002300: 362e 3536 2c2d 3935 352e 3831 2037 3139  6.56,-955.81 719
+00002310: 2e39 2c2d 3936 312e 3936 222f 3e0a 3c74  .9,-961.96"/>.<t
+00002320: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00002330: 226d 6964 646c 6522 2078 3d22 3637 372e  "middle" x="677.
+00002340: 3522 2079 3d22 2d39 3837 2e38 2220 666f  5" y="-987.8" fo
+00002350: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00002360: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00002370: 653d 2231 342e 3030 223e 4a61 3c2f 7465  e="14.00">Ja</te
+00002380: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 4130  xt>.</g>.<!-- A0
+00002390: 3320 2d2d 3e0a 3c67 2069 643d 226e 6f64  3 -->.<g id="nod
+000023a0: 6537 2220 636c 6173 733d 226e 6f64 6522  e7" class="node"
+000023b0: 3e0a 3c74 6974 6c65 3e41 3033 3c2f 7469  >.<title>A03</ti
+000023c0: 746c 653e 0a3c 706f 6c79 676f 6e20 6669  tle>.<polygon fi
+000023d0: 6c6c 3d22 2363 6662 3938 3622 2073 7472  ll="#cfb986" str
+000023e0: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
+000023f0: 7473 3d22 3730 392e 352c 2d38 3533 2035  ts="709.5,-853 5
+00002400: 3733 2e35 2c2d 3835 3320 3537 332e 352c  73.5,-853 573.5,
+00002410: 2d37 3931 2037 3039 2e35 2c2d 3739 3120  -791 709.5,-791 
+00002420: 3730 392e 352c 2d38 3533 222f 3e0a 3c74  709.5,-853"/>.<t
+00002430: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00002440: 2273 7461 7274 2220 783d 2236 3236 2220  "start" x="626" 
+00002450: 793d 222d 3833 362e 3822 2066 6f6e 742d  y="-836.8" font-
+00002460: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00002470: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+00002480: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+00002490: 653d 2231 342e 3030 223e 4130 333c 2f74  e="14.00">A03</t
+000024a0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+000024b0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000024c0: 3d22 3538 352e 3522 2079 3d22 2d38 3234  ="585.5" y="-824
+000024d0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+000024e0: 2254 696d 6573 2c73 6572 6966 2220 7465  "Times,serif" te
+000024f0: 7874 2d64 6563 6f72 6174 696f 6e3d 2275  xt-decoration="u
+00002500: 6e64 6572 6c69 6e65 2220 666f 6e74 2d73  nderline" font-s
+00002510: 697a 653d 2231 322e 3030 223e 4869 6e77  ize="12.00">Hinw
+00002520: 6569 733a 3c2f 7465 7874 3e0a 3c74 6578  eis:</text>.<tex
+00002530: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00002540: 7461 7274 2220 783d 2235 3835 2e35 2220  tart" x="585.5" 
+00002550: 793d 222d 3831 322e 3422 2066 6f6e 742d  y="-812.4" font-
+00002560: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00002570: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00002580: 3132 2e30 3022 3e43 6c75 7374 6572 2041  12.00">Cluster A
+00002590: 626c 6568 6e75 6e67 3c2f 7465 7874 3e0a  blehnung</text>.
+000025a0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+000025b0: 723d 2273 7461 7274 2220 783d 2235 3835  r="start" x="585
+000025c0: 2e35 2220 793d 222d 3830 302e 3422 2066  .5" y="-800.4" f
+000025d0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+000025e0: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+000025f0: 7a65 3d22 3132 2e30 3022 3e52 6567 656c  ze="12.00">Regel
+00002600: 7a6f 6e65 2066 616c 7363 683c 2f74 6578  zone falsch</tex
+00002610: 743e 0a3c 2f67 3e0a 3c21 2d2d 2033 2623  t>.</g>.<!-- 3&#
+00002620: 3435 3b26 6774 3b41 3033 202d 2d3e 0a3c  45;&gt;A03 -->.<
+00002630: 6720 6964 3d22 6564 6765 3622 2063 6c61  g id="edge6" cla
+00002640: 7373 3d22 6564 6765 223e 0a3c 7469 746c  ss="edge">.<titl
+00002650: 653e 332d 2667 743b 4130 333c 2f74 6974  e>3-&gt;A03</tit
+00002660: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
+00002670: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
+00002680: 6163 6b22 2064 3d22 4d37 3431 2e39 312c  ack" d="M741.91,
+00002690: 2d39 3136 2e36 3643 3732 352e 3933 2c2d  -916.66C725.93,-
+000026a0: 3930 312e 3736 2037 3032 2e33 342c 2d38  901.76 702.34,-8
+000026b0: 3739 2e37 3520 3638 322e 3034 2c2d 3836  79.75 682.04,-86
+000026c0: 302e 3831 222f 3e0a 3c70 6f6c 7967 6f6e  0.81"/>.<polygon
+000026d0: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+000026e0: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+000026f0: 6e74 733d 2236 3834 2e36 372c 2d38 3538  nts="684.67,-858
+00002700: 2e34 3820 3637 342e 3937 2c2d 3835 342e  .48 674.97,-854.
+00002710: 3232 2036 3739 2e38 392c 2d38 3633 2e36  22 679.89,-863.6
+00002720: 2036 3834 2e36 372c 2d38 3538 2e34 3822   684.67,-858.48"
+00002730: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00002740: 6368 6f72 3d22 6d69 6464 6c65 2220 783d  chor="middle" x=
+00002750: 2237 3235 2e35 2220 793d 222d 3837 342e  "725.5" y="-874.
+00002760: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00002770: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00002780: 742d 7369 7a65 3d22 3134 2e30 3022 3e4e  t-size="14.00">N
+00002790: 6569 6e3c 2f74 6578 743e 0a3c 2f67 3e0a  ein</text>.</g>.
+000027a0: 3c21 2d2d 2034 202d 2d3e 0a3c 6720 6964  <!-- 4 -->.<g id
+000027b0: 3d22 6e6f 6465 3822 2063 6c61 7373 3d22  ="node8" class="
+000027c0: 6e6f 6465 223e 0a3c 7469 746c 653e 343c  node">.<title>4<
+000027d0: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
+000027e0: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
+000027f0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+00002800: 3133 3837 2e35 2c2d 3834 3043 3133 3837  1387.5,-840C1387
+00002810: 2e35 2c2d 3834 3020 3733 392e 352c 2d38  .5,-840 739.5,-8
+00002820: 3430 2037 3339 2e35 2c2d 3834 3020 3733  40 739.5,-840 73
+00002830: 332e 352c 2d38 3430 2037 3237 2e35 2c2d  3.5,-840 727.5,-
+00002840: 3833 3420 3732 372e 352c 2d38 3238 2037  834 727.5,-828 7
+00002850: 3237 2e35 2c2d 3832 3820 3732 372e 352c  27.5,-828 727.5,
+00002860: 2d38 3136 2037 3237 2e35 2c2d 3831 3620  -816 727.5,-816 
+00002870: 3732 372e 352c 2d38 3130 2037 3333 2e35  727.5,-810 733.5
+00002880: 2c2d 3830 3420 3733 392e 352c 2d38 3034  ,-804 739.5,-804
+00002890: 2037 3339 2e35 2c2d 3830 3420 3133 3837   739.5,-804 1387
+000028a0: 2e35 2c2d 3830 3420 3133 3837 2e35 2c2d  .5,-804 1387.5,-
+000028b0: 3830 3420 3133 3933 2e35 2c2d 3830 3420  804 1393.5,-804 
+000028c0: 3133 3939 2e35 2c2d 3831 3020 3133 3939  1399.5,-810 1399
+000028d0: 2e35 2c2d 3831 3620 3133 3939 2e35 2c2d  .5,-816 1399.5,-
+000028e0: 3831 3620 3133 3939 2e35 2c2d 3832 3820  816 1399.5,-828 
+000028f0: 3133 3939 2e35 2c2d 3832 3820 3133 3939  1399.5,-828 1399
+00002900: 2e35 2c2d 3833 3420 3133 3933 2e35 2c2d  .5,-834 1393.5,-
+00002910: 3834 3020 3133 3837 2e35 2c2d 3834 3022  840 1387.5,-840"
+00002920: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00002930: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00002940: 3734 312e 3522 2079 3d22 2d38 3139 2e33  741.5" y="-819.3
+00002950: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00002960: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00002970: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00002980: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00002990: 3e34 3a20 3c2f 7465 7874 3e0a 3c74 6578  >4: </text>.<tex
+000029a0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+000029b0: 7461 7274 2220 783d 2237 3631 2e35 2220  tart" x="761.5" 
+000029c0: 793d 222d 3831 392e 3322 2066 6f6e 742d  y="-819.3" font-
+000029d0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000029e0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+000029f0: 3134 2e30 3022 3e49 7374 2064 6173 2042  14.00">Ist das B
+00002a00: 696c 616e 7a69 6572 756e 6773 6765 6269  ilanzierungsgebi
+00002a10: 6574 207a 756d 2041 6b74 6976 6965 7275  et zum Aktivieru
+00002a20: 6e67 7362 6567 696e 6e20 696e 2064 6572  ngsbeginn in der
+00002a30: 2052 6567 656c 7a6f 6e65 2064 6573 2042   Regelzone des B
+00002a40: 494b 4f20 6726 2332 3532 3b6c 7469 673f  IKO g&#252;ltig?
+00002a50: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00002a60: 2d20 3326 2334 353b 2667 743b 3420 2d2d  - 3&#45;&gt;4 --
+00002a70: 3e0a 3c67 2069 643d 2265 6467 6537 2220  >.<g id="edge7" 
+00002a80: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
+00002a90: 6974 6c65 3e33 2d26 6774 3b34 3c2f 7469  itle>3-&gt;4</ti
+00002aa0: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00002ab0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00002ac0: 6c61 636b 2220 643d 224d 3830 382e 3138  lack" d="M808.18
+00002ad0: 2c2d 3931 362e 3533 4338 3631 2e35 372c  ,-916.53C861.57,
+00002ae0: 2d38 3936 2e39 3820 3934 382e 312c 2d38  -896.98 948.1,-8
+00002af0: 3635 2e32 3720 3130 3035 2e34 2c2d 3834  65.27 1005.4,-84
+00002b00: 342e 3238 222f 3e0a 3c70 6f6c 7967 6f6e  4.28"/>.<polygon
+00002b10: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00002b20: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+00002b30: 6e74 733d 2231 3030 362e 3439 2c2d 3834  nts="1006.49,-84
+00002b40: 372e 3631 2031 3031 342e 3638 2c2d 3834  7.61 1014.68,-84
+00002b50: 302e 3838 2031 3030 342e 3039 2c2d 3834  0.88 1004.09,-84
+00002b60: 312e 3034 2031 3030 362e 3439 2c2d 3834  1.04 1006.49,-84
+00002b70: 372e 3631 222f 3e0a 3c74 6578 7420 7465  7.61"/>.<text te
+00002b80: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00002b90: 6522 2078 3d22 3933 372e 3522 2079 3d22  e" x="937.5" y="
+00002ba0: 2d38 3734 2e38 2220 666f 6e74 2d66 616d  -874.8" font-fam
+00002bb0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00002bc0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00002bd0: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
+00002be0: 673e 0a3c 212d 2d20 4130 3420 2d2d 3e0a  g>.<!-- A04 -->.
+00002bf0: 3c67 2069 643d 226e 6f64 6539 2220 636c  <g id="node9" cl
+00002c00: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00002c10: 6c65 3e41 3034 3c2f 7469 746c 653e 0a3c  le>A04</title>.<
+00002c20: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
+00002c30: 6662 3938 3622 2073 7472 6f6b 653d 2262  fb986" stroke="b
+00002c40: 6c61 636b 2220 706f 696e 7473 3d22 3130  lack" points="10
+00002c50: 3531 2e35 2c2d 3734 3020 3833 352e 352c  51.5,-740 835.5,
+00002c60: 2d37 3430 2038 3335 2e35 2c2d 3637 3820  -740 835.5,-678 
+00002c70: 3130 3531 2e35 2c2d 3637 3820 3130 3531  1051.5,-678 1051
+00002c80: 2e35 2c2d 3734 3022 2f3e 0a3c 7465 7874  .5,-740"/>.<text
+00002c90: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00002ca0: 6172 7422 2078 3d22 3932 3822 2079 3d22  art" x="928" y="
+00002cb0: 2d37 3233 2e38 2220 666f 6e74 2d66 616d  -723.8" font-fam
+00002cc0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00002cd0: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00002ce0: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+00002cf0: 3134 2e30 3022 3e41 3034 3c2f 7465 7874  14.00">A04</text
+00002d00: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00002d10: 686f 723d 2273 7461 7274 2220 783d 2238  hor="start" x="8
+00002d20: 3437 2e35 2220 793d 222d 3731 312e 3422  47.5" y="-711.4"
+00002d30: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00002d40: 6d65 732c 7365 7269 6622 2074 6578 742d  mes,serif" text-
+00002d50: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00002d60: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00002d70: 3d22 3132 2e30 3022 3e48 696e 7765 6973  ="12.00">Hinweis
+00002d80: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00002d90: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00002da0: 7422 2078 3d22 3834 372e 3522 2079 3d22  t" x="847.5" y="
+00002db0: 2d36 3939 2e34 2220 666f 6e74 2d66 616d  -699.4" font-fam
+00002dc0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00002dd0: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+00002de0: 3030 223e 436c 7573 7465 7220 4162 6c65  00">Cluster Able
+00002df0: 686e 756e 673c 2f74 6578 743e 0a3c 7465  hnung</text>.<te
+00002e00: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00002e10: 7374 6172 7422 2078 3d22 3834 372e 3522  start" x="847.5"
+00002e20: 2079 3d22 2d36 3837 2e34 2220 666f 6e74   y="-687.4" font
+00002e30: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00002e40: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00002e50: 2231 322e 3030 223e 4269 6c61 6e7a 6965  "12.00">Bilanzie
+00002e60: 7275 6e67 7367 6562 6965 7420 6e69 6368  rungsgebiet nich
+00002e70: 7420 6726 2332 3532 3b6c 7469 673c 2f74  t g&#252;ltig</t
+00002e80: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2034  ext>.</g>.<!-- 4
+00002e90: 2623 3435 3b26 6774 3b41 3034 202d 2d3e  &#45;&gt;A04 -->
+00002ea0: 0a3c 6720 6964 3d22 6564 6765 3822 2063  .<g id="edge8" c
+00002eb0: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
+00002ec0: 746c 653e 342d 2667 743b 4130 343c 2f74  tle>4-&gt;A04</t
+00002ed0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
+00002ee0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
+00002ef0: 626c 6163 6b22 2064 3d22 4d31 3034 342e  black" d="M1044.
+00002f00: 3735 2c2d 3830 332e 3636 4331 3032 382e  75,-803.66C1028.
+00002f10: 3634 2c2d 3738 382e 3736 2031 3030 342e  64,-788.76 1004.
+00002f20: 3835 2c2d 3736 362e 3735 2039 3834 2e33  85,-766.75 984.3
+00002f30: 382c 2d37 3437 2e38 3122 2f3e 0a3c 706f  8,-747.81"/>.<po
+00002f40: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
+00002f50: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
+00002f60: 2220 706f 696e 7473 3d22 3938 362e 3936  " points="986.96
+00002f70: 2c2d 3734 352e 3433 2039 3737 2e32 342c  ,-745.43 977.24,
+00002f80: 2d37 3431 2e32 3120 3938 322e 3231 2c2d  -741.21 982.21,-
+00002f90: 3735 302e 3537 2039 3836 2e39 362c 2d37  750.57 986.96,-7
+00002fa0: 3435 2e34 3322 2f3e 0a3c 7465 7874 2074  45.43"/>.<text t
+00002fb0: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
+00002fc0: 6c65 2220 783d 2231 3032 382e 3522 2079  le" x="1028.5" y
+00002fd0: 3d22 2d37 3631 2e38 2220 666f 6e74 2d66  ="-761.8" font-f
+00002fe0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00002ff0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00003000: 342e 3030 223e 4e65 696e 3c2f 7465 7874  4.00">Nein</text
+00003010: 3e0a 3c2f 673e 0a3c 212d 2d20 3520 2d2d  >.</g>.<!-- 5 --
+00003020: 3e0a 3c67 2069 643d 226e 6f64 6531 3022  >.<g id="node10"
+00003030: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
+00003040: 7469 746c 653e 353c 2f74 6974 6c65 3e0a  title>5</title>.
+00003050: 3c70 6174 6820 6669 6c6c 3d22 2337 6161  <path fill="#7aa
+00003060: 6238 6122 2073 7472 6f6b 653d 2262 6c61  b8a" stroke="bla
+00003070: 636b 2220 643d 224d 3136 3535 2e35 2c2d  ck" d="M1655.5,-
+00003080: 3732 3743 3136 3535 2e35 2c2d 3732 3720  727C1655.5,-727 
+00003090: 3130 3831 2e35 2c2d 3732 3720 3130 3831  1081.5,-727 1081
+000030a0: 2e35 2c2d 3732 3720 3130 3735 2e35 2c2d  .5,-727 1075.5,-
+000030b0: 3732 3720 3130 3639 2e35 2c2d 3732 3120  727 1069.5,-721 
+000030c0: 3130 3639 2e35 2c2d 3731 3520 3130 3639  1069.5,-715 1069
+000030d0: 2e35 2c2d 3731 3520 3130 3639 2e35 2c2d  .5,-715 1069.5,-
+000030e0: 3730 3320 3130 3639 2e35 2c2d 3730 3320  703 1069.5,-703 
+000030f0: 3130 3639 2e35 2c2d 3639 3720 3130 3735  1069.5,-697 1075
+00003100: 2e35 2c2d 3639 3120 3130 3831 2e35 2c2d  .5,-691 1081.5,-
+00003110: 3639 3120 3130 3831 2e35 2c2d 3639 3120  691 1081.5,-691 
+00003120: 3136 3535 2e35 2c2d 3639 3120 3136 3535  1655.5,-691 1655
+00003130: 2e35 2c2d 3639 3120 3136 3631 2e35 2c2d  .5,-691 1661.5,-
+00003140: 3639 3120 3136 3637 2e35 2c2d 3639 3720  691 1667.5,-697 
+00003150: 3136 3637 2e35 2c2d 3730 3320 3136 3637  1667.5,-703 1667
+00003160: 2e35 2c2d 3730 3320 3136 3637 2e35 2c2d  .5,-703 1667.5,-
+00003170: 3731 3520 3136 3637 2e35 2c2d 3731 3520  715 1667.5,-715 
+00003180: 3136 3637 2e35 2c2d 3732 3120 3136 3631  1667.5,-721 1661
+00003190: 2e35 2c2d 3732 3720 3136 3535 2e35 2c2d  .5,-727 1655.5,-
+000031a0: 3732 3722 2f3e 0a3c 7465 7874 2074 6578  727"/>.<text tex
+000031b0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+000031c0: 2078 3d22 3130 3833 2e35 2220 793d 222d   x="1083.5" y="-
+000031d0: 3730 362e 3322 2066 6f6e 742d 6661 6d69  706.3" font-fami
+000031e0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+000031f0: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
+00003200: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
+00003210: 342e 3030 223e 353a 203c 2f74 6578 743e  4.00">5: </text>
+00003220: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00003230: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
+00003240: 3033 2e35 2220 793d 222d 3730 362e 3322  03.5" y="-706.3"
+00003250: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00003260: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00003270: 7369 7a65 3d22 3134 2e30 3022 3e49 7374  size="14.00">Ist
+00003280: 2064 6572 2026 2332 3230 3b4e 4220 7a75   der &#220;NB zu
+00003290: 6d20 416b 7469 7669 6572 756e 6773 6265  m Aktivierungsbe
+000032a0: 6769 6e6e 2066 2623 3235 323b 7220 6461  ginn f&#252;r da
+000032b0: 7320 4269 6c61 6e7a 6965 7275 6e67 7367  s Bilanzierungsg
+000032c0: 6562 6965 7420 7a75 7374 2623 3232 383b  ebiet zust&#228;
+000032d0: 6e64 6967 3f3c 2f74 6578 743e 0a3c 2f67  ndig?</text>.</g
+000032e0: 3e0a 3c21 2d2d 2034 2623 3435 3b26 6774  >.<!-- 4&#45;&gt
+000032f0: 3b35 202d 2d3e 0a3c 6720 6964 3d22 6564  ;5 -->.<g id="ed
+00003300: 6765 3922 2063 6c61 7373 3d22 6564 6765  ge9" class="edge
+00003310: 223e 0a3c 7469 746c 653e 342d 2667 743b  ">.<title>4-&gt;
+00003320: 353c 2f74 6974 6c65 3e0a 3c70 6174 6820  5</title>.<path 
+00003330: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00003340: 6b65 3d22 626c 6163 6b22 2064 3d22 4d31  ke="black" d="M1
+00003350: 3131 312e 3439 2c2d 3830 332e 3533 4331  111.49,-803.53C1
+00003360: 3136 352e 3135 2c2d 3738 3420 3132 3532  165.15,-784 1252
+00003370: 2e30 382c 2d37 3532 2e33 3720 3133 3039  .08,-752.37 1309
+00003380: 2e37 372c 2d37 3331 2e33 3822 2f3e 0a3c  .77,-731.38"/>.<
+00003390: 706f 6c79 676f 6e20 6669 6c6c 3d22 626c  polygon fill="bl
+000033a0: 6163 6b22 2073 7472 6f6b 653d 2262 6c61  ack" stroke="bla
+000033b0: 636b 2220 706f 696e 7473 3d22 3133 3130  ck" points="1310
+000033c0: 2e39 312c 2d37 3334 2e36 3820 3133 3139  .91,-734.68 1319
+000033d0: 2e31 312c 2d37 3237 2e39 3720 3133 3038  .11,-727.97 1308
+000033e0: 2e35 322c 2d37 3238 2e31 2031 3331 302e  .52,-728.1 1310.
+000033f0: 3931 2c2d 3733 342e 3638 222f 3e0a 3c74  91,-734.68"/>.<t
+00003400: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00003410: 226d 6964 646c 6522 2078 3d22 3132 3431  "middle" x="1241
+00003420: 2e35 2220 793d 222d 3736 312e 3822 2066  .5" y="-761.8" f
+00003430: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00003440: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00003450: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
+00003460: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
+00003470: 3035 202d 2d3e 0a3c 6720 6964 3d22 6e6f  05 -->.<g id="no
+00003480: 6465 3131 2220 636c 6173 733d 226e 6f64  de11" class="nod
+00003490: 6522 3e0a 3c74 6974 6c65 3e41 3035 3c2f  e">.<title>A05</
+000034a0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
+000034b0: 6669 6c6c 3d22 2363 6662 3938 3622 2073  fill="#cfb986" s
+000034c0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
+000034d0: 696e 7473 3d22 3133 3335 2c2d 3632 3720  ints="1335,-627 
+000034e0: 3131 3932 2c2d 3632 3720 3131 3932 2c2d  1192,-627 1192,-
+000034f0: 3536 3520 3133 3335 2c2d 3536 3520 3133  565 1335,-565 13
+00003500: 3335 2c2d 3632 3722 2f3e 0a3c 7465 7874  35,-627"/>.<text
+00003510: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00003520: 6172 7422 2078 3d22 3132 3438 2220 793d  art" x="1248" y=
+00003530: 222d 3631 302e 3822 2066 6f6e 742d 6661  "-610.8" font-fa
+00003540: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00003550: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+00003560: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+00003570: 2231 342e 3030 223e 4130 353c 2f74 6578  "14.00">A05</tex
+00003580: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00003590: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+000035a0: 3132 3034 2220 793d 222d 3539 382e 3422  1204" y="-598.4"
+000035b0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+000035c0: 6d65 732c 7365 7269 6622 2074 6578 742d  mes,serif" text-
+000035d0: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+000035e0: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+000035f0: 3d22 3132 2e30 3022 3e48 696e 7765 6973  ="12.00">Hinweis
+00003600: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00003610: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00003620: 7422 2078 3d22 3132 3034 2220 793d 222d  t" x="1204" y="-
+00003630: 3538 362e 3422 2066 6f6e 742d 6661 6d69  586.4" font-fami
+00003640: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00003650: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
+00003660: 3022 3e43 6c75 7374 6572 2041 626c 6568  0">Cluster Ableh
+00003670: 6e75 6e67 3c2f 7465 7874 3e0a 3c74 6578  nung</text>.<tex
+00003680: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00003690: 7461 7274 2220 783d 2231 3230 3422 2079  tart" x="1204" y
+000036a0: 3d22 2d35 3734 2e34 2220 666f 6e74 2d66  ="-574.4" font-f
+000036b0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+000036c0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+000036d0: 322e 3030 223e 4b65 696e 6520 4265 7265  2.00">Keine Bere
+000036e0: 6368 7469 6775 6e67 3c2f 7465 7874 3e0a  chtigung</text>.
+000036f0: 3c2f 673e 0a3c 212d 2d20 3526 2334 353b  </g>.<!-- 5&#45;
+00003700: 2667 743b 4130 3520 2d2d 3e0a 3c67 2069  &gt;A05 -->.<g i
+00003710: 643d 2265 6467 6531 3022 2063 6c61 7373  d="edge10" class
+00003720: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
+00003730: 352d 2667 743b 4130 353c 2f74 6974 6c65  5-&gt;A05</title
+00003740: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
+00003750: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00003760: 6b22 2064 3d22 4d31 3335 322e 3039 2c2d  k" d="M1352.09,-
+00003770: 3639 302e 3636 4331 3333 382e 3133 2c2d  690.66C1338.13,-
+00003780: 3637 352e 3839 2031 3331 372e 3535 2c2d  675.89 1317.55,-
+00003790: 3635 342e 3134 2031 3239 392e 3735 2c2d  654.14 1299.75,-
+000037a0: 3633 352e 3332 222f 3e0a 3c70 6f6c 7967  635.32"/>.<polyg
+000037b0: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+000037c0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+000037d0: 6f69 6e74 733d 2231 3330 322e 3531 2c2d  oints="1302.51,-
+000037e0: 3633 332e 3134 2031 3239 332e 3039 2c2d  633.14 1293.09,-
+000037f0: 3632 382e 3238 2031 3239 372e 3432 2c2d  628.28 1297.42,-
+00003800: 3633 372e 3935 2031 3330 322e 3531 2c2d  637.95 1302.51,-
+00003810: 3633 332e 3134 222f 3e0a 3c74 6578 7420  633.14"/>.<text 
+00003820: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
+00003830: 646c 6522 2078 3d22 3133 3339 2e35 2220  dle" x="1339.5" 
+00003840: 793d 222d 3634 382e 3822 2066 6f6e 742d  y="-648.8" font-
+00003850: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00003860: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00003870: 3134 2e30 3022 3e4e 6569 6e3c 2f74 6578  14.00">Nein</tex
+00003880: 743e 0a3c 2f67 3e0a 3c21 2d2d 2036 202d  t>.</g>.<!-- 6 -
+00003890: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3132  ->.<g id="node12
+000038a0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
+000038b0: 3c74 6974 6c65 3e36 3c2f 7469 746c 653e  <title>6</title>
+000038c0: 0a3c 7061 7468 2066 696c 6c3d 2223 3761  .<path fill="#7a
+000038d0: 6162 3861 2220 7374 726f 6b65 3d22 626c  ab8a" stroke="bl
+000038e0: 6163 6b22 2064 3d22 4d31 3838 382c 2d36  ack" d="M1888,-6
+000038f0: 3134 4331 3838 382c 2d36 3134 2031 3336  14C1888,-614 136
+00003900: 352c 2d36 3134 2031 3336 352c 2d36 3134  5,-614 1365,-614
+00003910: 2031 3335 392c 2d36 3134 2031 3335 332c   1359,-614 1353,
+00003920: 2d36 3038 2031 3335 332c 2d36 3032 2031  -608 1353,-602 1
+00003930: 3335 332c 2d36 3032 2031 3335 332c 2d35  353,-602 1353,-5
+00003940: 3930 2031 3335 332c 2d35 3930 2031 3335  90 1353,-590 135
+00003950: 332c 2d35 3834 2031 3335 392c 2d35 3738  3,-584 1359,-578
+00003960: 2031 3336 352c 2d35 3738 2031 3336 352c   1365,-578 1365,
+00003970: 2d35 3738 2031 3838 382c 2d35 3738 2031  -578 1888,-578 1
+00003980: 3838 382c 2d35 3738 2031 3839 342c 2d35  888,-578 1894,-5
+00003990: 3738 2031 3930 302c 2d35 3834 2031 3930  78 1900,-584 190
+000039a0: 302c 2d35 3930 2031 3930 302c 2d35 3930  0,-590 1900,-590
+000039b0: 2031 3930 302c 2d36 3032 2031 3930 302c   1900,-602 1900,
+000039c0: 2d36 3032 2031 3930 302c 2d36 3038 2031  -602 1900,-608 1
+000039d0: 3839 342c 2d36 3134 2031 3838 382c 2d36  894,-614 1888,-6
+000039e0: 3134 222f 3e0a 3c74 6578 7420 7465 7874  14"/>.<text text
+000039f0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00003a00: 783d 2231 3336 3722 2079 3d22 2d35 3933  x="1367" y="-593
+00003a10: 2e33 2220 666f 6e74 2d66 616d 696c 793d  .3" font-family=
+00003a20: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00003a30: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
+00003a40: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00003a50: 3022 3e36 3a20 3c2f 7465 7874 3e0a 3c74  0">6: </text>.<t
+00003a60: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00003a70: 2273 7461 7274 2220 783d 2231 3338 3722  "start" x="1387"
+00003a80: 2079 3d22 2d35 3933 2e33 2220 666f 6e74   y="-593.3" font
+00003a90: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00003aa0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00003ab0: 2231 342e 3030 223e 4578 6973 7469 6572  "14.00">Existier
+00003ac0: 7420 6265 7265 6974 7320 6569 6e20 6162  t bereits ein ab
+00003ad0: 7765 6963 6865 6e64 6573 2054 7570 656c  weichendes Tupel
+00003ae0: 2075 6e74 6572 2064 6572 2049 4420 6465   unter der ID de
+00003af0: 7320 4d61 4269 532d 5a50 3f3c 2f74 6578  s MaBiS-ZP?</tex
+00003b00: 743e 0a3c 2f67 3e0a 3c21 2d2d 2035 2623  t>.</g>.<!-- 5&#
+00003b10: 3435 3b26 6774 3b36 202d 2d3e 0a3c 6720  45;&gt;6 -->.<g 
+00003b20: 6964 3d22 6564 6765 3131 2220 636c 6173  id="edge11" clas
+00003b30: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
+00003b40: 3e35 2d26 6774 3b36 3c2f 7469 746c 653e  >5-&gt;6</title>
+00003b50: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
+00003b60: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00003b70: 2220 643d 224d 3134 3039 2e31 2c2d 3639  " d="M1409.1,-69
+00003b80: 302e 3533 4331 3435 342e 3138 2c2d 3637  0.53C1454.18,-67
+00003b90: 312e 3134 2031 3532 372e 3032 2c2d 3633  1.14 1527.02,-63
+00003ba0: 392e 3820 3135 3735 2e38 312c 2d36 3138  9.8 1575.81,-618
+00003bb0: 2e38 3122 2f3e 0a3c 706f 6c79 676f 6e20  .81"/>.<polygon 
+00003bc0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+00003bd0: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
+00003be0: 7473 3d22 3135 3736 2e39 352c 2d36 3232  ts="1576.95,-622
+00003bf0: 2e31 3320 3135 3834 2e37 352c 2d36 3134  .13 1584.75,-614
+00003c00: 2e39 3620 3135 3734 2e31 382c 2d36 3135  .96 1574.18,-615
+00003c10: 2e37 2031 3537 362e 3935 2c2d 3632 322e  .7 1576.95,-622.
+00003c20: 3133 222f 3e0a 3c74 6578 7420 7465 7874  13"/>.<text text
+00003c30: 2d61 6e63 686f 723d 226d 6964 646c 6522  -anchor="middle"
+00003c40: 2078 3d22 3135 3230 2e35 2220 793d 222d   x="1520.5" y="-
+00003c50: 3634 382e 3822 2066 6f6e 742d 6661 6d69  648.8" font-fami
+00003c60: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00003c70: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00003c80: 3022 3e4a 613c 2f74 6578 743e 0a3c 2f67  0">Ja</text>.</g
+00003c90: 3e0a 3c21 2d2d 2041 3036 202d 2d3e 0a3c  >.<!-- A06 -->.<
+00003ca0: 6720 6964 3d22 6e6f 6465 3133 2220 636c  g id="node13" cl
+00003cb0: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00003cc0: 6c65 3e41 3036 3c2f 7469 746c 653e 0a3c  le>A06</title>.<
+00003cd0: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
+00003ce0: 6662 3938 3622 2073 7472 6f6b 653d 2262  fb986" stroke="b
+00003cf0: 6c61 636b 2220 706f 696e 7473 3d22 3135  lack" points="15
+00003d00: 3731 2c2d 3531 3420 3132 3832 2c2d 3531  71,-514 1282,-51
+00003d10: 3420 3132 3832 2c2d 3435 3220 3135 3731  4 1282,-452 1571
+00003d20: 2c2d 3435 3220 3135 3731 2c2d 3531 3422  ,-452 1571,-514"
+00003d30: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00003d40: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00003d50: 3134 3131 2220 793d 222d 3439 372e 3822  1411" y="-497.8"
+00003d60: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00003d70: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00003d80: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
+00003d90: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00003da0: 4130 363c 2f74 6578 743e 0a3c 7465 7874  A06</text>.<text
+00003db0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00003dc0: 6172 7422 2078 3d22 3132 3934 2220 793d  art" x="1294" y=
+00003dd0: 222d 3438 352e 3422 2066 6f6e 742d 6661  "-485.4" font-fa
+00003de0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00003df0: 6622 2074 6578 742d 6465 636f 7261 7469  f" text-decorati
+00003e00: 6f6e 3d22 756e 6465 726c 696e 6522 2066  on="underline" f
+00003e10: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00003e20: 3e48 696e 7765 6973 3a3c 2f74 6578 743e  >Hinweis:</text>
+00003e30: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00003e40: 6f72 3d22 7374 6172 7422 2078 3d22 3132  or="start" x="12
+00003e50: 3934 2220 793d 222d 3437 332e 3422 2066  94" y="-473.4" f
+00003e60: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00003e70: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00003e80: 7a65 3d22 3132 2e30 3022 3e43 6c75 7374  ze="12.00">Clust
+00003e90: 6572 2041 626c 6568 6e75 6e67 3c2f 7465  er Ablehnung</te
+00003ea0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00003eb0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00003ec0: 2231 3239 3422 2079 3d22 2d34 3631 2e34  "1294" y="-461.4
+00003ed0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00003ee0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00003ef0: 2d73 697a 653d 2231 322e 3030 223e 4162  -size="12.00">Ab
+00003f00: 7765 6963 6865 6e64 6572 204d 6142 6953  weichender MaBiS
+00003f10: 2d5a 5020 6265 7265 6974 7320 766f 7268  -ZP bereits vorh
+00003f20: 616e 6465 6e3c 2f74 6578 743e 0a3c 2f67  anden</text>.</g
+00003f30: 3e0a 3c21 2d2d 2036 2623 3435 3b26 6774  >.<!-- 6&#45;&gt
+00003f40: 3b41 3036 202d 2d3e 0a3c 6720 6964 3d22  ;A06 -->.<g id="
+00003f50: 6564 6765 3132 2220 636c 6173 733d 2265  edge12" class="e
+00003f60: 6467 6522 3e0a 3c74 6974 6c65 3e36 2d26  dge">.<title>6-&
+00003f70: 6774 3b41 3036 3c2f 7469 746c 653e 0a3c  gt;A06</title>.<
+00003f80: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
+00003f90: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00003fa0: 643d 224d 3135 3935 2e32 352c 2d35 3737  d="M1595.25,-577
+00003fb0: 2e36 3643 3135 3637 2e34 332c 2d35 3632  .66C1567.43,-562
+00003fc0: 2e32 3220 3135 3235 2e38 362c 2d35 3339  .22 1525.86,-539
+00003fd0: 2e31 3420 3134 3930 2e39 342c 2d35 3139  .14 1490.94,-519
+00003fe0: 2e37 3622 2f3e 0a3c 706f 6c79 676f 6e20  .76"/>.<polygon 
+00003ff0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
+00004000: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
+00004010: 7473 3d22 3134 3933 2e30 352c 2d35 3136  ts="1493.05,-516
+00004020: 2e39 3320 3134 3832 2e36 312c 2d35 3135  .93 1482.61,-515
+00004030: 2e31 3420 3134 3839 2e36 352c 2d35 3233  .14 1489.65,-523
+00004040: 2e30 3520 3134 3933 2e30 352c 2d35 3136  .05 1493.05,-516
+00004050: 2e39 3322 2f3e 0a3c 7465 7874 2074 6578  .93"/>.<text tex
+00004060: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
+00004070: 2220 783d 2231 3534 352e 3522 2079 3d22  " x="1545.5" y="
+00004080: 2d35 3335 2e38 2220 666f 6e74 2d66 616d  -535.8" font-fam
+00004090: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+000040a0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+000040b0: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
+000040c0: 673e 0a3c 212d 2d20 3720 2d2d 3e0a 3c67  g>.<!-- 7 -->.<g
+000040d0: 2069 643d 226e 6f64 6531 3422 2063 6c61   id="node14" cla
+000040e0: 7373 3d22 6e6f 6465 223e 0a3c 7469 746c  ss="node">.<titl
+000040f0: 653e 373c 2f74 6974 6c65 3e0a 3c70 6174  e>7</title>.<pat
+00004100: 6820 6669 6c6c 3d22 2337 6161 6238 6122  h fill="#7aab8a"
+00004110: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00004120: 643d 224d 3237 3739 2e35 2c2d 3530 3143  d="M2779.5,-501C
+00004130: 3237 3739 2e35 2c2d 3530 3120 3136 3031  2779.5,-501 1601
+00004140: 2e35 2c2d 3530 3120 3136 3031 2e35 2c2d  .5,-501 1601.5,-
+00004150: 3530 3120 3135 3935 2e35 2c2d 3530 3120  501 1595.5,-501 
+00004160: 3135 3839 2e35 2c2d 3439 3520 3135 3839  1589.5,-495 1589
+00004170: 2e35 2c2d 3438 3920 3135 3839 2e35 2c2d  .5,-489 1589.5,-
+00004180: 3438 3920 3135 3839 2e35 2c2d 3437 3720  489 1589.5,-477 
+00004190: 3135 3839 2e35 2c2d 3437 3720 3135 3839  1589.5,-477 1589
+000041a0: 2e35 2c2d 3437 3120 3135 3935 2e35 2c2d  .5,-471 1595.5,-
+000041b0: 3436 3520 3136 3031 2e35 2c2d 3436 3520  465 1601.5,-465 
+000041c0: 3136 3031 2e35 2c2d 3436 3520 3237 3739  1601.5,-465 2779
+000041d0: 2e35 2c2d 3436 3520 3237 3739 2e35 2c2d  .5,-465 2779.5,-
+000041e0: 3436 3520 3237 3835 2e35 2c2d 3436 3520  465 2785.5,-465 
+000041f0: 3237 3931 2e35 2c2d 3437 3120 3237 3931  2791.5,-471 2791
+00004200: 2e35 2c2d 3437 3720 3237 3931 2e35 2c2d  .5,-477 2791.5,-
+00004210: 3437 3720 3237 3931 2e35 2c2d 3438 3920  477 2791.5,-489 
+00004220: 3237 3931 2e35 2c2d 3438 3920 3237 3931  2791.5,-489 2791
+00004230: 2e35 2c2d 3439 3520 3237 3835 2e35 2c2d  .5,-495 2785.5,-
+00004240: 3530 3120 3237 3739 2e35 2c2d 3530 3122  501 2779.5,-501"
+00004250: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00004260: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00004270: 3136 3033 2e35 2220 793d 222d 3438 302e  1603.5" y="-480.
+00004280: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
+00004290: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+000042a0: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+000042b0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+000042c0: 223e 373a 203c 2f74 6578 743e 0a3c 7465  ">7: </text>.<te
+000042d0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000042e0: 7374 6172 7422 2078 3d22 3136 3233 2e35  start" x="1623.5
+000042f0: 2220 793d 222d 3438 302e 3322 2066 6f6e  " y="-480.3" fon
+00004300: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00004310: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00004320: 3d22 3134 2e30 3022 3e45 7869 7374 6965  ="14.00">Existie
+00004330: 7274 2062 6572 6569 7473 2066 2623 3235  rt bereits f&#25
+00004340: 323b 7220 6461 7320 6765 6e61 6e6e 7465  2;r das genannte
+00004350: 2054 7570 656c 2061 7573 2041 6767 7265   Tupel aus Aggre
+00004360: 6761 7469 6f6e 732d 7665 7261 6e74 776f  gations-verantwo
+00004370: 7274 6c69 6368 6572 2c20 4269 6c61 6e7a  rtlicher, Bilanz
+00004380: 6965 7275 6e67 7367 6562 6965 742c 2053  ierungsgebiet, S
+00004390: 7061 6e6e 756e 6773 6562 656e 6520 756e  pannungsebene un
+000043a0: 6420 5a52 5420 6569 6e65 2061 6277 6569  d ZRT eine abwei
+000043b0: 6368 656e 6465 2049 4420 6465 7320 4d61  chende ID des Ma
+000043c0: 4269 532d 5a50 3f3c 2f74 6578 743e 0a3c  BiS-ZP?</text>.<
+000043d0: 2f67 3e0a 3c21 2d2d 2036 2623 3435 3b26  /g>.<!-- 6&#45;&
+000043e0: 6774 3b37 202d 2d3e 0a3c 6720 6964 3d22  gt;7 -->.<g id="
+000043f0: 6564 6765 3133 2220 636c 6173 733d 2265  edge13" class="e
+00004400: 6467 6522 3e0a 3c74 6974 6c65 3e36 2d26  dge">.<title>6-&
+00004410: 6774 3b37 3c2f 7469 746c 653e 0a3c 7061  gt;7</title>.<pa
+00004420: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
+00004430: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
+00004440: 224d 3137 3135 2e32 352c 2d35 3737 2e35  "M1715.25,-577.5
+00004450: 3343 3138 3137 2e32 362c 2d35 3537 2e34  3C1817.26,-557.4
+00004460: 3620 3139 3834 2e33 2c2d 3532 342e 3538  6 1984.3,-524.58
+00004470: 2032 3039 302e 3734 2c2d 3530 332e 3633   2090.74,-503.63
+00004480: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
+00004490: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+000044a0: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+000044b0: 2232 3039 312e 3139 2c2d 3530 372e 3131  "2091.19,-507.11
+000044c0: 2032 3130 302e 3332 2c2d 3530 312e 3735   2100.32,-501.75
+000044d0: 2032 3038 392e 3833 2c2d 3530 302e 3234   2089.83,-500.24
+000044e0: 2032 3039 312e 3139 2c2d 3530 372e 3131   2091.19,-507.11
+000044f0: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+00004500: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
+00004510: 3d22 3139 3539 2e35 2220 793d 222d 3533  ="1959.5" y="-53
+00004520: 352e 3822 2066 6f6e 742d 6661 6d69 6c79  5.8" font-family
+00004530: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00004540: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00004550: 3e4e 6569 6e3c 2f74 6578 743e 0a3c 2f67  >Nein</text>.</g
+00004560: 3e0a 3c21 2d2d 2041 3037 202d 2d3e 0a3c  >.<!-- A07 -->.<
+00004570: 6720 6964 3d22 6e6f 6465 3135 2220 636c  g id="node15" cl
+00004580: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00004590: 6c65 3e41 3037 3c2f 7469 746c 653e 0a3c  le>A07</title>.<
+000045a0: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
+000045b0: 6662 3938 3622 2073 7472 6f6b 653d 2262  fb986" stroke="b
+000045c0: 6c61 636b 2220 706f 696e 7473 3d22 3232  lack" points="22
+000045d0: 3530 2e35 2c2d 3430 3120 3139 3230 2e35  50.5,-401 1920.5
+000045e0: 2c2d 3430 3120 3139 3230 2e35 2c2d 3333  ,-401 1920.5,-33
+000045f0: 3920 3232 3530 2e35 2c2d 3333 3920 3232  9 2250.5,-339 22
+00004600: 3530 2e35 2c2d 3430 3122 2f3e 0a3c 7465  50.5,-401"/>.<te
+00004610: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00004620: 7374 6172 7422 2078 3d22 3230 3730 2220  start" x="2070" 
+00004630: 793d 222d 3338 342e 3822 2066 6f6e 742d  y="-384.8" font-
+00004640: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00004650: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+00004660: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+00004670: 653d 2231 342e 3030 223e 4130 373c 2f74  e="14.00">A07</t
+00004680: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00004690: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000046a0: 3d22 3139 3332 2e35 2220 793d 222d 3337  ="1932.5" y="-37
+000046b0: 322e 3422 2066 6f6e 742d 6661 6d69 6c79  2.4" font-family
+000046c0: 3d22 5469 6d65 732c 7365 7269 6622 2074  ="Times,serif" t
+000046d0: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
+000046e0: 756e 6465 726c 696e 6522 2066 6f6e 742d  underline" font-
+000046f0: 7369 7a65 3d22 3132 2e30 3022 3e48 696e  size="12.00">Hin
+00004700: 7765 6973 3a3c 2f74 6578 743e 0a3c 7465  weis:</text>.<te
+00004710: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00004720: 7374 6172 7422 2078 3d22 3139 3332 2e35  start" x="1932.5
+00004730: 2220 793d 222d 3336 302e 3422 2066 6f6e  " y="-360.4" fon
+00004740: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00004750: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00004760: 3d22 3132 2e30 3022 3e43 6c75 7374 6572  ="12.00">Cluster
+00004770: 2041 626c 6568 6e75 6e67 3c2f 7465 7874   Ablehnung</text
+00004780: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00004790: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+000047a0: 3933 322e 3522 2079 3d22 2d33 3438 2e34  932.5" y="-348.4
+000047b0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+000047c0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+000047d0: 2d73 697a 653d 2231 322e 3030 223e 4162  -size="12.00">Ab
+000047e0: 7765 6963 6865 6e64 6520 4944 207a 756d  weichende ID zum
+000047f0: 204d 6142 6953 2d5a 5020 6265 7265 6974   MaBiS-ZP bereit
+00004800: 7320 766f 7268 616e 6465 6e3c 2f74 6578  s vorhanden</tex
+00004810: 743e 0a3c 2f67 3e0a 3c21 2d2d 2037 2623  t>.</g>.<!-- 7&#
+00004820: 3435 3b26 6774 3b41 3037 202d 2d3e 0a3c  45;&gt;A07 -->.<
+00004830: 6720 6964 3d22 6564 6765 3134 2220 636c  g id="edge14" cl
+00004840: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00004850: 6c65 3e37 2d26 6774 3b41 3037 3c2f 7469  le>7-&gt;A07</ti
+00004860: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00004870: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00004880: 6c61 636b 2220 643d 224d 3231 3734 2e30  lack" d="M2174.0
+00004890: 392c 2d34 3634 2e36 3643 3231 3630 2e31  9,-464.66C2160.1
+000048a0: 332c 2d34 3439 2e38 3920 3231 3339 2e35  3,-449.89 2139.5
+000048b0: 352c 2d34 3238 2e31 3420 3231 3231 2e37  5,-428.14 2121.7
+000048c0: 352c 2d34 3039 2e33 3222 2f3e 0a3c 706f  5,-409.32"/>.<po
+000048d0: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
+000048e0: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
+000048f0: 2220 706f 696e 7473 3d22 3231 3234 2e35  " points="2124.5
+00004900: 312c 2d34 3037 2e31 3420 3231 3135 2e30  1,-407.14 2115.0
+00004910: 392c 2d34 3032 2e32 3820 3231 3139 2e34  9,-402.28 2119.4
+00004920: 322c 2d34 3131 2e39 3520 3231 3234 2e35  2,-411.95 2124.5
+00004930: 312c 2d34 3037 2e31 3422 2f3e 0a3c 7465  1,-407.14"/>.<te
+00004940: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00004950: 6d69 6464 6c65 2220 783d 2232 3135 312e  middle" x="2151.
+00004960: 3522 2079 3d22 2d34 3232 2e38 2220 666f  5" y="-422.8" fo
+00004970: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00004980: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00004990: 653d 2231 342e 3030 223e 4a61 3c2f 7465  e="14.00">Ja</te
+000049a0: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3820  xt>.</g>.<!-- 8 
+000049b0: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6531  -->.<g id="node1
+000049c0: 3622 2063 6c61 7373 3d22 6e6f 6465 223e  6" class="node">
+000049d0: 0a3c 7469 746c 653e 383c 2f74 6974 6c65  .<title>8</title
+000049e0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
+000049f0: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
+00004a00: 6c61 636b 2220 643d 224d 3236 3536 2e35  lack" d="M2656.5
+00004a10: 2c2d 3338 3843 3236 3536 2e35 2c2d 3338  ,-388C2656.5,-38
+00004a20: 3820 3232 3830 2e35 2c2d 3338 3820 3232  8 2280.5,-388 22
+00004a30: 3830 2e35 2c2d 3338 3820 3232 3734 2e35  80.5,-388 2274.5
+00004a40: 2c2d 3338 3820 3232 3638 2e35 2c2d 3338  ,-388 2268.5,-38
+00004a50: 3220 3232 3638 2e35 2c2d 3337 3620 3232  2 2268.5,-376 22
+00004a60: 3638 2e35 2c2d 3337 3620 3232 3638 2e35  68.5,-376 2268.5
+00004a70: 2c2d 3336 3420 3232 3638 2e35 2c2d 3336  ,-364 2268.5,-36
+00004a80: 3420 3232 3638 2e35 2c2d 3335 3820 3232  4 2268.5,-358 22
+00004a90: 3734 2e35 2c2d 3335 3220 3232 3830 2e35  74.5,-352 2280.5
+00004aa0: 2c2d 3335 3220 3232 3830 2e35 2c2d 3335  ,-352 2280.5,-35
+00004ab0: 3220 3236 3536 2e35 2c2d 3335 3220 3236  2 2656.5,-352 26
+00004ac0: 3536 2e35 2c2d 3335 3220 3236 3632 2e35  56.5,-352 2662.5
+00004ad0: 2c2d 3335 3220 3236 3638 2e35 2c2d 3335  ,-352 2668.5,-35
+00004ae0: 3820 3236 3638 2e35 2c2d 3336 3420 3236  8 2668.5,-364 26
+00004af0: 3638 2e35 2c2d 3336 3420 3236 3638 2e35  68.5,-364 2668.5
+00004b00: 2c2d 3337 3620 3236 3638 2e35 2c2d 3337  ,-376 2668.5,-37
+00004b10: 3620 3236 3638 2e35 2c2d 3338 3220 3236  6 2668.5,-382 26
+00004b20: 3632 2e35 2c2d 3338 3820 3236 3536 2e35  62.5,-388 2656.5
+00004b30: 2c2d 3338 3822 2f3e 0a3c 7465 7874 2074  ,-388"/>.<text t
+00004b40: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00004b50: 7422 2078 3d22 3232 3832 2e35 2220 793d  t" x="2282.5" y=
+00004b60: 222d 3336 372e 3322 2066 6f6e 742d 6661  "-367.3" font-fa
+00004b70: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00004b80: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+00004b90: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+00004ba0: 2231 342e 3030 223e 383a 203c 2f74 6578  "14.00">8: </tex
+00004bb0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00004bc0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00004bd0: 3233 3032 2e35 2220 793d 222d 3336 372e  2302.5" y="-367.
+00004be0: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
+00004bf0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00004c00: 742d 7369 7a65 3d22 3134 2e30 3022 3e49  t-size="14.00">I
+00004c10: 7374 2064 6572 2026 2332 3230 3b4e 4220  st der &#220;NB 
+00004c20: 7a75 7220 416b 7469 7669 6572 756e 6720  zur Aktivierung 
+00004c30: 6465 7320 5a52 5420 6265 7265 6368 7469  des ZRT berechti
+00004c40: 6774 3f3c 2f74 6578 743e 0a3c 2f67 3e0a  gt?</text>.</g>.
+00004c50: 3c21 2d2d 2037 2623 3435 3b26 6774 3b38  <!-- 7&#45;&gt;8
+00004c60: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
+00004c70: 3135 2220 636c 6173 733d 2265 6467 6522  15" class="edge"
+00004c80: 3e0a 3c74 6974 6c65 3e37 2d26 6774 3b38  >.<title>7-&gt;8
+00004c90: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+00004ca0: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00004cb0: 653d 2262 6c61 636b 2220 643d 224d 3232  e="black" d="M22
+00004cc0: 3334 2e32 342c 2d34 3634 2e35 3343 3232  34.24,-464.53C22
+00004cd0: 3833 2e30 322c 2d34 3435 2e30 3620 3233  83.02,-445.06 23
+00004ce0: 3631 2e39 362c 2d34 3133 2e35 3420 3234  61.96,-413.54 24
+00004cf0: 3134 2e35 342c 2d33 3932 2e35 3522 2f3e  14.54,-392.55"/>
+00004d00: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00004d10: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+00004d20: 6c61 636b 2220 706f 696e 7473 3d22 3234  lack" points="24
+00004d30: 3135 2e36 322c 2d33 3935 2e38 3820 3234  15.62,-395.88 24
+00004d40: 3233 2e36 312c 2d33 3838 2e39 3320 3234  23.61,-388.93 24
+00004d50: 3133 2e30 322c 2d33 3839 2e33 3820 3234  13.02,-389.38 24
+00004d60: 3135 2e36 322c 2d33 3935 2e38 3822 2f3e  15.62,-395.88"/>
+00004d70: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00004d80: 6f72 3d22 6d69 6464 6c65 2220 783d 2232  or="middle" x="2
+00004d90: 3336 332e 3522 2079 3d22 2d34 3232 2e38  363.5" y="-422.8
+00004da0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00004db0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00004dc0: 2d73 697a 653d 2231 342e 3030 223e 4e65  -size="14.00">Ne
+00004dd0: 696e 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  in</text>.</g>.<
+00004de0: 212d 2d20 4130 3820 2d2d 3e0a 3c67 2069  !-- A08 -->.<g i
+00004df0: 643d 226e 6f64 6531 3722 2063 6c61 7373  d="node17" class
+00004e00: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
+00004e10: 4130 383c 2f74 6974 6c65 3e0a 3c70 6f6c  A08</title>.<pol
+00004e20: 7967 6f6e 2066 696c 6c3d 2223 6366 6239  ygon fill="#cfb9
+00004e30: 3836 2220 7374 726f 6b65 3d22 626c 6163  86" stroke="blac
+00004e40: 6b22 2070 6f69 6e74 733d 2232 3439 362c  k" points="2496,
+00004e50: 2d32 3838 2032 3237 332c 2d32 3838 2032  -288 2273,-288 2
+00004e60: 3237 332c 2d32 3236 2032 3439 362c 2d32  273,-226 2496,-2
+00004e70: 3236 2032 3439 362c 2d32 3838 222f 3e0a  26 2496,-288"/>.
+00004e80: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00004e90: 723d 2273 7461 7274 2220 783d 2232 3336  r="start" x="236
+00004ea0: 3922 2079 3d22 2d32 3731 2e38 2220 666f  9" y="-271.8" fo
+00004eb0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00004ec0: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+00004ed0: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
+00004ee0: 7369 7a65 3d22 3134 2e30 3022 3e41 3038  size="14.00">A08
+00004ef0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+00004f00: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00004f10: 2220 783d 2232 3238 3522 2079 3d22 2d32  " x="2285" y="-2
+00004f20: 3539 2e34 2220 666f 6e74 2d66 616d 696c  59.4" font-famil
+00004f30: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00004f40: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
+00004f50: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
+00004f60: 2d73 697a 653d 2231 322e 3030 223e 4869  -size="12.00">Hi
+00004f70: 6e77 6569 733a 3c2f 7465 7874 3e0a 3c74  nweis:</text>.<t
+00004f80: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00004f90: 2273 7461 7274 2220 783d 2232 3238 3522  "start" x="2285"
+00004fa0: 2079 3d22 2d32 3437 2e34 2220 666f 6e74   y="-247.4" font
+00004fb0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00004fc0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00004fd0: 2231 322e 3030 223e 436c 7573 7465 7220  "12.00">Cluster 
+00004fe0: 4162 6c65 686e 756e 673c 2f74 6578 743e  Ablehnung</text>
+00004ff0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00005000: 6f72 3d22 7374 6172 7422 2078 3d22 3232  or="start" x="22
+00005010: 3835 2220 793d 222d 3233 352e 3422 2066  85" y="-235.4" f
+00005020: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00005030: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00005040: 7a65 3d22 3132 2e30 3022 3e5a 5254 2041  ze="12.00">ZRT A
+00005050: 6b74 6976 6965 7275 6e67 206e 6963 6874  ktivierung nicht
+00005060: 2062 6572 6563 6874 6967 743c 2f74 6578   berechtigt</tex
+00005070: 743e 0a3c 2f67 3e0a 3c21 2d2d 2038 2623  t>.</g>.<!-- 8&#
+00005080: 3435 3b26 6774 3b41 3038 202d 2d3e 0a3c  45;&gt;A08 -->.<
+00005090: 6720 6964 3d22 6564 6765 3136 2220 636c  g id="edge16" cl
+000050a0: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+000050b0: 6c65 3e38 2d26 6774 3b41 3038 3c2f 7469  le>8-&gt;A08</ti
+000050c0: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+000050d0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+000050e0: 6c61 636b 2220 643d 224d 3234 3535 2e33  lack" d="M2455.3
+000050f0: 382c 2d33 3531 2e36 3643 3234 3434 2e34  8,-351.66C2444.4
+00005100: 2c2d 3333 372e 3136 2032 3432 382e 3333  ,-337.16 2428.33
+00005110: 2c2d 3331 352e 3932 2032 3431 342e 3237  ,-315.92 2414.27
+00005120: 2c2d 3239 372e 3333 222f 3e0a 3c70 6f6c  ,-297.33"/>.<pol
+00005130: 7967 6f6e 2066 696c 6c3d 2262 6c61 636b  ygon fill="black
+00005140: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00005150: 2070 6f69 6e74 733d 2232 3431 372e 3038   points="2417.08
+00005160: 2c2d 3239 352e 3235 2032 3430 382e 3236  ,-295.25 2408.26
+00005170: 2c2d 3238 392e 3339 2032 3431 312e 352c  ,-289.39 2411.5,
+00005180: 2d32 3939 2e34 3820 3234 3137 2e30 382c  -299.48 2417.08,
+00005190: 2d32 3935 2e32 3522 2f3e 0a3c 7465 7874  -295.25"/>.<text
+000051a0: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
+000051b0: 6464 6c65 2220 783d 2232 3434 392e 3522  ddle" x="2449.5"
+000051c0: 2079 3d22 2d33 3039 2e38 2220 666f 6e74   y="-309.8" font
+000051d0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+000051e0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+000051f0: 2231 342e 3030 223e 4e65 696e 3c2f 7465  "14.00">Nein</te
+00005200: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3920  xt>.</g>.<!-- 9 
+00005210: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6531  -->.<g id="node1
+00005220: 3822 2063 6c61 7373 3d22 6e6f 6465 223e  8" class="node">
+00005230: 0a3c 7469 746c 653e 393c 2f74 6974 6c65  .<title>9</title
+00005240: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
+00005250: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
+00005260: 6c61 636b 2220 643d 224d 3238 3032 2e35  lack" d="M2802.5
+00005270: 2c2d 3237 3543 3238 3032 2e35 2c2d 3237  ,-275C2802.5,-27
+00005280: 3520 3235 3236 2e35 2c2d 3237 3520 3235  5 2526.5,-275 25
+00005290: 3236 2e35 2c2d 3237 3520 3235 3230 2e35  26.5,-275 2520.5
+000052a0: 2c2d 3237 3520 3235 3134 2e35 2c2d 3236  ,-275 2514.5,-26
+000052b0: 3920 3235 3134 2e35 2c2d 3236 3320 3235  9 2514.5,-263 25
+000052c0: 3134 2e35 2c2d 3236 3320 3235 3134 2e35  14.5,-263 2514.5
+000052d0: 2c2d 3235 3120 3235 3134 2e35 2c2d 3235  ,-251 2514.5,-25
+000052e0: 3120 3235 3134 2e35 2c2d 3234 3520 3235  1 2514.5,-245 25
+000052f0: 3230 2e35 2c2d 3233 3920 3235 3236 2e35  20.5,-239 2526.5
+00005300: 2c2d 3233 3920 3235 3236 2e35 2c2d 3233  ,-239 2526.5,-23
+00005310: 3920 3238 3032 2e35 2c2d 3233 3920 3238  9 2802.5,-239 28
+00005320: 3032 2e35 2c2d 3233 3920 3238 3038 2e35  02.5,-239 2808.5
+00005330: 2c2d 3233 3920 3238 3134 2e35 2c2d 3234  ,-239 2814.5,-24
+00005340: 3520 3238 3134 2e35 2c2d 3235 3120 3238  5 2814.5,-251 28
+00005350: 3134 2e35 2c2d 3235 3120 3238 3134 2e35  14.5,-251 2814.5
+00005360: 2c2d 3236 3320 3238 3134 2e35 2c2d 3236  ,-263 2814.5,-26
+00005370: 3320 3238 3134 2e35 2c2d 3236 3920 3238  3 2814.5,-269 28
+00005380: 3038 2e35 2c2d 3237 3520 3238 3032 2e35  08.5,-275 2802.5
+00005390: 2c2d 3237 3522 2f3e 0a3c 7465 7874 2074  ,-275"/>.<text t
+000053a0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+000053b0: 7422 2078 3d22 3235 3238 2e35 2220 793d  t" x="2528.5" y=
+000053c0: 222d 3235 342e 3322 2066 6f6e 742d 6661  "-254.3" font-fa
+000053d0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+000053e0: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+000053f0: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+00005400: 2231 342e 3030 223e 393a 203c 2f74 6578  "14.00">9: </tex
+00005410: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00005420: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00005430: 3235 3438 2e35 2220 793d 222d 3235 342e  2548.5" y="-254.
+00005440: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
+00005450: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00005460: 742d 7369 7a65 3d22 3134 2e30 3022 3e50  t-size="14.00">P
+00005470: 6173 7374 2064 6965 204f 4249 532d 4b65  asst die OBIS-Ke
+00005480: 6e6e 7a61 686c 207a 756d 205a 5254 3f3c  nnzahl zum ZRT?<
+00005490: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+000054a0: 2038 2623 3435 3b26 6774 3b39 202d 2d3e   8&#45;&gt;9 -->
+000054b0: 0a3c 6720 6964 3d22 6564 6765 3137 2220  .<g id="edge17" 
+000054c0: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
+000054d0: 6974 6c65 3e38 2d26 6774 3b39 3c2f 7469  itle>8-&gt;9</ti
+000054e0: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+000054f0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00005500: 6c61 636b 2220 643d 224d 3234 3939 2e31  lack" d="M2499.1
+00005510: 322c 2d33 3531 2e36 3643 3235 3332 2e36  2,-351.66C2532.6
+00005520: 382c 2d33 3332 2e36 3520 3235 3836 2e36  8,-332.65 2586.6
+00005530: 372c 2d33 3032 2e30 3820 3236 3233 2e37  7,-302.08 2623.7
+00005540: 382c 2d32 3831 2e30 3622 2f3e 0a3c 706f  8,-281.06"/>.<po
+00005550: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
+00005560: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
+00005570: 2220 706f 696e 7473 3d22 3236 3235 2e34  " points="2625.4
+00005580: 372c 2d32 3834 2e31 3220 3236 3332 2e34  7,-284.12 2632.4
+00005590: 352c 2d32 3736 2e31 3520 3236 3232 2e30  5,-276.15 2622.0
+000055a0: 322c 2d32 3738 2e30 3320 3236 3235 2e34  2,-278.03 2625.4
+000055b0: 372c 2d32 3834 2e31 3222 2f3e 0a3c 7465  7,-284.12"/>.<te
+000055c0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000055d0: 6d69 6464 6c65 2220 783d 2232 3538 352e  middle" x="2585.
+000055e0: 3522 2079 3d22 2d33 3039 2e38 2220 666f  5" y="-309.8" fo
+000055f0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00005600: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00005610: 653d 2231 342e 3030 223e 4a61 3c2f 7465  e="14.00">Ja</te
+00005620: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 4130  xt>.</g>.<!-- A0
+00005630: 3920 2d2d 3e0a 3c67 2069 643d 226e 6f64  9 -->.<g id="nod
+00005640: 6531 3922 2063 6c61 7373 3d22 6e6f 6465  e19" class="node
+00005650: 223e 0a3c 7469 746c 653e 4130 393c 2f74  ">.<title>A09</t
+00005660: 6974 6c65 3e0a 3c70 6f6c 7967 6f6e 2066  itle>.<polygon f
+00005670: 696c 6c3d 2223 6366 6239 3836 2220 7374  ill="#cfb986" st
+00005680: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+00005690: 6e74 733d 2232 3633 322e 352c 2d31 3735  nts="2632.5,-175
+000056a0: 2032 3439 302e 352c 2d31 3735 2032 3439   2490.5,-175 249
+000056b0: 302e 352c 2d31 3133 2032 3633 322e 352c  0.5,-113 2632.5,
+000056c0: 2d31 3133 2032 3633 322e 352c 2d31 3735  -113 2632.5,-175
+000056d0: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+000056e0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+000056f0: 2232 3534 3622 2079 3d22 2d31 3538 2e38  "2546" y="-158.8
+00005700: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00005710: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00005720: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00005730: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00005740: 3e41 3039 3c2f 7465 7874 3e0a 3c74 6578  >A09</text>.<tex
+00005750: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00005760: 7461 7274 2220 783d 2232 3530 322e 3522  tart" x="2502.5"
+00005770: 2079 3d22 2d31 3436 2e34 2220 666f 6e74   y="-146.4" font
+00005780: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00005790: 6572 6966 2220 7465 7874 2d64 6563 6f72  erif" text-decor
+000057a0: 6174 696f 6e3d 2275 6e64 6572 6c69 6e65  ation="underline
+000057b0: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+000057c0: 3030 223e 4869 6e77 6569 733a 3c2f 7465  00">Hinweis:</te
+000057d0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+000057e0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+000057f0: 2232 3530 322e 3522 2079 3d22 2d31 3334  "2502.5" y="-134
+00005800: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00005810: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00005820: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
+00005830: 436c 7573 7465 7220 4162 6c65 686e 756e  Cluster Ablehnun
+00005840: 673c 2f74 6578 743e 0a3c 7465 7874 2074  g</text>.<text t
+00005850: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00005860: 7422 2078 3d22 3235 3032 2e35 2220 793d  t" x="2502.5" y=
+00005870: 222d 3132 322e 3422 2066 6f6e 742d 6661  "-122.4" font-fa
+00005880: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00005890: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
+000058a0: 2e30 3022 3e4f 4249 5320 6e69 6368 7420  .00">OBIS nicht 
+000058b0: 7061 7373 656e 643c 2f74 6578 743e 0a3c  passend</text>.<
+000058c0: 2f67 3e0a 3c21 2d2d 2039 2623 3435 3b26  /g>.<!-- 9&#45;&
+000058d0: 6774 3b41 3039 202d 2d3e 0a3c 6720 6964  gt;A09 -->.<g id
+000058e0: 3d22 6564 6765 3138 2220 636c 6173 733d  ="edge18" class=
+000058f0: 2265 6467 6522 3e0a 3c74 6974 6c65 3e39  "edge">.<title>9
+00005900: 2d26 6774 3b41 3039 3c2f 7469 746c 653e  -&gt;A09</title>
+00005910: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
+00005920: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00005930: 2220 643d 224d 3236 3438 2e34 312c 2d32  " d="M2648.41,-2
+00005940: 3338 2e36 3643 3236 3334 2e37 372c 2d32  38.66C2634.77,-2
+00005950: 3233 2e39 3620 3236 3134 2e37 2c2d 3230  23.96 2614.7,-20
+00005960: 322e 3334 2032 3539 372e 3239 2c2d 3138  2.34 2597.29,-18
+00005970: 332e 3537 222f 3e0a 3c70 6f6c 7967 6f6e  3.57"/>.<polygon
+00005980: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00005990: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+000059a0: 6e74 733d 2232 3539 392e 3931 2c2d 3138  nts="2599.91,-18
+000059b0: 312e 3234 2032 3539 302e 3534 2c2d 3137  1.24 2590.54,-17
+000059c0: 362e 3239 2032 3539 342e 3738 2c2d 3138  6.29 2594.78,-18
+000059d0: 362e 3031 2032 3539 392e 3931 2c2d 3138  6.01 2599.91,-18
+000059e0: 312e 3234 222f 3e0a 3c74 6578 7420 7465  1.24"/>.<text te
+000059f0: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00005a00: 6522 2078 3d22 3236 3336 2e35 2220 793d  e" x="2636.5" y=
+00005a10: 222d 3139 362e 3822 2066 6f6e 742d 6661  "-196.8" font-fa
+00005a20: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00005a30: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+00005a40: 2e30 3022 3e4e 6569 6e3c 2f74 6578 743e  .00">Nein</text>
+00005a50: 0a3c 2f67 3e0a 3c21 2d2d 2031 3020 2d2d  .</g>.<!-- 10 --
+00005a60: 3e0a 3c67 2069 643d 226e 6f64 6532 3022  >.<g id="node20"
+00005a70: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
+00005a80: 7469 746c 653e 3130 3c2f 7469 746c 653e  title>10</title>
+00005a90: 0a3c 7061 7468 2066 696c 6c3d 2223 3761  .<path fill="#7a
+00005aa0: 6162 3861 2220 7374 726f 6b65 3d22 626c  ab8a" stroke="bl
+00005ab0: 6163 6b22 2064 3d22 4d33 3137 322e 352c  ack" d="M3172.5,
+00005ac0: 2d31 3632 4333 3137 322e 352c 2d31 3632  -162C3172.5,-162
+00005ad0: 2032 3636 322e 352c 2d31 3632 2032 3636   2662.5,-162 266
+00005ae0: 322e 352c 2d31 3632 2032 3635 362e 352c  2.5,-162 2656.5,
+00005af0: 2d31 3632 2032 3635 302e 352c 2d31 3536  -162 2650.5,-156
+00005b00: 2032 3635 302e 352c 2d31 3530 2032 3635   2650.5,-150 265
+00005b10: 302e 352c 2d31 3530 2032 3635 302e 352c  0.5,-150 2650.5,
+00005b20: 2d31 3338 2032 3635 302e 352c 2d31 3338  -138 2650.5,-138
+00005b30: 2032 3635 302e 352c 2d31 3332 2032 3635   2650.5,-132 265
+00005b40: 362e 352c 2d31 3236 2032 3636 322e 352c  6.5,-126 2662.5,
+00005b50: 2d31 3236 2032 3636 322e 352c 2d31 3236  -126 2662.5,-126
+00005b60: 2033 3137 322e 352c 2d31 3236 2033 3137   3172.5,-126 317
+00005b70: 322e 352c 2d31 3236 2033 3137 382e 352c  2.5,-126 3178.5,
+00005b80: 2d31 3236 2033 3138 342e 352c 2d31 3332  -126 3184.5,-132
+00005b90: 2033 3138 342e 352c 2d31 3338 2033 3138   3184.5,-138 318
+00005ba0: 342e 352c 2d31 3338 2033 3138 342e 352c  4.5,-138 3184.5,
+00005bb0: 2d31 3530 2033 3138 342e 352c 2d31 3530  -150 3184.5,-150
+00005bc0: 2033 3138 342e 352c 2d31 3536 2033 3137   3184.5,-156 317
+00005bd0: 382e 352c 2d31 3632 2033 3137 322e 352c  8.5,-162 3172.5,
+00005be0: 2d31 3632 222f 3e0a 3c74 6578 7420 7465  -162"/>.<text te
+00005bf0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00005c00: 2220 783d 2232 3636 342e 3522 2079 3d22  " x="2664.5" y="
+00005c10: 2d31 3431 2e33 2220 666f 6e74 2d66 616d  -141.3" font-fam
+00005c20: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00005c30: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00005c40: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+00005c50: 3134 2e30 3022 3e31 303a 203c 2f74 6578  14.00">10: </tex
+00005c60: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00005c70: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00005c80: 3236 3934 2e35 2220 793d 222d 3134 312e  2694.5" y="-141.
+00005c90: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
+00005ca0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00005cb0: 742d 7369 7a65 3d22 3134 2e30 3022 3e49  t-size="14.00">I
+00005cc0: 7374 2064 6572 204d 6142 6953 2d5a 5020  st der MaBiS-ZP 
+00005cd0: 7a75 6d20 5a65 6974 7075 6e6b 7420 6465  zum Zeitpunkt de
+00005ce0: 7220 416b 7469 7669 6572 756e 6720 6265  r Aktivierung be
+00005cf0: 7265 6974 7320 616b 7469 7669 6572 743f  reits aktiviert?
+00005d00: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00005d10: 2d20 3926 2334 353b 2667 743b 3130 202d  - 9&#45;&gt;10 -
+00005d20: 2d3e 0a3c 6720 6964 3d22 6564 6765 3139  ->.<g id="edge19
+00005d30: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
+00005d40: 3c74 6974 6c65 3e39 2d26 6774 3b31 303c  <title>9-&gt;10<
+00005d50: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
+00005d60: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
+00005d70: 3d22 626c 6163 6b22 2064 3d22 4d32 3730  ="black" d="M270
+00005d80: 342e 3331 2c2d 3233 382e 3533 4332 3734  4.31,-238.53C274
+00005d90: 382e 3433 2c2d 3231 392e 3138 2032 3831  8.43,-219.18 281
+00005da0: 392e 3634 2c2d 3138 372e 3933 2032 3836  9.64,-187.93 286
+00005db0: 372e 3439 2c2d 3136 362e 3934 222f 3e0a  7.49,-166.94"/>.
+00005dc0: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
+00005dd0: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
+00005de0: 6163 6b22 2070 6f69 6e74 733d 2232 3836  ack" points="286
+00005df0: 382e 3739 2c2d 3137 302e 3139 2032 3837  8.79,-170.19 287
+00005e00: 362e 3534 2c2d 3136 322e 3937 2032 3836  6.54,-162.97 286
+00005e10: 352e 3937 2c2d 3136 332e 3738 2032 3836  5.97,-163.78 286
+00005e20: 382e 3739 2c2d 3137 302e 3139 222f 3e0a  8.79,-170.19"/>.
+00005e30: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00005e40: 723d 226d 6964 646c 6522 2078 3d22 3238  r="middle" x="28
+00005e50: 3133 2e35 2220 793d 222d 3139 362e 3822  13.5" y="-196.8"
+00005e60: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00005e70: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00005e80: 7369 7a65 3d22 3134 2e30 3022 3e4a 613c  size="14.00">Ja<
+00005e90: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+00005ea0: 2041 3130 202d 2d3e 0a3c 6720 6964 3d22   A10 -->.<g id="
+00005eb0: 6e6f 6465 3231 2220 636c 6173 733d 226e  node21" class="n
+00005ec0: 6f64 6522 3e0a 3c74 6974 6c65 3e41 3130  ode">.<title>A10
+00005ed0: 3c2f 7469 746c 653e 0a3c 706f 6c79 676f  </title>.<polygo
+00005ee0: 6e20 6669 6c6c 3d22 2363 6662 3938 3622  n fill="#cfb986"
+00005ef0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00005f00: 706f 696e 7473 3d22 3239 3130 2e35 2c2d  points="2910.5,-
+00005f10: 3632 2032 3732 342e 352c 2d36 3220 3237  62 2724.5,-62 27
+00005f20: 3234 2e35 2c30 2032 3931 302e 352c 3020  24.5,0 2910.5,0 
+00005f30: 3239 3130 2e35 2c2d 3632 222f 3e0a 3c74  2910.5,-62"/>.<t
+00005f40: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00005f50: 2273 7461 7274 2220 783d 2232 3830 3222  "start" x="2802"
+00005f60: 2079 3d22 2d34 352e 3822 2066 6f6e 742d   y="-45.8" font-
+00005f70: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00005f80: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+00005f90: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+00005fa0: 653d 2231 342e 3030 223e 4131 303c 2f74  e="14.00">A10</t
+00005fb0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00005fc0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00005fd0: 3d22 3237 3336 2e35 2220 793d 222d 3333  ="2736.5" y="-33
+00005fe0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00005ff0: 2254 696d 6573 2c73 6572 6966 2220 7465  "Times,serif" te
+00006000: 7874 2d64 6563 6f72 6174 696f 6e3d 2275  xt-decoration="u
+00006010: 6e64 6572 6c69 6e65 2220 666f 6e74 2d73  nderline" font-s
+00006020: 697a 653d 2231 322e 3030 223e 4869 6e77  ize="12.00">Hinw
+00006030: 6569 733a 3c2f 7465 7874 3e0a 3c74 6578  eis:</text>.<tex
+00006040: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00006050: 7461 7274 2220 783d 2232 3733 362e 3522  tart" x="2736.5"
+00006060: 2079 3d22 2d32 312e 3422 2066 6f6e 742d   y="-21.4" font-
+00006070: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00006080: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00006090: 3132 2e30 3022 3e43 6c75 7374 6572 2041  12.00">Cluster A
+000060a0: 626c 6568 6e75 6e67 3c2f 7465 7874 3e0a  blehnung</text>.
+000060b0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+000060c0: 723d 2273 7461 7274 2220 783d 2232 3733  r="start" x="273
+000060d0: 362e 3522 2079 3d22 2d39 2e34 2220 666f  6.5" y="-9.4" fo
+000060e0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000060f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00006100: 653d 2231 322e 3030 223e 4d61 4269 532d  e="12.00">MaBiS-
+00006110: 5a50 2062 6572 6569 7473 2061 6b74 6976  ZP bereits aktiv
+00006120: 6965 7274 3c2f 7465 7874 3e0a 3c2f 673e  iert</text>.</g>
+00006130: 0a3c 212d 2d20 3130 2623 3435 3b26 6774  .<!-- 10&#45;&gt
+00006140: 3b41 3130 202d 2d3e 0a3c 6720 6964 3d22  ;A10 -->.<g id="
+00006150: 6564 6765 3230 2220 636c 6173 733d 2265  edge20" class="e
+00006160: 6467 6522 3e0a 3c74 6974 6c65 3e31 302d  dge">.<title>10-
+00006170: 2667 743b 4131 303c 2f74 6974 6c65 3e0a  &gt;A10</title>.
+00006180: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
+00006190: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+000061a0: 2064 3d22 4d32 3930 312e 3838 2c2d 3132   d="M2901.88,-12
+000061b0: 352e 3636 4332 3838 382e 3633 2c2d 3131  5.66C2888.63,-11
+000061c0: 302e 3936 2032 3836 392e 3135 2c2d 3839  0.96 2869.15,-89
+000061d0: 2e33 3420 3238 3532 2e32 352c 2d37 302e  .34 2852.25,-70.
+000061e0: 3537 222f 3e0a 3c70 6f6c 7967 6f6e 2066  57"/>.<polygon f
+000061f0: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
+00006200: 6b65 3d22 626c 6163 6b22 2070 6f69 6e74  ke="black" point
+00006210: 733d 2232 3835 352c 2d36 382e 3420 3238  s="2855,-68.4 28
+00006220: 3435 2e37 312c 2d36 332e 3331 2032 3834  45.71,-63.31 284
+00006230: 392e 382c 2d37 332e 3038 2032 3835 352c  9.8,-73.08 2855,
+00006240: 2d36 382e 3422 2f3e 0a3c 7465 7874 2074  -68.4"/>.<text t
+00006250: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
+00006260: 6c65 2220 783d 2232 3838 302e 3522 2079  le" x="2880.5" y
+00006270: 3d22 2d38 332e 3822 2066 6f6e 742d 6661  ="-83.8" font-fa
+00006280: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00006290: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+000062a0: 2e30 3022 3e4a 613c 2f74 6578 743e 0a3c  .00">Ja</text>.<
+000062b0: 2f67 3e0a 3c21 2d2d 2041 3131 202d 2d3e  /g>.<!-- A11 -->
+000062c0: 0a3c 6720 6964 3d22 6e6f 6465 3232 2220  .<g id="node22" 
+000062d0: 636c 6173 733d 226e 6f64 6522 3e0a 3c74  class="node">.<t
+000062e0: 6974 6c65 3e41 3131 3c2f 7469 746c 653e  itle>A11</title>
+000062f0: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00006300: 2363 6662 3938 3622 2073 7472 6f6b 653d  #cfb986" stroke=
+00006310: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+00006320: 3331 3036 2e35 2c2d 3632 2032 3932 382e  3106.5,-62 2928.
+00006330: 352c 2d36 3220 3239 3238 2e35 2c30 2033  5,-62 2928.5,0 3
+00006340: 3130 362e 352c 3020 3331 3036 2e35 2c2d  106.5,0 3106.5,-
+00006350: 3632 222f 3e0a 3c74 6578 7420 7465 7874  62"/>.<text text
+00006360: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00006370: 783d 2233 3030 3222 2079 3d22 2d34 352e  x="3002" y="-45.
+00006380: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00006390: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+000063a0: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+000063b0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+000063c0: 223e 4131 313c 2f74 6578 743e 0a3c 7465  ">A11</text>.<te
+000063d0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000063e0: 7374 6172 7422 2078 3d22 3239 3430 2e35  start" x="2940.5
+000063f0: 2220 793d 222d 3333 2e34 2220 666f 6e74  " y="-33.4" font
+00006400: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00006410: 6572 6966 2220 7465 7874 2d64 6563 6f72  erif" text-decor
+00006420: 6174 696f 6e3d 2275 6e64 6572 6c69 6e65  ation="underline
+00006430: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+00006440: 3030 223e 4869 6e77 6569 733a 3c2f 7465  00">Hinweis:</te
+00006450: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00006460: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00006470: 2232 3934 302e 3522 2079 3d22 2d32 312e  "2940.5" y="-21.
+00006480: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00006490: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+000064a0: 742d 7369 7a65 3d22 3132 2e30 3022 3e43  t-size="12.00">C
+000064b0: 6c75 7374 6572 3a20 5a75 7374 696d 6d75  luster: Zustimmu
+000064c0: 6e67 3c2f 7465 7874 3e0a 3c74 6578 7420  ng</text>.<text 
+000064d0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+000064e0: 7274 2220 783d 2232 3934 302e 3522 2079  rt" x="2940.5" y
+000064f0: 3d22 2d39 2e34 2220 666f 6e74 2d66 616d  ="-9.4" font-fam
+00006500: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00006510: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+00006520: 3030 223e 416b 7469 7669 6572 756e 6720  00">Aktivierung 
+00006530: 6475 7263 6867 6566 2623 3235 323b 6872  durchgef&#252;hr
+00006540: 743c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  t</text>.</g>.<!
+00006550: 2d2d 2031 3026 2334 353b 2667 743b 4131  -- 10&#45;&gt;A1
+00006560: 3120 2d2d 3e0a 3c67 2069 643d 2265 6467  1 -->.<g id="edg
+00006570: 6532 3122 2063 6c61 7373 3d22 6564 6765  e21" class="edge
+00006580: 223e 0a3c 7469 746c 653e 3130 2d26 6774  ">.<title>10-&gt
+00006590: 3b41 3131 3c2f 7469 746c 653e 0a3c 7061  ;A11</title>.<pa
+000065a0: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
+000065b0: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
+000065c0: 224d 3239 3333 2e31 322c 2d31 3235 2e36  "M2933.12,-125.6
+000065d0: 3643 3239 3436 2e33 372c 2d31 3130 2e39  6C2946.37,-110.9
+000065e0: 3620 3239 3635 2e38 352c 2d38 392e 3334  6 2965.85,-89.34
+000065f0: 2032 3938 322e 3735 2c2d 3730 2e35 3722   2982.75,-70.57"
+00006600: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
+00006610: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00006620: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+00006630: 3239 3835 2e32 2c2d 3733 2e30 3820 3239  2985.2,-73.08 29
+00006640: 3839 2e32 392c 2d36 332e 3331 2032 3938  89.29,-63.31 298
+00006650: 302c 2d36 382e 3420 3239 3835 2e32 2c2d  0,-68.4 2985.2,-
+00006660: 3733 2e30 3822 2f3e 0a3c 7465 7874 2074  73.08"/>.<text t
+00006670: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
+00006680: 6c65 2220 783d 2232 3939 302e 3522 2079  le" x="2990.5" y
+00006690: 3d22 2d38 332e 3822 2066 6f6e 742d 6661  ="-83.8" font-fa
+000066a0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+000066b0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+000066c0: 2e30 3022 3e4e 6569 6e3c 2f74 6578 743e  .00">Nein</text>
+000066d0: 0a3c 2f67 3e0a 3c2f 673e 0a3c 2f73 7667  .</g>.</g>.</svg
+000066e0: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
+000066f0: 2020 3c2f 673e 0a3c 2f73 7667 3e0a         </g>.</svg>.
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0015.puml` & `ebdtable2graph-0.1.9/unittests/output/E_0015.puml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0015.puml.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0015.puml.svg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0025.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0025.dot.svg`

 * *Files 8% similar despite different names*

```diff
@@ -11,844 +11,861 @@
 000000a0: 3134 3439 2e33 3333 3333 3333 3333 3333  1449.33333333333
 000000b0: 3333 7078 2220 7669 6577 426f 783d 2230  33px" viewBox="0
 000000c0: 2030 2031 3434 392e 3333 3333 3333 3333   0 1449.33333333
 000000d0: 3333 3333 3320 3836 322e 3636 3636 3636  33333 862.666666
 000000e0: 3636 3636 3636 3622 2068 6569 6768 743d  6666666" height=
 000000f0: 2238 3632 2e36 3636 3636 3636 3636 3636  "862.66666666666
 00000100: 3636 7078 223e 0a20 203c 673e 0a20 2020  66px">.  <g>.   
-00000110: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
-00000120: 7261 6e73 6c61 7465 2833 3739 2e38 3535  ranslate(379.855
-00000130: 3935 3835 3539 3537 3234 362c 2038 362e  95855957246, 86.
-00000140: 3236 3636 3636 3636 3636 3636 3634 2920  26666666666664) 
-00000150: 7363 616c 6528 3120 3129 2074 7261 6e73  scale(1 1) trans
-00000160: 6c61 7465 2830 2c20 3029 2073 6361 6c65  late(0, 0) scale
-00000170: 2833 2e39 3031 3530 3939 3339 3337 3136  (3.9015099393716
-00000180: 3936 3320 332e 3930 3135 3039 3933 3933  963 3.9015099393
-00000190: 3731 3639 3633 2920 223e 3c73 6f64 6970  716963) "><sodip
-000001a0: 6f64 693a 6e61 6d65 6476 6965 7720 786d  odi:namedview xm
-000001b0: 6c6e 733a 736f 6469 706f 6469 3d22 6874  lns:sodipodi="ht
-000001c0: 7470 3a2f 2f73 6f64 6970 6f64 692e 736f  tp://sodipodi.so
-000001d0: 7572 6365 666f 7267 652e 6e65 742f 4454  urceforge.net/DT
-000001e0: 442f 736f 6469 706f 6469 2d30 2e64 7464  D/sodipodi-0.dtd
-000001f0: 2220 786d 6c6e 733a 696e 6b73 6361 7065  " xmlns:inkscape
-00000200: 3d22 6874 7470 3a2f 2f77 7777 2e69 6e6b  ="http://www.ink
-00000210: 7363 6170 652e 6f72 672f 6e61 6d65 7370  scape.org/namesp
-00000220: 6163 6573 2f69 6e6b 7363 6170 6522 2069  aces/inkscape" i
-00000230: 643d 226e 616d 6564 7669 6577 3722 2070  d="namedview7" p
-00000240: 6167 6563 6f6c 6f72 3d22 2366 6666 6666  agecolor="#fffff
-00000250: 6622 2062 6f72 6465 7263 6f6c 6f72 3d22  f" bordercolor="
-00000260: 2339 3939 3939 3922 2062 6f72 6465 726f  #999999" bordero
-00000270: 7061 6369 7479 3d22 3122 2069 6e6b 7363  pacity="1" inksc
-00000280: 6170 653a 7061 6765 7368 6164 6f77 3d22  ape:pageshadow="
-00000290: 3022 2069 6e6b 7363 6170 653a 7061 6765  0" inkscape:page
-000002a0: 6f70 6163 6974 793d 2230 2220 696e 6b73  opacity="0" inks
-000002b0: 6361 7065 3a70 6167 6563 6865 636b 6572  cape:pagechecker
-000002c0: 626f 6172 643d 2230 2220 696e 6b73 6361  board="0" inksca
-000002d0: 7065 3a64 6f63 756d 656e 742d 756e 6974  pe:document-unit
-000002e0: 733d 226d 6d22 2073 686f 7767 7269 643d  s="mm" showgrid=
-000002f0: 2266 616c 7365 2220 6669 742d 6d61 7267  "false" fit-marg
-00000300: 696e 2d74 6f70 3d22 3022 2066 6974 2d6d  in-top="0" fit-m
-00000310: 6172 6769 6e2d 6c65 6674 3d22 3022 2066  argin-left="0" f
-00000320: 6974 2d6d 6172 6769 6e2d 7269 6768 743d  it-margin-right=
-00000330: 2230 2220 6669 742d 6d61 7267 696e 2d62  "0" fit-margin-b
-00000340: 6f74 746f 6d3d 2230 2220 696e 6b73 6361  ottom="0" inksca
-00000350: 7065 3a7a 6f6f 6d3d 2230 2e36 3430 3532  pe:zoom="0.64052
-00000360: 3332 3922 2069 6e6b 7363 6170 653a 6378  329" inkscape:cx
-00000370: 3d22 3133 302e 3336 3231 3622 2069 6e6b  ="130.36216" ink
-00000380: 7363 6170 653a 6379 3d22 3431 322e 3136  scape:cy="412.16
-00000390: 3322 2069 6e6b 7363 6170 653a 7769 6e64  3" inkscape:wind
-000003a0: 6f77 2d77 6964 7468 3d22 3135 3132 2220  ow-width="1512" 
-000003b0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000003c0: 6865 6967 6874 3d22 3931 3622 2069 6e6b  height="916" ink
-000003d0: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
-000003e0: 3338 3430 2220 696e 6b73 6361 7065 3a77  3840" inkscape:w
-000003f0: 696e 646f 772d 793d 2231 3336 2220 696e  indow-y="136" in
-00000400: 6b73 6361 7065 3a77 696e 646f 772d 6d61  kscape:window-ma
-00000410: 7869 6d69 7a65 643d 2230 2220 696e 6b73  ximized="0" inks
-00000420: 6361 7065 3a63 7572 7265 6e74 2d6c 6179  cape:current-lay
-00000430: 6572 3d22 6c61 7965 7231 222f 3e0a 2020  er="layer1"/>.  
-00000440: 3c64 6566 7320 6964 3d22 6465 6673 3222  <defs id="defs2"
-00000450: 3e0a 2020 2020 3c63 6c69 7050 6174 6820  >.    <clipPath 
-00000460: 636c 6970 5061 7468 556e 6974 733d 2275  clipPathUnits="u
-00000470: 7365 7253 7061 6365 4f6e 5573 6522 2069  serSpaceOnUse" i
-00000480: 643d 2263 6c69 7050 6174 6832 3322 3e0a  d="clipPath23">.
-00000490: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000004a0: 2030 2c35 3638 2e31 3536 2048 2035 3739   0,568.156 H 579
-000004b0: 2e32 3336 2056 2030 2048 2030 205a 2220  .236 V 0 H 0 Z" 
-000004c0: 6964 3d22 7061 7468 3231 222f 3e0a 2020  id="path21"/>.  
-000004d0: 2020 3c2f 636c 6970 5061 7468 3e0a 2020    </clipPath>.  
-000004e0: 3c2f 6465 6673 3e0a 2020 3c67 2078 6d6c  </defs>.  <g xml
-000004f0: 6e73 3a69 6e6b 7363 6170 653d 2268 7474  ns:inkscape="htt
-00000500: 703a 2f2f 7777 772e 696e 6b73 6361 7065  p://www.inkscape
-00000510: 2e6f 7267 2f6e 616d 6573 7061 6365 732f  .org/namespaces/
-00000520: 696e 6b73 6361 7065 2220 696e 6b73 6361  inkscape" inksca
-00000530: 7065 3a6c 6162 656c 3d22 4c61 7965 7220  pe:label="Layer 
-00000540: 3122 2069 6e6b 7363 6170 653a 6772 6f75  1" inkscape:grou
-00000550: 706d 6f64 653d 226c 6179 6572 2220 6964  pmode="layer" id
-00000560: 3d22 6c61 7965 7231 2220 7472 616e 7366  ="layer1" transf
-00000570: 6f72 6d3d 2274 7261 6e73 6c61 7465 282d  orm="translate(-
-00000580: 3136 2e35 3431 3933 372c 2d35 352e 3330  16.541937,-55.30
-00000590: 3532 3637 2922 3e0a 2020 2020 3c67 2069  5267)">.    <g i
-000005a0: 643d 2267 3139 2220 636c 6970 2d70 6174  d="g19" clip-pat
-000005b0: 683d 2275 726c 2823 636c 6970 5061 7468  h="url(#clipPath
-000005c0: 3233 2922 2074 7261 6e73 666f 726d 3d22  23)" transform="
-000005d0: 6d61 7472 6978 2830 2e33 3532 3737 3737  matrix(0.3527777
-000005e0: 372c 302c 302c 2d30 2e33 3532 3737 3737  7,0,0,-0.3527777
-000005f0: 372c 302e 3031 3031 3730 3233 2c32 3433  7,0.01017023,243
-00000600: 2e37 3336 3735 2922 2073 7479 6c65 3d22  .73675)" style="
-00000610: 6f70 6163 6974 793a 302e 3222 3e0a 2020  opacity:0.2">.  
-00000620: 2020 2020 3c67 2069 643d 2267 3235 2220      <g id="g25" 
-00000630: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000640: 6c61 7465 2831 3232 2e34 3434 2c33 322e  late(122.444,32.
-00000650: 3731 3935 2922 3e0a 2020 2020 2020 2020  7195)">.        
-00000660: 3c70 6174 6820 643d 226d 2030 2c30 2068  <path d="m 0,0 h
-00000670: 202d 3536 2e31 3034 2063 202d 3131 2c30   -56.104 c -11,0
-00000680: 202d 3139 2e38 3938 2c39 2e31 3233 202d   -19.898,9.123 -
-00000690: 3139 2e34 3633 2c32 302e 3131 3520 3130  19.463,20.115 10
-000006a0: 2e35 3934 2c32 3637 2e31 3931 2032 3331  .594,267.191 231
-000006b0: 2e32 3737 2c34 3831 2e33 3032 2035 3031  .277,481.302 501
-000006c0: 2e30 3239 2c34 3831 2e33 3032 2076 202d  .029,481.302 v -
-000006d0: 3536 2e30 3220 6320 302c 2d31 302e 3938  56.02 c 0,-10.98
-000006e0: 202d 382e 3638 382c 2d31 392e 3839 3220   -8.688,-19.892 
-000006f0: 2d31 392e 3635 382c 2d32 302e 3339 3320  -19.658,-20.393 
-00000700: 4320 3138 302e 3239 2c34 3134 2e36 3937  C 180.29,414.697
-00000710: 2030 2c32 3238 2e30 3035 2030 2c30 2220   0,228.005 0,0" 
-00000720: 7374 796c 653d 2266 696c 6c3a 2336 6561  style="fill:#6ea
-00000730: 6438 333b 6669 6c6c 2d6f 7061 6369 7479  d83;fill-opacity
-00000740: 3a31 3b66 696c 6c2d 7275 6c65 3a6e 6f6e  :1;fill-rule:non
-00000750: 7a65 726f 3b73 7472 6f6b 653a 6e6f 6e65  zero;stroke:none
-00000760: 2220 6964 3d22 7061 7468 3237 222f 3e0a  " id="path27"/>.
-00000770: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
-00000780: 203c 6720 6964 3d22 6732 3922 2074 7261   <g id="g29" tra
-00000790: 6e73 666f 726d 3d22 7472 616e 736c 6174  nsform="translat
-000007a0: 6528 3237 332e 3738 3238 2c33 322e 3731  e(273.7828,32.71
-000007b0: 3935 2922 3e0a 2020 2020 2020 2020 3c70  95)">.        <p
-000007c0: 6174 6820 643d 226d 2030 2c30 2068 202d  ath d="m 0,0 h -
-000007d0: 3535 2e39 3236 2063 202d 3131 2e32 3238  55.926 c -11.228
-000007e0: 2c30 202d 3230 2e30 3931 2c39 2e34 3832  ,0 -20.091,9.482
-000007f0: 202d 3139 2e34 3335 2c32 302e 3639 2031   -19.435,20.69 1
-00000800: 302e 3734 342c 3138 332e 3433 3920 3136  0.744,183.439 16
-00000810: 332e 3338 392c 3332 392e 3338 3820 3334  3.389,329.388 34
-00000820: 392e 3438 352c 3332 392e 3338 3820 7620  9.485,329.388 v 
-00000830: 2d35 362e 3236 3320 6320 302c 2d31 302e  -56.263 c 0,-10.
-00000840: 3730 3920 2d38 2e32 3733 2c2d 3139 2e36  709 -8.273,-19.6
-00000850: 3137 202d 3138 2e39 3537 2c2d 3230 2e33  17 -18.957,-20.3
-00000860: 3520 4320 3131 322e 3831 392c 3236 332e  5 C 112.819,263.
-00000870: 3639 3620 302c 3134 342e 3737 3420 302c  696 0,144.774 0,
-00000880: 3022 2073 7479 6c65 3d22 6669 6c6c 3a23  0" style="fill:#
-00000890: 3665 6164 3833 3b66 696c 6c2d 6f70 6163  6ead83;fill-opac
-000008a0: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
-000008b0: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
-000008c0: 6f6e 6522 2069 643d 2270 6174 6833 3122  one" id="path31"
-000008d0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
-000008e0: 2020 2020 3c67 2069 643d 2267 3333 2220      <g id="g33" 
-000008f0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000900: 6c61 7465 2834 3235 2e37 3636 372c 3332  late(425.7667,32
-00000910: 2e37 3139 3529 223e 0a20 2020 2020 2020  .7195)">.       
-00000920: 203c 7061 7468 2064 3d22 6d20 302c 3020   <path d="m 0,0 
-00000930: 6820 2d35 352e 3434 3520 6320 2d31 312e  h -55.445 c -11.
-00000940: 3635 332c 3020 2d32 302e 3630 342c 3130  653,0 -20.604,10
-00000950: 2e31 3720 2d31 392e 3333 342c 3231 2e37  .17 -19.334,21.7
-00000960: 3533 2031 302e 3836 362c 3939 2e30 3332  53 10.866,99.032
-00000970: 2039 352e 3033 312c 3137 362e 3334 3120   95.031,176.341 
-00000980: 3139 362e 3931 392c 3137 362e 3334 3120  196.919,176.341 
-00000990: 7620 2d35 372e 3031 3120 6320 302c 2d31  v -57.011 c 0,-1
-000009a0: 302e 3034 3620 2d37 2e32 3833 2c2d 3138  0.046 -7.283,-18
-000009b0: 2e37 3535 202d 3137 2e32 3239 2c2d 3230  .755 -17.229,-20
-000009c0: 2e31 3635 2043 2034 352e 3638 382c 3131  .165 C 45.688,11
-000009d0: 322e 3532 3220 302c 3631 2e34 3937 2030  2.522 0,61.497 0
-000009e0: 2c30 2220 7374 796c 653d 2266 696c 6c3a  ,0" style="fill:
-000009f0: 2336 6561 6438 333b 6669 6c6c 2d6f 7061  #6ead83;fill-opa
-00000a00: 6369 7479 3a31 3b66 696c 6c2d 7275 6c65  city:1;fill-rule
-00000a10: 3a6e 6f6e 7a65 726f 3b73 7472 6f6b 653a  :nonzero;stroke:
-00000a20: 6e6f 6e65 2220 6964 3d22 7061 7468 3335  none" id="path35
-00000a30: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
-00000a40: 2020 203c 2f67 3e0a 2020 3c2f 673e 0a3c     </g>.  </g>.<
-00000a50: 2f67 3e0a 2020 2020 3c73 7667 2077 6964  /g>.    <svg wid
-00000a60: 7468 3d22 3130 3837 7074 2220 6865 6967  th="1087pt" heig
-00000a70: 6874 3d22 3634 3770 7422 2076 6965 7742  ht="647pt" viewB
-00000a80: 6f78 3d22 302e 3030 2030 2e30 3020 3130  ox="0.00 0.00 10
-00000a90: 3837 2e30 3020 3634 372e 3030 223e 0a3c  87.00 647.00">.<
-00000aa0: 6720 6964 3d22 6772 6170 6830 2220 636c  g id="graph0" cl
-00000ab0: 6173 733d 2267 7261 7068 2220 7472 616e  ass="graph" tran
-00000ac0: 7366 6f72 6d3d 2273 6361 6c65 2831 2031  sform="scale(1 1
-00000ad0: 2920 726f 7461 7465 2830 2920 7472 616e  ) rotate(0) tran
-00000ae0: 736c 6174 6528 3420 3634 3329 223e 0a3c  slate(4 643)">.<
-00000af0: 7469 746c 653e 443c 2f74 6974 6c65 3e0a  title>D</title>.
-00000b00: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00000b10: 723d 2273 7461 7274 2220 783d 2232 302e  r="start" x="20.
-00000b20: 3522 2079 3d22 2d36 3231 2e36 2220 666f  5" y="-621.6" fo
-00000b30: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00000b40: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
-00000b50: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
-00000b60: 7369 7a65 3d22 3138 2e30 3022 3e37 2e34  size="18.00">7.4
-00000b70: 3120 4144 3a20 2623 3232 303b 6265 726d  1 AD: &#220;berm
-00000b80: 6974 746c 756e 6720 5072 2623 3235 323b  ittlung Pr&#252;
-00000b90: 666d 6974 7465 696c 756e 6720 6626 2332  fmitteilung f&#2
-00000ba0: 3532 3b72 2064 6965 2042 696c 616e 7a6b  52;r die Bilanzk
-00000bb0: 7265 6973 7375 6d6d 656e 7a65 6974 7265  reissummenzeitre
-00000bc0: 6968 6520 766f 6d20 424b 5620 616e 2042  ihe vom BKV an B
-00000bd0: 494b 4f20 756e 6420 2623 3232 303b 4e42  IKO und &#220;NB
-00000be0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00000bf0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00000c00: 2220 783d 2233 3731 2e35 2220 793d 222d  " x="371.5" y="-
-00000c10: 3539 312e 3222 2066 6f6e 742d 6661 6d69  591.2" font-fami
-00000c20: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00000c30: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
-00000c40: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
-00000c50: 362e 3030 223e 372e 3431 2e32 2045 5f30  6.00">7.41.2 E_0
-00000c60: 3032 355f 5072 2623 3235 323b 666d 6974  025_Pr&#252;fmit
-00000c70: 7465 696c 756e 6720 7072 2623 3235 323b  teilung pr&#252;
-00000c80: 6665 6e3c 2f74 6578 743e 0a3c 212d 2d20  fen</text>.<!-- 
-00000c90: 5374 6172 7420 2d2d 3e0a 3c67 2069 643d  Start -->.<g id=
-00000ca0: 226e 6f64 6531 2220 636c 6173 733d 226e  "node1" class="n
-00000cb0: 6f64 6522 3e0a 3c74 6974 6c65 3e53 7461  ode">.<title>Sta
-00000cc0: 7274 3c2f 7469 746c 653e 0a3c 706f 6c79  rt</title>.<poly
-00000cd0: 676f 6e20 6669 6c6c 3d22 2337 6138 6461  gon fill="#7a8da
-00000ce0: 3122 2073 7472 6f6b 653d 2262 6c61 636b  1" stroke="black
-00000cf0: 2220 706f 696e 7473 3d22 3431 302e 352c  " points="410.5,
-00000d00: 2d35 3431 2032 3335 2e35 2c2d 3534 3120  -541 235.5,-541 
-00000d10: 3233 352e 352c 2d34 3937 2034 3130 2e35  235.5,-497 410.5
-00000d20: 2c2d 3439 3720 3431 302e 352c 2d35 3431  ,-497 410.5,-541
-00000d30: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00000d40: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00000d50: 2232 3934 2e35 2220 793d 222d 3532 312e  "294.5" y="-521.
-00000d60: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00000d70: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00000d80: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
-00000d90: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00000da0: 223e 455f 3030 3235 3c2f 7465 7874 3e0a  ">E_0025</text>.
-00000db0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00000dc0: 723d 2273 7461 7274 2220 783d 2232 3439  r="start" x="249
-00000dd0: 2e35 2220 793d 222d 3530 392e 3422 2066  .5" y="-509.4" f
-00000de0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00000df0: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00000e00: 6967 6874 3d22 626f 6c64 2220 7465 7874  ight="bold" text
-00000e10: 2d64 6563 6f72 6174 696f 6e3d 2275 6e64  -decoration="und
-00000e20: 6572 6c69 6e65 2220 666f 6e74 2d73 697a  erline" font-siz
-00000e30: 653d 2231 322e 3030 223e 5072 2623 3235  e="12.00">Pr&#25
-00000e40: 323b 6665 6e64 6520 526f 6c6c 653a 3c2f  2;fende Rolle:</
-00000e50: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00000e60: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00000e70: 783d 2233 3535 2e35 2220 793d 222d 3530  x="355.5" y="-50
-00000e80: 392e 3422 2066 6f6e 742d 6661 6d69 6c79  9.4" font-family
-00000e90: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00000ea0: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
-00000eb0: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
-00000ec0: 3030 223e 2042 494b 4f3c 2f74 6578 743e  00"> BIKO</text>
-00000ed0: 0a3c 2f67 3e0a 3c21 2d2d 2031 202d 2d3e  .</g>.<!-- 1 -->
-00000ee0: 0a3c 6720 6964 3d22 6e6f 6465 3222 2063  .<g id="node2" c
-00000ef0: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00000f00: 746c 653e 313c 2f74 6974 6c65 3e0a 3c70  tle>1</title>.<p
-00000f10: 6174 6820 6669 6c6c 3d22 2337 6161 6238  ath fill="#7aab8
-00000f20: 6122 2073 7472 6f6b 653d 2262 6c61 636b  a" stroke="black
-00000f30: 2220 643d 224d 3633 342c 2d34 3630 4336  " d="M634,-460C6
-00000f40: 3334 2c2d 3436 3020 3132 2c2d 3436 3020  34,-460 12,-460 
-00000f50: 3132 2c2d 3436 3020 362c 2d34 3630 2030  12,-460 6,-460 0
-00000f60: 2c2d 3435 3420 302c 2d34 3438 2030 2c2d  ,-454 0,-448 0,-
-00000f70: 3434 3820 302c 2d34 3336 2030 2c2d 3433  448 0,-436 0,-43
-00000f80: 3620 302c 2d34 3330 2036 2c2d 3432 3420  6 0,-430 6,-424 
-00000f90: 3132 2c2d 3432 3420 3132 2c2d 3432 3420  12,-424 12,-424 
-00000fa0: 3633 342c 2d34 3234 2036 3334 2c2d 3432  634,-424 634,-42
-00000fb0: 3420 3634 302c 2d34 3234 2036 3436 2c2d  4 640,-424 646,-
-00000fc0: 3433 3020 3634 362c 2d34 3336 2036 3436  430 646,-436 646
-00000fd0: 2c2d 3433 3620 3634 362c 2d34 3438 2036  ,-436 646,-448 6
-00000fe0: 3436 2c2d 3434 3820 3634 362c 2d34 3534  46,-448 646,-454
-00000ff0: 2036 3430 2c2d 3436 3020 3633 342c 2d34   640,-460 634,-4
-00001000: 3630 222f 3e0a 3c74 6578 7420 7465 7874  60"/>.<text text
-00001010: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00001020: 783d 2231 3422 2079 3d22 2d34 3339 2e33  x="14" y="-439.3
-00001030: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00001040: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00001050: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
-00001060: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00001070: 3e31 3a20 3c2f 7465 7874 3e0a 3c74 6578  >1: </text>.<tex
-00001080: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00001090: 7461 7274 2220 783d 2233 3422 2079 3d22  tart" x="34" y="
-000010a0: 2d34 3339 2e33 2220 666f 6e74 2d66 616d  -439.3" font-fam
-000010b0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-000010c0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-000010d0: 3030 223e 4572 666f 6c67 7420 6465 7220  00">Erfolgt der 
-000010e0: 4569 6e67 616e 6720 6465 7220 5072 2623  Eingang der Pr&#
-000010f0: 3235 323b 666d 6974 7465 696c 756e 6720  252;fmitteilung 
-00001100: 6e61 6368 2041 626c 6175 6620 6465 7220  nach Ablauf der 
-00001110: 436c 6561 7269 6e67 6672 6973 7420 6626  Clearingfrist f&
-00001120: 2332 3532 3b72 2064 6965 204b 424b 413f  #252;r die KBKA?
-00001130: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00001140: 2d20 5374 6172 7426 2334 353b 2667 743b  - Start&#45;&gt;
-00001150: 3120 2d2d 3e0a 3c67 2069 643d 2265 6467  1 -->.<g id="edg
-00001160: 6531 2220 636c 6173 733d 2265 6467 6522  e1" class="edge"
-00001170: 3e0a 3c74 6974 6c65 3e53 7461 7274 2d26  >.<title>Start-&
-00001180: 6774 3b31 3c2f 7469 746c 653e 0a3c 7061  gt;1</title>.<pa
-00001190: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-000011a0: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
-000011b0: 224d 3332 332c 2d34 3936 2e37 3143 3332  "M323,-496.71C32
-000011c0: 332c 2d34 3838 2e38 3220 3332 332c 2d34  3,-488.82 323,-4
-000011d0: 3739 2e37 3520 3332 332c 2d34 3731 2e33  79.75 323,-471.3
-000011e0: 3322 2f3e 0a3c 706f 6c79 676f 6e20 6669  3"/>.<polygon fi
-000011f0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-00001200: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-00001210: 3d22 3332 362e 352c 2d34 3731 2e35 3720  ="326.5,-471.57 
-00001220: 3332 332c 2d34 3631 2e35 3720 3331 392e  323,-461.57 319.
-00001230: 352c 2d34 3731 2e35 3720 3332 362e 352c  5,-471.57 326.5,
-00001240: 2d34 3731 2e35 3722 2f3e 0a3c 2f67 3e0a  -471.57"/>.</g>.
-00001250: 3c21 2d2d 2041 3031 202d 2d3e 0a3c 6720  <!-- A01 -->.<g 
-00001260: 6964 3d22 6e6f 6465 3322 2063 6c61 7373  id="node3" class
-00001270: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
-00001280: 4130 313c 2f74 6974 6c65 3e0a 3c70 6f6c  A01</title>.<pol
-00001290: 7967 6f6e 2066 696c 6c3d 2223 6363 6139  ygon fill="#cca9
-000012a0: 6162 2220 7374 726f 6b65 3d22 626c 6163  ab" stroke="blac
-000012b0: 6b22 2070 6f69 6e74 733d 2233 3737 2e35  k" points="377.5
-000012c0: 2c2d 3337 3320 3233 322e 352c 2d33 3733  ,-373 232.5,-373
-000012d0: 2032 3332 2e35 2c2d 3332 3320 3337 372e   232.5,-323 377.
-000012e0: 352c 2d33 3233 2033 3737 2e35 2c2d 3337  5,-323 377.5,-37
-000012f0: 3322 2f3e 0a3c 7465 7874 2074 6578 742d  3"/>.<text text-
-00001300: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00001310: 3d22 3238 392e 3522 2079 3d22 2d33 3536  ="289.5" y="-356
-00001320: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00001330: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00001340: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-00001350: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00001360: 3022 3e41 3031 3c2f 7465 7874 3e0a 3c74  0">A01</text>.<t
-00001370: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00001380: 2273 7461 7274 2220 783d 2232 3434 2e35  "start" x="244.5
-00001390: 2220 793d 222d 3334 342e 3422 2066 6f6e  " y="-344.4" fon
-000013a0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000013b0: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
-000013c0: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
-000013d0: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
-000013e0: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
-000013f0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00001400: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00001410: 3d22 3234 342e 3522 2079 3d22 2d33 3332  ="244.5" y="-332
-00001420: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
-00001430: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00001440: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
-00001450: 4672 6973 7426 2332 3532 3b62 6572 7363  Frist&#252;bersc
-00001460: 6872 6569 7475 6e67 3c2f 7465 7874 3e0a  hreitung</text>.
-00001470: 3c2f 673e 0a3c 212d 2d20 3126 2334 353b  </g>.<!-- 1&#45;
-00001480: 2667 743b 4130 3120 2d2d 3e0a 3c67 2069  &gt;A01 -->.<g i
-00001490: 643d 2265 6467 6532 2220 636c 6173 733d  d="edge2" class=
-000014a0: 2265 6467 6522 3e0a 3c74 6974 6c65 3e31  "edge">.<title>1
-000014b0: 2d26 6774 3b41 3031 3c2f 7469 746c 653e  -&gt;A01</title>
-000014c0: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
-000014d0: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-000014e0: 2220 643d 224d 3331 392e 3631 2c2d 3432  " d="M319.61,-42
-000014f0: 332e 3743 3331 372e 3433 2c2d 3431 322e  3.7C317.43,-412.
-00001500: 3535 2033 3134 2e35 322c 2d33 3937 2e36  55 314.52,-397.6
-00001510: 3720 3331 312e 3837 2c2d 3338 342e 3132  7 311.87,-384.12
-00001520: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
-00001530: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
-00001540: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
-00001550: 2233 3135 2e33 372c 2d33 3833 2e38 2033  "315.37,-383.8 3
-00001560: 3130 2e30 322c 2d33 3734 2e36 3620 3330  10.02,-374.66 30
-00001570: 382e 352c 2d33 3835 2e31 3420 3331 352e  8.5,-385.14 315.
-00001580: 3337 2c2d 3338 332e 3822 2f3e 0a3c 7465  37,-383.8"/>.<te
-00001590: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-000015a0: 6d69 6464 6c65 2220 783d 2233 3234 2220  middle" x="324" 
-000015b0: 793d 222d 3339 342e 3822 2066 6f6e 742d  y="-394.8" font-
-000015c0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-000015d0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-000015e0: 3134 2e30 3022 3e4a 613c 2f74 6578 743e  14.00">Ja</text>
-000015f0: 0a3c 2f67 3e0a 3c21 2d2d 2032 202d 2d3e  .</g>.<!-- 2 -->
-00001600: 0a3c 6720 6964 3d22 6e6f 6465 3422 2063  .<g id="node4" c
-00001610: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00001620: 746c 653e 323c 2f74 6974 6c65 3e0a 3c70  tle>2</title>.<p
-00001630: 6174 6820 6669 6c6c 3d22 2337 6161 6238  ath fill="#7aab8
-00001640: 6122 2073 7472 6f6b 653d 2262 6c61 636b  a" stroke="black
-00001650: 2220 643d 224d 3836 302c 2d33 3636 4338  " d="M860,-366C8
-00001660: 3630 2c2d 3336 3620 3430 382c 2d33 3636  60,-366 408,-366
-00001670: 2034 3038 2c2d 3336 3620 3430 322c 2d33   408,-366 402,-3
-00001680: 3636 2033 3936 2c2d 3336 3020 3339 362c  66 396,-360 396,
-00001690: 2d33 3534 2033 3936 2c2d 3335 3420 3339  -354 396,-354 39
-000016a0: 362c 2d33 3432 2033 3936 2c2d 3334 3220  6,-342 396,-342 
-000016b0: 3339 362c 2d33 3336 2034 3032 2c2d 3333  396,-336 402,-33
-000016c0: 3020 3430 382c 2d33 3330 2034 3038 2c2d  0 408,-330 408,-
-000016d0: 3333 3020 3836 302c 2d33 3330 2038 3630  330 860,-330 860
-000016e0: 2c2d 3333 3020 3836 362c 2d33 3330 2038  ,-330 866,-330 8
-000016f0: 3732 2c2d 3333 3620 3837 322c 2d33 3432  72,-336 872,-342
-00001700: 2038 3732 2c2d 3334 3220 3837 322c 2d33   872,-342 872,-3
-00001710: 3534 2038 3732 2c2d 3335 3420 3837 322c  54 872,-354 872,
-00001720: 2d33 3630 2038 3636 2c2d 3336 3620 3836  -360 866,-366 86
-00001730: 302c 2d33 3636 222f 3e0a 3c74 6578 7420  0,-366"/>.<text 
-00001740: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00001750: 7274 2220 783d 2234 3130 2220 793d 222d  rt" x="410" y="-
-00001760: 3334 352e 3322 2066 6f6e 742d 6661 6d69  345.3" font-fami
-00001770: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00001780: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
-00001790: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
-000017a0: 342e 3030 223e 323a 203c 2f74 6578 743e  4.00">2: </text>
-000017b0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-000017c0: 6f72 3d22 7374 6172 7422 2078 3d22 3433  or="start" x="43
-000017d0: 3022 2079 3d22 2d33 3435 2e33 2220 666f  0" y="-345.3" fo
-000017e0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-000017f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00001800: 653d 2231 342e 3030 223e 4265 6669 6e64  e="14.00">Befind
-00001810: 6574 2073 6963 6820 6465 7220 4d61 4269  et sich der MaBi
-00001820: 532d 5a50 2061 7566 2064 6572 2041 6767  S-ZP auf der Agg
-00001830: 7265 6761 7469 6f6e 7365 6265 6e65 2052  regationsebene R
-00001840: 5a3f 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  Z?</text>.</g>.<
-00001850: 212d 2d20 3126 2334 353b 2667 743b 3220  !-- 1&#45;&gt;2 
-00001860: 2d2d 3e0a 3c67 2069 643d 2265 6467 6533  -->.<g id="edge3
-00001870: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
-00001880: 3c74 6974 6c65 3e31 2d26 6774 3b32 3c2f  <title>1-&gt;2</
-00001890: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
-000018a0: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
-000018b0: 2262 6c61 636b 2220 643d 224d 3338 312e  "black" d="M381.
-000018c0: 3836 2c2d 3432 332e 3539 4334 3333 2e35  86,-423.59C433.5
-000018d0: 392c 2d34 3038 2e32 3820 3530 382e 3936  9,-408.28 508.96
-000018e0: 2c2d 3338 352e 3939 2035 3633 2e38 322c  ,-385.99 563.82,
-000018f0: 2d33 3639 2e37 3622 2f3e 0a3c 706f 6c79  -369.76"/>.<poly
-00001900: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-00001910: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00001920: 706f 696e 7473 3d22 3536 342e 382c 2d33  points="564.8,-3
-00001930: 3733 2e31 3220 3537 332e 342c 2d33 3636  73.12 573.4,-366
-00001940: 2e39 3320 3536 322e 3832 2c2d 3336 362e  .93 562.82,-366.
-00001950: 3431 2035 3634 2e38 2c2d 3337 332e 3132  41 564.8,-373.12
-00001960: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00001970: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
-00001980: 3d22 3530 3522 2079 3d22 2d33 3934 2e38  ="505" y="-394.8
-00001990: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-000019a0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-000019b0: 2d73 697a 653d 2231 342e 3030 223e 4e65  -size="14.00">Ne
-000019c0: 696e 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  in</text>.</g>.<
-000019d0: 212d 2d20 3320 2d2d 3e0a 3c67 2069 643d  !-- 3 -->.<g id=
-000019e0: 226e 6f64 6535 2220 636c 6173 733d 226e  "node5" class="n
-000019f0: 6f64 6522 3e0a 3c74 6974 6c65 3e33 3c2f  ode">.<title>3</
-00001a00: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
-00001a10: 6c3d 2223 3761 6162 3861 2220 7374 726f  l="#7aab8a" stro
-00001a20: 6b65 3d22 626c 6163 6b22 2064 3d22 4d35  ke="black" d="M5
-00001a30: 3534 2e35 2c2d 3236 3543 3535 342e 352c  54.5,-265C554.5,
-00001a40: 2d32 3635 2039 332e 352c 2d32 3635 2039  -265 93.5,-265 9
-00001a50: 332e 352c 2d32 3635 2038 372e 352c 2d32  3.5,-265 87.5,-2
-00001a60: 3635 2038 312e 352c 2d32 3539 2038 312e  65 81.5,-259 81.
-00001a70: 352c 2d32 3533 2038 312e 352c 2d32 3533  5,-253 81.5,-253
-00001a80: 2038 312e 352c 2d32 3331 2038 312e 352c   81.5,-231 81.5,
-00001a90: 2d32 3331 2038 312e 352c 2d32 3235 2038  -231 81.5,-225 8
-00001aa0: 372e 352c 2d32 3139 2039 332e 352c 2d32  7.5,-219 93.5,-2
-00001ab0: 3139 2039 332e 352c 2d32 3139 2035 3534  19 93.5,-219 554
-00001ac0: 2e35 2c2d 3231 3920 3535 342e 352c 2d32  .5,-219 554.5,-2
-00001ad0: 3139 2035 3630 2e35 2c2d 3231 3920 3536  19 560.5,-219 56
-00001ae0: 362e 352c 2d32 3235 2035 3636 2e35 2c2d  6.5,-225 566.5,-
-00001af0: 3233 3120 3536 362e 352c 2d32 3331 2035  231 566.5,-231 5
-00001b00: 3636 2e35 2c2d 3235 3320 3536 362e 352c  66.5,-253 566.5,
-00001b10: 2d32 3533 2035 3636 2e35 2c2d 3235 3920  -253 566.5,-259 
-00001b20: 3536 302e 352c 2d32 3635 2035 3534 2e35  560.5,-265 554.5
-00001b30: 2c2d 3236 3522 2f3e 0a3c 7465 7874 2074  ,-265"/>.<text t
-00001b40: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00001b50: 7422 2078 3d22 3935 2e35 2220 793d 222d  t" x="95.5" y="-
-00001b60: 3234 352e 3822 2066 6f6e 742d 6661 6d69  245.8" font-fami
-00001b70: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00001b80: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
-00001b90: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
-00001ba0: 342e 3030 223e 333a 203c 2f74 6578 743e  4.00">3: </text>
-00001bb0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00001bc0: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
-00001bd0: 352e 3522 2079 3d22 2d32 3435 2e38 2220  5.5" y="-245.8" 
-00001be0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00001bf0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00001c00: 697a 653d 2231 342e 3030 223e 4861 7420  ize="14.00">Hat 
-00001c10: 6465 7220 424b 5620 6626 2332 3532 3b72  der BKV f&#252;r
-00001c20: 2064 656e 2042 4b20 6469 6573 6573 204d   den BK dieses M
-00001c30: 6142 6953 2d5a 5020 696e 2064 6965 7365  aBiS-ZP in diese
-00001c40: 6d20 4269 6c61 6e7a 6965 2d3c 2f74 6578  m Bilanzie-</tex
-00001c50: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00001c60: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00001c70: 3935 2e35 2220 793d 222d 3233 312e 3822  95.5" y="-231.8"
-00001c80: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00001c90: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00001ca0: 7369 7a65 3d22 3134 2e30 3022 3e72 756e  size="14.00">run
-00001cb0: 6773 6d6f 6e61 7420 6469 6520 4167 6772  gsmonat die Aggr
-00001cc0: 6567 6174 696f 6e73 6562 656e 6520 525a  egationsebene RZ
-00001cd0: 2061 6262 6573 7465 6c6c 743f 3c2f 7465   abbestellt?</te
-00001ce0: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3226  xt>.</g>.<!-- 2&
-00001cf0: 2334 353b 2667 743b 3320 2d2d 3e0a 3c67  #45;&gt;3 -->.<g
-00001d00: 2069 643d 2265 6467 6534 2220 636c 6173   id="edge4" clas
-00001d10: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-00001d20: 3e32 2d26 6774 3b33 3c2f 7469 746c 653e  >2-&gt;3</title>
-00001d30: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
-00001d40: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-00001d50: 2220 643d 224d 3538 322e 3131 2c2d 3332  " d="M582.11,-32
-00001d60: 392e 3539 4335 3332 2e38 312c 2d33 3133  9.59C532.81,-313
-00001d70: 2e30 3520 3435 382e 3032 2c2d 3238 372e  .05 458.02,-287.
-00001d80: 3936 2034 3031 2e36 322c 2d32 3639 2e30  96 401.62,-269.0
-00001d90: 3422 2f3e 0a3c 706f 6c79 676f 6e20 6669  4"/>.<polygon fi
-00001da0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-00001db0: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-00001dc0: 3d22 3430 322e 3939 2c2d 3236 352e 3831  ="402.99,-265.81
-00001dd0: 2033 3932 2e33 392c 2d32 3635 2e39 3520   392.39,-265.95 
-00001de0: 3430 302e 3736 2c2d 3237 322e 3434 2034  400.76,-272.44 4
-00001df0: 3032 2e39 392c 2d32 3635 2e38 3122 2f3e  02.99,-265.81"/>
-00001e00: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00001e10: 6f72 3d22 6d69 6464 6c65 2220 783d 2235  or="middle" x="5
-00001e20: 3234 2220 793d 222d 3239 332e 3822 2066  24" y="-293.8" f
-00001e30: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001e40: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00001e50: 7a65 3d22 3134 2e30 3022 3e4e 6569 6e3c  ze="14.00">Nein<
-00001e60: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
-00001e70: 2035 202d 2d3e 0a3c 6720 6964 3d22 6e6f   5 -->.<g id="no
-00001e80: 6465 3922 2063 6c61 7373 3d22 6e6f 6465  de9" class="node
-00001e90: 223e 0a3c 7469 746c 653e 353c 2f74 6974  ">.<title>5</tit
-00001ea0: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-00001eb0: 2337 6161 6238 6122 2073 7472 6f6b 653d  #7aab8a" stroke=
-00001ec0: 2262 6c61 636b 2220 643d 224d 3130 3637  "black" d="M1067
-00001ed0: 2c2d 3237 3243 3130 3637 2c2d 3237 3220  ,-272C1067,-272 
-00001ee0: 3539 372c 2d32 3732 2035 3937 2c2d 3237  597,-272 597,-27
-00001ef0: 3220 3539 312c 2d32 3732 2035 3835 2c2d  2 591,-272 585,-
-00001f00: 3236 3620 3538 352c 2d32 3630 2035 3835  266 585,-260 585
-00001f10: 2c2d 3236 3020 3538 352c 2d32 3234 2035  ,-260 585,-224 5
-00001f20: 3835 2c2d 3232 3420 3538 352c 2d32 3138  85,-224 585,-218
-00001f30: 2035 3931 2c2d 3231 3220 3539 372c 2d32   591,-212 597,-2
-00001f40: 3132 2035 3937 2c2d 3231 3220 3130 3637  12 597,-212 1067
-00001f50: 2c2d 3231 3220 3130 3637 2c2d 3231 3220  ,-212 1067,-212 
-00001f60: 3130 3733 2c2d 3231 3220 3130 3739 2c2d  1073,-212 1079,-
-00001f70: 3231 3820 3130 3739 2c2d 3232 3420 3130  218 1079,-224 10
-00001f80: 3739 2c2d 3232 3420 3130 3739 2c2d 3236  79,-224 1079,-26
-00001f90: 3020 3130 3739 2c2d 3236 3020 3130 3739  0 1079,-260 1079
-00001fa0: 2c2d 3236 3620 3130 3733 2c2d 3237 3220  ,-266 1073,-272 
-00001fb0: 3130 3637 2c2d 3237 3222 2f3e 0a3c 7465  1067,-272"/>.<te
-00001fc0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00001fd0: 7374 6172 7422 2078 3d22 3539 3922 2079  start" x="599" y
-00001fe0: 3d22 2d32 3532 2e38 2220 666f 6e74 2d66  ="-252.8" font-f
-00001ff0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00002000: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
-00002010: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
-00002020: 3d22 3134 2e30 3022 3e35 3a20 3c2f 7465  ="14.00">5: </te
-00002030: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00002040: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00002050: 2236 3139 2220 793d 222d 3235 322e 3822  "619" y="-252.8"
-00002060: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00002070: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00002080: 7369 7a65 3d22 3134 2e30 3022 3e48 6174  size="14.00">Hat
-00002090: 2064 6572 2042 4b56 2064 656d 2042 494b   der BKV dem BIK
-000020a0: 4f20 6626 2332 3532 3b72 2064 6965 7365  O f&#252;r diese
-000020b0: 6e20 4269 6c61 6e7a 6965 7275 6e67 736d  n Bilanzierungsm
-000020c0: 6f6e 6174 2062 6572 6569 7473 3c2f 7465  onat bereits</te
-000020d0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-000020e0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-000020f0: 2235 3939 2220 793d 222d 3233 382e 3822  "599" y="-238.8"
-00002100: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00002110: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00002120: 7369 7a65 3d22 3134 2e30 3022 3e6d 6974  size="14.00">mit
-00002130: 6765 7465 696c 742c 2064 6173 7320 6469  geteilt, dass di
-00002140: 6520 7765 6974 6572 656e 2050 7226 2332  e weiteren Pr&#2
-00002150: 3532 3b66 756e 6765 6e20 6175 6620 4562  52;fungen auf Eb
-00002160: 656e 6520 6465 7320 4247 3c2f 7465 7874  ene des BG</text
-00002170: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00002180: 686f 723d 2273 7461 7274 2220 783d 2235  hor="start" x="5
-00002190: 3939 2220 793d 222d 3232 342e 3822 2066  99" y="-224.8" f
-000021a0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-000021b0: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-000021c0: 7a65 3d22 3134 2e30 3022 3e73 7461 7474  ze="14.00">statt
-000021d0: 6669 6e64 656e 206d 2623 3235 323b 7373  finden m&#252;ss
-000021e0: 656e 3f3c 2f74 6578 743e 0a3c 2f67 3e0a  en?</text>.</g>.
-000021f0: 3c21 2d2d 2032 2623 3435 3b26 6774 3b35  <!-- 2&#45;&gt;5
-00002200: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
-00002210: 3522 2063 6c61 7373 3d22 6564 6765 223e  5" class="edge">
-00002220: 0a3c 7469 746c 653e 322d 2667 743b 353c  .<title>2-&gt;5<
-00002230: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00002240: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00002250: 3d22 626c 6163 6b22 2064 3d22 4d36 3637  ="black" d="M667
-00002260: 2e31 342c 2d33 3239 2e35 3943 3639 332e  .14,-329.59C693.
-00002270: 3938 2c2d 3331 352e 3520 3733 322e 3633  98,-315.5 732.63
-00002280: 2c2d 3239 352e 3139 2037 3635 2e37 372c  ,-295.19 765.77,
-00002290: 2d32 3737 2e37 3922 2f3e 0a3c 706f 6c79  -277.79"/>.<poly
-000022a0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-000022b0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-000022c0: 706f 696e 7473 3d22 3736 372e 3239 2c2d  points="767.29,-
-000022d0: 3238 302e 3934 2037 3734 2e35 322c 2d32  280.94 774.52,-2
-000022e0: 3733 2e31 3920 3736 342e 3034 2c2d 3237  73.19 764.04,-27
-000022f0: 342e 3735 2037 3637 2e32 392c 2d32 3830  4.75 767.29,-280
-00002300: 2e39 3422 2f3e 0a3c 7465 7874 2074 6578  .94"/>.<text tex
-00002310: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-00002320: 2220 783d 2237 3436 2220 793d 222d 3239  " x="746" y="-29
-00002330: 332e 3822 2066 6f6e 742d 6661 6d69 6c79  3.8" font-family
-00002340: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00002350: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00002360: 3e4a 613c 2f74 6578 743e 0a3c 2f67 3e0a  >Ja</text>.</g>.
-00002370: 3c21 2d2d 2045 6e64 6520 2d2d 3e0a 3c67  <!-- Ende -->.<g
-00002380: 2069 643d 226e 6f64 6536 2220 636c 6173   id="node6" clas
-00002390: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
-000023a0: 3e45 6e64 653c 2f74 6974 6c65 3e0a 3c70  >Ende</title>.<p
-000023b0: 6f6c 7967 6f6e 2066 696c 6c3d 2223 3761  olygon fill="#7a
-000023c0: 3864 6131 2220 7374 726f 6b65 3d22 626c  8da1" stroke="bl
-000023d0: 6163 6b22 2070 6f69 6e74 733d 2236 3339  ack" points="639
-000023e0: 2e35 2c2d 3433 2035 3734 2e35 2c2d 3433  .5,-43 574.5,-43
-000023f0: 2035 3734 2e35 2c2d 3720 3633 392e 352c   574.5,-7 639.5,
-00002400: 2d37 2036 3339 2e35 2c2d 3433 222f 3e0a  -7 639.5,-43"/>.
-00002410: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00002420: 723d 226d 6964 646c 6522 2078 3d22 3630  r="middle" x="60
-00002430: 3722 2079 3d22 2d32 312e 3322 2066 6f6e  7" y="-21.3" fon
-00002440: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00002450: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00002460: 3d22 3134 2e30 3022 3e45 6e64 653c 2f74  ="14.00">Ende</t
-00002470: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2033  ext>.</g>.<!-- 3
-00002480: 2623 3435 3b26 6774 3b45 6e64 6520 2d2d  &#45;&gt;Ende --
-00002490: 3e0a 3c67 2069 643d 2265 6467 6537 2220  >.<g id="edge7" 
-000024a0: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
-000024b0: 6974 6c65 3e33 2d26 6774 3b45 6e64 653c  itle>3-&gt;Ende<
-000024c0: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-000024d0: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-000024e0: 3d22 626c 6163 6b22 2064 3d22 4d34 3835  ="black" d="M485
-000024f0: 2e39 362c 2d32 3138 2e36 4335 3231 2e31  .96,-218.6C521.1
-00002500: 372c 2d32 3036 2e36 3620 3535 352e 3234  7,-206.66 555.24
-00002510: 2c2d 3138 382e 3532 2035 3830 2c2d 3136  ,-188.52 580,-16
-00002520: 3120 3630 362e 3133 2c2d 3133 312e 3935  1 606.13,-131.95
-00002530: 2036 3039 2e39 2c2d 3834 2e39 3520 3630   609.9,-84.95 60
-00002540: 392e 3231 2c2d 3534 2e37 3722 2f3e 0a3c  9.21,-54.77"/>.<
-00002550: 706f 6c79 676f 6e20 6669 6c6c 3d22 626c  polygon fill="bl
-00002560: 6163 6b22 2073 7472 6f6b 653d 2262 6c61  ack" stroke="bla
-00002570: 636b 2220 706f 696e 7473 3d22 3631 322e  ck" points="612.
-00002580: 3731 2c2d 3534 2e37 2036 3038 2e37 382c  71,-54.7 608.78,
-00002590: 2d34 342e 3836 2036 3035 2e37 322c 2d35  -44.86 605.72,-5
-000025a0: 3520 3631 322e 3731 2c2d 3534 2e37 222f  5 612.71,-54.7"/
-000025b0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-000025c0: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
-000025d0: 3631 3322 2079 3d22 2d31 3237 2e33 2220  613" y="-127.3" 
-000025e0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000025f0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00002600: 697a 653d 2231 342e 3030 223e 4a61 3c2f  ize="14.00">Ja</
-00002610: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00002620: 3420 2d2d 3e0a 3c67 2069 643d 226e 6f64  4 -->.<g id="nod
-00002630: 6537 2220 636c 6173 733d 226e 6f64 6522  e7" class="node"
-00002640: 3e0a 3c74 6974 6c65 3e34 3c2f 7469 746c  >.<title>4</titl
-00002650: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
-00002660: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
-00002670: 626c 6163 6b22 2064 3d22 4d35 3539 2c2d  black" d="M559,-
-00002680: 3136 3143 3535 392c 2d31 3631 2038 392c  161C559,-161 89,
-00002690: 2d31 3631 2038 392c 2d31 3631 2038 332c  -161 89,-161 83,
-000026a0: 2d31 3631 2037 372c 2d31 3535 2037 372c  -161 77,-155 77,
-000026b0: 2d31 3439 2037 372c 2d31 3439 2037 372c  -149 77,-149 77,
-000026c0: 2d31 3133 2037 372c 2d31 3133 2037 372c  -113 77,-113 77,
-000026d0: 2d31 3037 2038 332c 2d31 3031 2038 392c  -107 83,-101 89,
-000026e0: 2d31 3031 2038 392c 2d31 3031 2035 3539  -101 89,-101 559
-000026f0: 2c2d 3130 3120 3535 392c 2d31 3031 2035  ,-101 559,-101 5
-00002700: 3635 2c2d 3130 3120 3537 312c 2d31 3037  65,-101 571,-107
-00002710: 2035 3731 2c2d 3131 3320 3537 312c 2d31   571,-113 571,-1
-00002720: 3133 2035 3731 2c2d 3134 3920 3537 312c  13 571,-149 571,
-00002730: 2d31 3439 2035 3731 2c2d 3135 3520 3536  -149 571,-155 56
-00002740: 352c 2d31 3631 2035 3539 2c2d 3136 3122  5,-161 559,-161"
-00002750: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
-00002760: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00002770: 3931 2220 793d 222d 3134 312e 3822 2066  91" y="-141.8" f
-00002780: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00002790: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-000027a0: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-000027b0: 2d73 697a 653d 2231 342e 3030 223e 343a  -size="14.00">4:
-000027c0: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
-000027d0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-000027e0: 7422 2078 3d22 3131 3122 2079 3d22 2d31  t" x="111" y="-1
-000027f0: 3431 2e38 2220 666f 6e74 2d66 616d 696c  41.8" font-famil
-00002800: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00002810: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00002820: 223e 4861 7420 6465 7220 424b 5620 6465  ">Hat der BKV de
-00002830: 6d20 4249 4b4f 2066 2623 3235 323b 7220  m BIKO f&#252;r 
-00002840: 6469 6573 656e 2042 696c 616e 7a69 6572  diesen Bilanzier
-00002850: 756e 6773 6d6f 6e61 7420 6265 7265 6974  ungsmonat bereit
-00002860: 733c 2f74 6578 743e 0a3c 7465 7874 2074  s</text>.<text t
-00002870: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00002880: 7422 2078 3d22 3931 2220 793d 222d 3132  t" x="91" y="-12
-00002890: 372e 3822 2066 6f6e 742d 6661 6d69 6c79  7.8" font-family
-000028a0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-000028b0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-000028c0: 3e6d 6974 6765 7465 696c 742c 2064 6173  >mitgeteilt, das
-000028d0: 7320 6469 6520 7765 6974 6572 656e 2050  s die weiteren P
-000028e0: 7226 2332 3532 3b66 756e 6765 6e20 6175  r&#252;fungen au
-000028f0: 6620 4562 656e 6520 6465 7320 4247 3c2f  f Ebene des BG</
-00002900: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00002910: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00002920: 783d 2239 3122 2079 3d22 2d31 3133 2e38  x="91" y="-113.8
-00002930: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00002940: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00002950: 2d73 697a 653d 2231 342e 3030 223e 7374  -size="14.00">st
-00002960: 6174 7466 696e 6465 6e20 6d26 2332 3532  attfinden m&#252
-00002970: 3b73 7365 6e3f 3c2f 7465 7874 3e0a 3c2f  ;ssen?</text>.</
-00002980: 673e 0a3c 212d 2d20 3326 2334 353b 2667  g>.<!-- 3&#45;&g
-00002990: 743b 3420 2d2d 3e0a 3c67 2069 643d 2265  t;4 -->.<g id="e
-000029a0: 6467 6536 2220 636c 6173 733d 2265 6467  dge6" class="edg
-000029b0: 6522 3e0a 3c74 6974 6c65 3e33 2d26 6774  e">.<title>3-&gt
-000029c0: 3b34 3c2f 7469 746c 653e 0a3c 7061 7468  ;4</title>.<path
-000029d0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
-000029e0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-000029f0: 3332 342c 2d32 3138 2e36 3843 3332 342c  324,-218.68C324,
-00002a00: 2d32 3035 2e34 3820 3332 342c 2d31 3838  -205.48 324,-188
-00002a10: 2e33 3520 3332 342c 2d31 3732 2e38 3122  .35 324,-172.81"
-00002a20: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
-00002a30: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00002a40: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00002a50: 3332 372e 352c 2d31 3732 2e38 3420 3332  327.5,-172.84 32
-00002a60: 342c 2d31 3632 2e38 3420 3332 302e 352c  4,-162.84 320.5,
-00002a70: 2d31 3732 2e38 3420 3332 372e 352c 2d31  -172.84 327.5,-1
-00002a80: 3732 2e38 3422 2f3e 0a3c 7465 7874 2074  72.84"/>.<text t
-00002a90: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00002aa0: 6c65 2220 783d 2233 3431 2220 793d 222d  le" x="341" y="-
-00002ab0: 3138 322e 3822 2066 6f6e 742d 6661 6d69  182.8" font-fami
-00002ac0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00002ad0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00002ae0: 3022 3e4e 6569 6e3c 2f74 6578 743e 0a3c  0">Nein</text>.<
-00002af0: 2f67 3e0a 3c21 2d2d 2034 2623 3435 3b26  /g>.<!-- 4&#45;&
-00002b00: 6774 3b45 6e64 6520 2d2d 3e0a 3c67 2069  gt;Ende -->.<g i
-00002b10: 643d 2265 6467 6539 2220 636c 6173 733d  d="edge9" class=
-00002b20: 2265 6467 6522 3e0a 3c74 6974 6c65 3e34  "edge">.<title>4
-00002b30: 2d26 6774 3b45 6e64 653c 2f74 6974 6c65  -&gt;Ende</title
-00002b40: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00002b50: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00002b60: 6b22 2064 3d22 4d34 3033 2e39 362c 2d31  k" d="M403.96,-1
-00002b70: 3030 2e36 3143 3435 352e 3733 2c2d 3831  00.61C455.73,-81
-00002b80: 2e35 3920 3532 312e 3134 2c2d 3537 2e35  .59 521.14,-57.5
-00002b90: 3520 3536 332e 3531 2c2d 3431 2e39 3822  5 563.51,-41.98"
-00002ba0: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
-00002bb0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00002bc0: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00002bd0: 3536 342e 3639 2c2d 3435 2e32 3820 3537  564.69,-45.28 57
-00002be0: 322e 3837 2c2d 3338 2e35 3420 3536 322e  2.87,-38.54 562.
-00002bf0: 3237 2c2d 3338 2e37 3120 3536 342e 3639  27,-38.71 564.69
-00002c00: 2c2d 3435 2e32 3822 2f3e 0a3c 7465 7874  ,-45.28"/>.<text
-00002c10: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00002c20: 6464 6c65 2220 783d 2234 3938 2220 793d  ddle" x="498" y=
-00002c30: 222d 3731 2e38 2220 666f 6e74 2d66 616d  "-71.8" font-fam
-00002c40: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00002c50: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00002c60: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
-00002c70: 673e 0a3c 212d 2d20 4130 3220 2d2d 3e0a  g>.<!-- A02 -->.
-00002c80: 3c67 2069 643d 226e 6f64 6538 2220 636c  <g id="node8" cl
-00002c90: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
-00002ca0: 6c65 3e41 3032 3c2f 7469 746c 653e 0a3c  le>A02</title>.<
-00002cb0: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
-00002cc0: 6361 3961 6222 2073 7472 6f6b 653d 2262  ca9ab" stroke="b
-00002cd0: 6c61 636b 2220 706f 696e 7473 3d22 3433  lack" points="43
-00002ce0: 302e 352c 2d35 3020 3231 372e 352c 2d35  0.5,-50 217.5,-5
-00002cf0: 3020 3231 372e 352c 3020 3433 302e 352c  0 217.5,0 430.5,
-00002d00: 3020 3433 302e 352c 2d35 3022 2f3e 0a3c  0 430.5,-50"/>.<
-00002d10: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00002d20: 3d22 7374 6172 7422 2078 3d22 3330 382e  ="start" x="308.
-00002d30: 3522 2079 3d22 2d33 332e 3822 2066 6f6e  5" y="-33.8" fon
-00002d40: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00002d50: 7365 7269 6622 2066 6f6e 742d 7765 6967  serif" font-weig
-00002d60: 6874 3d22 626f 6c64 2220 666f 6e74 2d73  ht="bold" font-s
-00002d70: 697a 653d 2231 342e 3030 223e 4130 323c  ize="14.00">A02<
-00002d80: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00002d90: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00002da0: 2078 3d22 3232 392e 3522 2079 3d22 2d32   x="229.5" y="-2
-00002db0: 312e 3422 2066 6f6e 742d 6661 6d69 6c79  1.4" font-family
-00002dc0: 3d22 5469 6d65 732c 7365 7269 6622 2074  ="Times,serif" t
-00002dd0: 6578 742d 6465 636f 7261 7469 6f6e 3d22  ext-decoration="
-00002de0: 756e 6465 726c 696e 6522 2066 6f6e 742d  underline" font-
-00002df0: 7369 7a65 3d22 3132 2e30 3022 3e48 696e  size="12.00">Hin
-00002e00: 7765 6973 3a3c 2f74 6578 743e 0a3c 7465  weis:</text>.<te
-00002e10: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00002e20: 7374 6172 7422 2078 3d22 3232 392e 3522  start" x="229.5"
-00002e30: 2079 3d22 2d39 2e34 2220 666f 6e74 2d66   y="-9.4" font-f
-00002e40: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00002e50: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00002e60: 322e 3030 223e 4661 6c73 6368 6520 4167  2.00">Falsche Ag
-00002e70: 6772 6567 6174 696f 6e73 6562 656e 6520  gregationsebene 
-00002e80: 4247 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  BG</text>.</g>.<
-00002e90: 212d 2d20 3426 2334 353b 2667 743b 4130  !-- 4&#45;&gt;A0
-00002ea0: 3220 2d2d 3e0a 3c67 2069 643d 2265 6467  2 -->.<g id="edg
-00002eb0: 6538 2220 636c 6173 733d 2265 6467 6522  e8" class="edge"
-00002ec0: 3e0a 3c74 6974 6c65 3e34 2d26 6774 3b41  >.<title>4-&gt;A
-00002ed0: 3032 3c2f 7469 746c 653e 0a3c 7061 7468  02</title>.<path
-00002ee0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
-00002ef0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00002f00: 3332 342c 2d31 3030 2e37 3543 3332 342c  324,-100.75C324,
-00002f10: 2d38 382e 3631 2033 3234 2c2d 3734 2e34  -88.61 324,-74.4
-00002f20: 2033 3234 2c2d 3631 2e36 3622 2f3e 0a3c   324,-61.66"/>.<
-00002f30: 706f 6c79 676f 6e20 6669 6c6c 3d22 626c  polygon fill="bl
-00002f40: 6163 6b22 2073 7472 6f6b 653d 2262 6c61  ack" stroke="bla
-00002f50: 636b 2220 706f 696e 7473 3d22 3332 372e  ck" points="327.
-00002f60: 352c 2d36 312e 3937 2033 3234 2c2d 3531  5,-61.97 324,-51
-00002f70: 2e39 3720 3332 302e 352c 2d36 312e 3937  .97 320.5,-61.97
-00002f80: 2033 3237 2e35 2c2d 3631 2e39 3722 2f3e   327.5,-61.97"/>
-00002f90: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00002fa0: 6f72 3d22 6d69 6464 6c65 2220 783d 2233  or="middle" x="3
-00002fb0: 3431 2220 793d 222d 3731 2e38 2220 666f  41" y="-71.8" fo
-00002fc0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00002fd0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00002fe0: 653d 2231 342e 3030 223e 4e65 696e 3c2f  e="14.00">Nein</
-00002ff0: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00003000: 3526 2334 353b 2667 743b 456e 6465 202d  5&#45;&gt;Ende -
-00003010: 2d3e 0a3c 6720 6964 3d22 6564 6765 3131  ->.<g id="edge11
-00003020: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
-00003030: 3c74 6974 6c65 3e35 2d26 6774 3b45 6e64  <title>5-&gt;End
-00003040: 653c 2f74 6974 6c65 3e0a 3c70 6174 6820  e</title>.<path 
-00003050: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
-00003060: 6b65 3d22 626c 6163 6b22 2064 3d22 4d37  ke="black" d="M7
-00003070: 3537 2e39 352c 2d32 3131 2e35 3543 3733  57.95,-211.55C73
-00003080: 322e 3131 2c2d 3139 382e 3736 2037 3034  2.11,-198.76 704
-00003090: 2e32 382c 2d31 3831 2e38 3620 3638 332c  .28,-181.86 683,
-000030a0: 2d31 3631 2036 3531 2e34 392c 2d31 3330  -161 651.49,-130
-000030b0: 2e31 3120 3632 392e 3136 2c2d 3833 2e33  .11 629.16,-83.3
-000030c0: 3820 3631 372e 3138 2c2d 3533 2e37 3922  8 617.18,-53.79"
-000030d0: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
-000030e0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-000030f0: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00003100: 3632 302e 3535 2c2d 3532 2e38 2036 3133  620.55,-52.8 613
-00003110: 2e36 352c 2d34 342e 3736 2036 3134 2e30  .65,-44.76 614.0
-00003120: 332c 2d35 352e 3335 2036 3230 2e35 352c  3,-55.35 620.55,
-00003130: 2d35 322e 3822 2f3e 0a3c 7465 7874 2074  -52.8"/>.<text t
-00003140: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00003150: 6c65 2220 783d 2237 3030 2220 793d 222d  le" x="700" y="-
-00003160: 3132 372e 3322 2066 6f6e 742d 6661 6d69  127.3" font-fami
-00003170: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00003180: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00003190: 3022 3e4e 6569 6e3c 2f74 6578 743e 0a3c  0">Nein</text>.<
-000031a0: 2f67 3e0a 3c21 2d2d 2041 3033 202d 2d3e  /g>.<!-- A03 -->
-000031b0: 0a3c 6720 6964 3d22 6e6f 6465 3130 2220  .<g id="node10" 
-000031c0: 636c 6173 733d 226e 6f64 6522 3e0a 3c74  class="node">.<t
-000031d0: 6974 6c65 3e41 3033 3c2f 7469 746c 653e  itle>A03</title>
-000031e0: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
-000031f0: 2363 6361 3961 6222 2073 7472 6f6b 653d  #cca9ab" stroke=
-00003200: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00003210: 3933 372e 352c 2d31 3536 2037 3236 2e35  937.5,-156 726.5
-00003220: 2c2d 3135 3620 3732 362e 352c 2d31 3036  ,-156 726.5,-106
-00003230: 2039 3337 2e35 2c2d 3130 3620 3933 372e   937.5,-106 937.
-00003240: 352c 2d31 3536 222f 3e0a 3c74 6578 7420  5,-156"/>.<text 
-00003250: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00003260: 7274 2220 783d 2238 3136 2e35 2220 793d  rt" x="816.5" y=
-00003270: 222d 3133 392e 3822 2066 6f6e 742d 6661  "-139.8" font-fa
-00003280: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00003290: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-000032a0: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-000032b0: 2231 342e 3030 223e 4130 333c 2f74 6578  "14.00">A03</tex
-000032c0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-000032d0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-000032e0: 3733 382e 3522 2079 3d22 2d31 3237 2e34  738.5" y="-127.4
-000032f0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00003300: 696d 6573 2c73 6572 6966 2220 7465 7874  imes,serif" text
-00003310: 2d64 6563 6f72 6174 696f 6e3d 2275 6e64  -decoration="und
-00003320: 6572 6c69 6e65 2220 666f 6e74 2d73 697a  erline" font-siz
-00003330: 653d 2231 322e 3030 223e 4869 6e77 6569  e="12.00">Hinwei
-00003340: 733a 3c2f 7465 7874 3e0a 3c74 6578 7420  s:</text>.<text 
-00003350: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00003360: 7274 2220 783d 2237 3338 2e35 2220 793d  rt" x="738.5" y=
-00003370: 222d 3131 352e 3422 2066 6f6e 742d 6661  "-115.4" font-fa
-00003380: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00003390: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
-000033a0: 2e30 3022 3e46 616c 7363 6865 2041 6767  .00">Falsche Agg
-000033b0: 7265 6761 7469 6f6e 7365 6265 6e65 2052  regationsebene R
-000033c0: 5a3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  Z</text>.</g>.<!
-000033d0: 2d2d 2035 2623 3435 3b26 6774 3b41 3033  -- 5&#45;&gt;A03
-000033e0: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
-000033f0: 3130 2220 636c 6173 733d 2265 6467 6522  10" class="edge"
-00003400: 3e0a 3c74 6974 6c65 3e35 2d26 6774 3b41  >.<title>5-&gt;A
-00003410: 3033 3c2f 7469 746c 653e 0a3c 7061 7468  03</title>.<path
-00003420: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
-00003430: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00003440: 3833 322c 2d32 3131 2e35 4338 3332 2c2d  832,-211.5C832,-
-00003450: 3139 382e 3031 2038 3332 2c2d 3138 312e  198.01 832,-181.
-00003460: 3920 3833 322c 2d31 3637 2e37 3222 2f3e  9 832,-167.72"/>
-00003470: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
-00003480: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
-00003490: 6c61 636b 2220 706f 696e 7473 3d22 3833  lack" points="83
-000034a0: 352e 352c 2d31 3637 2e38 3820 3833 322c  5.5,-167.88 832,
-000034b0: 2d31 3537 2e38 3820 3832 382e 352c 2d31  -157.88 828.5,-1
-000034c0: 3637 2e38 3820 3833 352e 352c 2d31 3637  67.88 835.5,-167
-000034d0: 2e38 3822 2f3e 0a3c 7465 7874 2074 6578  .88"/>.<text tex
-000034e0: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-000034f0: 2220 783d 2238 3339 2220 793d 222d 3138  " x="839" y="-18
-00003500: 322e 3822 2066 6f6e 742d 6661 6d69 6c79  2.8" font-family
-00003510: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00003520: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00003530: 3e4a 613c 2f74 6578 743e 0a3c 2f67 3e0a  >Ja</text>.</g>.
-00003540: 3c2f 673e 0a3c 2f73 7667 3e0a 2020 3c2f  </g>.</svg>.  </
-00003550: 673e 0a3c 2f73 7667 3e0a                 g>.</svg>.
+00000110: 203c 7376 6720 7665 7273 696f 6e3d 2231   <svg version="1
+00000120: 2e31 2220 7769 6474 683d 2231 3434 392e  .1" width="1449.
+00000130: 3333 3333 3333 3333 3333 3333 3370 7822  3333333333333px"
+00000140: 2076 6965 7742 6f78 3d22 3020 3020 3134   viewBox="0 0 14
+00000150: 3439 2e33 3333 3333 3333 3333 3333 3333  49.3333333333333
+00000160: 2038 3632 2e36 3636 3636 3636 3636 3636   862.66666666666
+00000170: 3636 2220 6865 6967 6874 3d22 3836 322e  66" height="862.
+00000180: 3636 3636 3636 3636 3636 3636 3670 7822  6666666666666px"
+00000190: 3e0a 2020 3c70 6f6c 7967 6f6e 2066 696c  >.  <polygon fil
+000001a0: 6c3d 2223 6633 6631 6636 2220 706f 696e  l="#f3f1f6" poin
+000001b0: 7473 3d22 302c 3020 3134 3439 2e33 3333  ts="0,0 1449.333
+000001c0: 3333 3333 3333 3333 3333 2c30 2031 3434  3333333333,0 144
+000001d0: 392e 3333 3333 3333 3333 3333 3333 332c  9.3333333333333,
+000001e0: 3836 322e 3636 3636 3636 3636 3636 3636  862.666666666666
+000001f0: 3620 302c 3836 322e 3636 3636 3636 3636  6 0,862.66666666
+00000200: 3636 3636 3622 2f3e 3c67 3e0a 2020 2020  66666"/><g>.    
+00000210: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
+00000220: 616e 736c 6174 6528 3337 392e 3835 3539  anslate(379.8559
+00000230: 3538 3535 3935 3732 3436 2c20 3836 2e32  5855957246, 86.2
+00000240: 3636 3636 3636 3636 3636 3636 3429 2073  6666666666664) s
+00000250: 6361 6c65 2831 2031 2920 7472 616e 736c  cale(1 1) transl
+00000260: 6174 6528 302c 2030 2920 7363 616c 6528  ate(0, 0) scale(
+00000270: 332e 3930 3135 3039 3933 3933 3731 3639  3.90150993937169
+00000280: 3633 2033 2e39 3031 3530 3939 3339 3337  63 3.90150993937
+00000290: 3136 3936 3329 2022 3e3c 736f 6469 706f  16963) "><sodipo
+000002a0: 6469 3a6e 616d 6564 7669 6577 2078 6d6c  di:namedview xml
+000002b0: 6e73 3a73 6f64 6970 6f64 693d 2268 7474  ns:sodipodi="htt
+000002c0: 703a 2f2f 736f 6469 706f 6469 2e73 6f75  p://sodipodi.sou
+000002d0: 7263 6566 6f72 6765 2e6e 6574 2f44 5444  rceforge.net/DTD
+000002e0: 2f73 6f64 6970 6f64 692d 302e 6474 6422  /sodipodi-0.dtd"
+000002f0: 2078 6d6c 6e73 3a69 6e6b 7363 6170 653d   xmlns:inkscape=
+00000300: 2268 7474 703a 2f2f 7777 772e 696e 6b73  "http://www.inks
+00000310: 6361 7065 2e6f 7267 2f6e 616d 6573 7061  cape.org/namespa
+00000320: 6365 732f 696e 6b73 6361 7065 2220 6964  ces/inkscape" id
+00000330: 3d22 6e61 6d65 6476 6965 7737 2220 7061  ="namedview7" pa
+00000340: 6765 636f 6c6f 723d 2223 6666 6666 6666  gecolor="#ffffff
+00000350: 2220 626f 7264 6572 636f 6c6f 723d 2223  " bordercolor="#
+00000360: 3939 3939 3939 2220 626f 7264 6572 6f70  999999" borderop
+00000370: 6163 6974 793d 2231 2220 696e 6b73 6361  acity="1" inksca
+00000380: 7065 3a70 6167 6573 6861 646f 773d 2230  pe:pageshadow="0
+00000390: 2220 696e 6b73 6361 7065 3a70 6167 656f  " inkscape:pageo
+000003a0: 7061 6369 7479 3d22 3022 2069 6e6b 7363  pacity="0" inksc
+000003b0: 6170 653a 7061 6765 6368 6563 6b65 7262  ape:pagecheckerb
+000003c0: 6f61 7264 3d22 3022 2069 6e6b 7363 6170  oard="0" inkscap
+000003d0: 653a 646f 6375 6d65 6e74 2d75 6e69 7473  e:document-units
+000003e0: 3d22 6d6d 2220 7368 6f77 6772 6964 3d22  ="mm" showgrid="
+000003f0: 6661 6c73 6522 2066 6974 2d6d 6172 6769  false" fit-margi
+00000400: 6e2d 746f 703d 2230 2220 6669 742d 6d61  n-top="0" fit-ma
+00000410: 7267 696e 2d6c 6566 743d 2230 2220 6669  rgin-left="0" fi
+00000420: 742d 6d61 7267 696e 2d72 6967 6874 3d22  t-margin-right="
+00000430: 3022 2066 6974 2d6d 6172 6769 6e2d 626f  0" fit-margin-bo
+00000440: 7474 6f6d 3d22 3022 2069 6e6b 7363 6170  ttom="0" inkscap
+00000450: 653a 7a6f 6f6d 3d22 302e 3634 3035 3233  e:zoom="0.640523
+00000460: 3239 2220 696e 6b73 6361 7065 3a63 783d  29" inkscape:cx=
+00000470: 2231 3330 2e33 3632 3136 2220 696e 6b73  "130.36216" inks
+00000480: 6361 7065 3a63 793d 2234 3132 2e31 3633  cape:cy="412.163
+00000490: 2220 696e 6b73 6361 7065 3a77 696e 646f  " inkscape:windo
+000004a0: 772d 7769 6474 683d 2231 3531 3222 2069  w-width="1512" i
+000004b0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d68  nkscape:window-h
+000004c0: 6569 6768 743d 2239 3136 2220 696e 6b73  eight="916" inks
+000004d0: 6361 7065 3a77 696e 646f 772d 783d 2233  cape:window-x="3
+000004e0: 3834 3022 2069 6e6b 7363 6170 653a 7769  840" inkscape:wi
+000004f0: 6e64 6f77 2d79 3d22 3133 3622 2069 6e6b  ndow-y="136" ink
+00000500: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
+00000510: 696d 697a 6564 3d22 3022 2069 6e6b 7363  imized="0" inksc
+00000520: 6170 653a 6375 7272 656e 742d 6c61 7965  ape:current-laye
+00000530: 723d 226c 6179 6572 3122 2f3e 0a20 203c  r="layer1"/>.  <
+00000540: 6465 6673 2069 643d 2264 6566 7332 223e  defs id="defs2">
+00000550: 0a20 2020 203c 636c 6970 5061 7468 2063  .    <clipPath c
+00000560: 6c69 7050 6174 6855 6e69 7473 3d22 7573  lipPathUnits="us
+00000570: 6572 5370 6163 654f 6e55 7365 2220 6964  erSpaceOnUse" id
+00000580: 3d22 636c 6970 5061 7468 3233 223e 0a20  ="clipPath23">. 
+00000590: 2020 2020 203c 7061 7468 2064 3d22 4d20       <path d="M 
+000005a0: 302c 3536 382e 3135 3620 4820 3537 392e  0,568.156 H 579.
+000005b0: 3233 3620 5620 3020 4820 3020 5a22 2069  236 V 0 H 0 Z" i
+000005c0: 643d 2270 6174 6832 3122 2f3e 0a20 2020  d="path21"/>.   
+000005d0: 203c 2f63 6c69 7050 6174 683e 0a20 203c   </clipPath>.  <
+000005e0: 2f64 6566 733e 0a20 203c 6720 786d 6c6e  /defs>.  <g xmln
+000005f0: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
+00000600: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
+00000610: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
+00000620: 6e6b 7363 6170 6522 2069 6e6b 7363 6170  nkscape" inkscap
+00000630: 653a 6c61 6265 6c3d 224c 6179 6572 2031  e:label="Layer 1
+00000640: 2220 696e 6b73 6361 7065 3a67 726f 7570  " inkscape:group
+00000650: 6d6f 6465 3d22 6c61 7965 7222 2069 643d  mode="layer" id=
+00000660: 226c 6179 6572 3122 2074 7261 6e73 666f  "layer1" transfo
+00000670: 726d 3d22 7472 616e 736c 6174 6528 2d31  rm="translate(-1
+00000680: 362e 3534 3139 3337 2c2d 3535 2e33 3035  6.541937,-55.305
+00000690: 3236 3729 223e 0a20 2020 203c 6720 6964  267)">.    <g id
+000006a0: 3d22 6731 3922 2063 6c69 702d 7061 7468  ="g19" clip-path
+000006b0: 3d22 7572 6c28 2363 6c69 7050 6174 6832  ="url(#clipPath2
+000006c0: 3329 2220 7472 616e 7366 6f72 6d3d 226d  3)" transform="m
+000006d0: 6174 7269 7828 302e 3335 3237 3737 3737  atrix(0.35277777
+000006e0: 2c30 2c30 2c2d 302e 3335 3237 3737 3737  ,0,0,-0.35277777
+000006f0: 2c30 2e30 3130 3137 3032 332c 3234 332e  ,0.01017023,243.
+00000700: 3733 3637 3529 2220 7374 796c 653d 226f  73675)" style="o
+00000710: 7061 6369 7479 3a30 2e32 223e 0a20 2020  pacity:0.2">.   
+00000720: 2020 203c 6720 6964 3d22 6732 3522 2074     <g id="g25" t
+00000730: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00000740: 6174 6528 3132 322e 3434 342c 3332 2e37  ate(122.444,32.7
+00000750: 3139 3529 223e 0a20 2020 2020 2020 203c  195)">.        <
+00000760: 7061 7468 2064 3d22 6d20 302c 3020 6820  path d="m 0,0 h 
+00000770: 2d35 362e 3130 3420 6320 2d31 312c 3020  -56.104 c -11,0 
+00000780: 2d31 392e 3839 382c 392e 3132 3320 2d31  -19.898,9.123 -1
+00000790: 392e 3436 332c 3230 2e31 3135 2031 302e  9.463,20.115 10.
+000007a0: 3539 342c 3236 372e 3139 3120 3233 312e  594,267.191 231.
+000007b0: 3237 372c 3438 312e 3330 3220 3530 312e  277,481.302 501.
+000007c0: 3032 392c 3438 312e 3330 3220 7620 2d35  029,481.302 v -5
+000007d0: 362e 3032 2063 2030 2c2d 3130 2e39 3820  6.02 c 0,-10.98 
+000007e0: 2d38 2e36 3838 2c2d 3139 2e38 3932 202d  -8.688,-19.892 -
+000007f0: 3139 2e36 3538 2c2d 3230 2e33 3933 2043  19.658,-20.393 C
+00000800: 2031 3830 2e32 392c 3431 342e 3639 3720   180.29,414.697 
+00000810: 302c 3232 382e 3030 3520 302c 3022 2073  0,228.005 0,0" s
+00000820: 7479 6c65 3d22 6669 6c6c 3a23 3665 6164  tyle="fill:#6ead
+00000830: 3833 3b66 696c 6c2d 6f70 6163 6974 793a  83;fill-opacity:
+00000840: 313b 6669 6c6c 2d72 756c 653a 6e6f 6e7a  1;fill-rule:nonz
+00000850: 6572 6f3b 7374 726f 6b65 3a6e 6f6e 6522  ero;stroke:none"
+00000860: 2069 643d 2270 6174 6832 3722 2f3e 0a20   id="path27"/>. 
+00000870: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00000880: 3c67 2069 643d 2267 3239 2220 7472 616e  <g id="g29" tran
+00000890: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000008a0: 2832 3733 2e37 3832 382c 3332 2e37 3139  (273.7828,32.719
+000008b0: 3529 223e 0a20 2020 2020 2020 203c 7061  5)">.        <pa
+000008c0: 7468 2064 3d22 6d20 302c 3020 6820 2d35  th d="m 0,0 h -5
+000008d0: 352e 3932 3620 6320 2d31 312e 3232 382c  5.926 c -11.228,
+000008e0: 3020 2d32 302e 3039 312c 392e 3438 3220  0 -20.091,9.482 
+000008f0: 2d31 392e 3433 352c 3230 2e36 3920 3130  -19.435,20.69 10
+00000900: 2e37 3434 2c31 3833 2e34 3339 2031 3633  .744,183.439 163
+00000910: 2e33 3839 2c33 3239 2e33 3838 2033 3439  .389,329.388 349
+00000920: 2e34 3835 2c33 3239 2e33 3838 2076 202d  .485,329.388 v -
+00000930: 3536 2e32 3633 2063 2030 2c2d 3130 2e37  56.263 c 0,-10.7
+00000940: 3039 202d 382e 3237 332c 2d31 392e 3631  09 -8.273,-19.61
+00000950: 3720 2d31 382e 3935 372c 2d32 302e 3335  7 -18.957,-20.35
+00000960: 2043 2031 3132 2e38 3139 2c32 3633 2e36   C 112.819,263.6
+00000970: 3936 2030 2c31 3434 2e37 3734 2030 2c30  96 0,144.774 0,0
+00000980: 2220 7374 796c 653d 2266 696c 6c3a 2336  " style="fill:#6
+00000990: 6561 6438 333b 6669 6c6c 2d6f 7061 6369  ead83;fill-opaci
+000009a0: 7479 3a31 3b66 696c 6c2d 7275 6c65 3a6e  ty:1;fill-rule:n
+000009b0: 6f6e 7a65 726f 3b73 7472 6f6b 653a 6e6f  onzero;stroke:no
+000009c0: 6e65 2220 6964 3d22 7061 7468 3331 222f  ne" id="path31"/
+000009d0: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
+000009e0: 2020 203c 6720 6964 3d22 6733 3322 2074     <g id="g33" t
+000009f0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00000a00: 6174 6528 3432 352e 3736 3637 2c33 322e  ate(425.7667,32.
+00000a10: 3731 3935 2922 3e0a 2020 2020 2020 2020  7195)">.        
+00000a20: 3c70 6174 6820 643d 226d 2030 2c30 2068  <path d="m 0,0 h
+00000a30: 202d 3535 2e34 3435 2063 202d 3131 2e36   -55.445 c -11.6
+00000a40: 3533 2c30 202d 3230 2e36 3034 2c31 302e  53,0 -20.604,10.
+00000a50: 3137 202d 3139 2e33 3334 2c32 312e 3735  17 -19.334,21.75
+00000a60: 3320 3130 2e38 3636 2c39 392e 3033 3220  3 10.866,99.032 
+00000a70: 3935 2e30 3331 2c31 3736 2e33 3431 2031  95.031,176.341 1
+00000a80: 3936 2e39 3139 2c31 3736 2e33 3431 2076  96.919,176.341 v
+00000a90: 202d 3537 2e30 3131 2063 2030 2c2d 3130   -57.011 c 0,-10
+00000aa0: 2e30 3436 202d 372e 3238 332c 2d31 382e  .046 -7.283,-18.
+00000ab0: 3735 3520 2d31 372e 3232 392c 2d32 302e  755 -17.229,-20.
+00000ac0: 3136 3520 4320 3435 2e36 3838 2c31 3132  165 C 45.688,112
+00000ad0: 2e35 3232 2030 2c36 312e 3439 3720 302c  .522 0,61.497 0,
+00000ae0: 3022 2073 7479 6c65 3d22 6669 6c6c 3a23  0" style="fill:#
+00000af0: 3665 6164 3833 3b66 696c 6c2d 6f70 6163  6ead83;fill-opac
+00000b00: 6974 793a 313b 6669 6c6c 2d72 756c 653a  ity:1;fill-rule:
+00000b10: 6e6f 6e7a 6572 6f3b 7374 726f 6b65 3a6e  nonzero;stroke:n
+00000b20: 6f6e 6522 2069 643d 2270 6174 6833 3522  one" id="path35"
+00000b30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
+00000b40: 2020 3c2f 673e 0a20 203c 2f67 3e0a 3c2f    </g>.  </g>.</
+00000b50: 673e 0a20 2020 203c 7376 6720 7769 6474  g>.    <svg widt
+00000b60: 683d 2231 3038 3770 7422 2068 6569 6768  h="1087pt" heigh
+00000b70: 743d 2236 3437 7074 2220 7669 6577 426f  t="647pt" viewBo
+00000b80: 783d 2230 2e30 3020 302e 3030 2031 3038  x="0.00 0.00 108
+00000b90: 372e 3030 2036 3437 2e30 3022 3e0a 3c67  7.00 647.00">.<g
+00000ba0: 2069 643d 2267 7261 7068 3022 2063 6c61   id="graph0" cla
+00000bb0: 7373 3d22 6772 6170 6822 2074 7261 6e73  ss="graph" trans
+00000bc0: 666f 726d 3d22 7363 616c 6528 3120 3129  form="scale(1 1)
+00000bd0: 2072 6f74 6174 6528 3029 2074 7261 6e73   rotate(0) trans
+00000be0: 6c61 7465 2834 2036 3433 2922 3e0a 3c74  late(4 643)">.<t
+00000bf0: 6974 6c65 3e44 3c2f 7469 746c 653e 0a3c  itle>D</title>.<
+00000c00: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00000c10: 3d22 7374 6172 7422 2078 3d22 3230 2e35  ="start" x="20.5
+00000c20: 2220 793d 222d 3632 312e 3622 2066 6f6e  " y="-621.6" fon
+00000c30: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00000c40: 7365 7269 6622 2066 6f6e 742d 7765 6967  serif" font-weig
+00000c50: 6874 3d22 626f 6c64 2220 666f 6e74 2d73  ht="bold" font-s
+00000c60: 697a 653d 2231 382e 3030 223e 372e 3431  ize="18.00">7.41
+00000c70: 2041 443a 2026 2332 3230 3b62 6572 6d69   AD: &#220;bermi
+00000c80: 7474 6c75 6e67 2050 7226 2332 3532 3b66  ttlung Pr&#252;f
+00000c90: 6d69 7474 6569 6c75 6e67 2066 2623 3235  mitteilung f&#25
+00000ca0: 323b 7220 6469 6520 4269 6c61 6e7a 6b72  2;r die Bilanzkr
+00000cb0: 6569 7373 756d 6d65 6e7a 6569 7472 6569  eissummenzeitrei
+00000cc0: 6865 2076 6f6d 2042 4b56 2061 6e20 4249  he vom BKV an BI
+00000cd0: 4b4f 2075 6e64 2026 2332 3230 3b4e 423c  KO und &#220;NB<
+00000ce0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00000cf0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00000d00: 2078 3d22 3337 312e 3522 2079 3d22 2d35   x="371.5" y="-5
+00000d10: 3931 2e32 2220 666f 6e74 2d66 616d 696c  91.2" font-famil
+00000d20: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00000d30: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
+00000d40: 6422 2066 6f6e 742d 7369 7a65 3d22 3136  d" font-size="16
+00000d50: 2e30 3022 3e37 2e34 312e 3220 455f 3030  .00">7.41.2 E_00
+00000d60: 3235 5f50 7226 2332 3532 3b66 6d69 7474  25_Pr&#252;fmitt
+00000d70: 6569 6c75 6e67 2070 7226 2332 3532 3b66  eilung pr&#252;f
+00000d80: 656e 3c2f 7465 7874 3e0a 3c21 2d2d 2053  en</text>.<!-- S
+00000d90: 7461 7274 202d 2d3e 0a3c 6720 6964 3d22  tart -->.<g id="
+00000da0: 6e6f 6465 3122 2063 6c61 7373 3d22 6e6f  node1" class="no
+00000db0: 6465 223e 0a3c 7469 746c 653e 5374 6172  de">.<title>Star
+00000dc0: 743c 2f74 6974 6c65 3e0a 3c70 6f6c 7967  t</title>.<polyg
+00000dd0: 6f6e 2066 696c 6c3d 2223 3761 3864 6131  on fill="#7a8da1
+00000de0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00000df0: 2070 6f69 6e74 733d 2234 3130 2e35 2c2d   points="410.5,-
+00000e00: 3534 3120 3233 352e 352c 2d35 3431 2032  541 235.5,-541 2
+00000e10: 3335 2e35 2c2d 3439 3720 3431 302e 352c  35.5,-497 410.5,
+00000e20: 2d34 3937 2034 3130 2e35 2c2d 3534 3122  -497 410.5,-541"
+00000e30: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00000e40: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00000e50: 3239 342e 3522 2079 3d22 2d35 3231 2e38  294.5" y="-521.8
+00000e60: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00000e70: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00000e80: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00000e90: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00000ea0: 3e45 5f30 3032 353c 2f74 6578 743e 0a3c  >E_0025</text>.<
+00000eb0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00000ec0: 3d22 7374 6172 7422 2078 3d22 3234 392e  ="start" x="249.
+00000ed0: 3522 2079 3d22 2d35 3039 2e34 2220 666f  5" y="-509.4" fo
+00000ee0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00000ef0: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+00000f00: 6768 743d 2262 6f6c 6422 2074 6578 742d  ght="bold" text-
+00000f10: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00000f20: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00000f30: 3d22 3132 2e30 3022 3e50 7226 2332 3532  ="12.00">Pr&#252
+00000f40: 3b66 656e 6465 2052 6f6c 6c65 3a3c 2f74  ;fende Rolle:</t
+00000f50: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00000f60: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00000f70: 3d22 3335 352e 3522 2079 3d22 2d35 3039  ="355.5" y="-509
+00000f80: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00000f90: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00000fa0: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
+00000fb0: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
+00000fc0: 3022 3e20 4249 4b4f 3c2f 7465 7874 3e0a  0"> BIKO</text>.
+00000fd0: 3c2f 673e 0a3c 212d 2d20 3120 2d2d 3e0a  </g>.<!-- 1 -->.
+00000fe0: 3c67 2069 643d 226e 6f64 6532 2220 636c  <g id="node2" cl
+00000ff0: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00001000: 6c65 3e31 3c2f 7469 746c 653e 0a3c 7061  le>1</title>.<pa
+00001010: 7468 2066 696c 6c3d 2223 3761 6162 3861  th fill="#7aab8a
+00001020: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00001030: 2064 3d22 4d36 3334 2c2d 3436 3043 3633   d="M634,-460C63
+00001040: 342c 2d34 3630 2031 322c 2d34 3630 2031  4,-460 12,-460 1
+00001050: 322c 2d34 3630 2036 2c2d 3436 3020 302c  2,-460 6,-460 0,
+00001060: 2d34 3534 2030 2c2d 3434 3820 302c 2d34  -454 0,-448 0,-4
+00001070: 3438 2030 2c2d 3433 3620 302c 2d34 3336  48 0,-436 0,-436
+00001080: 2030 2c2d 3433 3020 362c 2d34 3234 2031   0,-430 6,-424 1
+00001090: 322c 2d34 3234 2031 322c 2d34 3234 2036  2,-424 12,-424 6
+000010a0: 3334 2c2d 3432 3420 3633 342c 2d34 3234  34,-424 634,-424
+000010b0: 2036 3430 2c2d 3432 3420 3634 362c 2d34   640,-424 646,-4
+000010c0: 3330 2036 3436 2c2d 3433 3620 3634 362c  30 646,-436 646,
+000010d0: 2d34 3336 2036 3436 2c2d 3434 3820 3634  -436 646,-448 64
+000010e0: 362c 2d34 3438 2036 3436 2c2d 3435 3420  6,-448 646,-454 
+000010f0: 3634 302c 2d34 3630 2036 3334 2c2d 3436  640,-460 634,-46
+00001100: 3022 2f3e 0a3c 7465 7874 2074 6578 742d  0"/>.<text text-
+00001110: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00001120: 3d22 3134 2220 793d 222d 3433 392e 3322  ="14" y="-439.3"
+00001130: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00001140: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00001150: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
+00001160: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00001170: 313a 203c 2f74 6578 743e 0a3c 7465 7874  1: </text>.<text
+00001180: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00001190: 6172 7422 2078 3d22 3334 2220 793d 222d  art" x="34" y="-
+000011a0: 3433 392e 3322 2066 6f6e 742d 6661 6d69  439.3" font-fami
+000011b0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+000011c0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+000011d0: 3022 3e45 7266 6f6c 6774 2064 6572 2045  0">Erfolgt der E
+000011e0: 696e 6761 6e67 2064 6572 2050 7226 2332  ingang der Pr&#2
+000011f0: 3532 3b66 6d69 7474 6569 6c75 6e67 206e  52;fmitteilung n
+00001200: 6163 6820 4162 6c61 7566 2064 6572 2043  ach Ablauf der C
+00001210: 6c65 6172 696e 6766 7269 7374 2066 2623  learingfrist f&#
+00001220: 3235 323b 7220 6469 6520 4b42 4b41 3f3c  252;r die KBKA?<
+00001230: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+00001240: 2053 7461 7274 2623 3435 3b26 6774 3b31   Start&#45;&gt;1
+00001250: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
+00001260: 3122 2063 6c61 7373 3d22 6564 6765 223e  1" class="edge">
+00001270: 0a3c 7469 746c 653e 5374 6172 742d 2667  .<title>Start-&g
+00001280: 743b 313c 2f74 6974 6c65 3e0a 3c70 6174  t;1</title>.<pat
+00001290: 6820 6669 6c6c 3d22 6e6f 6e65 2220 7374  h fill="none" st
+000012a0: 726f 6b65 3d22 626c 6163 6b22 2064 3d22  roke="black" d="
+000012b0: 4d33 3233 2c2d 3439 362e 3731 4333 3233  M323,-496.71C323
+000012c0: 2c2d 3438 382e 3832 2033 3233 2c2d 3437  ,-488.82 323,-47
+000012d0: 392e 3735 2033 3233 2c2d 3437 312e 3333  9.75 323,-471.33
+000012e0: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
+000012f0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00001300: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+00001310: 2233 3236 2e35 2c2d 3437 312e 3537 2033  "326.5,-471.57 3
+00001320: 3233 2c2d 3436 312e 3537 2033 3139 2e35  23,-461.57 319.5
+00001330: 2c2d 3437 312e 3537 2033 3236 2e35 2c2d  ,-471.57 326.5,-
+00001340: 3437 312e 3537 222f 3e0a 3c2f 673e 0a3c  471.57"/>.</g>.<
+00001350: 212d 2d20 4130 3120 2d2d 3e0a 3c67 2069  !-- A01 -->.<g i
+00001360: 643d 226e 6f64 6533 2220 636c 6173 733d  d="node3" class=
+00001370: 226e 6f64 6522 3e0a 3c74 6974 6c65 3e41  "node">.<title>A
+00001380: 3031 3c2f 7469 746c 653e 0a3c 706f 6c79  01</title>.<poly
+00001390: 676f 6e20 6669 6c6c 3d22 2363 6662 3938  gon fill="#cfb98
+000013a0: 3622 2073 7472 6f6b 653d 2262 6c61 636b  6" stroke="black
+000013b0: 2220 706f 696e 7473 3d22 3337 372e 352c  " points="377.5,
+000013c0: 2d33 3733 2032 3332 2e35 2c2d 3337 3320  -373 232.5,-373 
+000013d0: 3233 322e 352c 2d33 3233 2033 3737 2e35  232.5,-323 377.5
+000013e0: 2c2d 3332 3320 3337 372e 352c 2d33 3733  ,-323 377.5,-373
+000013f0: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+00001400: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00001410: 2232 3839 2e35 2220 793d 222d 3335 362e  "289.5" y="-356.
+00001420: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00001430: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00001440: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+00001450: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00001460: 223e 4130 313c 2f74 6578 743e 0a3c 7465  ">A01</text>.<te
+00001470: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00001480: 7374 6172 7422 2078 3d22 3234 342e 3522  start" x="244.5"
+00001490: 2079 3d22 2d33 3434 2e34 2220 666f 6e74   y="-344.4" font
+000014a0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+000014b0: 6572 6966 2220 7465 7874 2d64 6563 6f72  erif" text-decor
+000014c0: 6174 696f 6e3d 2275 6e64 6572 6c69 6e65  ation="underline
+000014d0: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+000014e0: 3030 223e 4869 6e77 6569 733a 3c2f 7465  00">Hinweis:</te
+000014f0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00001500: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00001510: 2232 3434 2e35 2220 793d 222d 3333 322e  "244.5" y="-332.
+00001520: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00001530: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00001540: 742d 7369 7a65 3d22 3132 2e30 3022 3e46  t-size="12.00">F
+00001550: 7269 7374 2623 3235 323b 6265 7273 6368  rist&#252;bersch
+00001560: 7265 6974 756e 673c 2f74 6578 743e 0a3c  reitung</text>.<
+00001570: 2f67 3e0a 3c21 2d2d 2031 2623 3435 3b26  /g>.<!-- 1&#45;&
+00001580: 6774 3b41 3031 202d 2d3e 0a3c 6720 6964  gt;A01 -->.<g id
+00001590: 3d22 6564 6765 3222 2063 6c61 7373 3d22  ="edge2" class="
+000015a0: 6564 6765 223e 0a3c 7469 746c 653e 312d  edge">.<title>1-
+000015b0: 2667 743b 4130 313c 2f74 6974 6c65 3e0a  &gt;A01</title>.
+000015c0: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
+000015d0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+000015e0: 2064 3d22 4d33 3139 2e36 312c 2d34 3233   d="M319.61,-423
+000015f0: 2e37 4333 3137 2e34 332c 2d34 3132 2e35  .7C317.43,-412.5
+00001600: 3520 3331 342e 3532 2c2d 3339 372e 3637  5 314.52,-397.67
+00001610: 2033 3131 2e38 372c 2d33 3834 2e31 3222   311.87,-384.12"
+00001620: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
+00001630: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00001640: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+00001650: 3331 352e 3337 2c2d 3338 332e 3820 3331  315.37,-383.8 31
+00001660: 302e 3032 2c2d 3337 342e 3636 2033 3038  0.02,-374.66 308
+00001670: 2e35 2c2d 3338 352e 3134 2033 3135 2e33  .5,-385.14 315.3
+00001680: 372c 2d33 3833 2e38 222f 3e0a 3c74 6578  7,-383.8"/>.<tex
+00001690: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
+000016a0: 6964 646c 6522 2078 3d22 3332 3422 2079  iddle" x="324" y
+000016b0: 3d22 2d33 3934 2e38 2220 666f 6e74 2d66  ="-394.8" font-f
+000016c0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+000016d0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+000016e0: 342e 3030 223e 4a61 3c2f 7465 7874 3e0a  4.00">Ja</text>.
+000016f0: 3c2f 673e 0a3c 212d 2d20 3220 2d2d 3e0a  </g>.<!-- 2 -->.
+00001700: 3c67 2069 643d 226e 6f64 6534 2220 636c  <g id="node4" cl
+00001710: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00001720: 6c65 3e32 3c2f 7469 746c 653e 0a3c 7061  le>2</title>.<pa
+00001730: 7468 2066 696c 6c3d 2223 3761 6162 3861  th fill="#7aab8a
+00001740: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00001750: 2064 3d22 4d38 3630 2c2d 3336 3643 3836   d="M860,-366C86
+00001760: 302c 2d33 3636 2034 3038 2c2d 3336 3620  0,-366 408,-366 
+00001770: 3430 382c 2d33 3636 2034 3032 2c2d 3336  408,-366 402,-36
+00001780: 3620 3339 362c 2d33 3630 2033 3936 2c2d  6 396,-360 396,-
+00001790: 3335 3420 3339 362c 2d33 3534 2033 3936  354 396,-354 396
+000017a0: 2c2d 3334 3220 3339 362c 2d33 3432 2033  ,-342 396,-342 3
+000017b0: 3936 2c2d 3333 3620 3430 322c 2d33 3330  96,-336 402,-330
+000017c0: 2034 3038 2c2d 3333 3020 3430 382c 2d33   408,-330 408,-3
+000017d0: 3330 2038 3630 2c2d 3333 3020 3836 302c  30 860,-330 860,
+000017e0: 2d33 3330 2038 3636 2c2d 3333 3020 3837  -330 866,-330 87
+000017f0: 322c 2d33 3336 2038 3732 2c2d 3334 3220  2,-336 872,-342 
+00001800: 3837 322c 2d33 3432 2038 3732 2c2d 3335  872,-342 872,-35
+00001810: 3420 3837 322c 2d33 3534 2038 3732 2c2d  4 872,-354 872,-
+00001820: 3336 3020 3836 362c 2d33 3636 2038 3630  360 866,-366 860
+00001830: 2c2d 3336 3622 2f3e 0a3c 7465 7874 2074  ,-366"/>.<text t
+00001840: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00001850: 7422 2078 3d22 3431 3022 2079 3d22 2d33  t" x="410" y="-3
+00001860: 3435 2e33 2220 666f 6e74 2d66 616d 696c  45.3" font-famil
+00001870: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00001880: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
+00001890: 6422 2066 6f6e 742d 7369 7a65 3d22 3134  d" font-size="14
+000018a0: 2e30 3022 3e32 3a20 3c2f 7465 7874 3e0a  .00">2: </text>.
+000018b0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+000018c0: 723d 2273 7461 7274 2220 783d 2234 3330  r="start" x="430
+000018d0: 2220 793d 222d 3334 352e 3322 2066 6f6e  " y="-345.3" fon
+000018e0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+000018f0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00001900: 3d22 3134 2e30 3022 3e42 6566 696e 6465  ="14.00">Befinde
+00001910: 7420 7369 6368 2064 6572 204d 6142 6953  t sich der MaBiS
+00001920: 2d5a 5020 6175 6620 6465 7220 4167 6772  -ZP auf der Aggr
+00001930: 6567 6174 696f 6e73 6562 656e 6520 525a  egationsebene RZ
+00001940: 3f3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  ?</text>.</g>.<!
+00001950: 2d2d 2031 2623 3435 3b26 6774 3b32 202d  -- 1&#45;&gt;2 -
+00001960: 2d3e 0a3c 6720 6964 3d22 6564 6765 3322  ->.<g id="edge3"
+00001970: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
+00001980: 7469 746c 653e 312d 2667 743b 323c 2f74  title>1-&gt;2</t
+00001990: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
+000019a0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
+000019b0: 626c 6163 6b22 2064 3d22 4d33 3831 2e38  black" d="M381.8
+000019c0: 362c 2d34 3233 2e35 3943 3433 332e 3539  6,-423.59C433.59
+000019d0: 2c2d 3430 382e 3238 2035 3038 2e39 362c  ,-408.28 508.96,
+000019e0: 2d33 3835 2e39 3920 3536 332e 3832 2c2d  -385.99 563.82,-
+000019f0: 3336 392e 3736 222f 3e0a 3c70 6f6c 7967  369.76"/>.<polyg
+00001a00: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00001a10: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00001a20: 6f69 6e74 733d 2235 3634 2e38 2c2d 3337  oints="564.8,-37
+00001a30: 332e 3132 2035 3733 2e34 2c2d 3336 362e  3.12 573.4,-366.
+00001a40: 3933 2035 3632 2e38 322c 2d33 3636 2e34  93 562.82,-366.4
+00001a50: 3120 3536 342e 382c 2d33 3733 2e31 3222  1 564.8,-373.12"
+00001a60: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00001a70: 6368 6f72 3d22 6d69 6464 6c65 2220 783d  chor="middle" x=
+00001a80: 2235 3035 2220 793d 222d 3339 342e 3822  "505" y="-394.8"
+00001a90: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00001aa0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00001ab0: 7369 7a65 3d22 3134 2e30 3022 3e4e 6569  size="14.00">Nei
+00001ac0: 6e3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  n</text>.</g>.<!
+00001ad0: 2d2d 2033 202d 2d3e 0a3c 6720 6964 3d22  -- 3 -->.<g id="
+00001ae0: 6e6f 6465 3522 2063 6c61 7373 3d22 6e6f  node5" class="no
+00001af0: 6465 223e 0a3c 7469 746c 653e 333c 2f74  de">.<title>3</t
+00001b00: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
+00001b10: 3d22 2337 6161 6238 6122 2073 7472 6f6b  ="#7aab8a" strok
+00001b20: 653d 2262 6c61 636b 2220 643d 224d 3535  e="black" d="M55
+00001b30: 342e 352c 2d32 3635 4335 3534 2e35 2c2d  4.5,-265C554.5,-
+00001b40: 3236 3520 3933 2e35 2c2d 3236 3520 3933  265 93.5,-265 93
+00001b50: 2e35 2c2d 3236 3520 3837 2e35 2c2d 3236  .5,-265 87.5,-26
+00001b60: 3520 3831 2e35 2c2d 3235 3920 3831 2e35  5 81.5,-259 81.5
+00001b70: 2c2d 3235 3320 3831 2e35 2c2d 3235 3320  ,-253 81.5,-253 
+00001b80: 3831 2e35 2c2d 3233 3120 3831 2e35 2c2d  81.5,-231 81.5,-
+00001b90: 3233 3120 3831 2e35 2c2d 3232 3520 3837  231 81.5,-225 87
+00001ba0: 2e35 2c2d 3231 3920 3933 2e35 2c2d 3231  .5,-219 93.5,-21
+00001bb0: 3920 3933 2e35 2c2d 3231 3920 3535 342e  9 93.5,-219 554.
+00001bc0: 352c 2d32 3139 2035 3534 2e35 2c2d 3231  5,-219 554.5,-21
+00001bd0: 3920 3536 302e 352c 2d32 3139 2035 3636  9 560.5,-219 566
+00001be0: 2e35 2c2d 3232 3520 3536 362e 352c 2d32  .5,-225 566.5,-2
+00001bf0: 3331 2035 3636 2e35 2c2d 3233 3120 3536  31 566.5,-231 56
+00001c00: 362e 352c 2d32 3533 2035 3636 2e35 2c2d  6.5,-253 566.5,-
+00001c10: 3235 3320 3536 362e 352c 2d32 3539 2035  253 566.5,-259 5
+00001c20: 3630 2e35 2c2d 3236 3520 3535 342e 352c  60.5,-265 554.5,
+00001c30: 2d32 3635 222f 3e0a 3c74 6578 7420 7465  -265"/>.<text te
+00001c40: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00001c50: 2220 783d 2239 352e 3522 2079 3d22 2d32  " x="95.5" y="-2
+00001c60: 3435 2e38 2220 666f 6e74 2d66 616d 696c  45.8" font-famil
+00001c70: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00001c80: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
+00001c90: 6422 2066 6f6e 742d 7369 7a65 3d22 3134  d" font-size="14
+00001ca0: 2e30 3022 3e33 3a20 3c2f 7465 7874 3e0a  .00">3: </text>.
+00001cb0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00001cc0: 723d 2273 7461 7274 2220 783d 2231 3135  r="start" x="115
+00001cd0: 2e35 2220 793d 222d 3234 352e 3822 2066  .5" y="-245.8" f
+00001ce0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00001cf0: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00001d00: 7a65 3d22 3134 2e30 3022 3e48 6174 2064  ze="14.00">Hat d
+00001d10: 6572 2042 4b56 2066 2623 3235 323b 7220  er BKV f&#252;r 
+00001d20: 6465 6e20 424b 2064 6965 7365 7320 4d61  den BK dieses Ma
+00001d30: 4269 532d 5a50 2069 6e20 6469 6573 656d  BiS-ZP in diesem
+00001d40: 2042 696c 616e 7a69 652d 3c2f 7465 7874   Bilanzie-</text
+00001d50: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00001d60: 686f 723d 2273 7461 7274 2220 783d 2239  hor="start" x="9
+00001d70: 352e 3522 2079 3d22 2d32 3331 2e38 2220  5.5" y="-231.8" 
+00001d80: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00001d90: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00001da0: 697a 653d 2231 342e 3030 223e 7275 6e67  ize="14.00">rung
+00001db0: 736d 6f6e 6174 2064 6965 2041 6767 7265  smonat die Aggre
+00001dc0: 6761 7469 6f6e 7365 6265 6e65 2052 5a20  gationsebene RZ 
+00001dd0: 6162 6265 7374 656c 6c74 3f3c 2f74 6578  abbestellt?</tex
+00001de0: 743e 0a3c 2f67 3e0a 3c21 2d2d 2032 2623  t>.</g>.<!-- 2&#
+00001df0: 3435 3b26 6774 3b33 202d 2d3e 0a3c 6720  45;&gt;3 -->.<g 
+00001e00: 6964 3d22 6564 6765 3422 2063 6c61 7373  id="edge4" class
+00001e10: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
+00001e20: 322d 2667 743b 333c 2f74 6974 6c65 3e0a  2-&gt;3</title>.
+00001e30: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
+00001e40: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00001e50: 2064 3d22 4d35 3832 2e31 312c 2d33 3239   d="M582.11,-329
+00001e60: 2e35 3943 3533 322e 3831 2c2d 3331 332e  .59C532.81,-313.
+00001e70: 3035 2034 3538 2e30 322c 2d32 3837 2e39  05 458.02,-287.9
+00001e80: 3620 3430 312e 3632 2c2d 3236 392e 3034  6 401.62,-269.04
+00001e90: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
+00001ea0: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00001eb0: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+00001ec0: 2234 3032 2e39 392c 2d32 3635 2e38 3120  "402.99,-265.81 
+00001ed0: 3339 322e 3339 2c2d 3236 352e 3935 2034  392.39,-265.95 4
+00001ee0: 3030 2e37 362c 2d32 3732 2e34 3420 3430  00.76,-272.44 40
+00001ef0: 322e 3939 2c2d 3236 352e 3831 222f 3e0a  2.99,-265.81"/>.
+00001f00: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00001f10: 723d 226d 6964 646c 6522 2078 3d22 3532  r="middle" x="52
+00001f20: 3422 2079 3d22 2d32 3933 2e38 2220 666f  4" y="-293.8" fo
+00001f30: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00001f40: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00001f50: 653d 2231 342e 3030 223e 4e65 696e 3c2f  e="14.00">Nein</
+00001f60: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
+00001f70: 3520 2d2d 3e0a 3c67 2069 643d 226e 6f64  5 -->.<g id="nod
+00001f80: 6539 2220 636c 6173 733d 226e 6f64 6522  e9" class="node"
+00001f90: 3e0a 3c74 6974 6c65 3e35 3c2f 7469 746c  >.<title>5</titl
+00001fa0: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
+00001fb0: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
+00001fc0: 626c 6163 6b22 2064 3d22 4d31 3036 372c  black" d="M1067,
+00001fd0: 2d32 3732 4331 3036 372c 2d32 3732 2035  -272C1067,-272 5
+00001fe0: 3937 2c2d 3237 3220 3539 372c 2d32 3732  97,-272 597,-272
+00001ff0: 2035 3931 2c2d 3237 3220 3538 352c 2d32   591,-272 585,-2
+00002000: 3636 2035 3835 2c2d 3236 3020 3538 352c  66 585,-260 585,
+00002010: 2d32 3630 2035 3835 2c2d 3232 3420 3538  -260 585,-224 58
+00002020: 352c 2d32 3234 2035 3835 2c2d 3231 3820  5,-224 585,-218 
+00002030: 3539 312c 2d32 3132 2035 3937 2c2d 3231  591,-212 597,-21
+00002040: 3220 3539 372c 2d32 3132 2031 3036 372c  2 597,-212 1067,
+00002050: 2d32 3132 2031 3036 372c 2d32 3132 2031  -212 1067,-212 1
+00002060: 3037 332c 2d32 3132 2031 3037 392c 2d32  073,-212 1079,-2
+00002070: 3138 2031 3037 392c 2d32 3234 2031 3037  18 1079,-224 107
+00002080: 392c 2d32 3234 2031 3037 392c 2d32 3630  9,-224 1079,-260
+00002090: 2031 3037 392c 2d32 3630 2031 3037 392c   1079,-260 1079,
+000020a0: 2d32 3636 2031 3037 332c 2d32 3732 2031  -266 1073,-272 1
+000020b0: 3036 372c 2d32 3732 222f 3e0a 3c74 6578  067,-272"/>.<tex
+000020c0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+000020d0: 7461 7274 2220 783d 2235 3939 2220 793d  tart" x="599" y=
+000020e0: 222d 3235 322e 3822 2066 6f6e 742d 6661  "-252.8" font-fa
+000020f0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00002100: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+00002110: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+00002120: 2231 342e 3030 223e 353a 203c 2f74 6578  "14.00">5: </tex
+00002130: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00002140: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00002150: 3631 3922 2079 3d22 2d32 3532 2e38 2220  619" y="-252.8" 
+00002160: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00002170: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00002180: 697a 653d 2231 342e 3030 223e 4861 7420  ize="14.00">Hat 
+00002190: 6465 7220 424b 5620 6465 6d20 4249 4b4f  der BKV dem BIKO
+000021a0: 2066 2623 3235 323b 7220 6469 6573 656e   f&#252;r diesen
+000021b0: 2042 696c 616e 7a69 6572 756e 6773 6d6f   Bilanzierungsmo
+000021c0: 6e61 7420 6265 7265 6974 733c 2f74 6578  nat bereits</tex
+000021d0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+000021e0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+000021f0: 3539 3922 2079 3d22 2d32 3338 2e38 2220  599" y="-238.8" 
+00002200: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00002210: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00002220: 697a 653d 2231 342e 3030 223e 6d69 7467  ize="14.00">mitg
+00002230: 6574 6569 6c74 2c20 6461 7373 2064 6965  eteilt, dass die
+00002240: 2077 6569 7465 7265 6e20 5072 2623 3235   weiteren Pr&#25
+00002250: 323b 6675 6e67 656e 2061 7566 2045 6265  2;fungen auf Ebe
+00002260: 6e65 2064 6573 2042 473c 2f74 6578 743e  ne des BG</text>
+00002270: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00002280: 6f72 3d22 7374 6172 7422 2078 3d22 3539  or="start" x="59
+00002290: 3922 2079 3d22 2d32 3234 2e38 2220 666f  9" y="-224.8" fo
+000022a0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000022b0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+000022c0: 653d 2231 342e 3030 223e 7374 6174 7466  e="14.00">stattf
+000022d0: 696e 6465 6e20 6d26 2332 3532 3b73 7365  inden m&#252;sse
+000022e0: 6e3f 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  n?</text>.</g>.<
+000022f0: 212d 2d20 3226 2334 353b 2667 743b 3520  !-- 2&#45;&gt;5 
+00002300: 2d2d 3e0a 3c67 2069 643d 2265 6467 6535  -->.<g id="edge5
+00002310: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
+00002320: 3c74 6974 6c65 3e32 2d26 6774 3b35 3c2f  <title>2-&gt;5</
+00002330: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+00002340: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00002350: 2262 6c61 636b 2220 643d 224d 3636 372e  "black" d="M667.
+00002360: 3134 2c2d 3332 392e 3539 4336 3933 2e39  14,-329.59C693.9
+00002370: 382c 2d33 3135 2e35 2037 3332 2e36 332c  8,-315.5 732.63,
+00002380: 2d32 3935 2e31 3920 3736 352e 3737 2c2d  -295.19 765.77,-
+00002390: 3237 372e 3739 222f 3e0a 3c70 6f6c 7967  277.79"/>.<polyg
+000023a0: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+000023b0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+000023c0: 6f69 6e74 733d 2237 3637 2e32 392c 2d32  oints="767.29,-2
+000023d0: 3830 2e39 3420 3737 342e 3532 2c2d 3237  80.94 774.52,-27
+000023e0: 332e 3139 2037 3634 2e30 342c 2d32 3734  3.19 764.04,-274
+000023f0: 2e37 3520 3736 372e 3239 2c2d 3238 302e  .75 767.29,-280.
+00002400: 3934 222f 3e0a 3c74 6578 7420 7465 7874  94"/>.<text text
+00002410: 2d61 6e63 686f 723d 226d 6964 646c 6522  -anchor="middle"
+00002420: 2078 3d22 3734 3622 2079 3d22 2d32 3933   x="746" y="-293
+00002430: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00002440: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00002450: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00002460: 4a61 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  Ja</text>.</g>.<
+00002470: 212d 2d20 456e 6465 202d 2d3e 0a3c 6720  !-- Ende -->.<g 
+00002480: 6964 3d22 6e6f 6465 3622 2063 6c61 7373  id="node6" class
+00002490: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
+000024a0: 456e 6465 3c2f 7469 746c 653e 0a3c 706f  Ende</title>.<po
+000024b0: 6c79 676f 6e20 6669 6c6c 3d22 2337 6138  lygon fill="#7a8
+000024c0: 6461 3122 2073 7472 6f6b 653d 2262 6c61  da1" stroke="bla
+000024d0: 636b 2220 706f 696e 7473 3d22 3633 392e  ck" points="639.
+000024e0: 352c 2d34 3320 3537 342e 352c 2d34 3320  5,-43 574.5,-43 
+000024f0: 3537 342e 352c 2d37 2036 3339 2e35 2c2d  574.5,-7 639.5,-
+00002500: 3720 3633 392e 352c 2d34 3322 2f3e 0a3c  7 639.5,-43"/>.<
+00002510: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00002520: 3d22 6d69 6464 6c65 2220 783d 2236 3037  ="middle" x="607
+00002530: 2220 793d 222d 3231 2e33 2220 666f 6e74  " y="-21.3" font
+00002540: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00002550: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00002560: 2231 342e 3030 223e 456e 6465 3c2f 7465  "14.00">Ende</te
+00002570: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3326  xt>.</g>.<!-- 3&
+00002580: 2334 353b 2667 743b 456e 6465 202d 2d3e  #45;&gt;Ende -->
+00002590: 0a3c 6720 6964 3d22 6564 6765 3722 2063  .<g id="edge7" c
+000025a0: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
+000025b0: 746c 653e 332d 2667 743b 456e 6465 3c2f  tle>3-&gt;Ende</
+000025c0: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+000025d0: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+000025e0: 2262 6c61 636b 2220 643d 224d 3438 352e  "black" d="M485.
+000025f0: 3936 2c2d 3231 382e 3643 3532 312e 3137  96,-218.6C521.17
+00002600: 2c2d 3230 362e 3636 2035 3535 2e32 342c  ,-206.66 555.24,
+00002610: 2d31 3838 2e35 3220 3538 302c 2d31 3631  -188.52 580,-161
+00002620: 2036 3036 2e31 332c 2d31 3331 2e39 3520   606.13,-131.95 
+00002630: 3630 392e 392c 2d38 342e 3935 2036 3039  609.9,-84.95 609
+00002640: 2e32 312c 2d35 342e 3737 222f 3e0a 3c70  .21,-54.77"/>.<p
+00002650: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
+00002660: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
+00002670: 6b22 2070 6f69 6e74 733d 2236 3132 2e37  k" points="612.7
+00002680: 312c 2d35 342e 3720 3630 382e 3738 2c2d  1,-54.7 608.78,-
+00002690: 3434 2e38 3620 3630 352e 3732 2c2d 3535  44.86 605.72,-55
+000026a0: 2036 3132 2e37 312c 2d35 342e 3722 2f3e   612.71,-54.7"/>
+000026b0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+000026c0: 6f72 3d22 6d69 6464 6c65 2220 783d 2236  or="middle" x="6
+000026d0: 3133 2220 793d 222d 3132 372e 3322 2066  13" y="-127.3" f
+000026e0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+000026f0: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00002700: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
+00002710: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2034  ext>.</g>.<!-- 4
+00002720: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
+00002730: 3722 2063 6c61 7373 3d22 6e6f 6465 223e  7" class="node">
+00002740: 0a3c 7469 746c 653e 343c 2f74 6974 6c65  .<title>4</title
+00002750: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
+00002760: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
+00002770: 6c61 636b 2220 643d 224d 3535 392c 2d31  lack" d="M559,-1
+00002780: 3631 4335 3539 2c2d 3136 3120 3839 2c2d  61C559,-161 89,-
+00002790: 3136 3120 3839 2c2d 3136 3120 3833 2c2d  161 89,-161 83,-
+000027a0: 3136 3120 3737 2c2d 3135 3520 3737 2c2d  161 77,-155 77,-
+000027b0: 3134 3920 3737 2c2d 3134 3920 3737 2c2d  149 77,-149 77,-
+000027c0: 3131 3320 3737 2c2d 3131 3320 3737 2c2d  113 77,-113 77,-
+000027d0: 3130 3720 3833 2c2d 3130 3120 3839 2c2d  107 83,-101 89,-
+000027e0: 3130 3120 3839 2c2d 3130 3120 3535 392c  101 89,-101 559,
+000027f0: 2d31 3031 2035 3539 2c2d 3130 3120 3536  -101 559,-101 56
+00002800: 352c 2d31 3031 2035 3731 2c2d 3130 3720  5,-101 571,-107 
+00002810: 3537 312c 2d31 3133 2035 3731 2c2d 3131  571,-113 571,-11
+00002820: 3320 3537 312c 2d31 3439 2035 3731 2c2d  3 571,-149 571,-
+00002830: 3134 3920 3537 312c 2d31 3535 2035 3635  149 571,-155 565
+00002840: 2c2d 3136 3120 3535 392c 2d31 3631 222f  ,-161 559,-161"/
+00002850: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00002860: 686f 723d 2273 7461 7274 2220 783d 2239  hor="start" x="9
+00002870: 3122 2079 3d22 2d31 3431 2e38 2220 666f  1" y="-141.8" fo
+00002880: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00002890: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+000028a0: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
+000028b0: 7369 7a65 3d22 3134 2e30 3022 3e34 3a20  size="14.00">4: 
+000028c0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+000028d0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+000028e0: 2220 783d 2231 3131 2220 793d 222d 3134  " x="111" y="-14
+000028f0: 312e 3822 2066 6f6e 742d 6661 6d69 6c79  1.8" font-family
+00002900: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00002910: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00002920: 3e48 6174 2064 6572 2042 4b56 2064 656d  >Hat der BKV dem
+00002930: 2042 494b 4f20 6626 2332 3532 3b72 2064   BIKO f&#252;r d
+00002940: 6965 7365 6e20 4269 6c61 6e7a 6965 7275  iesen Bilanzieru
+00002950: 6e67 736d 6f6e 6174 2062 6572 6569 7473  ngsmonat bereits
+00002960: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+00002970: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00002980: 2220 783d 2239 3122 2079 3d22 2d31 3237  " x="91" y="-127
+00002990: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+000029a0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+000029b0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+000029c0: 6d69 7467 6574 6569 6c74 2c20 6461 7373  mitgeteilt, dass
+000029d0: 2064 6965 2077 6569 7465 7265 6e20 5072   die weiteren Pr
+000029e0: 2623 3235 323b 6675 6e67 656e 2061 7566  &#252;fungen auf
+000029f0: 2045 6265 6e65 2064 6573 2042 473c 2f74   Ebene des BG</t
+00002a00: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00002a10: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00002a20: 3d22 3931 2220 793d 222d 3131 332e 3822  ="91" y="-113.8"
+00002a30: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00002a40: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00002a50: 7369 7a65 3d22 3134 2e30 3022 3e73 7461  size="14.00">sta
+00002a60: 7474 6669 6e64 656e 206d 2623 3235 323b  ttfinden m&#252;
+00002a70: 7373 656e 3f3c 2f74 6578 743e 0a3c 2f67  ssen?</text>.</g
+00002a80: 3e0a 3c21 2d2d 2033 2623 3435 3b26 6774  >.<!-- 3&#45;&gt
+00002a90: 3b34 202d 2d3e 0a3c 6720 6964 3d22 6564  ;4 -->.<g id="ed
+00002aa0: 6765 3622 2063 6c61 7373 3d22 6564 6765  ge6" class="edge
+00002ab0: 223e 0a3c 7469 746c 653e 332d 2667 743b  ">.<title>3-&gt;
+00002ac0: 343c 2f74 6974 6c65 3e0a 3c70 6174 6820  4</title>.<path 
+00002ad0: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00002ae0: 6b65 3d22 626c 6163 6b22 2064 3d22 4d33  ke="black" d="M3
+00002af0: 3234 2c2d 3231 382e 3638 4333 3234 2c2d  24,-218.68C324,-
+00002b00: 3230 352e 3438 2033 3234 2c2d 3138 382e  205.48 324,-188.
+00002b10: 3335 2033 3234 2c2d 3137 322e 3831 222f  35 324,-172.81"/
+00002b20: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+00002b30: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+00002b40: 626c 6163 6b22 2070 6f69 6e74 733d 2233  black" points="3
+00002b50: 3237 2e35 2c2d 3137 322e 3834 2033 3234  27.5,-172.84 324
+00002b60: 2c2d 3136 322e 3834 2033 3230 2e35 2c2d  ,-162.84 320.5,-
+00002b70: 3137 322e 3834 2033 3237 2e35 2c2d 3137  172.84 327.5,-17
+00002b80: 322e 3834 222f 3e0a 3c74 6578 7420 7465  2.84"/>.<text te
+00002b90: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00002ba0: 6522 2078 3d22 3334 3122 2079 3d22 2d31  e" x="341" y="-1
+00002bb0: 3832 2e38 2220 666f 6e74 2d66 616d 696c  82.8" font-famil
+00002bc0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00002bd0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00002be0: 223e 4e65 696e 3c2f 7465 7874 3e0a 3c2f  ">Nein</text>.</
+00002bf0: 673e 0a3c 212d 2d20 3426 2334 353b 2667  g>.<!-- 4&#45;&g
+00002c00: 743b 456e 6465 202d 2d3e 0a3c 6720 6964  t;Ende -->.<g id
+00002c10: 3d22 6564 6765 3922 2063 6c61 7373 3d22  ="edge9" class="
+00002c20: 6564 6765 223e 0a3c 7469 746c 653e 342d  edge">.<title>4-
+00002c30: 2667 743b 456e 6465 3c2f 7469 746c 653e  &gt;Ende</title>
+00002c40: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
+00002c50: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
+00002c60: 2220 643d 224d 3430 332e 3936 2c2d 3130  " d="M403.96,-10
+00002c70: 302e 3631 4334 3535 2e37 332c 2d38 312e  0.61C455.73,-81.
+00002c80: 3539 2035 3231 2e31 342c 2d35 372e 3535  59 521.14,-57.55
+00002c90: 2035 3633 2e35 312c 2d34 312e 3938 222f   563.51,-41.98"/
+00002ca0: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+00002cb0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+00002cc0: 626c 6163 6b22 2070 6f69 6e74 733d 2235  black" points="5
+00002cd0: 3634 2e36 392c 2d34 352e 3238 2035 3732  64.69,-45.28 572
+00002ce0: 2e38 372c 2d33 382e 3534 2035 3632 2e32  .87,-38.54 562.2
+00002cf0: 372c 2d33 382e 3731 2035 3634 2e36 392c  7,-38.71 564.69,
+00002d00: 2d34 352e 3238 222f 3e0a 3c74 6578 7420  -45.28"/>.<text 
+00002d10: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
+00002d20: 646c 6522 2078 3d22 3439 3822 2079 3d22  dle" x="498" y="
+00002d30: 2d37 312e 3822 2066 6f6e 742d 6661 6d69  -71.8" font-fami
+00002d40: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00002d50: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00002d60: 3022 3e4a 613c 2f74 6578 743e 0a3c 2f67  0">Ja</text>.</g
+00002d70: 3e0a 3c21 2d2d 2041 3032 202d 2d3e 0a3c  >.<!-- A02 -->.<
+00002d80: 6720 6964 3d22 6e6f 6465 3822 2063 6c61  g id="node8" cla
+00002d90: 7373 3d22 6e6f 6465 223e 0a3c 7469 746c  ss="node">.<titl
+00002da0: 653e 4130 323c 2f74 6974 6c65 3e0a 3c70  e>A02</title>.<p
+00002db0: 6f6c 7967 6f6e 2066 696c 6c3d 2223 6366  olygon fill="#cf
+00002dc0: 6239 3836 2220 7374 726f 6b65 3d22 626c  b986" stroke="bl
+00002dd0: 6163 6b22 2070 6f69 6e74 733d 2234 3330  ack" points="430
+00002de0: 2e35 2c2d 3530 2032 3137 2e35 2c2d 3530  .5,-50 217.5,-50
+00002df0: 2032 3137 2e35 2c30 2034 3330 2e35 2c30   217.5,0 430.5,0
+00002e00: 2034 3330 2e35 2c2d 3530 222f 3e0a 3c74   430.5,-50"/>.<t
+00002e10: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00002e20: 2273 7461 7274 2220 783d 2233 3038 2e35  "start" x="308.5
+00002e30: 2220 793d 222d 3333 2e38 2220 666f 6e74  " y="-33.8" font
+00002e40: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00002e50: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
+00002e60: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
+00002e70: 7a65 3d22 3134 2e30 3022 3e41 3032 3c2f  ze="14.00">A02</
+00002e80: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00002e90: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00002ea0: 783d 2232 3239 2e35 2220 793d 222d 3231  x="229.5" y="-21
+00002eb0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00002ec0: 2254 696d 6573 2c73 6572 6966 2220 7465  "Times,serif" te
+00002ed0: 7874 2d64 6563 6f72 6174 696f 6e3d 2275  xt-decoration="u
+00002ee0: 6e64 6572 6c69 6e65 2220 666f 6e74 2d73  nderline" font-s
+00002ef0: 697a 653d 2231 322e 3030 223e 4869 6e77  ize="12.00">Hinw
+00002f00: 6569 733a 3c2f 7465 7874 3e0a 3c74 6578  eis:</text>.<tex
+00002f10: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00002f20: 7461 7274 2220 783d 2232 3239 2e35 2220  tart" x="229.5" 
+00002f30: 793d 222d 392e 3422 2066 6f6e 742d 6661  y="-9.4" font-fa
+00002f40: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00002f50: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
+00002f60: 2e30 3022 3e46 616c 7363 6865 2041 6767  .00">Falsche Agg
+00002f70: 7265 6761 7469 6f6e 7365 6265 6e65 2042  regationsebene B
+00002f80: 473c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  G</text>.</g>.<!
+00002f90: 2d2d 2034 2623 3435 3b26 6774 3b41 3032  -- 4&#45;&gt;A02
+00002fa0: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
+00002fb0: 3822 2063 6c61 7373 3d22 6564 6765 223e  8" class="edge">
+00002fc0: 0a3c 7469 746c 653e 342d 2667 743b 4130  .<title>4-&gt;A0
+00002fd0: 323c 2f74 6974 6c65 3e0a 3c70 6174 6820  2</title>.<path 
+00002fe0: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00002ff0: 6b65 3d22 626c 6163 6b22 2064 3d22 4d33  ke="black" d="M3
+00003000: 3234 2c2d 3130 302e 3735 4333 3234 2c2d  24,-100.75C324,-
+00003010: 3838 2e36 3120 3332 342c 2d37 342e 3420  88.61 324,-74.4 
+00003020: 3332 342c 2d36 312e 3636 222f 3e0a 3c70  324,-61.66"/>.<p
+00003030: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
+00003040: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
+00003050: 6b22 2070 6f69 6e74 733d 2233 3237 2e35  k" points="327.5
+00003060: 2c2d 3631 2e39 3720 3332 342c 2d35 312e  ,-61.97 324,-51.
+00003070: 3937 2033 3230 2e35 2c2d 3631 2e39 3720  97 320.5,-61.97 
+00003080: 3332 372e 352c 2d36 312e 3937 222f 3e0a  327.5,-61.97"/>.
+00003090: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+000030a0: 723d 226d 6964 646c 6522 2078 3d22 3334  r="middle" x="34
+000030b0: 3122 2079 3d22 2d37 312e 3822 2066 6f6e  1" y="-71.8" fon
+000030c0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+000030d0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+000030e0: 3d22 3134 2e30 3022 3e4e 6569 6e3c 2f74  ="14.00">Nein</t
+000030f0: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2035  ext>.</g>.<!-- 5
+00003100: 2623 3435 3b26 6774 3b45 6e64 6520 2d2d  &#45;&gt;Ende --
+00003110: 3e0a 3c67 2069 643d 2265 6467 6531 3122  >.<g id="edge11"
+00003120: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
+00003130: 7469 746c 653e 352d 2667 743b 456e 6465  title>5-&gt;Ende
+00003140: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+00003150: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00003160: 653d 2262 6c61 636b 2220 643d 224d 3735  e="black" d="M75
+00003170: 372e 3935 2c2d 3231 312e 3535 4337 3332  7.95,-211.55C732
+00003180: 2e31 312c 2d31 3938 2e37 3620 3730 342e  .11,-198.76 704.
+00003190: 3238 2c2d 3138 312e 3836 2036 3833 2c2d  28,-181.86 683,-
+000031a0: 3136 3120 3635 312e 3439 2c2d 3133 302e  161 651.49,-130.
+000031b0: 3131 2036 3239 2e31 362c 2d38 332e 3338  11 629.16,-83.38
+000031c0: 2036 3137 2e31 382c 2d35 332e 3739 222f   617.18,-53.79"/
+000031d0: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
+000031e0: 2262 6c61 636b 2220 7374 726f 6b65 3d22  "black" stroke="
+000031f0: 626c 6163 6b22 2070 6f69 6e74 733d 2236  black" points="6
+00003200: 3230 2e35 352c 2d35 322e 3820 3631 332e  20.55,-52.8 613.
+00003210: 3635 2c2d 3434 2e37 3620 3631 342e 3033  65,-44.76 614.03
+00003220: 2c2d 3535 2e33 3520 3632 302e 3535 2c2d  ,-55.35 620.55,-
+00003230: 3532 2e38 222f 3e0a 3c74 6578 7420 7465  52.8"/>.<text te
+00003240: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00003250: 6522 2078 3d22 3730 3022 2079 3d22 2d31  e" x="700" y="-1
+00003260: 3237 2e33 2220 666f 6e74 2d66 616d 696c  27.3" font-famil
+00003270: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00003280: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00003290: 223e 4e65 696e 3c2f 7465 7874 3e0a 3c2f  ">Nein</text>.</
+000032a0: 673e 0a3c 212d 2d20 4130 3320 2d2d 3e0a  g>.<!-- A03 -->.
+000032b0: 3c67 2069 643d 226e 6f64 6531 3022 2063  <g id="node10" c
+000032c0: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
+000032d0: 746c 653e 4130 333c 2f74 6974 6c65 3e0a  tle>A03</title>.
+000032e0: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2223  <polygon fill="#
+000032f0: 6366 6239 3836 2220 7374 726f 6b65 3d22  cfb986" stroke="
+00003300: 626c 6163 6b22 2070 6f69 6e74 733d 2239  black" points="9
+00003310: 3337 2e35 2c2d 3135 3620 3732 362e 352c  37.5,-156 726.5,
+00003320: 2d31 3536 2037 3236 2e35 2c2d 3130 3620  -156 726.5,-106 
+00003330: 3933 372e 352c 2d31 3036 2039 3337 2e35  937.5,-106 937.5
+00003340: 2c2d 3135 3622 2f3e 0a3c 7465 7874 2074  ,-156"/>.<text t
+00003350: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00003360: 7422 2078 3d22 3831 362e 3522 2079 3d22  t" x="816.5" y="
+00003370: 2d31 3339 2e38 2220 666f 6e74 2d66 616d  -139.8" font-fam
+00003380: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00003390: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+000033a0: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+000033b0: 3134 2e30 3022 3e41 3033 3c2f 7465 7874  14.00">A03</text
+000033c0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+000033d0: 686f 723d 2273 7461 7274 2220 783d 2237  hor="start" x="7
+000033e0: 3338 2e35 2220 793d 222d 3132 372e 3422  38.5" y="-127.4"
+000033f0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00003400: 6d65 732c 7365 7269 6622 2074 6578 742d  mes,serif" text-
+00003410: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00003420: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00003430: 3d22 3132 2e30 3022 3e48 696e 7765 6973  ="12.00">Hinweis
+00003440: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00003450: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00003460: 7422 2078 3d22 3733 382e 3522 2079 3d22  t" x="738.5" y="
+00003470: 2d31 3135 2e34 2220 666f 6e74 2d66 616d  -115.4" font-fam
+00003480: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00003490: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
+000034a0: 3030 223e 4661 6c73 6368 6520 4167 6772  00">Falsche Aggr
+000034b0: 6567 6174 696f 6e73 6562 656e 6520 525a  egationsebene RZ
+000034c0: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+000034d0: 2d20 3526 2334 353b 2667 743b 4130 3320  - 5&#45;&gt;A03 
+000034e0: 2d2d 3e0a 3c67 2069 643d 2265 6467 6531  -->.<g id="edge1
+000034f0: 3022 2063 6c61 7373 3d22 6564 6765 223e  0" class="edge">
+00003500: 0a3c 7469 746c 653e 352d 2667 743b 4130  .<title>5-&gt;A0
+00003510: 333c 2f74 6974 6c65 3e0a 3c70 6174 6820  3</title>.<path 
+00003520: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00003530: 6b65 3d22 626c 6163 6b22 2064 3d22 4d38  ke="black" d="M8
+00003540: 3332 2c2d 3231 312e 3543 3833 322c 2d31  32,-211.5C832,-1
+00003550: 3938 2e30 3120 3833 322c 2d31 3831 2e39  98.01 832,-181.9
+00003560: 2038 3332 2c2d 3136 372e 3732 222f 3e0a   832,-167.72"/>.
+00003570: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
+00003580: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
+00003590: 6163 6b22 2070 6f69 6e74 733d 2238 3335  ack" points="835
+000035a0: 2e35 2c2d 3136 372e 3838 2038 3332 2c2d  .5,-167.88 832,-
+000035b0: 3135 372e 3838 2038 3238 2e35 2c2d 3136  157.88 828.5,-16
+000035c0: 372e 3838 2038 3335 2e35 2c2d 3136 372e  7.88 835.5,-167.
+000035d0: 3838 222f 3e0a 3c74 6578 7420 7465 7874  88"/>.<text text
+000035e0: 2d61 6e63 686f 723d 226d 6964 646c 6522  -anchor="middle"
+000035f0: 2078 3d22 3833 3922 2079 3d22 2d31 3832   x="839" y="-182
+00003600: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00003610: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00003620: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00003630: 4a61 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  Ja</text>.</g>.<
+00003640: 2f67 3e0a 3c2f 7376 673e 0a20 203c 2f67  /g>.</svg>.  </g
+00003650: 3e0a 3c2f 7376 673e 0a20 203c 2f67 3e0a  >.</svg>.  </g>.
+00003660: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0025.puml` & `ebdtable2graph-0.1.9/unittests/output/E_0025.puml`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0025.puml.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0025.puml.svg`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0401.dot` & `ebdtable2graph-0.1.9/unittests/output/E_0401.dot`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 digraph D {
     labelloc="t";
     label=<<B><FONT POINT-SIZE="18">6.2 AD: Lieferende LF an NB</FONT></B><BR/><BR/><B><FONT POINT-SIZE="16">6.2.1 E_0401_Abmeldung prüfen</FONT></B><BR/><BR/><BR/><BR/>>;
     "Start" [margin="0.2,0.12", shape=box, style=filled, fillcolor="#7a8da1", label=<<B>E_0401</B><BR align="center"/><FONT point-size="12"><B><U>Prüfende Rolle:</U> NB</B></FONT><BR align="center"/>>];
     "1" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>1: </B>Liegt ein Transaktionsgrund vor, der eine Abmeldung nur in<BR align="left"/>die Zukunft zulässt?<BR align="left"/>Das ist bei den folgenden Transaktionsgründen der Fall:<BR align="left"/> Wechsel<BR align="left"/> Ende der ESV ohne Folgelieferung<BR align="left"/> Aufhebung einer zukünftigen Zuordnung wegen<BR align="left"/>aufgehobenem Vertragsverhältnis<BR align="left"/>>];
     "2" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>2: </B>Liegt ein Transaktionsgrund vor, welcher mitteilt, dass der<BR align="left"/>Kunde vor Lieferbeginn ausgezogen ist, bzw. die<BR align="left"/>Marktlokation vor Lieferbeginn stillgelegt wurde?<BR align="left"/>Das ist bei den folgenden Transaktionsgründen der Fall:<BR align="left"/> Aufhebung einer zukünftigen Zuordnung wegen Auszug<BR align="left"/>des Kunden<BR align="left"/> Aufhebung einer zukünftigen Zuordnung wegen<BR align="left"/>Stilllegung<BR align="left"/>>];
     "3" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>3: </B>Liegt das Abmeldedatum mindestens einen Tag nach dem<BR align="left"/>Eingangsdatum der Abmeldung?<BR align="left"/>>];
-    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei Aufhebung einer zu-<BR align="left"/>künftigen Zuordnung wegen Auszug oder Still-<BR align="left"/>legung.<BR align="left"/></FONT>>];
+    "A01" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A01</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei Aufhebung einer zu-<BR align="left"/>künftigen Zuordnung wegen Auszug oder Still-<BR align="left"/>legung.<BR align="left"/></FONT>>];
     "4" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>4: </B>Liegt das Eingangsdatum mindestens 6 WT vor dem<BR align="left"/>Abmeldedatum?<BR align="left"/>>];
-    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei Transaktionsgründen für<BR align="left"/>eine Abmeldung in der Zukunft.<BR align="left"/></FONT>>];
+    "A02" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A02</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei Transaktionsgründen für<BR align="left"/>eine Abmeldung in der Zukunft.<BR align="left"/></FONT>>];
     "5" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>5: </B>Liegt der Transaktionsgrund<BR align="left"/>• Aufhebung einer zukünftigen Zuordnung wegen auf-<BR align="left"/>gehobenem Vertragsverhältnis<BR align="left"/>vor?<BR align="left"/>>];
     "6" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>6: </B>Handelt es sich um eine Marktlokation, deren Mess-<BR align="left"/>lokationen vollständig mit iMS ausgestattet sind oder/und<BR align="left"/>deren Prognosegrundlage auf Basis von Werten erfolgt?<BR align="left"/>>];
     "7" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>7: </B>Liegt das Abmeldedatum mindestens einen Tag nach dem<BR align="left"/>Eingangsdatum der Abmeldung?<BR align="left"/>>];
-    "A03" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A03</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Eingangsfrist bei iMS/kME mit RLM nicht ein-<BR align="left"/>gehalten.<BR align="left"/></FONT>>];
+    "A03" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A03</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Eingangsfrist bei iMS/kME mit RLM nicht ein-<BR align="left"/>gehalten.<BR align="left"/></FONT>>];
     "8" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>8: </B>Liegt das Eingangsdatum der Abmeldung mehr als sechs<BR align="left"/>Wochen nach dem Abmeldedatum der Abmeldung?<BR align="left"/>>];
-    "A04" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A04</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei kME ohne RLM/mME/<BR align="left"/>Pauschalanlage.<BR align="left"/></FONT>>];
+    "A04" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A04</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Fristüberschreitung bei kME ohne RLM/mME/<BR align="left"/>Pauschalanlage.<BR align="left"/></FONT>>];
     "9" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>9: </B>Erfolgt die Aufhebung einer zukünftigen Zuordnung zu dem<BR align="left"/>gleichen Datum (Zeitpunkt), welcher dem Lieferanten im<BR align="left"/>Lieferbeginn bestätigt wurde?<BR align="left"/>>];
-    "A05" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A05</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Die Aufhebung einer zukünftigen Zuordnung<BR align="left"/>muss zum Datum (Zeitpunkt) angegeben werden,<BR align="left"/>wie im Lieferbeginn bestätigt.<BR align="left"/></FONT>>];
+    "A05" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A05</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Die Aufhebung einer zukünftigen Zuordnung<BR align="left"/>muss zum Datum (Zeitpunkt) angegeben werden,<BR align="left"/>wie im Lieferbeginn bestätigt.<BR align="left"/></FONT>>];
     "10" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>10: </B>Wurde die Zuordnung des anfragenden Lieferanten zur<BR align="left"/>Marktlokation zum identischen Abmeldedatum bereits durch<BR align="left"/>eine Bestätigung in den folgenden Prozessschritten beendet?<BR align="left"/>Fall:<BR align="left"/> SD: Lieferende von LF an NB, Prozessschritt 2 "Antwort<BR align="left"/>auf Abmeldung"<BR align="left"/> SD: Lieferende von NB an LF, Prozessschritt 2 "Antwort<BR align="left"/>auf Abmeldung"<BR align="left"/> SD: Lieferbeginn, Prozessschritt 4 "Beantwortung der<BR align="left"/>Abmeldeanfrage" oder die Bestätigung erfolgt durch<BR align="left"/>die Fristverstreichung<BR align="left"/>>];
-    "A06" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A06</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Bestätigung der Abmeldung<BR align="left"/></FONT>>];
+    "A06" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A06</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Bestätigung der Abmeldung<BR align="left"/></FONT>>];
     "11" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>11: </B>Ist der anfragende LF am Folgetag des Abmeldungsdatum der<BR align="left"/>Marktlokation noch zugeordnet?<BR align="left"/>>];
     "12" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>12: </B>Liegt ein Transaktionsgrund vor, aus welchem hervorgeht,<BR align="left"/>dass der Anschlussnutzer ausgezogen ist?<BR align="left"/>Das ist bei den folgenden Transaktionsgründen der Fall:<BR align="left"/> Ein-/Auszug (Umzug)<BR align="left"/> Auszug wegen Stilllegung<BR align="left"/>>];
-    "A07" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A07</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Lieferende zum Abmeldedatum wurde bereits<BR align="left"/>bestätigt<BR align="left"/></FONT>>];
+    "A07" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A07</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Lieferende zum Abmeldedatum wurde bereits<BR align="left"/>bestätigt<BR align="left"/></FONT>>];
     "13" [margin="0.2,0.12", shape=box, style="filled,rounded", fillcolor="#7aab8a", label=<<B>13: </B>Liegt in der bereits bestätigten Abmeldung ein<BR align="left"/>Transaktionsgrund vor, aus welchem nicht hervorgeht, dass<BR align="left"/>der Anschlussnutzer ausgezogen ist?<BR align="left"/>Das ist bei den folgenden Transaktionsgründen der Fall:<BR align="left"/> Ein-/Auszug (Umzug)<BR align="left"/> Auszug wegen Stilllegung<BR align="left"/> Aufhebung einer zukünftigen Zuordnung wegen<BR align="left"/>Stilllegung<BR align="left"/>>];
-    "A08" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A08</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Lieferende zum Abmeldedatum wurde aus<BR align="left"/>gleichem Grund bereits bestätigt.<BR align="left"/></FONT>>];
-    "A09" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cca9ab", label=<<B>A09</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Erneute Bestätigung der Abmeldung aufgrund der<BR align="left"/>Information, dass der Anschlussnutzer nicht mehr<BR align="left"/>an der Marktlokation vorhanden ist.<BR align="left"/>Hinweis: Das bisher bestätigte Bilanzierungsende<BR align="left"/>bleibt unverändert bestehen.<BR align="left"/></FONT>>];
+    "A08" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A08</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Ablehnung<BR align="left"/>Lieferende zum Abmeldedatum wurde aus<BR align="left"/>gleichem Grund bereits bestätigt.<BR align="left"/></FONT>>];
+    "A09" [margin="0.17,0.08", shape=box, style=filled, fillcolor="#cfb986", label=<<B>A09</B><BR align="center"/><FONT point-size="12"><U>Hinweis:</U><BR align="left"/>Cluster: Zustimmung<BR align="left"/>Erneute Bestätigung der Abmeldung aufgrund der<BR align="left"/>Information, dass der Anschlussnutzer nicht mehr<BR align="left"/>an der Marktlokation vorhanden ist.<BR align="left"/>Hinweis: Das bisher bestätigte Bilanzierungsende<BR align="left"/>bleibt unverändert bestehen.<BR align="left"/></FONT>>];
 
     "Start" -> "1";
     "1" -> "4" [label="Ja"];
     "1" -> "2" [label="Nein"];
     "2" -> "3" [label="Ja"];
     "2" -> "6" [label="Nein"];
     "3" -> "A01" [label="Nein"];
```

### Comparing `ebdtable2graph-0.1.8/unittests/output/E_0401.dot.svg` & `ebdtable2graph-0.1.9/unittests/output/E_0401.dot.svg`

 * *Files 4% similar despite different names*

```diff
@@ -9,2316 +9,2330 @@
 00000080: 3939 392f 786c 696e 6b22 2076 6572 7369  999/xlink" versi
 00000090: 6f6e 3d22 312e 3122 2077 6964 7468 3d22  on="1.1" width="
 000000a0: 3238 3430 2e30 7078 2220 7669 6577 426f  2840.0px" viewBo
 000000b0: 783d 2230 2030 2032 3834 302e 3020 3230  x="0 0 2840.0 20
 000000c0: 3632 2e36 3636 3636 3636 3636 3636 3635  62.6666666666665
 000000d0: 2220 6865 6967 6874 3d22 3230 3632 2e36  " height="2062.6
 000000e0: 3636 3636 3636 3636 3636 3635 7078 223e  666666666665px">
-000000f0: 0a20 203c 673e 0a20 2020 203c 6720 7472  .  <g>.    <g tr
-00000100: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00000110: 7465 2835 3935 2e35 3435 3333 3933 3438  te(595.545339348
-00000120: 3236 3138 2c20 3230 362e 3236 3636 3636  2618, 206.266666
-00000130: 3636 3636 3636 3629 2073 6361 6c65 2831  6666666) scale(1
-00000140: 2031 2920 7472 616e 736c 6174 6528 302c   1) translate(0,
-00000150: 2030 2920 7363 616c 6528 392e 3332 3836   0) scale(9.3286
-00000160: 3438 3935 3835 3930 3433 3820 392e 3332  48958590438 9.32
-00000170: 3836 3438 3935 3835 3930 3433 3829 2022  8648958590438) "
-00000180: 3e3c 736f 6469 706f 6469 3a6e 616d 6564  ><sodipodi:named
-00000190: 7669 6577 2078 6d6c 6e73 3a73 6f64 6970  view xmlns:sodip
-000001a0: 6f64 693d 2268 7474 703a 2f2f 736f 6469  odi="http://sodi
-000001b0: 706f 6469 2e73 6f75 7263 6566 6f72 6765  podi.sourceforge
-000001c0: 2e6e 6574 2f44 5444 2f73 6f64 6970 6f64  .net/DTD/sodipod
-000001d0: 692d 302e 6474 6422 2078 6d6c 6e73 3a69  i-0.dtd" xmlns:i
-000001e0: 6e6b 7363 6170 653d 2268 7474 703a 2f2f  nkscape="http://
-000001f0: 7777 772e 696e 6b73 6361 7065 2e6f 7267  www.inkscape.org
-00000200: 2f6e 616d 6573 7061 6365 732f 696e 6b73  /namespaces/inks
-00000210: 6361 7065 2220 6964 3d22 6e61 6d65 6476  cape" id="namedv
-00000220: 6965 7737 2220 7061 6765 636f 6c6f 723d  iew7" pagecolor=
-00000230: 2223 6666 6666 6666 2220 626f 7264 6572  "#ffffff" border
-00000240: 636f 6c6f 723d 2223 3939 3939 3939 2220  color="#999999" 
-00000250: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
-00000260: 2220 696e 6b73 6361 7065 3a70 6167 6573  " inkscape:pages
-00000270: 6861 646f 773d 2230 2220 696e 6b73 6361  hadow="0" inksca
-00000280: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
-00000290: 3022 2069 6e6b 7363 6170 653a 7061 6765  0" inkscape:page
-000002a0: 6368 6563 6b65 7262 6f61 7264 3d22 3022  checkerboard="0"
-000002b0: 2069 6e6b 7363 6170 653a 646f 6375 6d65   inkscape:docume
-000002c0: 6e74 2d75 6e69 7473 3d22 6d6d 2220 7368  nt-units="mm" sh
-000002d0: 6f77 6772 6964 3d22 6661 6c73 6522 2066  owgrid="false" f
-000002e0: 6974 2d6d 6172 6769 6e2d 746f 703d 2230  it-margin-top="0
-000002f0: 2220 6669 742d 6d61 7267 696e 2d6c 6566  " fit-margin-lef
-00000300: 743d 2230 2220 6669 742d 6d61 7267 696e  t="0" fit-margin
-00000310: 2d72 6967 6874 3d22 3022 2066 6974 2d6d  -right="0" fit-m
-00000320: 6172 6769 6e2d 626f 7474 6f6d 3d22 3022  argin-bottom="0"
-00000330: 2069 6e6b 7363 6170 653a 7a6f 6f6d 3d22   inkscape:zoom="
-00000340: 302e 3634 3035 3233 3239 2220 696e 6b73  0.64052329" inks
-00000350: 6361 7065 3a63 783d 2231 3330 2e33 3632  cape:cx="130.362
-00000360: 3136 2220 696e 6b73 6361 7065 3a63 793d  16" inkscape:cy=
-00000370: 2234 3132 2e31 3633 2220 696e 6b73 6361  "412.163" inksca
-00000380: 7065 3a77 696e 646f 772d 7769 6474 683d  pe:window-width=
-00000390: 2231 3531 3222 2069 6e6b 7363 6170 653a  "1512" inkscape:
-000003a0: 7769 6e64 6f77 2d68 6569 6768 743d 2239  window-height="9
-000003b0: 3136 2220 696e 6b73 6361 7065 3a77 696e  16" inkscape:win
-000003c0: 646f 772d 783d 2233 3834 3022 2069 6e6b  dow-x="3840" ink
-000003d0: 7363 6170 653a 7769 6e64 6f77 2d79 3d22  scape:window-y="
-000003e0: 3133 3622 2069 6e6b 7363 6170 653a 7769  136" inkscape:wi
-000003f0: 6e64 6f77 2d6d 6178 696d 697a 6564 3d22  ndow-maximized="
-00000400: 3022 2069 6e6b 7363 6170 653a 6375 7272  0" inkscape:curr
-00000410: 656e 742d 6c61 7965 723d 226c 6179 6572  ent-layer="layer
-00000420: 3122 2f3e 0a20 203c 6465 6673 2069 643d  1"/>.  <defs id=
-00000430: 2264 6566 7332 223e 0a20 2020 203c 636c  "defs2">.    <cl
-00000440: 6970 5061 7468 2063 6c69 7050 6174 6855  ipPath clipPathU
-00000450: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00000460: 6e55 7365 2220 6964 3d22 636c 6970 5061  nUse" id="clipPa
-00000470: 7468 3233 223e 0a20 2020 2020 203c 7061  th23">.      <pa
-00000480: 7468 2064 3d22 4d20 302c 3536 382e 3135  th d="M 0,568.15
-00000490: 3620 4820 3537 392e 3233 3620 5620 3020  6 H 579.236 V 0 
-000004a0: 4820 3020 5a22 2069 643d 2270 6174 6832  H 0 Z" id="path2
-000004b0: 3122 2f3e 0a20 2020 203c 2f63 6c69 7050  1"/>.    </clipP
-000004c0: 6174 683e 0a20 203c 2f64 6566 733e 0a20  ath>.  </defs>. 
-000004d0: 203c 6720 786d 6c6e 733a 696e 6b73 6361   <g xmlns:inksca
-000004e0: 7065 3d22 6874 7470 3a2f 2f77 7777 2e69  pe="http://www.i
-000004f0: 6e6b 7363 6170 652e 6f72 672f 6e61 6d65  nkscape.org/name
-00000500: 7370 6163 6573 2f69 6e6b 7363 6170 6522  spaces/inkscape"
-00000510: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
-00000520: 224c 6179 6572 2031 2220 696e 6b73 6361  "Layer 1" inksca
-00000530: 7065 3a67 726f 7570 6d6f 6465 3d22 6c61  pe:groupmode="la
-00000540: 7965 7222 2069 643d 226c 6179 6572 3122  yer" id="layer1"
-00000550: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00000560: 736c 6174 6528 2d31 362e 3534 3139 3337  slate(-16.541937
-00000570: 2c2d 3535 2e33 3035 3236 3729 223e 0a20  ,-55.305267)">. 
-00000580: 2020 203c 6720 6964 3d22 6731 3922 2063     <g id="g19" c
-00000590: 6c69 702d 7061 7468 3d22 7572 6c28 2363  lip-path="url(#c
-000005a0: 6c69 7050 6174 6832 3329 2220 7472 616e  lipPath23)" tran
-000005b0: 7366 6f72 6d3d 226d 6174 7269 7828 302e  sform="matrix(0.
-000005c0: 3335 3237 3737 3737 2c30 2c30 2c2d 302e  35277777,0,0,-0.
-000005d0: 3335 3237 3737 3737 2c30 2e30 3130 3137  35277777,0.01017
-000005e0: 3032 332c 3234 332e 3733 3637 3529 2220  023,243.73675)" 
-000005f0: 7374 796c 653d 226f 7061 6369 7479 3a30  style="opacity:0
-00000600: 2e32 223e 0a20 2020 2020 203c 6720 6964  .2">.      <g id
-00000610: 3d22 6732 3522 2074 7261 6e73 666f 726d  ="g25" transform
-00000620: 3d22 7472 616e 736c 6174 6528 3132 322e  ="translate(122.
-00000630: 3434 342c 3332 2e37 3139 3529 223e 0a20  444,32.7195)">. 
-00000640: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
-00000650: 6d20 302c 3020 6820 2d35 362e 3130 3420  m 0,0 h -56.104 
-00000660: 6320 2d31 312c 3020 2d31 392e 3839 382c  c -11,0 -19.898,
-00000670: 392e 3132 3320 2d31 392e 3436 332c 3230  9.123 -19.463,20
-00000680: 2e31 3135 2031 302e 3539 342c 3236 372e  .115 10.594,267.
-00000690: 3139 3120 3233 312e 3237 372c 3438 312e  191 231.277,481.
-000006a0: 3330 3220 3530 312e 3032 392c 3438 312e  302 501.029,481.
-000006b0: 3330 3220 7620 2d35 362e 3032 2063 2030  302 v -56.02 c 0
-000006c0: 2c2d 3130 2e39 3820 2d38 2e36 3838 2c2d  ,-10.98 -8.688,-
-000006d0: 3139 2e38 3932 202d 3139 2e36 3538 2c2d  19.892 -19.658,-
-000006e0: 3230 2e33 3933 2043 2031 3830 2e32 392c  20.393 C 180.29,
-000006f0: 3431 342e 3639 3720 302c 3232 382e 3030  414.697 0,228.00
-00000700: 3520 302c 3022 2073 7479 6c65 3d22 6669  5 0,0" style="fi
-00000710: 6c6c 3a23 3665 6164 3833 3b66 696c 6c2d  ll:#6ead83;fill-
-00000720: 6f70 6163 6974 793a 313b 6669 6c6c 2d72  opacity:1;fill-r
-00000730: 756c 653a 6e6f 6e7a 6572 6f3b 7374 726f  ule:nonzero;stro
-00000740: 6b65 3a6e 6f6e 6522 2069 643d 2270 6174  ke:none" id="pat
-00000750: 6832 3722 2f3e 0a20 2020 2020 203c 2f67  h27"/>.      </g
-00000760: 3e0a 2020 2020 2020 3c67 2069 643d 2267  >.      <g id="g
-00000770: 3239 2220 7472 616e 7366 6f72 6d3d 2274  29" transform="t
-00000780: 7261 6e73 6c61 7465 2832 3733 2e37 3832  ranslate(273.782
-00000790: 382c 3332 2e37 3139 3529 223e 0a20 2020  8,32.7195)">.   
-000007a0: 2020 2020 203c 7061 7468 2064 3d22 6d20       <path d="m 
-000007b0: 302c 3020 6820 2d35 352e 3932 3620 6320  0,0 h -55.926 c 
-000007c0: 2d31 312e 3232 382c 3020 2d32 302e 3039  -11.228,0 -20.09
-000007d0: 312c 392e 3438 3220 2d31 392e 3433 352c  1,9.482 -19.435,
-000007e0: 3230 2e36 3920 3130 2e37 3434 2c31 3833  20.69 10.744,183
-000007f0: 2e34 3339 2031 3633 2e33 3839 2c33 3239  .439 163.389,329
-00000800: 2e33 3838 2033 3439 2e34 3835 2c33 3239  .388 349.485,329
-00000810: 2e33 3838 2076 202d 3536 2e32 3633 2063  .388 v -56.263 c
-00000820: 2030 2c2d 3130 2e37 3039 202d 382e 3237   0,-10.709 -8.27
-00000830: 332c 2d31 392e 3631 3720 2d31 382e 3935  3,-19.617 -18.95
-00000840: 372c 2d32 302e 3335 2043 2031 3132 2e38  7,-20.35 C 112.8
-00000850: 3139 2c32 3633 2e36 3936 2030 2c31 3434  19,263.696 0,144
-00000860: 2e37 3734 2030 2c30 2220 7374 796c 653d  .774 0,0" style=
-00000870: 2266 696c 6c3a 2336 6561 6438 333b 6669  "fill:#6ead83;fi
-00000880: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
-00000890: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
-000008a0: 7472 6f6b 653a 6e6f 6e65 2220 6964 3d22  troke:none" id="
-000008b0: 7061 7468 3331 222f 3e0a 2020 2020 2020  path31"/>.      
-000008c0: 3c2f 673e 0a20 2020 2020 203c 6720 6964  </g>.      <g id
-000008d0: 3d22 6733 3322 2074 7261 6e73 666f 726d  ="g33" transform
-000008e0: 3d22 7472 616e 736c 6174 6528 3432 352e  ="translate(425.
-000008f0: 3736 3637 2c33 322e 3731 3935 2922 3e0a  7667,32.7195)">.
-00000900: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
-00000910: 226d 2030 2c30 2068 202d 3535 2e34 3435  "m 0,0 h -55.445
-00000920: 2063 202d 3131 2e36 3533 2c30 202d 3230   c -11.653,0 -20
-00000930: 2e36 3034 2c31 302e 3137 202d 3139 2e33  .604,10.17 -19.3
-00000940: 3334 2c32 312e 3735 3320 3130 2e38 3636  34,21.753 10.866
-00000950: 2c39 392e 3033 3220 3935 2e30 3331 2c31  ,99.032 95.031,1
-00000960: 3736 2e33 3431 2031 3936 2e39 3139 2c31  76.341 196.919,1
-00000970: 3736 2e33 3431 2076 202d 3537 2e30 3131  76.341 v -57.011
-00000980: 2063 2030 2c2d 3130 2e30 3436 202d 372e   c 0,-10.046 -7.
-00000990: 3238 332c 2d31 382e 3735 3520 2d31 372e  283,-18.755 -17.
-000009a0: 3232 392c 2d32 302e 3136 3520 4320 3435  229,-20.165 C 45
-000009b0: 2e36 3838 2c31 3132 2e35 3232 2030 2c36  .688,112.522 0,6
-000009c0: 312e 3439 3720 302c 3022 2073 7479 6c65  1.497 0,0" style
-000009d0: 3d22 6669 6c6c 3a23 3665 6164 3833 3b66  ="fill:#6ead83;f
-000009e0: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
-000009f0: 6c6c 2d72 756c 653a 6e6f 6e7a 6572 6f3b  ll-rule:nonzero;
-00000a00: 7374 726f 6b65 3a6e 6f6e 6522 2069 643d  stroke:none" id=
-00000a10: 2270 6174 6833 3522 2f3e 0a20 2020 2020  "path35"/>.     
-00000a20: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a20   </g>.    </g>. 
-00000a30: 203c 2f67 3e0a 3c2f 673e 0a20 2020 203c   </g>.</g>.    <
-00000a40: 7376 6720 7769 6474 683d 2232 3133 3070  svg width="2130p
-00000a50: 7422 2068 6569 6768 743d 2231 3534 3770  t" height="1547p
-00000a60: 7422 2076 6965 7742 6f78 3d22 302e 3030  t" viewBox="0.00
-00000a70: 2030 2e30 3020 3231 3239 2e35 3020 3135   0.00 2129.50 15
-00000a80: 3437 2e30 3022 3e0a 3c67 2069 643d 2267  47.00">.<g id="g
-00000a90: 7261 7068 3022 2063 6c61 7373 3d22 6772  raph0" class="gr
-00000aa0: 6170 6822 2074 7261 6e73 666f 726d 3d22  aph" transform="
-00000ab0: 7363 616c 6528 3120 3129 2072 6f74 6174  scale(1 1) rotat
-00000ac0: 6528 3029 2074 7261 6e73 6c61 7465 2834  e(0) translate(4
-00000ad0: 2031 3534 3329 223e 0a3c 7469 746c 653e   1543)">.<title>
-00000ae0: 443c 2f74 6974 6c65 3e0a 3c74 6578 7420  D</title>.<text 
-00000af0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00000b00: 7274 2220 783d 2239 3136 2e37 3522 2079  rt" x="916.75" y
-00000b10: 3d22 2d31 3532 312e 3622 2066 6f6e 742d  ="-1521.6" font-
-00000b20: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00000b30: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
-00000b40: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
-00000b50: 653d 2231 382e 3030 223e 362e 3220 4144  e="18.00">6.2 AD
-00000b60: 3a20 4c69 6566 6572 656e 6465 204c 4620  : Lieferende LF 
-00000b70: 616e 204e 423c 2f74 6578 743e 0a3c 7465  an NB</text>.<te
-00000b80: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00000b90: 7374 6172 7422 2078 3d22 3931 332e 3735  start" x="913.75
-00000ba0: 2220 793d 222d 3134 3931 2e32 2220 666f  " y="-1491.2" fo
-00000bb0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00000bc0: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
-00000bd0: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
-00000be0: 7369 7a65 3d22 3136 2e30 3022 3e36 2e32  size="16.00">6.2
-00000bf0: 2e31 2045 5f30 3430 315f 4162 6d65 6c64  .1 E_0401_Abmeld
-00000c00: 756e 6720 7072 2623 3235 323b 6665 6e3c  ung pr&#252;fen<
-00000c10: 2f74 6578 743e 0a3c 212d 2d20 5374 6172  /text>.<!-- Star
-00000c20: 7420 2d2d 3e0a 3c67 2069 643d 226e 6f64  t -->.<g id="nod
-00000c30: 6531 2220 636c 6173 733d 226e 6f64 6522  e1" class="node"
-00000c40: 3e0a 3c74 6974 6c65 3e53 7461 7274 3c2f  >.<title>Start</
-00000c50: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-00000c60: 6669 6c6c 3d22 2337 6138 6461 3122 2073  fill="#7a8da1" s
-00000c70: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00000c80: 696e 7473 3d22 3134 3234 2c2d 3134 3431  ints="1424,-1441
-00000c90: 2031 3236 332c 2d31 3434 3120 3132 3633   1263,-1441 1263
-00000ca0: 2c2d 3133 3937 2031 3432 342c 2d31 3339  ,-1397 1424,-139
-00000cb0: 3720 3134 3234 2c2d 3134 3431 222f 3e0a  7 1424,-1441"/>.
-00000cc0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00000cd0: 723d 2273 7461 7274 2220 783d 2231 3331  r="start" x="131
-00000ce0: 3522 2079 3d22 2d31 3432 312e 3822 2066  5" y="-1421.8" f
-00000cf0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00000d00: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00000d10: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00000d20: 2d73 697a 653d 2231 342e 3030 223e 455f  -size="14.00">E_
-00000d30: 3034 3031 3c2f 7465 7874 3e0a 3c74 6578  0401</text>.<tex
-00000d40: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00000d50: 7461 7274 2220 783d 2231 3237 3722 2079  tart" x="1277" y
-00000d60: 3d22 2d31 3430 392e 3422 2066 6f6e 742d  ="-1409.4" font-
-00000d70: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00000d80: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
-00000d90: 3d22 626f 6c64 2220 7465 7874 2d64 6563  ="bold" text-dec
-00000da0: 6f72 6174 696f 6e3d 2275 6e64 6572 6c69  oration="underli
-00000db0: 6e65 2220 666f 6e74 2d73 697a 653d 2231  ne" font-size="1
-00000dc0: 322e 3030 223e 5072 2623 3235 323b 6665  2.00">Pr&#252;fe
-00000dd0: 6e64 6520 526f 6c6c 653a 3c2f 7465 7874  nde Rolle:</text
-00000de0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00000df0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00000e00: 3338 3322 2079 3d22 2d31 3430 392e 3422  383" y="-1409.4"
-00000e10: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00000e20: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00000e30: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
-00000e40: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
-00000e50: 204e 423c 2f74 6578 743e 0a3c 2f67 3e0a   NB</text>.</g>.
-00000e60: 3c21 2d2d 2031 202d 2d3e 0a3c 6720 6964  <!-- 1 -->.<g id
-00000e70: 3d22 6e6f 6465 3222 2063 6c61 7373 3d22  ="node2" class="
-00000e80: 6e6f 6465 223e 0a3c 7469 746c 653e 313c  node">.<title>1<
-00000e90: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00000ea0: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
-00000eb0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00000ec0: 3135 3730 2e35 2c2d 3133 3630 4331 3537  1570.5,-1360C157
-00000ed0: 302e 352c 2d31 3336 3020 3131 3136 2e35  0.5,-1360 1116.5
-00000ee0: 2c2d 3133 3630 2031 3131 362e 352c 2d31  ,-1360 1116.5,-1
-00000ef0: 3336 3020 3131 3130 2e35 2c2d 3133 3630  360 1110.5,-1360
-00000f00: 2031 3130 342e 352c 2d31 3335 3420 3131   1104.5,-1354 11
-00000f10: 3034 2e35 2c2d 3133 3438 2031 3130 342e  04.5,-1348 1104.
-00000f20: 352c 2d31 3334 3820 3131 3034 2e35 2c2d  5,-1348 1104.5,-
-00000f30: 3132 3536 2031 3130 342e 352c 2d31 3235  1256 1104.5,-125
-00000f40: 3620 3131 3034 2e35 2c2d 3132 3530 2031  6 1104.5,-1250 1
-00000f50: 3131 302e 352c 2d31 3234 3420 3131 3136  110.5,-1244 1116
-00000f60: 2e35 2c2d 3132 3434 2031 3131 362e 352c  .5,-1244 1116.5,
-00000f70: 2d31 3234 3420 3135 3730 2e35 2c2d 3132  -1244 1570.5,-12
-00000f80: 3434 2031 3537 302e 352c 2d31 3234 3420  44 1570.5,-1244 
-00000f90: 3135 3736 2e35 2c2d 3132 3434 2031 3538  1576.5,-1244 158
-00000fa0: 322e 352c 2d31 3235 3020 3135 3832 2e35  2.5,-1250 1582.5
-00000fb0: 2c2d 3132 3536 2031 3538 322e 352c 2d31  ,-1256 1582.5,-1
-00000fc0: 3235 3620 3135 3832 2e35 2c2d 3133 3438  256 1582.5,-1348
-00000fd0: 2031 3538 322e 352c 2d31 3334 3820 3135   1582.5,-1348 15
-00000fe0: 3832 2e35 2c2d 3133 3534 2031 3537 362e  82.5,-1354 1576.
-00000ff0: 352c 2d31 3336 3020 3135 3730 2e35 2c2d  5,-1360 1570.5,-
-00001000: 3133 3630 222f 3e0a 3c74 6578 7420 7465  1360"/>.<text te
-00001010: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00001020: 2220 783d 2231 3131 382e 3522 2079 3d22  " x="1118.5" y="
-00001030: 2d31 3334 302e 3822 2066 6f6e 742d 6661  -1340.8" font-fa
-00001040: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00001050: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
-00001060: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
-00001070: 2231 342e 3030 223e 313a 203c 2f74 6578  "14.00">1: </tex
-00001080: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00001090: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-000010a0: 3131 3338 2e35 2220 793d 222d 3133 3430  1138.5" y="-1340
-000010b0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-000010c0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000010d0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000010e0: 4c69 6567 7420 6569 6e20 5472 616e 7361  Liegt ein Transa
-000010f0: 6b74 696f 6e73 6772 756e 6420 766f 722c  ktionsgrund vor,
-00001100: 2064 6572 2065 696e 6520 4162 6d65 6c64   der eine Abmeld
-00001110: 756e 6720 6e75 7220 696e 3c2f 7465 7874  ung nur in</text
-00001120: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00001130: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00001140: 3131 382e 3522 2079 3d22 2d31 3332 362e  118.5" y="-1326.
-00001150: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00001160: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00001170: 742d 7369 7a65 3d22 3134 2e30 3022 3e64  t-size="14.00">d
-00001180: 6965 205a 756b 756e 6674 207a 756c 2623  ie Zukunft zul&#
-00001190: 3232 383b 7373 743f 3c2f 7465 7874 3e0a  228;sst?</text>.
-000011a0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-000011b0: 723d 2273 7461 7274 2220 783d 2231 3131  r="start" x="111
-000011c0: 382e 3522 2079 3d22 2d31 3331 322e 3822  8.5" y="-1312.8"
-000011d0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-000011e0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-000011f0: 7369 7a65 3d22 3134 2e30 3022 3e44 6173  size="14.00">Das
-00001200: 2069 7374 2062 6569 2064 656e 2066 6f6c   ist bei den fol
-00001210: 6765 6e64 656e 2054 7261 6e73 616b 7469  genden Transakti
-00001220: 6f6e 7367 7226 2332 3532 3b6e 6465 6e20  onsgr&#252;nden 
-00001230: 6465 7220 4661 6c6c 3a3c 2f74 6578 743e  der Fall:</text>
-00001240: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00001250: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
-00001260: 3138 2e35 2220 793d 222d 3132 3938 2e38  18.5" y="-1298.8
-00001270: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00001280: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00001290: 2d73 697a 653d 2231 342e 3030 223e 2623  -size="14.00">&#
-000012a0: 3631 3539 393b 2057 6563 6873 656c 3c2f  61599; Wechsel</
-000012b0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-000012c0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-000012d0: 783d 2231 3131 382e 3522 2079 3d22 2d31  x="1118.5" y="-1
-000012e0: 3238 342e 3822 2066 6f6e 742d 6661 6d69  284.8" font-fami
-000012f0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00001300: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00001310: 3022 3e26 2336 3135 3939 3b20 456e 6465  0">&#61599; Ende
-00001320: 2064 6572 2045 5356 206f 686e 6520 466f   der ESV ohne Fo
-00001330: 6c67 656c 6965 6665 7275 6e67 3c2f 7465  lgelieferung</te
-00001340: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00001350: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00001360: 2231 3131 382e 3522 2079 3d22 2d31 3237  "1118.5" y="-127
-00001370: 302e 3822 2066 6f6e 742d 6661 6d69 6c79  0.8" font-family
-00001380: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00001390: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-000013a0: 3e26 2336 3135 3939 3b20 4175 6668 6562  >&#61599; Aufheb
-000013b0: 756e 6720 6569 6e65 7220 7a75 6b26 2332  ung einer zuk&#2
-000013c0: 3532 3b6e 6674 6967 656e 205a 756f 7264  52;nftigen Zuord
-000013d0: 6e75 6e67 2077 6567 656e 3c2f 7465 7874  nung wegen</text
-000013e0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-000013f0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00001400: 3131 382e 3522 2079 3d22 2d31 3235 362e  118.5" y="-1256.
-00001410: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00001420: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00001430: 742d 7369 7a65 3d22 3134 2e30 3022 3e61  t-size="14.00">a
-00001440: 7566 6765 686f 6265 6e65 6d20 5665 7274  ufgehobenem Vert
-00001450: 7261 6773 7665 7268 2623 3232 383b 6c74  ragsverh&#228;lt
-00001460: 6e69 733c 2f74 6578 743e 0a3c 2f67 3e0a  nis</text>.</g>.
-00001470: 3c21 2d2d 2053 7461 7274 2623 3435 3b26  <!-- Start&#45;&
-00001480: 6774 3b31 202d 2d3e 0a3c 6720 6964 3d22  gt;1 -->.<g id="
-00001490: 6564 6765 3122 2063 6c61 7373 3d22 6564  edge1" class="ed
-000014a0: 6765 223e 0a3c 7469 746c 653e 5374 6172  ge">.<title>Star
-000014b0: 742d 2667 743b 313c 2f74 6974 6c65 3e0a  t-&gt;1</title>.
-000014c0: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-000014d0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-000014e0: 2064 3d22 4d31 3334 332e 352c 2d31 3339   d="M1343.5,-139
-000014f0: 362e 3634 4331 3334 332e 352c 2d31 3338  6.64C1343.5,-138
-00001500: 392e 3235 2031 3334 332e 352c 2d31 3338  9.25 1343.5,-138
-00001510: 302e 3532 2031 3334 332e 352c 2d31 3337  0.52 1343.5,-137
-00001520: 312e 3432 222f 3e0a 3c70 6f6c 7967 6f6e  1.42"/>.<polygon
-00001530: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-00001540: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00001550: 6e74 733d 2231 3334 372c 2d31 3337 312e  nts="1347,-1371.
-00001560: 3720 3133 3433 2e35 2c2d 3133 3631 2e37  7 1343.5,-1361.7
-00001570: 2031 3334 302c 2d31 3337 312e 3720 3133   1340,-1371.7 13
-00001580: 3437 2c2d 3133 3731 2e37 222f 3e0a 3c2f  47,-1371.7"/>.</
-00001590: 673e 0a3c 212d 2d20 3220 2d2d 3e0a 3c67  g>.<!-- 2 -->.<g
-000015a0: 2069 643d 226e 6f64 6533 2220 636c 6173   id="node3" clas
-000015b0: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
-000015c0: 3e32 3c2f 7469 746c 653e 0a3c 7061 7468  >2</title>.<path
-000015d0: 2066 696c 6c3d 2223 3761 6162 3861 2220   fill="#7aab8a" 
-000015e0: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
-000015f0: 3d22 4d31 3333 342e 352c 2d31 3139 3343  ="M1334.5,-1193C
-00001600: 3133 3334 2e35 2c2d 3131 3933 2038 3838  1334.5,-1193 888
-00001610: 2e35 2c2d 3131 3933 2038 3838 2e35 2c2d  .5,-1193 888.5,-
-00001620: 3131 3933 2038 3832 2e35 2c2d 3131 3933  1193 882.5,-1193
-00001630: 2038 3736 2e35 2c2d 3131 3837 2038 3736   876.5,-1187 876
-00001640: 2e35 2c2d 3131 3831 2038 3736 2e35 2c2d  .5,-1181 876.5,-
-00001650: 3131 3831 2038 3736 2e35 2c2d 3130 3735  1181 876.5,-1075
-00001660: 2038 3736 2e35 2c2d 3130 3735 2038 3736   876.5,-1075 876
-00001670: 2e35 2c2d 3130 3639 2038 3832 2e35 2c2d  .5,-1069 882.5,-
-00001680: 3130 3633 2038 3838 2e35 2c2d 3130 3633  1063 888.5,-1063
-00001690: 2038 3838 2e35 2c2d 3130 3633 2031 3333   888.5,-1063 133
-000016a0: 342e 352c 2d31 3036 3320 3133 3334 2e35  4.5,-1063 1334.5
-000016b0: 2c2d 3130 3633 2031 3334 302e 352c 2d31  ,-1063 1340.5,-1
-000016c0: 3036 3320 3133 3436 2e35 2c2d 3130 3639  063 1346.5,-1069
-000016d0: 2031 3334 362e 352c 2d31 3037 3520 3133   1346.5,-1075 13
-000016e0: 3436 2e35 2c2d 3130 3735 2031 3334 362e  46.5,-1075 1346.
-000016f0: 352c 2d31 3138 3120 3133 3436 2e35 2c2d  5,-1181 1346.5,-
-00001700: 3131 3831 2031 3334 362e 352c 2d31 3138  1181 1346.5,-118
-00001710: 3720 3133 3430 2e35 2c2d 3131 3933 2031  7 1340.5,-1193 1
-00001720: 3333 342e 352c 2d31 3139 3322 2f3e 0a3c  334.5,-1193"/>.<
-00001730: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00001740: 3d22 7374 6172 7422 2078 3d22 3839 302e  ="start" x="890.
-00001750: 3522 2079 3d22 2d31 3137 332e 3822 2066  5" y="-1173.8" f
-00001760: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001770: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00001780: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00001790: 2d73 697a 653d 2231 342e 3030 223e 323a  -size="14.00">2:
-000017a0: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
-000017b0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-000017c0: 7422 2078 3d22 3931 302e 3522 2079 3d22  t" x="910.5" y="
-000017d0: 2d31 3137 332e 3822 2066 6f6e 742d 6661  -1173.8" font-fa
-000017e0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-000017f0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
-00001800: 2e30 3022 3e4c 6965 6774 2065 696e 2054  .00">Liegt ein T
-00001810: 7261 6e73 616b 7469 6f6e 7367 7275 6e64  ransaktionsgrund
-00001820: 2076 6f72 2c20 7765 6c63 6865 7220 6d69   vor, welcher mi
-00001830: 7474 6569 6c74 2c20 6461 7373 2064 6572  tteilt, dass der
-00001840: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00001850: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00001860: 2220 783d 2238 3930 2e35 2220 793d 222d  " x="890.5" y="-
-00001870: 3131 3539 2e38 2220 666f 6e74 2d66 616d  1159.8" font-fam
-00001880: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00001890: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-000018a0: 3030 223e 4b75 6e64 6520 766f 7220 4c69  00">Kunde vor Li
-000018b0: 6566 6572 6265 6769 6e6e 2061 7573 6765  eferbeginn ausge
-000018c0: 7a6f 6765 6e20 6973 742c 2062 7a77 2e20  zogen ist, bzw. 
-000018d0: 6469 653c 2f74 6578 743e 0a3c 7465 7874  die</text>.<text
-000018e0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-000018f0: 6172 7422 2078 3d22 3839 302e 3522 2079  art" x="890.5" y
-00001900: 3d22 2d31 3134 352e 3822 2066 6f6e 742d  ="-1145.8" font-
-00001910: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00001920: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00001930: 3134 2e30 3022 3e4d 6172 6b74 6c6f 6b61  14.00">Marktloka
-00001940: 7469 6f6e 2076 6f72 204c 6965 6665 7262  tion vor Lieferb
-00001950: 6567 696e 6e20 7374 696c 6c67 656c 6567  eginn stillgeleg
-00001960: 7420 7775 7264 653f 3c2f 7465 7874 3e0a  t wurde?</text>.
-00001970: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00001980: 723d 2273 7461 7274 2220 783d 2238 3930  r="start" x="890
-00001990: 2e35 2220 793d 222d 3131 3331 2e38 2220  .5" y="-1131.8" 
-000019a0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000019b0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-000019c0: 697a 653d 2231 342e 3030 223e 4461 7320  ize="14.00">Das 
-000019d0: 6973 7420 6265 6920 6465 6e20 666f 6c67  ist bei den folg
-000019e0: 656e 6465 6e20 5472 616e 7361 6b74 696f  enden Transaktio
-000019f0: 6e73 6772 2623 3235 323b 6e64 656e 2064  nsgr&#252;nden d
-00001a00: 6572 2046 616c 6c3a 3c2f 7465 7874 3e0a  er Fall:</text>.
-00001a10: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00001a20: 723d 2273 7461 7274 2220 783d 2238 3930  r="start" x="890
-00001a30: 2e35 2220 793d 222d 3131 3137 2e38 2220  .5" y="-1117.8" 
-00001a40: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00001a50: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00001a60: 697a 653d 2231 342e 3030 223e 2623 3631  ize="14.00">&#61
-00001a70: 3539 393b 2041 7566 6865 6275 6e67 2065  599; Aufhebung e
-00001a80: 696e 6572 207a 756b 2623 3235 323b 6e66  iner zuk&#252;nf
-00001a90: 7469 6765 6e20 5a75 6f72 646e 756e 6720  tigen Zuordnung 
-00001aa0: 7765 6765 6e20 4175 737a 7567 3c2f 7465  wegen Auszug</te
-00001ab0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00001ac0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00001ad0: 2238 3930 2e35 2220 793d 222d 3131 3033  "890.5" y="-1103
-00001ae0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00001af0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00001b00: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-00001b10: 6465 7320 4b75 6e64 656e 3c2f 7465 7874  des Kunden</text
-00001b20: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00001b30: 686f 723d 2273 7461 7274 2220 783d 2238  hor="start" x="8
-00001b40: 3930 2e35 2220 793d 222d 3130 3839 2e38  90.5" y="-1089.8
-00001b50: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00001b60: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00001b70: 2d73 697a 653d 2231 342e 3030 223e 2623  -size="14.00">&#
-00001b80: 3631 3539 393b 2041 7566 6865 6275 6e67  61599; Aufhebung
-00001b90: 2065 696e 6572 207a 756b 2623 3235 323b   einer zuk&#252;
-00001ba0: 6e66 7469 6765 6e20 5a75 6f72 646e 756e  nftigen Zuordnun
-00001bb0: 6720 7765 6765 6e3c 2f74 6578 743e 0a3c  g wegen</text>.<
-00001bc0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00001bd0: 3d22 7374 6172 7422 2078 3d22 3839 302e  ="start" x="890.
-00001be0: 3522 2079 3d22 2d31 3037 352e 3822 2066  5" y="-1075.8" f
-00001bf0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001c00: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00001c10: 7a65 3d22 3134 2e30 3022 3e53 7469 6c6c  ze="14.00">Still
-00001c20: 6c65 6775 6e67 3c2f 7465 7874 3e0a 3c2f  legung</text>.</
-00001c30: 673e 0a3c 212d 2d20 3126 2334 353b 2667  g>.<!-- 1&#45;&g
-00001c40: 743b 3220 2d2d 3e0a 3c67 2069 643d 2265  t;2 -->.<g id="e
-00001c50: 6467 6533 2220 636c 6173 733d 2265 6467  dge3" class="edg
-00001c60: 6522 3e0a 3c74 6974 6c65 3e31 2d26 6774  e">.<title>1-&gt
-00001c70: 3b32 3c2f 7469 746c 653e 0a3c 7061 7468  ;2</title>.<path
-00001c80: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
-00001c90: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00001ca0: 3132 3636 2e32 352c 2d31 3234 332e 3733  1266.25,-1243.73
-00001cb0: 4331 3234 372e 3437 2c2d 3132 3239 2e38  C1247.47,-1229.8
-00001cc0: 3120 3132 3237 2e31 372c 2d31 3231 342e  1 1227.17,-1214.
-00001cd0: 3735 2031 3230 372e 3633 2c2d 3132 3030  75 1207.63,-1200
-00001ce0: 2e32 3722 2f3e 0a3c 706f 6c79 676f 6e20  .27"/>.<polygon 
-00001cf0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00001d00: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
-00001d10: 7473 3d22 3132 3039 2e37 362c 2d31 3139  ts="1209.76,-119
-00001d20: 372e 3439 2031 3139 392e 3634 2c2d 3131  7.49 1199.64,-11
-00001d30: 3934 2e33 3420 3132 3035 2e35 392c 2d31  94.34 1205.59,-1
-00001d40: 3230 332e 3131 2031 3230 392e 3736 2c2d  203.11 1209.76,-
-00001d50: 3131 3937 2e34 3922 2f3e 0a3c 7465 7874  1197.49"/>.<text
-00001d60: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00001d70: 6464 6c65 2220 783d 2231 3235 372e 3522  ddle" x="1257.5"
-00001d80: 2079 3d22 2d31 3231 342e 3822 2066 6f6e   y="-1214.8" fon
-00001d90: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00001da0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00001db0: 3d22 3134 2e30 3022 3e4e 6569 6e3c 2f74  ="14.00">Nein</t
-00001dc0: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2034  ext>.</g>.<!-- 4
-00001dd0: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
-00001de0: 3622 2063 6c61 7373 3d22 6e6f 6465 223e  6" class="node">
-00001df0: 0a3c 7469 746c 653e 343c 2f74 6974 6c65  .<title>4</title
-00001e00: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
-00001e10: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
-00001e20: 6c61 636b 2220 643d 224d 3137 3736 2c2d  lack" d="M1776,-
-00001e30: 3131 3531 4331 3737 362c 2d31 3135 3120  1151C1776,-1151 
-00001e40: 3133 3737 2c2d 3131 3531 2031 3337 372c  1377,-1151 1377,
-00001e50: 2d31 3135 3120 3133 3731 2c2d 3131 3531  -1151 1371,-1151
-00001e60: 2031 3336 352c 2d31 3134 3520 3133 3635   1365,-1145 1365
-00001e70: 2c2d 3131 3339 2031 3336 352c 2d31 3133  ,-1139 1365,-113
-00001e80: 3920 3133 3635 2c2d 3131 3137 2031 3336  9 1365,-1117 136
-00001e90: 352c 2d31 3131 3720 3133 3635 2c2d 3131  5,-1117 1365,-11
-00001ea0: 3131 2031 3337 312c 2d31 3130 3520 3133  11 1371,-1105 13
-00001eb0: 3737 2c2d 3131 3035 2031 3337 372c 2d31  77,-1105 1377,-1
-00001ec0: 3130 3520 3137 3736 2c2d 3131 3035 2031  105 1776,-1105 1
-00001ed0: 3737 362c 2d31 3130 3520 3137 3832 2c2d  776,-1105 1782,-
-00001ee0: 3131 3035 2031 3738 382c 2d31 3131 3120  1105 1788,-1111 
-00001ef0: 3137 3838 2c2d 3131 3137 2031 3738 382c  1788,-1117 1788,
-00001f00: 2d31 3131 3720 3137 3838 2c2d 3131 3339  -1117 1788,-1139
-00001f10: 2031 3738 382c 2d31 3133 3920 3137 3838   1788,-1139 1788
-00001f20: 2c2d 3131 3435 2031 3738 322c 2d31 3135  ,-1145 1782,-115
-00001f30: 3120 3137 3736 2c2d 3131 3531 222f 3e0a  1 1776,-1151"/>.
-00001f40: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00001f50: 723d 2273 7461 7274 2220 783d 2231 3337  r="start" x="137
-00001f60: 3922 2079 3d22 2d31 3133 312e 3822 2066  9" y="-1131.8" f
-00001f70: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00001f80: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00001f90: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00001fa0: 2d73 697a 653d 2231 342e 3030 223e 343a  -size="14.00">4:
-00001fb0: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
-00001fc0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00001fd0: 7422 2078 3d22 3133 3939 2220 793d 222d  t" x="1399" y="-
-00001fe0: 3131 3331 2e38 2220 666f 6e74 2d66 616d  1131.8" font-fam
-00001ff0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00002000: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00002010: 3030 223e 4c69 6567 7420 6461 7320 4569  00">Liegt das Ei
-00002020: 6e67 616e 6773 6461 7475 6d20 6d69 6e64  ngangsdatum mind
-00002030: 6573 7465 6e73 2036 2057 5420 766f 7220  estens 6 WT vor 
-00002040: 6465 6d3c 2f74 6578 743e 0a3c 7465 7874  dem</text>.<text
-00002050: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00002060: 6172 7422 2078 3d22 3133 3739 2220 793d  art" x="1379" y=
-00002070: 222d 3131 3137 2e38 2220 666f 6e74 2d66  "-1117.8" font-f
-00002080: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00002090: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-000020a0: 342e 3030 223e 4162 6d65 6c64 6564 6174  4.00">Abmeldedat
-000020b0: 756d 3f3c 2f74 6578 743e 0a3c 2f67 3e0a  um?</text>.</g>.
-000020c0: 3c21 2d2d 2031 2623 3435 3b26 6774 3b34  <!-- 1&#45;&gt;4
-000020d0: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
-000020e0: 3222 2063 6c61 7373 3d22 6564 6765 223e  2" class="edge">
-000020f0: 0a3c 7469 746c 653e 312d 2667 743b 343c  .<title>1-&gt;4<
-00002100: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00002110: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00002120: 3d22 626c 6163 6b22 2064 3d22 4d31 3432  ="black" d="M142
-00002130: 312e 3039 2c2d 3132 3433 2e37 3343 3134  1.09,-1243.73C14
-00002140: 3630 2c2d 3132 3135 2031 3530 352e 3437  60,-1215 1505.47
-00002150: 2c2d 3131 3831 2e34 3420 3135 3337 2e31  ,-1181.44 1537.1
-00002160: 332c 2d31 3135 382e 3036 222f 3e0a 3c70  3,-1158.06"/>.<p
-00002170: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00002180: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-00002190: 6b22 2070 6f69 6e74 733d 2231 3533 382e  k" points="1538.
-000021a0: 392c 2d31 3136 312e 3131 2031 3534 342e  9,-1161.11 1544.
-000021b0: 3836 2c2d 3131 3532 2e33 3520 3135 3334  86,-1152.35 1534
-000021c0: 2e37 342c 2d31 3135 352e 3438 2031 3533  .74,-1155.48 153
-000021d0: 382e 392c 2d31 3136 312e 3131 222f 3e0a  8.9,-1161.11"/>.
-000021e0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-000021f0: 723d 226d 6964 646c 6522 2078 3d22 3134  r="middle" x="14
-00002200: 3636 2e35 2220 793d 222d 3132 3134 2e38  66.5" y="-1214.8
-00002210: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00002220: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00002230: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
-00002240: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00002250: 2d20 3320 2d2d 3e0a 3c67 2069 643d 226e  - 3 -->.<g id="n
-00002260: 6f64 6534 2220 636c 6173 733d 226e 6f64  ode4" class="nod
-00002270: 6522 3e0a 3c74 6974 6c65 3e33 3c2f 7469  e">.<title>3</ti
-00002280: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
-00002290: 2223 3761 6162 3861 2220 7374 726f 6b65  "#7aab8a" stroke
-000022a0: 3d22 626c 6163 6b22 2064 3d22 4d31 3333  ="black" d="M133
-000022b0: 362c 2d39 3938 4331 3333 362c 2d39 3938  6,-998C1336,-998
-000022c0: 2038 3939 2c2d 3939 3820 3839 392c 2d39   899,-998 899,-9
-000022d0: 3938 2038 3933 2c2d 3939 3820 3838 372c  98 893,-998 887,
-000022e0: 2d39 3932 2038 3837 2c2d 3938 3620 3838  -992 887,-986 88
-000022f0: 372c 2d39 3836 2038 3837 2c2d 3936 3420  7,-986 887,-964 
-00002300: 3838 372c 2d39 3634 2038 3837 2c2d 3935  887,-964 887,-95
-00002310: 3820 3839 332c 2d39 3532 2038 3939 2c2d  8 893,-952 899,-
-00002320: 3935 3220 3839 392c 2d39 3532 2031 3333  952 899,-952 133
-00002330: 362c 2d39 3532 2031 3333 362c 2d39 3532  6,-952 1336,-952
-00002340: 2031 3334 322c 2d39 3532 2031 3334 382c   1342,-952 1348,
-00002350: 2d39 3538 2031 3334 382c 2d39 3634 2031  -958 1348,-964 1
-00002360: 3334 382c 2d39 3634 2031 3334 382c 2d39  348,-964 1348,-9
-00002370: 3836 2031 3334 382c 2d39 3836 2031 3334  86 1348,-986 134
-00002380: 382c 2d39 3932 2031 3334 322c 2d39 3938  8,-992 1342,-998
-00002390: 2031 3333 362c 2d39 3938 222f 3e0a 3c74   1336,-998"/>.<t
-000023a0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-000023b0: 2273 7461 7274 2220 783d 2239 3031 2220  "start" x="901" 
-000023c0: 793d 222d 3937 382e 3822 2066 6f6e 742d  y="-978.8" font-
-000023d0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-000023e0: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
-000023f0: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
-00002400: 653d 2231 342e 3030 223e 333a 203c 2f74  e="14.00">3: </t
-00002410: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00002420: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00002430: 3d22 3932 3122 2079 3d22 2d39 3738 2e38  ="921" y="-978.8
-00002440: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00002450: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00002460: 2d73 697a 653d 2231 342e 3030 223e 4c69  -size="14.00">Li
-00002470: 6567 7420 6461 7320 4162 6d65 6c64 6564  egt das Abmelded
-00002480: 6174 756d 206d 696e 6465 7374 656e 7320  atum mindestens 
-00002490: 6569 6e65 6e20 5461 6720 6e61 6368 2064  einen Tag nach d
-000024a0: 656d 3c2f 7465 7874 3e0a 3c74 6578 7420  em</text>.<text 
-000024b0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-000024c0: 7274 2220 783d 2239 3031 2220 793d 222d  rt" x="901" y="-
-000024d0: 3936 342e 3822 2066 6f6e 742d 6661 6d69  964.8" font-fami
-000024e0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-000024f0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00002500: 3022 3e45 696e 6761 6e67 7364 6174 756d  0">Eingangsdatum
-00002510: 2064 6572 2041 626d 656c 6475 6e67 3f3c   der Abmeldung?<
-00002520: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
-00002530: 2032 2623 3435 3b26 6774 3b33 202d 2d3e   2&#45;&gt;3 -->
-00002540: 0a3c 6720 6964 3d22 6564 6765 3422 2063  .<g id="edge4" c
-00002550: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00002560: 746c 653e 322d 2667 743b 333c 2f74 6974  tle>2-&gt;3</tit
-00002570: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-00002580: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00002590: 6163 6b22 2064 3d22 4d31 3131 342e 3036  ack" d="M1114.06
-000025a0: 2c2d 3130 3632 2e35 3243 3131 3134 2e37  ,-1062.52C1114.7
-000025b0: 392c 2d31 3034 342e 3236 2031 3131 352e  9,-1044.26 1115.
-000025c0: 3535 2c2d 3130 3235 2e31 3120 3131 3136  55,-1025.11 1116
-000025d0: 2e31 372c 2d31 3030 392e 3438 222f 3e0a  .17,-1009.48"/>.
-000025e0: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
-000025f0: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
-00002600: 6163 6b22 2070 6f69 6e74 733d 2231 3131  ack" points="111
-00002610: 392e 3635 2c2d 3130 3039 2e39 3420 3131  9.65,-1009.94 11
-00002620: 3136 2e35 352c 2d39 3939 2e38 2031 3131  16.55,-999.8 111
-00002630: 322e 3636 2c2d 3130 3039 2e36 3620 3131  2.66,-1009.66 11
-00002640: 3139 2e36 352c 2d31 3030 392e 3934 222f  19.65,-1009.94"/
-00002650: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00002660: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
-00002670: 3131 3231 2e35 2220 793d 222d 3130 3333  1121.5" y="-1033
-00002680: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00002690: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000026a0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000026b0: 4a61 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  Ja</text>.</g>.<
-000026c0: 212d 2d20 3620 2d2d 3e0a 3c67 2069 643d  !-- 6 -->.<g id=
-000026d0: 226e 6f64 6539 2220 636c 6173 733d 226e  "node9" class="n
-000026e0: 6f64 6522 3e0a 3c74 6974 6c65 3e36 3c2f  ode">.<title>6</
-000026f0: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
-00002700: 6c3d 2223 3761 6162 3861 2220 7374 726f  l="#7aab8a" stro
-00002710: 6b65 3d22 626c 6163 6b22 2064 3d22 4d38  ke="black" d="M8
-00002720: 3537 2c2d 3130 3035 4338 3537 2c2d 3130  57,-1005C857,-10
-00002730: 3035 2034 3336 2c2d 3130 3035 2034 3336  05 436,-1005 436
-00002740: 2c2d 3130 3035 2034 3330 2c2d 3130 3035  ,-1005 430,-1005
-00002750: 2034 3234 2c2d 3939 3920 3432 342c 2d39   424,-999 424,-9
-00002760: 3933 2034 3234 2c2d 3939 3320 3432 342c  93 424,-993 424,
-00002770: 2d39 3537 2034 3234 2c2d 3935 3720 3432  -957 424,-957 42
-00002780: 342c 2d39 3531 2034 3330 2c2d 3934 3520  4,-951 430,-945 
-00002790: 3433 362c 2d39 3435 2034 3336 2c2d 3934  436,-945 436,-94
-000027a0: 3520 3835 372c 2d39 3435 2038 3537 2c2d  5 857,-945 857,-
-000027b0: 3934 3520 3836 332c 2d39 3435 2038 3639  945 863,-945 869
-000027c0: 2c2d 3935 3120 3836 392c 2d39 3537 2038  ,-951 869,-957 8
-000027d0: 3639 2c2d 3935 3720 3836 392c 2d39 3933  69,-957 869,-993
-000027e0: 2038 3639 2c2d 3939 3320 3836 392c 2d39   869,-993 869,-9
-000027f0: 3939 2038 3633 2c2d 3130 3035 2038 3537  99 863,-1005 857
-00002800: 2c2d 3130 3035 222f 3e0a 3c74 6578 7420  ,-1005"/>.<text 
-00002810: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00002820: 7274 2220 783d 2234 3338 2220 793d 222d  rt" x="438" y="-
-00002830: 3938 352e 3822 2066 6f6e 742d 6661 6d69  985.8" font-fami
-00002840: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00002850: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
-00002860: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
-00002870: 342e 3030 223e 363a 203c 2f74 6578 743e  4.00">6: </text>
-00002880: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00002890: 6f72 3d22 7374 6172 7422 2078 3d22 3435  or="start" x="45
-000028a0: 3822 2079 3d22 2d39 3835 2e38 2220 666f  8" y="-985.8" fo
-000028b0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-000028c0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-000028d0: 653d 2231 342e 3030 223e 4861 6e64 656c  e="14.00">Handel
-000028e0: 7420 6573 2073 6963 6820 756d 2065 696e  t es sich um ein
-000028f0: 6520 4d61 726b 746c 6f6b 6174 696f 6e2c  e Marktlokation,
-00002900: 2064 6572 656e 204d 6573 732d 3c2f 7465   deren Mess-</te
-00002910: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00002920: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00002930: 2234 3338 2220 793d 222d 3937 312e 3822  "438" y="-971.8"
-00002940: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00002950: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00002960: 7369 7a65 3d22 3134 2e30 3022 3e6c 6f6b  size="14.00">lok
-00002970: 6174 696f 6e65 6e20 766f 6c6c 7374 2623  ationen vollst&#
-00002980: 3232 383b 6e64 6967 206d 6974 2069 4d53  228;ndig mit iMS
-00002990: 2061 7573 6765 7374 6174 7465 7420 7369   ausgestattet si
-000029a0: 6e64 206f 6465 722f 756e 643c 2f74 6578  nd oder/und</tex
-000029b0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-000029c0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-000029d0: 3433 3822 2079 3d22 2d39 3537 2e38 2220  438" y="-957.8" 
-000029e0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000029f0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00002a00: 697a 653d 2231 342e 3030 223e 6465 7265  ize="14.00">dere
-00002a10: 6e20 5072 6f67 6e6f 7365 6772 756e 646c  n Prognosegrundl
-00002a20: 6167 6520 6175 6620 4261 7369 7320 766f  age auf Basis vo
-00002a30: 6e20 5765 7274 656e 2065 7266 6f6c 6774  n Werten erfolgt
-00002a40: 3f3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  ?</text>.</g>.<!
-00002a50: 2d2d 2032 2623 3435 3b26 6774 3b36 202d  -- 2&#45;&gt;6 -
-00002a60: 2d3e 0a3c 6720 6964 3d22 6564 6765 3522  ->.<g id="edge5"
-00002a70: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
-00002a80: 7469 746c 653e 322d 2667 743b 363c 2f74  title>2-&gt;6</t
-00002a90: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00002aa0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-00002ab0: 626c 6163 6b22 2064 3d22 4d39 3132 2e39  black" d="M912.9
-00002ac0: 352c 2d31 3036 322e 3532 4338 3536 2e30  5,-1062.52C856.0
-00002ad0: 342c 2d31 3034 342e 3034 2037 3936 2e33  4,-1044.04 796.3
-00002ae0: 352c 2d31 3032 342e 3636 2037 3437 2e39  5,-1024.66 747.9
-00002af0: 332c 2d31 3030 382e 3934 222f 3e0a 3c70  3,-1008.94"/>.<p
-00002b00: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00002b10: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-00002b20: 6b22 2070 6f69 6e74 733d 2237 3439 2e31  k" points="749.1
-00002b30: 372c 2d31 3030 352e 3636 2037 3338 2e35  7,-1005.66 738.5
-00002b40: 382c 2d31 3030 352e 3920 3734 372e 3031  8,-1005.9 747.01
-00002b50: 2c2d 3130 3132 2e33 3220 3734 392e 3137  ,-1012.32 749.17
-00002b60: 2c2d 3130 3035 2e36 3622 2f3e 0a3c 7465  ,-1005.66"/>.<te
-00002b70: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00002b80: 6d69 6464 6c65 2220 783d 2238 3637 2e35  middle" x="867.5
-00002b90: 2220 793d 222d 3130 3333 2e38 2220 666f  " y="-1033.8" fo
-00002ba0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00002bb0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00002bc0: 653d 2231 342e 3030 223e 4e65 696e 3c2f  e="14.00">Nein</
-00002bd0: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00002be0: 4130 3120 2d2d 3e0a 3c67 2069 643d 226e  A01 -->.<g id="n
-00002bf0: 6f64 6535 2220 636c 6173 733d 226e 6f64  ode5" class="nod
-00002c00: 6522 3e0a 3c74 6974 6c65 3e41 3031 3c2f  e">.<title>A01</
-00002c10: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-00002c20: 6669 6c6c 3d22 2363 6361 3961 6222 2073  fill="#cca9ab" s
-00002c30: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00002c40: 696e 7473 3d22 3132 3539 2c2d 3838 3720  ints="1259,-887 
-00002c50: 3935 342c 2d38 3837 2039 3534 2c2d 3830  954,-887 954,-80
-00002c60: 3120 3132 3539 2c2d 3830 3120 3132 3539  1 1259,-801 1259
-00002c70: 2c2d 3838 3722 2f3e 0a3c 7465 7874 2074  ,-887"/>.<text t
-00002c80: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00002c90: 7422 2078 3d22 3130 3931 2220 793d 222d  t" x="1091" y="-
-00002ca0: 3837 302e 3822 2066 6f6e 742d 6661 6d69  870.8" font-fami
-00002cb0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00002cc0: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
-00002cd0: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
-00002ce0: 342e 3030 223e 4130 313c 2f74 6578 743e  4.00">A01</text>
-00002cf0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00002d00: 6f72 3d22 7374 6172 7422 2078 3d22 3936  or="start" x="96
-00002d10: 3622 2079 3d22 2d38 3538 2e34 2220 666f  6" y="-858.4" fo
-00002d20: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00002d30: 2c73 6572 6966 2220 7465 7874 2d64 6563  ,serif" text-dec
-00002d40: 6f72 6174 696f 6e3d 2275 6e64 6572 6c69  oration="underli
-00002d50: 6e65 2220 666f 6e74 2d73 697a 653d 2231  ne" font-size="1
-00002d60: 322e 3030 223e 4869 6e77 6569 733a 3c2f  2.00">Hinweis:</
-00002d70: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00002d80: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00002d90: 783d 2239 3636 2220 793d 222d 3834 362e  x="966" y="-846.
-00002da0: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-00002db0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00002dc0: 742d 7369 7a65 3d22 3132 2e30 3022 3e43  t-size="12.00">C
-00002dd0: 6c75 7374 6572 3a20 4162 6c65 686e 756e  luster: Ablehnun
-00002de0: 673c 2f74 6578 743e 0a3c 7465 7874 2074  g</text>.<text t
-00002df0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00002e00: 7422 2078 3d22 3936 3622 2079 3d22 2d38  t" x="966" y="-8
-00002e10: 3334 2e34 2220 666f 6e74 2d66 616d 696c  34.4" font-famil
-00002e20: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00002e30: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00002e40: 223e 4672 6973 7426 2332 3532 3b62 6572  ">Frist&#252;ber
-00002e50: 7363 6872 6569 7475 6e67 2062 6569 2041  schreitung bei A
-00002e60: 7566 6865 6275 6e67 2065 696e 6572 207a  ufhebung einer z
-00002e70: 752d 3c2f 7465 7874 3e0a 3c74 6578 7420  u-</text>.<text 
-00002e80: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00002e90: 7274 2220 783d 2239 3636 2220 793d 222d  rt" x="966" y="-
-00002ea0: 3832 322e 3422 2066 6f6e 742d 6661 6d69  822.4" font-fami
-00002eb0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00002ec0: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
-00002ed0: 3022 3e6b 2623 3235 323b 6e66 7469 6765  0">k&#252;nftige
-00002ee0: 6e20 5a75 6f72 646e 756e 6720 7765 6765  n Zuordnung wege
-00002ef0: 6e20 4175 737a 7567 206f 6465 7220 5374  n Auszug oder St
-00002f00: 696c 6c2d 3c2f 7465 7874 3e0a 3c74 6578  ill-</text>.<tex
-00002f10: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00002f20: 7461 7274 2220 783d 2239 3636 2220 793d  tart" x="966" y=
-00002f30: 222d 3831 302e 3422 2066 6f6e 742d 6661  "-810.4" font-fa
-00002f40: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00002f50: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
-00002f60: 2e30 3022 3e6c 6567 756e 672e 3c2f 7465  .00">legung.</te
-00002f70: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3326  xt>.</g>.<!-- 3&
-00002f80: 2334 353b 2667 743b 4130 3120 2d2d 3e0a  #45;&gt;A01 -->.
-00002f90: 3c67 2069 643d 2265 6467 6536 2220 636c  <g id="edge6" cl
-00002fa0: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
-00002fb0: 6c65 3e33 2d26 6774 3b41 3031 3c2f 7469  le>3-&gt;A01</ti
-00002fc0: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
-00002fd0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
-00002fe0: 6c61 636b 2220 643d 224d 3131 3135 2e35  lack" d="M1115.5
-00002ff0: 382c 2d39 3531 2e35 3343 3131 3134 2e33  8,-951.53C1114.3
-00003000: 342c 2d39 3336 2e38 3820 3131 3132 2e36  4,-936.88 1112.6
-00003010: 352c 2d39 3137 2e31 3220 3131 3131 2e30  5,-917.12 1111.0
-00003020: 372c 2d38 3938 2e35 3922 2f3e 0a3c 706f  7,-898.59"/>.<po
-00003030: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
-00003040: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
-00003050: 2220 706f 696e 7473 3d22 3131 3134 2e35  " points="1114.5
-00003060: 372c 2d38 3938 2e34 3420 3131 3130 2e32  7,-898.44 1110.2
-00003070: 332c 2d38 3838 2e37 3820 3131 3037 2e36  3,-888.78 1107.6
-00003080: 2c2d 3839 392e 3034 2031 3131 342e 3537  ,-899.04 1114.57
-00003090: 2c2d 3839 382e 3434 222f 3e0a 3c74 6578  ,-898.44"/>.<tex
-000030a0: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
-000030b0: 6964 646c 6522 2078 3d22 3131 3239 2e35  iddle" x="1129.5
-000030c0: 2220 793d 222d 3930 382e 3822 2066 6f6e  " y="-908.8" fon
-000030d0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000030e0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000030f0: 3d22 3134 2e30 3022 3e4e 6569 6e3c 2f74  ="14.00">Nein</t
-00003100: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2039  ext>.</g>.<!-- 9
-00003110: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
-00003120: 3134 2220 636c 6173 733d 226e 6f64 6522  14" class="node"
-00003130: 3e0a 3c74 6974 6c65 3e39 3c2f 7469 746c  >.<title>9</titl
-00003140: 653e 0a3c 7061 7468 2066 696c 6c3d 2223  e>.<path fill="#
-00003150: 3761 6162 3861 2220 7374 726f 6b65 3d22  7aab8a" stroke="
-00003160: 626c 6163 6b22 2064 3d22 4d31 3831 332c  black" d="M1813,
-00003170: 2d38 3734 4331 3831 332c 2d38 3734 2031  -874C1813,-874 1
-00003180: 3336 302c 2d38 3734 2031 3336 302c 2d38  360,-874 1360,-8
-00003190: 3734 2031 3335 342c 2d38 3734 2031 3334  74 1354,-874 134
-000031a0: 382c 2d38 3638 2031 3334 382c 2d38 3632  8,-868 1348,-862
-000031b0: 2031 3334 382c 2d38 3632 2031 3334 382c   1348,-862 1348,
-000031c0: 2d38 3236 2031 3334 382c 2d38 3236 2031  -826 1348,-826 1
-000031d0: 3334 382c 2d38 3230 2031 3335 342c 2d38  348,-820 1354,-8
-000031e0: 3134 2031 3336 302c 2d38 3134 2031 3336  14 1360,-814 136
-000031f0: 302c 2d38 3134 2031 3831 332c 2d38 3134  0,-814 1813,-814
-00003200: 2031 3831 332c 2d38 3134 2031 3831 392c   1813,-814 1819,
-00003210: 2d38 3134 2031 3832 352c 2d38 3230 2031  -814 1825,-820 1
-00003220: 3832 352c 2d38 3236 2031 3832 352c 2d38  825,-826 1825,-8
-00003230: 3236 2031 3832 352c 2d38 3632 2031 3832  26 1825,-862 182
-00003240: 352c 2d38 3632 2031 3832 352c 2d38 3638  5,-862 1825,-868
-00003250: 2031 3831 392c 2d38 3734 2031 3831 332c   1819,-874 1813,
-00003260: 2d38 3734 222f 3e0a 3c74 6578 7420 7465  -874"/>.<text te
-00003270: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00003280: 2220 783d 2231 3336 3222 2079 3d22 2d38  " x="1362" y="-8
-00003290: 3534 2e38 2220 666f 6e74 2d66 616d 696c  54.8" font-famil
-000032a0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-000032b0: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
-000032c0: 6422 2066 6f6e 742d 7369 7a65 3d22 3134  d" font-size="14
-000032d0: 2e30 3022 3e39 3a20 3c2f 7465 7874 3e0a  .00">9: </text>.
-000032e0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-000032f0: 723d 2273 7461 7274 2220 783d 2231 3338  r="start" x="138
-00003300: 3222 2079 3d22 2d38 3534 2e38 2220 666f  2" y="-854.8" fo
-00003310: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00003320: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00003330: 653d 2231 342e 3030 223e 4572 666f 6c67  e="14.00">Erfolg
-00003340: 7420 6469 6520 4175 6668 6562 756e 6720  t die Aufhebung 
-00003350: 6569 6e65 7220 7a75 6b26 2332 3532 3b6e  einer zuk&#252;n
-00003360: 6674 6967 656e 205a 756f 7264 6e75 6e67  ftigen Zuordnung
-00003370: 207a 7520 6465 6d3c 2f74 6578 743e 0a3c   zu dem</text>.<
-00003380: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00003390: 3d22 7374 6172 7422 2078 3d22 3133 3632  ="start" x="1362
-000033a0: 2220 793d 222d 3834 302e 3822 2066 6f6e  " y="-840.8" fon
-000033b0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000033c0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000033d0: 3d22 3134 2e30 3022 3e67 6c65 6963 6865  ="14.00">gleiche
-000033e0: 6e20 4461 7475 6d20 285a 6569 7470 756e  n Datum (Zeitpun
-000033f0: 6b74 292c 2077 656c 6368 6572 2064 656d  kt), welcher dem
-00003400: 204c 6965 6665 7261 6e74 656e 2069 6d3c   Lieferanten im<
-00003410: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00003420: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00003430: 2078 3d22 3133 3632 2220 793d 222d 3832   x="1362" y="-82
-00003440: 362e 3822 2066 6f6e 742d 6661 6d69 6c79  6.8" font-family
-00003450: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00003460: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00003470: 3e4c 6965 6665 7262 6567 696e 6e20 6265  >Lieferbeginn be
-00003480: 7374 2623 3232 383b 7469 6774 2077 7572  st&#228;tigt wur
-00003490: 6465 3f3c 2f74 6578 743e 0a3c 2f67 3e0a  de?</text>.</g>.
-000034a0: 3c21 2d2d 2033 2623 3435 3b26 6774 3b39  <!-- 3&#45;&gt;9
-000034b0: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
-000034c0: 3722 2063 6c61 7373 3d22 6564 6765 223e  7" class="edge">
-000034d0: 0a3c 7469 746c 653e 332d 2667 743b 393c  .<title>3-&gt;9<
-000034e0: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-000034f0: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00003500: 3d22 626c 6163 6b22 2064 3d22 4d31 3139  ="black" d="M119
-00003510: 392e 3139 2c2d 3935 312e 3533 4331 3237  9.19,-951.53C127
-00003520: 332e 3632 2c2d 3933 312e 3036 2031 3338  3.62,-931.06 138
-00003530: 342e 3431 2c2d 3930 302e 3539 2031 3436  4.41,-900.59 146
-00003540: 382e 3435 2c2d 3837 372e 3437 222f 3e0a  8.45,-877.47"/>.
-00003550: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
-00003560: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
-00003570: 6163 6b22 2070 6f69 6e74 733d 2231 3436  ack" points="146
-00003580: 392e 3137 2c2d 3838 302e 3920 3134 3737  9.17,-880.9 1477
-00003590: 2e38 382c 2d38 3734 2e38 3820 3134 3637  .88,-874.88 1467
-000035a0: 2e33 312c 2d38 3734 2e31 3520 3134 3639  .31,-874.15 1469
-000035b0: 2e31 372c 2d38 3830 2e39 222f 3e0a 3c74  .17,-880.9"/>.<t
-000035c0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-000035d0: 226d 6964 646c 6522 2078 3d22 3133 3732  "middle" x="1372
-000035e0: 2e35 2220 793d 222d 3930 382e 3822 2066  .5" y="-908.8" f
-000035f0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00003600: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00003610: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
-00003620: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
-00003630: 3032 202d 2d3e 0a3c 6720 6964 3d22 6e6f  02 -->.<g id="no
-00003640: 6465 3722 2063 6c61 7373 3d22 6e6f 6465  de7" class="node
-00003650: 223e 0a3c 7469 746c 653e 4130 323c 2f74  ">.<title>A02</t
-00003660: 6974 6c65 3e0a 3c70 6f6c 7967 6f6e 2066  itle>.<polygon f
-00003670: 696c 6c3d 2223 6363 6139 6162 2220 7374  ill="#cca9ab" st
-00003680: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00003690: 6e74 733d 2232 3132 312e 352c 2d31 3031  nts="2121.5,-101
-000036a0: 3220 3137 3939 2e35 2c2d 3130 3132 2031  2 1799.5,-1012 1
-000036b0: 3739 392e 352c 2d39 3338 2032 3132 312e  799.5,-938 2121.
-000036c0: 352c 2d39 3338 2032 3132 312e 352c 2d31  5,-938 2121.5,-1
-000036d0: 3031 3222 2f3e 0a3c 7465 7874 2074 6578  012"/>.<text tex
-000036e0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-000036f0: 2078 3d22 3139 3435 2220 793d 222d 3939   x="1945" y="-99
-00003700: 352e 3822 2066 6f6e 742d 6661 6d69 6c79  5.8" font-family
-00003710: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00003720: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
-00003730: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00003740: 3030 223e 4130 323c 2f74 6578 743e 0a3c  00">A02</text>.<
-00003750: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00003760: 3d22 7374 6172 7422 2078 3d22 3138 3131  ="start" x="1811
-00003770: 2e35 2220 793d 222d 3938 332e 3422 2066  .5" y="-983.4" f
-00003780: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00003790: 732c 7365 7269 6622 2074 6578 742d 6465  s,serif" text-de
-000037a0: 636f 7261 7469 6f6e 3d22 756e 6465 726c  coration="underl
-000037b0: 696e 6522 2066 6f6e 742d 7369 7a65 3d22  ine" font-size="
-000037c0: 3132 2e30 3022 3e48 696e 7765 6973 3a3c  12.00">Hinweis:<
-000037d0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-000037e0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-000037f0: 2078 3d22 3138 3131 2e35 2220 793d 222d   x="1811.5" y="-
-00003800: 3937 312e 3422 2066 6f6e 742d 6661 6d69  971.4" font-fami
-00003810: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00003820: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
-00003830: 3022 3e43 6c75 7374 6572 3a20 4162 6c65  0">Cluster: Able
-00003840: 686e 756e 673c 2f74 6578 743e 0a3c 7465  hnung</text>.<te
-00003850: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00003860: 7374 6172 7422 2078 3d22 3138 3131 2e35  start" x="1811.5
-00003870: 2220 793d 222d 3935 392e 3422 2066 6f6e  " y="-959.4" fon
-00003880: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00003890: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000038a0: 3d22 3132 2e30 3022 3e46 7269 7374 2623  ="12.00">Frist&#
-000038b0: 3235 323b 6265 7273 6368 7265 6974 756e  252;berschreitun
-000038c0: 6720 6265 6920 5472 616e 7361 6b74 696f  g bei Transaktio
-000038d0: 6e73 6772 2623 3235 323b 6e64 656e 2066  nsgr&#252;nden f
-000038e0: 2623 3235 323b 723c 2f74 6578 743e 0a3c  &#252;r</text>.<
-000038f0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00003900: 3d22 7374 6172 7422 2078 3d22 3138 3131  ="start" x="1811
-00003910: 2e35 2220 793d 222d 3934 372e 3422 2066  .5" y="-947.4" f
-00003920: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00003930: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00003940: 7a65 3d22 3132 2e30 3022 3e65 696e 6520  ze="12.00">eine 
-00003950: 4162 6d65 6c64 756e 6720 696e 2064 6572  Abmeldung in der
-00003960: 205a 756b 756e 6674 2e3c 2f74 6578 743e   Zukunft.</text>
-00003970: 0a3c 2f67 3e0a 3c21 2d2d 2034 2623 3435  .</g>.<!-- 4&#45
-00003980: 3b26 6774 3b41 3032 202d 2d3e 0a3c 6720  ;&gt;A02 -->.<g 
-00003990: 6964 3d22 6564 6765 3822 2063 6c61 7373  id="edge8" class
-000039a0: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
-000039b0: 342d 2667 743b 4130 323c 2f74 6974 6c65  4-&gt;A02</title
-000039c0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-000039d0: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-000039e0: 6b22 2064 3d22 4d31 3633 332e 3537 2c2d  k" d="M1633.57,-
-000039f0: 3131 3034 2e35 3643 3136 3932 2e34 322c  1104.56C1692.42,
-00003a00: 2d31 3038 312e 3432 2031 3738 352e 3435  -1081.42 1785.45
-00003a10: 2c2d 3130 3434 2e38 3320 3138 3537 2e32  ,-1044.83 1857.2
-00003a20: 352c 2d31 3031 362e 3622 2f3e 0a3c 706f  5,-1016.6"/>.<po
-00003a30: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
-00003a40: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
-00003a50: 2220 706f 696e 7473 3d22 3138 3538 2e32  " points="1858.2
-00003a60: 352c 2d31 3031 392e 3937 2031 3836 362e  5,-1019.97 1866.
-00003a70: 3238 2c2d 3130 3133 2e30 3520 3138 3535  28,-1013.05 1855
-00003a80: 2e36 392c 2d31 3031 332e 3435 2031 3835  .69,-1013.45 185
-00003a90: 382e 3235 2c2d 3130 3139 2e39 3722 2f3e  8.25,-1019.97"/>
-00003aa0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00003ab0: 6f72 3d22 6d69 6464 6c65 2220 783d 2231  or="middle" x="1
-00003ac0: 3833 302e 3522 2079 3d22 2d31 3033 332e  830.5" y="-1033.
-00003ad0: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00003ae0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00003af0: 742d 7369 7a65 3d22 3134 2e30 3022 3e4e  t-size="14.00">N
-00003b00: 6569 6e3c 2f74 6578 743e 0a3c 2f67 3e0a  ein</text>.</g>.
-00003b10: 3c21 2d2d 2035 202d 2d3e 0a3c 6720 6964  <!-- 5 -->.<g id
-00003b20: 3d22 6e6f 6465 3822 2063 6c61 7373 3d22  ="node8" class="
-00003b30: 6e6f 6465 223e 0a3c 7469 746c 653e 353c  node">.<title>5<
-00003b40: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00003b50: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
-00003b60: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-00003b70: 3137 3639 2e35 2c2d 3130 3132 4331 3736  1769.5,-1012C176
-00003b80: 392e 352c 2d31 3031 3220 3133 3739 2e35  9.5,-1012 1379.5
-00003b90: 2c2d 3130 3132 2031 3337 392e 352c 2d31  ,-1012 1379.5,-1
-00003ba0: 3031 3220 3133 3733 2e35 2c2d 3130 3132  012 1373.5,-1012
-00003bb0: 2031 3336 372e 352c 2d31 3030 3620 3133   1367.5,-1006 13
-00003bc0: 3637 2e35 2c2d 3130 3030 2031 3336 372e  67.5,-1000 1367.
-00003bd0: 352c 2d31 3030 3020 3133 3637 2e35 2c2d  5,-1000 1367.5,-
-00003be0: 3935 3020 3133 3637 2e35 2c2d 3935 3020  950 1367.5,-950 
-00003bf0: 3133 3637 2e35 2c2d 3934 3420 3133 3733  1367.5,-944 1373
-00003c00: 2e35 2c2d 3933 3820 3133 3739 2e35 2c2d  .5,-938 1379.5,-
-00003c10: 3933 3820 3133 3739 2e35 2c2d 3933 3820  938 1379.5,-938 
-00003c20: 3137 3639 2e35 2c2d 3933 3820 3137 3639  1769.5,-938 1769
-00003c30: 2e35 2c2d 3933 3820 3137 3735 2e35 2c2d  .5,-938 1775.5,-
-00003c40: 3933 3820 3137 3831 2e35 2c2d 3934 3420  938 1781.5,-944 
-00003c50: 3137 3831 2e35 2c2d 3935 3020 3137 3831  1781.5,-950 1781
-00003c60: 2e35 2c2d 3935 3020 3137 3831 2e35 2c2d  .5,-950 1781.5,-
-00003c70: 3130 3030 2031 3738 312e 352c 2d31 3030  1000 1781.5,-100
-00003c80: 3020 3137 3831 2e35 2c2d 3130 3036 2031  0 1781.5,-1006 1
-00003c90: 3737 352e 352c 2d31 3031 3220 3137 3639  775.5,-1012 1769
-00003ca0: 2e35 2c2d 3130 3132 222f 3e0a 3c74 6578  .5,-1012"/>.<tex
-00003cb0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-00003cc0: 7461 7274 2220 783d 2231 3338 312e 3522  tart" x="1381.5"
-00003cd0: 2079 3d22 2d39 3932 2e38 2220 666f 6e74   y="-992.8" font
-00003ce0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00003cf0: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-00003d00: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-00003d10: 7a65 3d22 3134 2e30 3022 3e35 3a20 3c2f  ze="14.00">5: </
-00003d20: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00003d30: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00003d40: 783d 2231 3430 312e 3522 2079 3d22 2d39  x="1401.5" y="-9
-00003d50: 3932 2e38 2220 666f 6e74 2d66 616d 696c  92.8" font-famil
-00003d60: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00003d70: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00003d80: 223e 4c69 6567 7420 6465 7220 5472 616e  ">Liegt der Tran
-00003d90: 7361 6b74 696f 6e73 6772 756e 643c 2f74  saktionsgrund</t
-00003da0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-00003db0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-00003dc0: 3d22 3133 3831 2e35 2220 793d 222d 3937  ="1381.5" y="-97
-00003dd0: 382e 3822 2066 6f6e 742d 6661 6d69 6c79  8.8" font-family
-00003de0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00003df0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00003e00: 3e26 2338 3232 363b 2041 7566 6865 6275  >&#8226; Aufhebu
-00003e10: 6e67 2065 696e 6572 207a 756b 2623 3235  ng einer zuk&#25
-00003e20: 323b 6e66 7469 6765 6e20 5a75 6f72 646e  2;nftigen Zuordn
-00003e30: 756e 6720 7765 6765 6e20 6175 662d 3c2f  ung wegen auf-</
-00003e40: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00003e50: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00003e60: 783d 2231 3338 312e 3522 2079 3d22 2d39  x="1381.5" y="-9
-00003e70: 3634 2e38 2220 666f 6e74 2d66 616d 696c  64.8" font-famil
-00003e80: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00003e90: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00003ea0: 223e 6765 686f 6265 6e65 6d20 5665 7274  ">gehobenem Vert
-00003eb0: 7261 6773 7665 7268 2623 3232 383b 6c74  ragsverh&#228;lt
-00003ec0: 6e69 733c 2f74 6578 743e 0a3c 7465 7874  nis</text>.<text
-00003ed0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00003ee0: 6172 7422 2078 3d22 3133 3831 2e35 2220  art" x="1381.5" 
-00003ef0: 793d 222d 3935 302e 3822 2066 6f6e 742d  y="-950.8" font-
-00003f00: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00003f10: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00003f20: 3134 2e30 3022 3e76 6f72 3f3c 2f74 6578  14.00">vor?</tex
-00003f30: 743e 0a3c 2f67 3e0a 3c21 2d2d 2034 2623  t>.</g>.<!-- 4&#
-00003f40: 3435 3b26 6774 3b35 202d 2d3e 0a3c 6720  45;&gt;5 -->.<g 
-00003f50: 6964 3d22 6564 6765 3922 2063 6c61 7373  id="edge9" class
-00003f60: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
-00003f70: 342d 2667 743b 353c 2f74 6974 6c65 3e0a  4-&gt;5</title>.
-00003f80: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00003f90: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00003fa0: 2064 3d22 4d31 3537 362e 322c 2d31 3130   d="M1576.2,-110
-00003fb0: 342e 3732 4331 3537 352e 3932 2c2d 3130  4.72C1575.92,-10
-00003fc0: 3833 2e34 3720 3135 3735 2e34 392c 2d31  83.47 1575.49,-1
-00003fd0: 3035 302e 3738 2031 3537 352e 3133 2c2d  050.78 1575.13,-
-00003fe0: 3130 3233 2e36 3622 2f3e 0a3c 706f 6c79  1023.66"/>.<poly
-00003ff0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-00004000: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00004010: 706f 696e 7473 3d22 3135 3738 2e36 332c  points="1578.63,
-00004020: 2d31 3032 332e 3920 3135 3735 2c2d 3130  -1023.9 1575,-10
-00004030: 3133 2e39 3520 3135 3731 2e36 342c 2d31  13.95 1571.64,-1
-00004040: 3032 332e 3939 2031 3537 382e 3633 2c2d  023.99 1578.63,-
-00004050: 3130 3233 2e39 222f 3e0a 3c74 6578 7420  1023.9"/>.<text 
-00004060: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
-00004070: 646c 6522 2078 3d22 3135 3831 2e35 2220  dle" x="1581.5" 
-00004080: 793d 222d 3130 3333 2e38 2220 666f 6e74  y="-1033.8" font
-00004090: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-000040a0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-000040b0: 2231 342e 3030 223e 4a61 3c2f 7465 7874  "14.00">Ja</text
-000040c0: 3e0a 3c2f 673e 0a3c 212d 2d20 3526 2334  >.</g>.<!-- 5&#4
-000040d0: 353b 2667 743b 3920 2d2d 3e0a 3c67 2069  5;&gt;9 -->.<g i
-000040e0: 643d 2265 6467 6531 3022 2063 6c61 7373  d="edge10" class
-000040f0: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
-00004100: 352d 2667 743b 393c 2f74 6974 6c65 3e0a  5-&gt;9</title>.
-00004110: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00004120: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00004130: 2064 3d22 4d31 3537 372e 3837 2c2d 3933   d="M1577.87,-93
-00004140: 372e 3732 4331 3537 392e 3338 2c2d 3932  7.72C1579.38,-92
-00004150: 312e 3520 3135 3831 2e31 372c 2d39 3032  1.5 1581.17,-902
-00004160: 2e33 2031 3538 322e 3732 2c2d 3838 352e  .3 1582.72,-885.
-00004170: 3622 2f3e 0a3c 706f 6c79 676f 6e20 6669  6"/>.<polygon fi
-00004180: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-00004190: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-000041a0: 3d22 3135 3836 2e31 372c 2d38 3836 2e32  ="1586.17,-886.2
-000041b0: 3820 3135 3833 2e36 322c 2d38 3736 2031  8 1583.62,-876 1
-000041c0: 3537 392e 322c 2d38 3835 2e36 3420 3135  579.2,-885.64 15
-000041d0: 3836 2e31 372c 2d38 3836 2e32 3822 2f3e  86.17,-886.28"/>
-000041e0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-000041f0: 6f72 3d22 6d69 6464 6c65 2220 783d 2231  or="middle" x="1
-00004200: 3538 372e 3522 2079 3d22 2d39 3038 2e38  587.5" y="-908.8
-00004210: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00004220: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00004230: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
-00004240: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00004250: 2d20 3130 202d 2d3e 0a3c 6720 6964 3d22  - 10 -->.<g id="
-00004260: 6e6f 6465 3136 2220 636c 6173 733d 226e  node16" class="n
-00004270: 6f64 6522 3e0a 3c74 6974 6c65 3e31 303c  ode">.<title>10<
-00004280: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00004290: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
-000042a0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
-000042b0: 3133 3635 2e35 2c2d 3735 3043 3133 3635  1365.5,-750C1365
-000042c0: 2e35 2c2d 3735 3020 3932 312e 352c 2d37  .5,-750 921.5,-7
-000042d0: 3530 2039 3231 2e35 2c2d 3735 3020 3931  50 921.5,-750 91
-000042e0: 352e 352c 2d37 3530 2039 3039 2e35 2c2d  5.5,-750 909.5,-
-000042f0: 3734 3420 3930 392e 352c 2d37 3338 2039  744 909.5,-738 9
-00004300: 3039 2e35 2c2d 3733 3820 3930 392e 352c  09.5,-738 909.5,
-00004310: 2d35 3930 2039 3039 2e35 2c2d 3539 3020  -590 909.5,-590 
-00004320: 3930 392e 352c 2d35 3834 2039 3135 2e35  909.5,-584 915.5
-00004330: 2c2d 3537 3820 3932 312e 352c 2d35 3738  ,-578 921.5,-578
-00004340: 2039 3231 2e35 2c2d 3537 3820 3133 3635   921.5,-578 1365
-00004350: 2e35 2c2d 3537 3820 3133 3635 2e35 2c2d  .5,-578 1365.5,-
-00004360: 3537 3820 3133 3731 2e35 2c2d 3537 3820  578 1371.5,-578 
-00004370: 3133 3737 2e35 2c2d 3538 3420 3133 3737  1377.5,-584 1377
-00004380: 2e35 2c2d 3539 3020 3133 3737 2e35 2c2d  .5,-590 1377.5,-
-00004390: 3539 3020 3133 3737 2e35 2c2d 3733 3820  590 1377.5,-738 
-000043a0: 3133 3737 2e35 2c2d 3733 3820 3133 3737  1377.5,-738 1377
-000043b0: 2e35 2c2d 3734 3420 3133 3731 2e35 2c2d  .5,-744 1371.5,-
-000043c0: 3735 3020 3133 3635 2e35 2c2d 3735 3022  750 1365.5,-750"
-000043d0: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
-000043e0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-000043f0: 3932 332e 3522 2079 3d22 2d37 3330 2e38  923.5" y="-730.8
-00004400: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00004410: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00004420: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
-00004430: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00004440: 3e31 303a 203c 2f74 6578 743e 0a3c 7465  >10: </text>.<te
-00004450: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00004460: 7374 6172 7422 2078 3d22 3935 332e 3522  start" x="953.5"
-00004470: 2079 3d22 2d37 3330 2e38 2220 666f 6e74   y="-730.8" font
-00004480: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00004490: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-000044a0: 2231 342e 3030 223e 5775 7264 6520 6469  "14.00">Wurde di
-000044b0: 6520 5a75 6f72 646e 756e 6720 6465 7320  e Zuordnung des 
-000044c0: 616e 6672 6167 656e 6465 6e20 4c69 6566  anfragenden Lief
-000044d0: 6572 616e 7465 6e20 7a75 723c 2f74 6578  eranten zur</tex
-000044e0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-000044f0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00004500: 3932 332e 3522 2079 3d22 2d37 3136 2e38  923.5" y="-716.8
-00004510: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00004520: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00004530: 2d73 697a 653d 2231 342e 3030 223e 4d61  -size="14.00">Ma
-00004540: 726b 746c 6f6b 6174 696f 6e20 7a75 6d20  rktlokation zum 
-00004550: 6964 656e 7469 7363 6865 6e20 4162 6d65  identischen Abme
-00004560: 6c64 6564 6174 756d 2062 6572 6569 7473  ldedatum bereits
-00004570: 2064 7572 6368 3c2f 7465 7874 3e0a 3c74   durch</text>.<t
-00004580: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004590: 2273 7461 7274 2220 783d 2239 3233 2e35  "start" x="923.5
-000045a0: 2220 793d 222d 3730 322e 3822 2066 6f6e  " y="-702.8" fon
-000045b0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000045c0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000045d0: 3d22 3134 2e30 3022 3e65 696e 6520 4265  ="14.00">eine Be
-000045e0: 7374 2623 3232 383b 7469 6775 6e67 2069  st&#228;tigung i
-000045f0: 6e20 6465 6e20 666f 6c67 656e 6465 6e20  n den folgenden 
-00004600: 5072 6f7a 6573 7373 6368 7269 7474 656e  Prozessschritten
-00004610: 2062 6565 6e64 6574 3f3c 2f74 6578 743e   beendet?</text>
-00004620: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00004630: 6f72 3d22 7374 6172 7422 2078 3d22 3932  or="start" x="92
-00004640: 332e 3522 2079 3d22 2d36 3838 2e38 2220  3.5" y="-688.8" 
-00004650: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00004660: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00004670: 697a 653d 2231 342e 3030 223e 4661 6c6c  ize="14.00">Fall
-00004680: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
-00004690: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-000046a0: 7422 2078 3d22 3932 332e 3522 2079 3d22  t" x="923.5" y="
-000046b0: 2d36 3734 2e38 2220 666f 6e74 2d66 616d  -674.8" font-fam
-000046c0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-000046d0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-000046e0: 3030 223e 2623 3631 3539 393b 2053 443a  00">&#61599; SD:
-000046f0: 204c 6965 6665 7265 6e64 6520 766f 6e20   Lieferende von 
-00004700: 4c46 2061 6e20 4e42 2c20 5072 6f7a 6573  LF an NB, Prozes
-00004710: 7373 6368 7269 7474 2032 2022 416e 7477  sschritt 2 "Antw
-00004720: 6f72 743c 2f74 6578 743e 0a3c 7465 7874  ort</text>.<text
-00004730: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00004740: 6172 7422 2078 3d22 3932 332e 3522 2079  art" x="923.5" y
-00004750: 3d22 2d36 3630 2e38 2220 666f 6e74 2d66  ="-660.8" font-f
-00004760: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00004770: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00004780: 342e 3030 223e 6175 6620 4162 6d65 6c64  4.00">auf Abmeld
-00004790: 756e 6722 3c2f 7465 7874 3e0a 3c74 6578  ung"</text>.<tex
-000047a0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
-000047b0: 7461 7274 2220 783d 2239 3233 2e35 2220  tart" x="923.5" 
-000047c0: 793d 222d 3634 362e 3822 2066 6f6e 742d  y="-646.8" font-
-000047d0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-000047e0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-000047f0: 3134 2e30 3022 3e26 2336 3135 3939 3b20  14.00">&#61599; 
-00004800: 5344 3a20 4c69 6566 6572 656e 6465 2076  SD: Lieferende v
-00004810: 6f6e 204e 4220 616e 204c 462c 2050 726f  on NB an LF, Pro
-00004820: 7a65 7373 7363 6872 6974 7420 3220 2241  zessschritt 2 "A
-00004830: 6e74 776f 7274 3c2f 7465 7874 3e0a 3c74  ntwort</text>.<t
-00004840: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004850: 2273 7461 7274 2220 783d 2239 3233 2e35  "start" x="923.5
-00004860: 2220 793d 222d 3633 322e 3822 2066 6f6e  " y="-632.8" fon
-00004870: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00004880: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00004890: 3d22 3134 2e30 3022 3e61 7566 2041 626d  ="14.00">auf Abm
-000048a0: 656c 6475 6e67 223c 2f74 6578 743e 0a3c  eldung"</text>.<
-000048b0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-000048c0: 3d22 7374 6172 7422 2078 3d22 3932 332e  ="start" x="923.
-000048d0: 3522 2079 3d22 2d36 3138 2e38 2220 666f  5" y="-618.8" fo
-000048e0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-000048f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00004900: 653d 2231 342e 3030 223e 2623 3631 3539  e="14.00">&#6159
-00004910: 393b 2053 443a 204c 6965 6665 7262 6567  9; SD: Lieferbeg
-00004920: 696e 6e2c 2050 726f 7a65 7373 7363 6872  inn, Prozessschr
-00004930: 6974 7420 3420 2242 6561 6e74 776f 7274  itt 4 "Beantwort
-00004940: 756e 6720 6465 723c 2f74 6578 743e 0a3c  ung der</text>.<
-00004950: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00004960: 3d22 7374 6172 7422 2078 3d22 3932 332e  ="start" x="923.
-00004970: 3522 2079 3d22 2d36 3034 2e38 2220 666f  5" y="-604.8" fo
-00004980: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00004990: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-000049a0: 653d 2231 342e 3030 223e 4162 6d65 6c64  e="14.00">Abmeld
-000049b0: 6561 6e66 7261 6765 2220 6f64 6572 2064  eanfrage" oder d
-000049c0: 6965 2042 6573 7426 2332 3238 3b74 6967  ie Best&#228;tig
-000049d0: 756e 6720 6572 666f 6c67 7420 6475 7263  ung erfolgt durc
-000049e0: 683c 2f74 6578 743e 0a3c 7465 7874 2074  h</text>.<text t
-000049f0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00004a00: 7422 2078 3d22 3932 332e 3522 2079 3d22  t" x="923.5" y="
-00004a10: 2d35 3930 2e38 2220 666f 6e74 2d66 616d  -590.8" font-fam
-00004a20: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00004a30: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00004a40: 3030 223e 6469 6520 4672 6973 7476 6572  00">die Fristver
-00004a50: 7374 7265 6963 6875 6e67 3c2f 7465 7874  streichung</text
-00004a60: 3e0a 3c2f 673e 0a3c 212d 2d20 3526 2334  >.</g>.<!-- 5&#4
-00004a70: 353b 2667 743b 3130 202d 2d3e 0a3c 6720  5;&gt;10 -->.<g 
-00004a80: 6964 3d22 6564 6765 3131 2220 636c 6173  id="edge11" clas
-00004a90: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-00004aa0: 3e35 2d26 6774 3b31 303c 2f74 6974 6c65  >5-&gt;10</title
-00004ab0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00004ac0: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00004ad0: 6b22 2064 3d22 4d31 3336 372e 3235 2c2d  k" d="M1367.25,-
-00004ae0: 3934 302e 3932 4331 3334 362e 3232 2c2d  940.92C1346.22,-
-00004af0: 3933 342e 3833 2031 3332 392e 3038 2c2d  934.83 1329.08,-
-00004b00: 3932 372e 3836 2031 3331 392e 352c 2d39  927.86 1319.5,-9
-00004b10: 3230 2031 3237 352e 3032 2c2d 3838 332e  20 1275.02,-883.
-00004b20: 3439 2031 3239 392e 3735 2c2d 3834 392e  49 1299.75,-849.
-00004b30: 3332 2031 3236 382e 352c 2d38 3031 2031  32 1268.5,-801 1
-00004b40: 3235 392e 322c 2d37 3836 2e36 3220 3132  259.2,-786.62 12
-00004b50: 3438 2e33 342c 2d37 3732 2e33 3120 3132  48.34,-772.31 12
-00004b60: 3336 2e39 372c 2d37 3538 2e36 3922 2f3e  36.97,-758.69"/>
-00004b70: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
-00004b80: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
-00004b90: 6c61 636b 2220 706f 696e 7473 3d22 3132  lack" points="12
-00004ba0: 3339 2e39 362c 2d37 3536 2e38 2031 3233  39.96,-756.8 123
-00004bb0: 302e 3832 2c2d 3735 312e 3435 2031 3233  0.82,-751.45 123
-00004bc0: 342e 3632 2c2d 3736 312e 3333 2031 3233  4.62,-761.33 123
-00004bd0: 392e 3936 2c2d 3735 362e 3822 2f3e 0a3c  9.96,-756.8"/>.<
-00004be0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00004bf0: 3d22 6d69 6464 6c65 2220 783d 2231 3331  ="middle" x="131
-00004c00: 302e 3522 2079 3d22 2d38 3430 2e33 2220  0.5" y="-840.3" 
-00004c10: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00004c20: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00004c30: 697a 653d 2231 342e 3030 223e 4e65 696e  ize="14.00">Nein
-00004c40: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00004c50: 2d20 3720 2d2d 3e0a 3c67 2069 643d 226e  - 7 -->.<g id="n
-00004c60: 6f64 6531 3022 2063 6c61 7373 3d22 6e6f  ode10" class="no
-00004c70: 6465 223e 0a3c 7469 746c 653e 373c 2f74  de">.<title>7</t
-00004c80: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00004c90: 3d22 2337 6161 6238 6122 2073 7472 6f6b  ="#7aab8a" strok
-00004ca0: 653d 2262 6c61 636b 2220 643d 224d 3434  e="black" d="M44
-00004cb0: 392c 2d38 3637 4334 3439 2c2d 3836 3720  9,-867C449,-867 
-00004cc0: 3132 2c2d 3836 3720 3132 2c2d 3836 3720  12,-867 12,-867 
-00004cd0: 362c 2d38 3637 2030 2c2d 3836 3120 302c  6,-867 0,-861 0,
-00004ce0: 2d38 3535 2030 2c2d 3835 3520 302c 2d38  -855 0,-855 0,-8
-00004cf0: 3333 2030 2c2d 3833 3320 302c 2d38 3237  33 0,-833 0,-827
-00004d00: 2036 2c2d 3832 3120 3132 2c2d 3832 3120   6,-821 12,-821 
-00004d10: 3132 2c2d 3832 3120 3434 392c 2d38 3231  12,-821 449,-821
-00004d20: 2034 3439 2c2d 3832 3120 3435 352c 2d38   449,-821 455,-8
-00004d30: 3231 2034 3631 2c2d 3832 3720 3436 312c  21 461,-827 461,
-00004d40: 2d38 3333 2034 3631 2c2d 3833 3320 3436  -833 461,-833 46
-00004d50: 312c 2d38 3535 2034 3631 2c2d 3835 3520  1,-855 461,-855 
-00004d60: 3436 312c 2d38 3631 2034 3535 2c2d 3836  461,-861 455,-86
-00004d70: 3720 3434 392c 2d38 3637 222f 3e0a 3c74  7 449,-867"/>.<t
-00004d80: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00004d90: 2273 7461 7274 2220 783d 2231 3422 2079  "start" x="14" y
-00004da0: 3d22 2d38 3437 2e38 2220 666f 6e74 2d66  ="-847.8" font-f
-00004db0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00004dc0: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
-00004dd0: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
-00004de0: 3d22 3134 2e30 3022 3e37 3a20 3c2f 7465  ="14.00">7: </te
-00004df0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00004e00: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00004e10: 2233 3422 2079 3d22 2d38 3437 2e38 2220  "34" y="-847.8" 
-00004e20: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00004e30: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00004e40: 697a 653d 2231 342e 3030 223e 4c69 6567  ize="14.00">Lieg
-00004e50: 7420 6461 7320 4162 6d65 6c64 6564 6174  t das Abmeldedat
-00004e60: 756d 206d 696e 6465 7374 656e 7320 6569  um mindestens ei
-00004e70: 6e65 6e20 5461 6720 6e61 6368 2064 656d  nen Tag nach dem
-00004e80: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00004e90: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00004ea0: 2220 783d 2231 3422 2079 3d22 2d38 3333  " x="14" y="-833
-00004eb0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00004ec0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00004ed0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-00004ee0: 4569 6e67 616e 6773 6461 7475 6d20 6465  Eingangsdatum de
-00004ef0: 7220 4162 6d65 6c64 756e 673f 3c2f 7465  r Abmeldung?</te
-00004f00: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3626  xt>.</g>.<!-- 6&
-00004f10: 2334 353b 2667 743b 3720 2d2d 3e0a 3c67  #45;&gt;7 -->.<g
-00004f20: 2069 643d 2265 6467 6531 3222 2063 6c61   id="edge12" cla
-00004f30: 7373 3d22 6564 6765 223e 0a3c 7469 746c  ss="edge">.<titl
-00004f40: 653e 362d 2667 743b 373c 2f74 6974 6c65  e>6-&gt;7</title
-00004f50: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00004f60: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00004f70: 6b22 2064 3d22 4d35 3531 2e35 382c 2d39  k" d="M551.58,-9
-00004f80: 3434 2e35 3743 3437 392e 3838 2c2d 3932  44.57C479.88,-92
-00004f90: 322e 3333 2033 3832 2e34 322c 2d38 3932  2.33 382.42,-892
-00004fa0: 2e31 3120 3331 332e 3734 2c2d 3837 302e  .11 313.74,-870.
-00004fb0: 3831 222f 3e0a 3c70 6f6c 7967 6f6e 2066  81"/>.<polygon f
-00004fc0: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
-00004fd0: 6b65 3d22 626c 6163 6b22 2070 6f69 6e74  ke="black" point
-00004fe0: 733d 2233 3135 2e30 312c 2d38 3637 2e35  s="315.01,-867.5
-00004ff0: 3420 3330 342e 3432 2c2d 3836 372e 3932  4 304.42,-867.92
-00005000: 2033 3132 2e39 342c 2d38 3734 2e32 3320   312.94,-874.23 
-00005010: 3331 352e 3031 2c2d 3836 372e 3534 222f  315.01,-867.54"/
-00005020: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00005030: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
-00005040: 3437 302e 3522 2079 3d22 2d39 3038 2e38  470.5" y="-908.8
-00005050: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00005060: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00005070: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
-00005080: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
-00005090: 2d20 3820 2d2d 3e0a 3c67 2069 643d 226e  - 8 -->.<g id="n
-000050a0: 6f64 6531 3222 2063 6c61 7373 3d22 6e6f  ode12" class="no
-000050b0: 6465 223e 0a3c 7469 746c 653e 383c 2f74  de">.<title>8</t
-000050c0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-000050d0: 3d22 2337 6161 6238 6122 2073 7472 6f6b  ="#7aab8a" strok
-000050e0: 653d 2262 6c61 636b 2220 643d 224d 3932  e="black" d="M92
-000050f0: 342c 2d38 3637 4339 3234 2c2d 3836 3720  4,-867C924,-867 
-00005100: 3439 312c 2d38 3637 2034 3931 2c2d 3836  491,-867 491,-86
-00005110: 3720 3438 352c 2d38 3637 2034 3739 2c2d  7 485,-867 479,-
-00005120: 3836 3120 3437 392c 2d38 3535 2034 3739  861 479,-855 479
-00005130: 2c2d 3835 3520 3437 392c 2d38 3333 2034  ,-855 479,-833 4
-00005140: 3739 2c2d 3833 3320 3437 392c 2d38 3237  79,-833 479,-827
-00005150: 2034 3835 2c2d 3832 3120 3439 312c 2d38   485,-821 491,-8
-00005160: 3231 2034 3931 2c2d 3832 3120 3932 342c  21 491,-821 924,
-00005170: 2d38 3231 2039 3234 2c2d 3832 3120 3933  -821 924,-821 93
-00005180: 302c 2d38 3231 2039 3336 2c2d 3832 3720  0,-821 936,-827 
-00005190: 3933 362c 2d38 3333 2039 3336 2c2d 3833  936,-833 936,-83
-000051a0: 3320 3933 362c 2d38 3535 2039 3336 2c2d  3 936,-855 936,-
-000051b0: 3835 3520 3933 362c 2d38 3631 2039 3330  855 936,-861 930
-000051c0: 2c2d 3836 3720 3932 342c 2d38 3637 222f  ,-867 924,-867"/
-000051d0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-000051e0: 686f 723d 2273 7461 7274 2220 783d 2234  hor="start" x="4
-000051f0: 3933 2220 793d 222d 3834 372e 3822 2066  93" y="-847.8" f
-00005200: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00005210: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
-00005220: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
-00005230: 2d73 697a 653d 2231 342e 3030 223e 383a  -size="14.00">8:
-00005240: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
-00005250: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
-00005260: 7422 2078 3d22 3531 3322 2079 3d22 2d38  t" x="513" y="-8
-00005270: 3437 2e38 2220 666f 6e74 2d66 616d 696c  47.8" font-famil
-00005280: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00005290: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-000052a0: 223e 4c69 6567 7420 6461 7320 4569 6e67  ">Liegt das Eing
-000052b0: 616e 6773 6461 7475 6d20 6465 7220 4162  angsdatum der Ab
-000052c0: 6d65 6c64 756e 6720 6d65 6872 2061 6c73  meldung mehr als
-000052d0: 2073 6563 6873 3c2f 7465 7874 3e0a 3c74   sechs</text>.<t
-000052e0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-000052f0: 2273 7461 7274 2220 783d 2234 3933 2220  "start" x="493" 
-00005300: 793d 222d 3833 332e 3822 2066 6f6e 742d  y="-833.8" font-
-00005310: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00005320: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00005330: 3134 2e30 3022 3e57 6f63 6865 6e20 6e61  14.00">Wochen na
-00005340: 6368 2064 656d 2041 626d 656c 6465 6461  ch dem Abmeldeda
-00005350: 7475 6d20 6465 7220 4162 6d65 6c64 756e  tum der Abmeldun
-00005360: 673f 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  g?</text>.</g>.<
-00005370: 212d 2d20 3626 2334 353b 2667 743b 3820  !-- 6&#45;&gt;8 
-00005380: 2d2d 3e0a 3c67 2069 643d 2265 6467 6531  -->.<g id="edge1
-00005390: 3322 2063 6c61 7373 3d22 6564 6765 223e  3" class="edge">
-000053a0: 0a3c 7469 746c 653e 362d 2667 743b 383c  .<title>6-&gt;8<
-000053b0: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-000053c0: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-000053d0: 3d22 626c 6163 6b22 2064 3d22 4d36 3630  ="black" d="M660
-000053e0: 2e33 342c 2d39 3434 2e37 3343 3636 392e  .34,-944.73C669.
-000053f0: 382c 2d39 3234 2e37 3220 3638 322e 3334  8,-924.72 682.34
-00005400: 2c2d 3839 382e 3220 3639 322e 3132 2c2d  ,-898.2 692.12,-
-00005410: 3837 372e 3533 222f 3e0a 3c70 6f6c 7967  877.53"/>.<polyg
-00005420: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
-00005430: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
-00005440: 6f69 6e74 733d 2236 3935 2e31 382c 2d38  oints="695.18,-8
-00005450: 3739 2e32 3320 3639 362e 332c 2d38 3638  79.23 696.3,-868
-00005460: 2e37 2036 3838 2e38 362c 2d38 3736 2e32  .7 688.86,-876.2
-00005470: 3420 3639 352e 3138 2c2d 3837 392e 3233  4 695.18,-879.23
-00005480: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00005490: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
-000054a0: 3d22 3639 362e 3522 2079 3d22 2d39 3038  ="696.5" y="-908
-000054b0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-000054c0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000054d0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000054e0: 4e65 696e 3c2f 7465 7874 3e0a 3c2f 673e  Nein</text>.</g>
-000054f0: 0a3c 212d 2d20 4130 3320 2d2d 3e0a 3c67  .<!-- A03 -->.<g
-00005500: 2069 643d 226e 6f64 6531 3122 2063 6c61   id="node11" cla
-00005510: 7373 3d22 6e6f 6465 223e 0a3c 7469 746c  ss="node">.<titl
-00005520: 653e 4130 333c 2f74 6974 6c65 3e0a 3c70  e>A03</title>.<p
-00005530: 6f6c 7967 6f6e 2066 696c 6c3d 2223 6363  olygon fill="#cc
-00005540: 6139 6162 2220 7374 726f 6b65 3d22 626c  a9ab" stroke="bl
-00005550: 6163 6b22 2070 6f69 6e74 733d 2233 3832  ack" points="382
-00005560: 2c2d 3730 3120 3739 2c2d 3730 3120 3739  ,-701 79,-701 79
-00005570: 2c2d 3632 3720 3338 322c 2d36 3237 2033  ,-627 382,-627 3
-00005580: 3832 2c2d 3730 3122 2f3e 0a3c 7465 7874  82,-701"/>.<text
-00005590: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-000055a0: 6172 7422 2078 3d22 3231 3522 2079 3d22  art" x="215" y="
-000055b0: 2d36 3834 2e38 2220 666f 6e74 2d66 616d  -684.8" font-fam
-000055c0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-000055d0: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
-000055e0: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
-000055f0: 3134 2e30 3022 3e41 3033 3c2f 7465 7874  14.00">A03</text
-00005600: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00005610: 686f 723d 2273 7461 7274 2220 783d 2239  hor="start" x="9
-00005620: 3122 2079 3d22 2d36 3732 2e34 2220 666f  1" y="-672.4" fo
-00005630: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00005640: 2c73 6572 6966 2220 7465 7874 2d64 6563  ,serif" text-dec
-00005650: 6f72 6174 696f 6e3d 2275 6e64 6572 6c69  oration="underli
-00005660: 6e65 2220 666f 6e74 2d73 697a 653d 2231  ne" font-size="1
-00005670: 322e 3030 223e 4869 6e77 6569 733a 3c2f  2.00">Hinweis:</
-00005680: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00005690: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-000056a0: 783d 2239 3122 2079 3d22 2d36 3630 2e34  x="91" y="-660.4
-000056b0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-000056c0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-000056d0: 2d73 697a 653d 2231 322e 3030 223e 436c  -size="12.00">Cl
-000056e0: 7573 7465 723a 2041 626c 6568 6e75 6e67  uster: Ablehnung
-000056f0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00005700: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00005710: 2220 783d 2239 3122 2079 3d22 2d36 3438  " x="91" y="-648
-00005720: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
-00005730: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00005740: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
-00005750: 4569 6e67 616e 6773 6672 6973 7420 6265  Eingangsfrist be
-00005760: 6920 694d 532f 6b4d 4520 6d69 7420 524c  i iMS/kME mit RL
-00005770: 4d20 6e69 6368 7420 6569 6e2d 3c2f 7465  M nicht ein-</te
-00005780: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00005790: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-000057a0: 2239 3122 2079 3d22 2d36 3336 2e34 2220  "91" y="-636.4" 
-000057b0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000057c0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-000057d0: 697a 653d 2231 322e 3030 223e 6765 6861  ize="12.00">geha
-000057e0: 6c74 656e 2e3c 2f74 6578 743e 0a3c 2f67  lten.</text>.</g
-000057f0: 3e0a 3c21 2d2d 2037 2623 3435 3b26 6774  >.<!-- 7&#45;&gt
-00005800: 3b41 3033 202d 2d3e 0a3c 6720 6964 3d22  ;A03 -->.<g id="
-00005810: 6564 6765 3134 2220 636c 6173 733d 2265  edge14" class="e
-00005820: 6467 6522 3e0a 3c74 6974 6c65 3e37 2d26  dge">.<title>7-&
-00005830: 6774 3b41 3033 3c2f 7469 746c 653e 0a3c  gt;A03</title>.<
-00005840: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
-00005850: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00005860: 643d 224d 3233 302e 352c 2d38 3230 2e38  d="M230.5,-820.8
-00005870: 3243 3233 302e 352c 2d37 3933 2e39 3420  2C230.5,-793.94 
-00005880: 3233 302e 352c 2d37 3437 2e39 2032 3330  230.5,-747.9 230
-00005890: 2e35 2c2d 3731 322e 3832 222f 3e0a 3c70  .5,-712.82"/>.<p
-000058a0: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-000058b0: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-000058c0: 6b22 2070 6f69 6e74 733d 2232 3334 2c2d  k" points="234,-
-000058d0: 3731 322e 3920 3233 302e 352c 2d37 3032  712.9 230.5,-702
-000058e0: 2e39 2032 3237 2c2d 3731 322e 3920 3233  .9 227,-712.9 23
-000058f0: 342c 2d37 3132 2e39 222f 3e0a 3c74 6578  4,-712.9"/>.<tex
-00005900: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
-00005910: 6964 646c 6522 2078 3d22 3234 372e 3522  iddle" x="247.5"
-00005920: 2079 3d22 2d37 3731 2e38 2220 666f 6e74   y="-771.8" font
-00005930: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00005940: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00005950: 2231 342e 3030 223e 4e65 696e 3c2f 7465  "14.00">Nein</te
-00005960: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3726  xt>.</g>.<!-- 7&
-00005970: 2334 353b 2667 743b 3130 202d 2d3e 0a3c  #45;&gt;10 -->.<
-00005980: 6720 6964 3d22 6564 6765 3135 2220 636c  g id="edge15" cl
-00005990: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
-000059a0: 6c65 3e37 2d26 6774 3b31 303c 2f74 6974  le>7-&gt;10</tit
-000059b0: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-000059c0: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-000059d0: 6163 6b22 2064 3d22 4d33 3433 2e34 392c  ack" d="M343.49,
-000059e0: 2d38 3230 2e35 3443 3338 332e 3139 2c2d  -820.54C383.19,-
-000059f0: 3831 332e 3334 2034 3238 2e31 392c 2d38  813.34 428.19,-8
-00005a00: 3035 2e39 3620 3436 392e 352c 2d38 3031  05.96 469.5,-801
-00005a10: 2035 3931 2e35 352c 2d37 3836 2e33 3420   591.55,-786.34 
-00005a20: 3632 342e 3231 2c2d 3830 332e 3032 2037  624.21,-803.02 7
-00005a30: 3435 2e35 2c2d 3738 3320 3830 312e 3334  45.5,-783 801.34
-00005a40: 2c2d 3737 332e 3738 2038 3134 2e31 322c  ,-773.78 814.12,
-00005a50: 2d37 3635 2e36 3920 3836 382e 352c 2d37  -765.69 868.5,-7
-00005a60: 3530 2038 3738 2e32 382c 2d37 3437 2e31  50 878.28,-747.1
-00005a70: 3820 3838 382e 3235 2c2d 3734 342e 3236  8 888.25,-744.26
-00005a80: 2038 3938 2e33 322c 2d37 3431 2e32 3922   898.32,-741.29"
-00005a90: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
-00005aa0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
-00005ab0: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
-00005ac0: 3839 392e 3232 2c2d 3734 342e 3638 2039  899.22,-744.68 9
-00005ad0: 3037 2e38 322c 2d37 3338 2e34 3820 3839  07.82,-738.48 89
-00005ae0: 372e 3233 2c2d 3733 372e 3936 2038 3939  7.23,-737.96 899
-00005af0: 2e32 322c 2d37 3434 2e36 3822 2f3e 0a3c  .22,-744.68"/>.<
-00005b00: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00005b10: 3d22 6d69 6464 6c65 2220 783d 2238 3136  ="middle" x="816
-00005b20: 2e35 2220 793d 222d 3737 312e 3822 2066  .5" y="-771.8" f
-00005b30: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
-00005b40: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
-00005b50: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
-00005b60: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
-00005b70: 3034 202d 2d3e 0a3c 6720 6964 3d22 6e6f  04 -->.<g id="no
-00005b80: 6465 3133 2220 636c 6173 733d 226e 6f64  de13" class="nod
-00005b90: 6522 3e0a 3c74 6974 6c65 3e41 3034 3c2f  e">.<title>A04</
-00005ba0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
-00005bb0: 6669 6c6c 3d22 2363 6361 3961 6222 2073  fill="#cca9ab" s
-00005bc0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00005bd0: 696e 7473 3d22 3835 392e 352c 2d37 3031  ints="859.5,-701
-00005be0: 2035 3535 2e35 2c2d 3730 3120 3535 352e   555.5,-701 555.
-00005bf0: 352c 2d36 3237 2038 3539 2e35 2c2d 3632  5,-627 859.5,-62
-00005c00: 3720 3835 392e 352c 2d37 3031 222f 3e0a  7 859.5,-701"/>.
-00005c10: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
-00005c20: 723d 2273 7461 7274 2220 783d 2236 3932  r="start" x="692
-00005c30: 2220 793d 222d 3638 342e 3822 2066 6f6e  " y="-684.8" fon
-00005c40: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00005c50: 7365 7269 6622 2066 6f6e 742d 7765 6967  serif" font-weig
-00005c60: 6874 3d22 626f 6c64 2220 666f 6e74 2d73  ht="bold" font-s
-00005c70: 697a 653d 2231 342e 3030 223e 4130 343c  ize="14.00">A04<
-00005c80: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00005c90: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00005ca0: 2078 3d22 3536 372e 3522 2079 3d22 2d36   x="567.5" y="-6
-00005cb0: 3732 2e34 2220 666f 6e74 2d66 616d 696c  72.4" font-famil
-00005cc0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00005cd0: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
-00005ce0: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
-00005cf0: 2d73 697a 653d 2231 322e 3030 223e 4869  -size="12.00">Hi
-00005d00: 6e77 6569 733a 3c2f 7465 7874 3e0a 3c74  nweis:</text>.<t
-00005d10: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00005d20: 2273 7461 7274 2220 783d 2235 3637 2e35  "start" x="567.5
-00005d30: 2220 793d 222d 3636 302e 3422 2066 6f6e  " y="-660.4" fon
-00005d40: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00005d50: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00005d60: 3d22 3132 2e30 3022 3e43 6c75 7374 6572  ="12.00">Cluster
-00005d70: 3a20 4162 6c65 686e 756e 673c 2f74 6578  : Ablehnung</tex
-00005d80: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00005d90: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00005da0: 3536 372e 3522 2079 3d22 2d36 3438 2e34  567.5" y="-648.4
-00005db0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00005dc0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00005dd0: 2d73 697a 653d 2231 322e 3030 223e 4672  -size="12.00">Fr
-00005de0: 6973 7426 2332 3532 3b62 6572 7363 6872  ist&#252;berschr
-00005df0: 6569 7475 6e67 2062 6569 206b 4d45 206f  eitung bei kME o
-00005e00: 686e 6520 524c 4d2f 6d4d 452f 3c2f 7465  hne RLM/mME/</te
-00005e10: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00005e20: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00005e30: 2235 3637 2e35 2220 793d 222d 3633 362e  "567.5" y="-636.
-00005e40: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-00005e50: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00005e60: 742d 7369 7a65 3d22 3132 2e30 3022 3e50  t-size="12.00">P
-00005e70: 6175 7363 6861 6c61 6e6c 6167 652e 3c2f  auschalanlage.</
-00005e80: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00005e90: 3826 2334 353b 2667 743b 4130 3420 2d2d  8&#45;&gt;A04 --
-00005ea0: 3e0a 3c67 2069 643d 2265 6467 6531 3622  >.<g id="edge16"
-00005eb0: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
-00005ec0: 7469 746c 653e 382d 2667 743b 4130 343c  title>8-&gt;A04<
-00005ed0: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
-00005ee0: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
-00005ef0: 3d22 626c 6163 6b22 2064 3d22 4d37 3037  ="black" d="M707
-00005f00: 2e35 2c2d 3832 302e 3832 4337 3037 2e35  .5,-820.82C707.5
-00005f10: 2c2d 3739 332e 3934 2037 3037 2e35 2c2d  ,-793.94 707.5,-
-00005f20: 3734 372e 3920 3730 372e 352c 2d37 3132  747.9 707.5,-712
-00005f30: 2e38 3222 2f3e 0a3c 706f 6c79 676f 6e20  .82"/>.<polygon 
-00005f40: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00005f50: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
-00005f60: 7473 3d22 3731 312c 2d37 3132 2e39 2037  ts="711,-712.9 7
-00005f70: 3037 2e35 2c2d 3730 322e 3920 3730 342c  07.5,-702.9 704,
-00005f80: 2d37 3132 2e39 2037 3131 2c2d 3731 322e  -712.9 711,-712.
-00005f90: 3922 2f3e 0a3c 7465 7874 2074 6578 742d  9"/>.<text text-
-00005fa0: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
-00005fb0: 783d 2237 3234 2e35 2220 793d 222d 3737  x="724.5" y="-77
-00005fc0: 312e 3822 2066 6f6e 742d 6661 6d69 6c79  1.8" font-family
-00005fd0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-00005fe0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-00005ff0: 3e4e 6569 6e3c 2f74 6578 743e 0a3c 2f67  >Nein</text>.</g
-00006000: 3e0a 3c21 2d2d 2038 2623 3435 3b26 6774  >.<!-- 8&#45;&gt
-00006010: 3b31 3020 2d2d 3e0a 3c67 2069 643d 2265  ;10 -->.<g id="e
-00006020: 6467 6531 3722 2063 6c61 7373 3d22 6564  dge17" class="ed
-00006030: 6765 223e 0a3c 7469 746c 653e 382d 2667  ge">.<title>8-&g
-00006040: 743b 3130 3c2f 7469 746c 653e 0a3c 7061  t;10</title>.<pa
-00006050: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
-00006060: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
-00006070: 224d 3834 382e 3335 2c2d 3832 302e 3532  "M848.35,-820.52
-00006080: 4338 3838 2e31 362c 2d38 3131 2e35 3520  C888.16,-811.55 
-00006090: 3933 302e 3836 2c2d 3739 392e 3334 2039  930.86,-799.34 9
-000060a0: 3638 2e35 2c2d 3738 3320 3938 352e 3738  68.5,-783 985.78
-000060b0: 2c2d 3737 352e 3520 3130 3033 2e31 382c  ,-775.5 1003.18,
-000060c0: 2d37 3636 2e32 3520 3130 3139 2e39 352c  -766.25 1019.95,
-000060d0: 2d37 3536 2e32 3622 2f3e 0a3c 706f 6c79  -756.26"/>.<poly
-000060e0: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
-000060f0: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00006100: 706f 696e 7473 3d22 3130 3231 2e37 332c  points="1021.73,
-00006110: 2d37 3539 2e32 3720 3130 3238 2e34 352c  -759.27 1028.45,
-00006120: 2d37 3531 2e30 3920 3130 3138 2e30 392c  -751.09 1018.09,
-00006130: 2d37 3533 2e32 3920 3130 3231 2e37 332c  -753.29 1021.73,
-00006140: 2d37 3539 2e32 3722 2f3e 0a3c 7465 7874  -759.27"/>.<text
-00006150: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00006160: 6464 6c65 2220 783d 2231 3030 302e 3522  ddle" x="1000.5"
-00006170: 2079 3d22 2d37 3731 2e38 2220 666f 6e74   y="-771.8" font
-00006180: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00006190: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-000061a0: 2231 342e 3030 223e 4a61 3c2f 7465 7874  "14.00">Ja</text
-000061b0: 3e0a 3c2f 673e 0a3c 212d 2d20 4130 3520  >.</g>.<!-- A05 
-000061c0: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6531  -->.<g id="node1
-000061d0: 3522 2063 6c61 7373 3d22 6e6f 6465 223e  5" class="node">
-000061e0: 0a3c 7469 746c 653e 4130 353c 2f74 6974  .<title>A05</tit
-000061f0: 6c65 3e0a 3c70 6f6c 7967 6f6e 2066 696c  le>.<polygon fil
-00006200: 6c3d 2223 6363 6139 6162 2220 7374 726f  l="#cca9ab" stro
-00006210: 6b65 3d22 626c 6163 6b22 2070 6f69 6e74  ke="black" point
-00006220: 733d 2231 3734 362e 352c 2d37 3037 2031  s="1746.5,-707 1
-00006230: 3432 362e 352c 2d37 3037 2031 3432 362e  426.5,-707 1426.
-00006240: 352c 2d36 3231 2031 3734 362e 352c 2d36  5,-621 1746.5,-6
-00006250: 3231 2031 3734 362e 352c 2d37 3037 222f  21 1746.5,-707"/
-00006260: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00006270: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00006280: 3537 3122 2079 3d22 2d36 3930 2e38 2220  571" y="-690.8" 
-00006290: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-000062a0: 6573 2c73 6572 6966 2220 666f 6e74 2d77  es,serif" font-w
-000062b0: 6569 6768 743d 2262 6f6c 6422 2066 6f6e  eight="bold" fon
-000062c0: 742d 7369 7a65 3d22 3134 2e30 3022 3e41  t-size="14.00">A
-000062d0: 3035 3c2f 7465 7874 3e0a 3c74 6578 7420  05</text>.<text 
-000062e0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-000062f0: 7274 2220 783d 2231 3433 382e 3522 2079  rt" x="1438.5" y
-00006300: 3d22 2d36 3738 2e34 2220 666f 6e74 2d66  ="-678.4" font-f
-00006310: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00006320: 6966 2220 7465 7874 2d64 6563 6f72 6174  if" text-decorat
-00006330: 696f 6e3d 2275 6e64 6572 6c69 6e65 2220  ion="underline" 
-00006340: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00006350: 223e 4869 6e77 6569 733a 3c2f 7465 7874  ">Hinweis:</text
-00006360: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00006370: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00006380: 3433 382e 3522 2079 3d22 2d36 3636 2e34  438.5" y="-666.4
-00006390: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-000063a0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-000063b0: 2d73 697a 653d 2231 322e 3030 223e 436c  -size="12.00">Cl
-000063c0: 7573 7465 723a 2041 626c 6568 6e75 6e67  uster: Ablehnung
-000063d0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-000063e0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-000063f0: 2220 783d 2231 3433 382e 3522 2079 3d22  " x="1438.5" y="
-00006400: 2d36 3534 2e34 2220 666f 6e74 2d66 616d  -654.4" font-fam
-00006410: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00006420: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
-00006430: 3030 223e 4469 6520 4175 6668 6562 756e  00">Die Aufhebun
-00006440: 6720 6569 6e65 7220 7a75 6b26 2332 3532  g einer zuk&#252
-00006450: 3b6e 6674 6967 656e 205a 756f 7264 6e75  ;nftigen Zuordnu
-00006460: 6e67 3c2f 7465 7874 3e0a 3c74 6578 7420  ng</text>.<text 
-00006470: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00006480: 7274 2220 783d 2231 3433 382e 3522 2079  rt" x="1438.5" y
-00006490: 3d22 2d36 3432 2e34 2220 666f 6e74 2d66  ="-642.4" font-f
-000064a0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-000064b0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-000064c0: 322e 3030 223e 6d75 7373 207a 756d 2044  2.00">muss zum D
-000064d0: 6174 756d 2028 5a65 6974 7075 6e6b 7429  atum (Zeitpunkt)
-000064e0: 2061 6e67 6567 6562 656e 2077 6572 6465   angegeben werde
-000064f0: 6e2c 3c2f 7465 7874 3e0a 3c74 6578 7420  n,</text>.<text 
-00006500: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00006510: 7274 2220 783d 2231 3433 382e 3522 2079  rt" x="1438.5" y
-00006520: 3d22 2d36 3330 2e34 2220 666f 6e74 2d66  ="-630.4" font-f
-00006530: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00006540: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00006550: 322e 3030 223e 7769 6520 696d 204c 6965  2.00">wie im Lie
-00006560: 6665 7262 6567 696e 6e20 6265 7374 2623  ferbeginn best&#
-00006570: 3232 383b 7469 6774 2e3c 2f74 6578 743e  228;tigt.</text>
-00006580: 0a3c 2f67 3e0a 3c21 2d2d 2039 2623 3435  .</g>.<!-- 9&#45
-00006590: 3b26 6774 3b41 3035 202d 2d3e 0a3c 6720  ;&gt;A05 -->.<g 
-000065a0: 6964 3d22 6564 6765 3138 2220 636c 6173  id="edge18" clas
-000065b0: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-000065c0: 3e39 2d26 6774 3b41 3035 3c2f 7469 746c  >9-&gt;A05</titl
-000065d0: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
-000065e0: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
-000065f0: 636b 2220 643d 224d 3135 3836 2e35 2c2d  ck" d="M1586.5,-
-00006600: 3831 332e 3631 4331 3538 362e 352c 2d37  813.61C1586.5,-7
-00006610: 3837 2e38 3420 3135 3836 2e35 2c2d 3734  87.84 1586.5,-74
-00006620: 392e 3733 2031 3538 362e 352c 2d37 3138  9.73 1586.5,-718
-00006630: 2e35 3622 2f3e 0a3c 706f 6c79 676f 6e20  .56"/>.<polygon 
-00006640: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-00006650: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
-00006660: 7473 3d22 3135 3930 2c2d 3731 382e 3934  ts="1590,-718.94
-00006670: 2031 3538 362e 352c 2d37 3038 2e39 3420   1586.5,-708.94 
-00006680: 3135 3833 2c2d 3731 382e 3934 2031 3539  1583,-718.94 159
-00006690: 302c 2d37 3138 2e39 3422 2f3e 0a3c 7465  0,-718.94"/>.<te
-000066a0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-000066b0: 6d69 6464 6c65 2220 783d 2231 3630 332e  middle" x="1603.
-000066c0: 3522 2079 3d22 2d37 3731 2e38 2220 666f  5" y="-771.8" fo
-000066d0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-000066e0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-000066f0: 653d 2231 342e 3030 223e 4e65 696e 3c2f  e="14.00">Nein</
-00006700: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00006710: 3926 2334 353b 2667 743b 3130 202d 2d3e  9&#45;&gt;10 -->
-00006720: 0a3c 6720 6964 3d22 6564 6765 3139 2220  .<g id="edge19" 
-00006730: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
-00006740: 6974 6c65 3e39 2d26 6774 3b31 303c 2f74  itle>9-&gt;10</t
-00006750: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00006760: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-00006770: 626c 6163 6b22 2064 3d22 4d31 3531 332e  black" d="M1513.
-00006780: 3335 2c2d 3831 332e 3631 4331 3437 322e  35,-813.61C1472.
-00006790: 3638 2c2d 3739 372e 3237 2031 3431 392e  68,-797.27 1419.
-000067a0: 3637 2c2d 3737 352e 3937 2031 3336 362e  67,-775.97 1366.
-000067b0: 3535 2c2d 3735 342e 3632 222f 3e0a 3c70  55,-754.62"/>.<p
-000067c0: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-000067d0: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-000067e0: 6b22 2070 6f69 6e74 733d 2231 3336 372e  k" points="1367.
-000067f0: 3931 2c2d 3735 312e 3420 3133 3537 2e33  91,-751.4 1357.3
-00006800: 332c 2d37 3530 2e39 3220 3133 3635 2e33  3,-750.92 1365.3
-00006810: 2c2d 3735 372e 3839 2031 3336 372e 3931  ,-757.89 1367.91
-00006820: 2c2d 3735 312e 3422 2f3e 0a3c 7465 7874  ,-751.4"/>.<text
-00006830: 2074 6578 742d 616e 6368 6f72 3d22 6d69   text-anchor="mi
-00006840: 6464 6c65 2220 783d 2231 3433 372e 3522  ddle" x="1437.5"
-00006850: 2079 3d22 2d37 3731 2e38 2220 666f 6e74   y="-771.8" font
-00006860: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00006870: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00006880: 2231 342e 3030 223e 4a61 3c2f 7465 7874  "14.00">Ja</text
-00006890: 3e0a 3c2f 673e 0a3c 212d 2d20 4130 3620  >.</g>.<!-- A06 
-000068a0: 2d2d 3e0a 3c67 2069 643d 226e 6f64 6531  -->.<g id="node1
-000068b0: 3722 2063 6c61 7373 3d22 6e6f 6465 223e  7" class="node">
-000068c0: 0a3c 7469 746c 653e 4130 363c 2f74 6974  .<title>A06</tit
-000068d0: 6c65 3e0a 3c70 6f6c 7967 6f6e 2066 696c  le>.<polygon fil
-000068e0: 6c3d 2223 6363 6139 6162 2220 7374 726f  l="#cca9ab" stro
-000068f0: 6b65 3d22 626c 6163 6b22 2070 6f69 6e74  ke="black" point
-00006900: 733d 2231 3135 362c 2d34 3137 2039 3633  s="1156,-417 963
-00006910: 2c2d 3431 3720 3936 332c 2d33 3535 2031  ,-417 963,-355 1
-00006920: 3135 362c 2d33 3535 2031 3135 362c 2d34  156,-355 1156,-4
-00006930: 3137 222f 3e0a 3c74 6578 7420 7465 7874  17"/>.<text text
-00006940: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00006950: 783d 2231 3034 3422 2079 3d22 2d34 3030  x="1044" y="-400
-00006960: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00006970: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00006980: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-00006990: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-000069a0: 3022 3e41 3036 3c2f 7465 7874 3e0a 3c74  0">A06</text>.<t
-000069b0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-000069c0: 2273 7461 7274 2220 783d 2239 3735 2220  "start" x="975" 
-000069d0: 793d 222d 3338 382e 3422 2066 6f6e 742d  y="-388.4" font-
-000069e0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-000069f0: 7269 6622 2074 6578 742d 6465 636f 7261  rif" text-decora
-00006a00: 7469 6f6e 3d22 756e 6465 726c 696e 6522  tion="underline"
-00006a10: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
-00006a20: 3022 3e48 696e 7765 6973 3a3c 2f74 6578  0">Hinweis:</tex
-00006a30: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00006a40: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00006a50: 3937 3522 2079 3d22 2d33 3736 2e34 2220  975" y="-376.4" 
-00006a60: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00006a70: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00006a80: 697a 653d 2231 322e 3030 223e 436c 7573  ize="12.00">Clus
-00006a90: 7465 723a 205a 7573 7469 6d6d 756e 673c  ter: Zustimmung<
-00006aa0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00006ab0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00006ac0: 2078 3d22 3937 3522 2079 3d22 2d33 3634   x="975" y="-364
-00006ad0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
-00006ae0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00006af0: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
-00006b00: 4265 7374 2623 3232 383b 7469 6775 6e67  Best&#228;tigung
-00006b10: 2064 6572 2041 626d 656c 6475 6e67 3c2f   der Abmeldung</
-00006b20: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
-00006b30: 3130 2623 3435 3b26 6774 3b41 3036 202d  10&#45;&gt;A06 -
-00006b40: 2d3e 0a3c 6720 6964 3d22 6564 6765 3231  ->.<g id="edge21
-00006b50: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
-00006b60: 3c74 6974 6c65 3e31 302d 2667 743b 4130  <title>10-&gt;A0
-00006b70: 363c 2f74 6974 6c65 3e0a 3c70 6174 6820  6</title>.<path 
-00006b80: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
-00006b90: 6b65 3d22 626c 6163 6b22 2064 3d22 4d31  ke="black" d="M1
-00006ba0: 3038 392e 3133 2c2d 3537 372e 3639 4331  089.13,-577.69C1
-00006bb0: 3038 302e 3839 2c2d 3536 312e 3420 3130  080.89,-561.4 10
-00006bc0: 3733 2e34 392c 2d35 3434 2e30 3820 3130  73.49,-544.08 10
-00006bd0: 3638 2e35 2c2d 3532 3720 3130 3539 2e31  68.5,-527 1059.1
-00006be0: 352c 2d34 3934 2e39 3820 3130 3537 2e32  5,-494.98 1057.2
-00006bf0: 332c 2d34 3537 2e31 3620 3130 3537 2e34  3,-457.16 1057.4
-00006c00: 362c 2d34 3238 2e39 222f 3e0a 3c70 6f6c  6,-428.9"/>.<pol
-00006c10: 7967 6f6e 2066 696c 6c3d 2262 6c61 636b  ygon fill="black
-00006c20: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00006c30: 2070 6f69 6e74 733d 2231 3036 302e 3936   points="1060.96
-00006c40: 2c2d 3432 3920 3130 3537 2e36 352c 2d34  ,-429 1057.65,-4
-00006c50: 3138 2e39 3420 3130 3533 2e39 362c 2d34  18.94 1053.96,-4
-00006c60: 3238 2e38 3720 3130 3630 2e39 362c 2d34  28.87 1060.96,-4
-00006c70: 3239 222f 3e0a 3c74 6578 7420 7465 7874  29"/>.<text text
-00006c80: 2d61 6e63 686f 723d 226d 6964 646c 6522  -anchor="middle"
-00006c90: 2078 3d22 3130 3835 2e35 2220 793d 222d   x="1085.5" y="-
-00006ca0: 3530 302e 3322 2066 6f6e 742d 6661 6d69  500.3" font-fami
-00006cb0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00006cc0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00006cd0: 3022 3e4e 6569 6e3c 2f74 6578 743e 0a3c  0">Nein</text>.<
-00006ce0: 2f67 3e0a 3c21 2d2d 2031 3120 2d2d 3e0a  /g>.<!-- 11 -->.
-00006cf0: 3c67 2069 643d 226e 6f64 6531 3822 2063  <g id="node18" c
-00006d00: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00006d10: 746c 653e 3131 3c2f 7469 746c 653e 0a3c  tle>11</title>.<
-00006d20: 7061 7468 2066 696c 6c3d 2223 3761 6162  path fill="#7aab
-00006d30: 3861 2220 7374 726f 6b65 3d22 626c 6163  8a" stroke="blac
-00006d40: 6b22 2064 3d22 4d31 3630 332e 352c 2d35  k" d="M1603.5,-5
-00006d50: 3237 4331 3630 332e 352c 2d35 3237 2031  27C1603.5,-527 1
-00006d60: 3132 332e 352c 2d35 3237 2031 3132 332e  123.5,-527 1123.
-00006d70: 352c 2d35 3237 2031 3131 372e 352c 2d35  5,-527 1117.5,-5
-00006d80: 3237 2031 3131 312e 352c 2d35 3231 2031  27 1111.5,-521 1
-00006d90: 3131 312e 352c 2d35 3135 2031 3131 312e  111.5,-515 1111.
-00006da0: 352c 2d35 3135 2031 3131 312e 352c 2d34  5,-515 1111.5,-4
-00006db0: 3933 2031 3131 312e 352c 2d34 3933 2031  93 1111.5,-493 1
-00006dc0: 3131 312e 352c 2d34 3837 2031 3131 372e  111.5,-487 1117.
-00006dd0: 352c 2d34 3831 2031 3132 332e 352c 2d34  5,-481 1123.5,-4
-00006de0: 3831 2031 3132 332e 352c 2d34 3831 2031  81 1123.5,-481 1
-00006df0: 3630 332e 352c 2d34 3831 2031 3630 332e  603.5,-481 1603.
-00006e00: 352c 2d34 3831 2031 3630 392e 352c 2d34  5,-481 1609.5,-4
-00006e10: 3831 2031 3631 352e 352c 2d34 3837 2031  81 1615.5,-487 1
-00006e20: 3631 352e 352c 2d34 3933 2031 3631 352e  615.5,-493 1615.
-00006e30: 352c 2d34 3933 2031 3631 352e 352c 2d35  5,-493 1615.5,-5
-00006e40: 3135 2031 3631 352e 352c 2d35 3135 2031  15 1615.5,-515 1
-00006e50: 3631 352e 352c 2d35 3231 2031 3630 392e  615.5,-521 1609.
-00006e60: 352c 2d35 3237 2031 3630 332e 352c 2d35  5,-527 1603.5,-5
-00006e70: 3237 222f 3e0a 3c74 6578 7420 7465 7874  27"/>.<text text
-00006e80: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00006e90: 783d 2231 3132 352e 3522 2079 3d22 2d35  x="1125.5" y="-5
-00006ea0: 3037 2e38 2220 666f 6e74 2d66 616d 696c  07.8" font-famil
-00006eb0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00006ec0: 666f 6e74 2d77 6569 6768 743d 2262 6f6c  font-weight="bol
-00006ed0: 6422 2066 6f6e 742d 7369 7a65 3d22 3134  d" font-size="14
-00006ee0: 2e30 3022 3e31 313a 203c 2f74 6578 743e  .00">11: </text>
-00006ef0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00006f00: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
-00006f10: 3535 2e35 2220 793d 222d 3530 372e 3822  55.5" y="-507.8"
-00006f20: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00006f30: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00006f40: 7369 7a65 3d22 3134 2e30 3022 3e49 7374  size="14.00">Ist
-00006f50: 2064 6572 2061 6e66 7261 6765 6e64 6520   der anfragende 
-00006f60: 4c46 2061 6d20 466f 6c67 6574 6167 2064  LF am Folgetag d
-00006f70: 6573 2041 626d 656c 6475 6e67 7364 6174  es Abmeldungsdat
-00006f80: 756d 2064 6572 3c2f 7465 7874 3e0a 3c74  um der</text>.<t
-00006f90: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00006fa0: 2273 7461 7274 2220 783d 2231 3132 352e  "start" x="1125.
-00006fb0: 3522 2079 3d22 2d34 3933 2e38 2220 666f  5" y="-493.8" fo
-00006fc0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
-00006fd0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
-00006fe0: 653d 2231 342e 3030 223e 4d61 726b 746c  e="14.00">Marktl
-00006ff0: 6f6b 6174 696f 6e20 6e6f 6368 207a 7567  okation noch zug
-00007000: 656f 7264 6e65 743f 3c2f 7465 7874 3e0a  eordnet?</text>.
-00007010: 3c2f 673e 0a3c 212d 2d20 3130 2623 3435  </g>.<!-- 10&#45
-00007020: 3b26 6774 3b31 3120 2d2d 3e0a 3c67 2069  ;&gt;11 -->.<g i
-00007030: 643d 2265 6467 6532 3022 2063 6c61 7373  d="edge20" class
-00007040: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
-00007050: 3130 2d26 6774 3b31 313c 2f74 6974 6c65  10-&gt;11</title
-00007060: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
-00007070: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
-00007080: 6b22 2064 3d22 4d31 3236 322e 3531 2c2d  k" d="M1262.51,-
-00007090: 3537 372e 3533 4331 3238 342e 3338 2c2d  577.53C1284.38,-
-000070a0: 3536 312e 3832 2031 3330 352e 3737 2c2d  561.82 1305.77,-
-000070b0: 3534 362e 3436 2031 3332 332e 322c 2d35  546.46 1323.2,-5
-000070c0: 3333 2e39 3522 2f3e 0a3c 706f 6c79 676f  33.95"/>.<polygo
-000070d0: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
-000070e0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-000070f0: 696e 7473 3d22 3133 3235 2e31 342c 2d35  ints="1325.14,-5
-00007100: 3336 2e38 3620 3133 3331 2e32 322c 2d35  36.86 1331.22,-5
-00007110: 3238 2e31 3920 3133 3231 2e30 352c 2d35  28.19 1321.05,-5
-00007120: 3331 2e31 3820 3133 3235 2e31 342c 2d35  31.18 1325.14,-5
-00007130: 3336 2e38 3622 2f3e 0a3c 7465 7874 2074  36.86"/>.<text t
-00007140: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-00007150: 6c65 2220 783d 2231 3331 302e 3522 2079  le" x="1310.5" y
-00007160: 3d22 2d35 3438 2e38 2220 666f 6e74 2d66  ="-548.8" font-f
-00007170: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00007180: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00007190: 342e 3030 223e 4a61 3c2f 7465 7874 3e0a  4.00">Ja</text>.
-000071a0: 3c2f 673e 0a3c 212d 2d20 3131 2623 3435  </g>.<!-- 11&#45
-000071b0: 3b26 6774 3b41 3036 202d 2d3e 0a3c 6720  ;&gt;A06 -->.<g 
-000071c0: 6964 3d22 6564 6765 3233 2220 636c 6173  id="edge23" clas
-000071d0: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
-000071e0: 3e31 312d 2667 743b 4130 363c 2f74 6974  >11-&gt;A06</tit
-000071f0: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
-00007200: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
-00007210: 6163 6b22 2064 3d22 4d31 3330 312e 3333  ack" d="M1301.33
-00007220: 2c2d 3438 302e 3636 4331 3236 322e 3232  ,-480.66C1262.22
-00007230: 2c2d 3436 362e 3436 2031 3231 302e 3737  ,-466.46 1210.77
-00007240: 2c2d 3434 372e 3532 2031 3136 352e 352c  ,-447.52 1165.5,
-00007250: 2d34 3330 2031 3135 382e 3539 2c2d 3432  -430 1158.59,-42
-00007260: 372e 3333 2031 3135 312e 3435 2c2d 3432  7.33 1151.45,-42
-00007270: 342e 3532 2031 3134 342e 3239 2c2d 3432  4.52 1144.29,-42
-00007280: 312e 3638 222f 3e0a 3c70 6f6c 7967 6f6e  1.68"/>.<polygon
-00007290: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-000072a0: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-000072b0: 6e74 733d 2231 3134 352e 3739 2c2d 3431  nts="1145.79,-41
-000072c0: 382e 3531 2031 3133 352e 322c 2d34 3138  8.51 1135.2,-418
-000072d0: 2e30 3520 3131 3433 2e32 2c2d 3432 352e  .05 1143.2,-425.
-000072e0: 3031 2031 3134 352e 3739 2c2d 3431 382e  01 1145.79,-418.
-000072f0: 3531 222f 3e0a 3c74 6578 7420 7465 7874  51"/>.<text text
-00007300: 2d61 6e63 686f 723d 226d 6964 646c 6522  -anchor="middle"
-00007310: 2078 3d22 3132 3538 2e35 2220 793d 222d   x="1258.5" y="-
-00007320: 3435 312e 3822 2066 6f6e 742d 6661 6d69  451.8" font-fami
-00007330: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00007340: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00007350: 3022 3e4a 613c 2f74 6578 743e 0a3c 2f67  0">Ja</text>.</g
-00007360: 3e0a 3c21 2d2d 2031 3220 2d2d 3e0a 3c67  >.<!-- 12 -->.<g
-00007370: 2069 643d 226e 6f64 6531 3922 2063 6c61   id="node19" cla
-00007380: 7373 3d22 6e6f 6465 223e 0a3c 7469 746c  ss="node">.<titl
-00007390: 653e 3132 3c2f 7469 746c 653e 0a3c 7061  e>12</title>.<pa
-000073a0: 7468 2066 696c 6c3d 2223 3761 6162 3861  th fill="#7aab8a
-000073b0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-000073c0: 2064 3d22 4d31 3633 392c 2d34 3330 4331   d="M1639,-430C1
-000073d0: 3633 392c 2d34 3330 2031 3138 362c 2d34  639,-430 1186,-4
-000073e0: 3330 2031 3138 362c 2d34 3330 2031 3138  30 1186,-430 118
-000073f0: 302c 2d34 3330 2031 3137 342c 2d34 3234  0,-430 1174,-424
-00007400: 2031 3137 342c 2d34 3138 2031 3137 342c   1174,-418 1174,
-00007410: 2d34 3138 2031 3137 342c 2d33 3534 2031  -418 1174,-354 1
-00007420: 3137 342c 2d33 3534 2031 3137 342c 2d33  174,-354 1174,-3
-00007430: 3438 2031 3138 302c 2d33 3432 2031 3138  48 1180,-342 118
-00007440: 362c 2d33 3432 2031 3138 362c 2d33 3432  6,-342 1186,-342
-00007450: 2031 3633 392c 2d33 3432 2031 3633 392c   1639,-342 1639,
-00007460: 2d33 3432 2031 3634 352c 2d33 3432 2031  -342 1645,-342 1
-00007470: 3635 312c 2d33 3438 2031 3635 312c 2d33  651,-348 1651,-3
-00007480: 3534 2031 3635 312c 2d33 3534 2031 3635  54 1651,-354 165
-00007490: 312c 2d34 3138 2031 3635 312c 2d34 3138  1,-418 1651,-418
-000074a0: 2031 3635 312c 2d34 3234 2031 3634 352c   1651,-424 1645,
-000074b0: 2d34 3330 2031 3633 392c 2d34 3330 222f  -430 1639,-430"/
-000074c0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-000074d0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-000074e0: 3138 3822 2079 3d22 2d34 3130 2e38 2220  188" y="-410.8" 
-000074f0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00007500: 6573 2c73 6572 6966 2220 666f 6e74 2d77  es,serif" font-w
-00007510: 6569 6768 743d 2262 6f6c 6422 2066 6f6e  eight="bold" fon
-00007520: 742d 7369 7a65 3d22 3134 2e30 3022 3e31  t-size="14.00">1
-00007530: 323a 203c 2f74 6578 743e 0a3c 7465 7874  2: </text>.<text
-00007540: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00007550: 6172 7422 2078 3d22 3132 3138 2220 793d  art" x="1218" y=
-00007560: 222d 3431 302e 3822 2066 6f6e 742d 6661  "-410.8" font-fa
-00007570: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-00007580: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
-00007590: 2e30 3022 3e4c 6965 6774 2065 696e 2054  .00">Liegt ein T
-000075a0: 7261 6e73 616b 7469 6f6e 7367 7275 6e64  ransaktionsgrund
-000075b0: 2076 6f72 2c20 6175 7320 7765 6c63 6865   vor, aus welche
-000075c0: 6d20 6865 7276 6f72 6765 6874 2c3c 2f74  m hervorgeht,</t
-000075d0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
-000075e0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
-000075f0: 3d22 3131 3838 2220 793d 222d 3339 362e  ="1188" y="-396.
-00007600: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
-00007610: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
-00007620: 742d 7369 7a65 3d22 3134 2e30 3022 3e64  t-size="14.00">d
-00007630: 6173 7320 6465 7220 416e 7363 686c 7573  ass der Anschlus
-00007640: 736e 7574 7a65 7220 6175 7367 657a 6f67  snutzer ausgezog
-00007650: 656e 2069 7374 3f3c 2f74 6578 743e 0a3c  en ist?</text>.<
-00007660: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00007670: 3d22 7374 6172 7422 2078 3d22 3131 3838  ="start" x="1188
-00007680: 2220 793d 222d 3338 322e 3822 2066 6f6e  " y="-382.8" fon
-00007690: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-000076a0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-000076b0: 3d22 3134 2e30 3022 3e44 6173 2069 7374  ="14.00">Das ist
-000076c0: 2062 6569 2064 656e 2066 6f6c 6765 6e64   bei den folgend
-000076d0: 656e 2054 7261 6e73 616b 7469 6f6e 7367  en Transaktionsg
-000076e0: 7226 2332 3532 3b6e 6465 6e20 6465 7220  r&#252;nden der 
-000076f0: 4661 6c6c 3a3c 2f74 6578 743e 0a3c 7465  Fall:</text>.<te
-00007700: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
-00007710: 7374 6172 7422 2078 3d22 3131 3838 2220  start" x="1188" 
-00007720: 793d 222d 3336 382e 3822 2066 6f6e 742d  y="-368.8" font-
-00007730: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00007740: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00007750: 3134 2e30 3022 3e26 2336 3135 3939 3b20  14.00">&#61599; 
-00007760: 4569 6e2d 2f41 7573 7a75 6720 2855 6d7a  Ein-/Auszug (Umz
-00007770: 7567 293c 2f74 6578 743e 0a3c 7465 7874  ug)</text>.<text
-00007780: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00007790: 6172 7422 2078 3d22 3131 3838 2220 793d  art" x="1188" y=
-000077a0: 222d 3335 342e 3822 2066 6f6e 742d 6661  "-354.8" font-fa
-000077b0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
-000077c0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
-000077d0: 2e30 3022 3e26 2336 3135 3939 3b20 4175  .00">&#61599; Au
-000077e0: 737a 7567 2077 6567 656e 2053 7469 6c6c  szug wegen Still
-000077f0: 6c65 6775 6e67 3c2f 7465 7874 3e0a 3c2f  legung</text>.</
-00007800: 673e 0a3c 212d 2d20 3131 2623 3435 3b26  g>.<!-- 11&#45;&
-00007810: 6774 3b31 3220 2d2d 3e0a 3c67 2069 643d  gt;12 -->.<g id=
-00007820: 2265 6467 6532 3222 2063 6c61 7373 3d22  "edge22" class="
-00007830: 6564 6765 223e 0a3c 7469 746c 653e 3131  edge">.<title>11
-00007840: 2d26 6774 3b31 323c 2f74 6974 6c65 3e0a  -&gt;12</title>.
-00007850: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
-00007860: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
-00007870: 2064 3d22 4d31 3337 322e 3935 2c2d 3438   d="M1372.95,-48
-00007880: 302e 3633 4331 3337 372e 3733 2c2d 3436  0.63C1377.73,-46
-00007890: 392e 3320 3133 3833 2e37 372c 2d34 3535  9.3 1383.77,-455
-000078a0: 2e30 3120 3133 3839 2e36 382c 2d34 3431  .01 1389.68,-441
-000078b0: 2e30 3222 2f3e 0a3c 706f 6c79 676f 6e20  .02"/>.<polygon 
-000078c0: 6669 6c6c 3d22 626c 6163 6b22 2073 7472  fill="black" str
-000078d0: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
-000078e0: 7473 3d22 3133 3932 2e38 392c 2d34 3432  ts="1392.89,-442
-000078f0: 2e34 3120 3133 3933 2e35 362c 2d34 3331  .41 1393.56,-431
-00007900: 2e38 3420 3133 3836 2e34 352c 2d34 3339  .84 1386.45,-439
-00007910: 2e36 3920 3133 3932 2e38 392c 2d34 3432  .69 1392.89,-442
-00007920: 2e34 3122 2f3e 0a3c 7465 7874 2074 6578  .41"/>.<text tex
-00007930: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-00007940: 2220 783d 2231 3430 332e 3522 2079 3d22  " x="1403.5" y="
-00007950: 2d34 3531 2e38 2220 666f 6e74 2d66 616d  -451.8" font-fam
-00007960: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00007970: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-00007980: 3030 223e 4e65 696e 3c2f 7465 7874 3e0a  00">Nein</text>.
-00007990: 3c2f 673e 0a3c 212d 2d20 4130 3720 2d2d  </g>.<!-- A07 --
-000079a0: 3e0a 3c67 2069 643d 226e 6f64 6532 3022  >.<g id="node20"
-000079b0: 2063 6c61 7373 3d22 6e6f 6465 223e 0a3c   class="node">.<
-000079c0: 7469 746c 653e 4130 373c 2f74 6974 6c65  title>A07</title
-000079d0: 3e0a 3c70 6f6c 7967 6f6e 2066 696c 6c3d  >.<polygon fill=
-000079e0: 2223 6363 6139 6162 2220 7374 726f 6b65  "#cca9ab" stroke
-000079f0: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
-00007a00: 2231 3434 392c 2d32 3633 2031 3135 302c  "1449,-263 1150,
-00007a10: 2d32 3633 2031 3135 302c 2d31 3839 2031  -263 1150,-189 1
-00007a20: 3434 392c 2d31 3839 2031 3434 392c 2d32  449,-189 1449,-2
-00007a30: 3633 222f 3e0a 3c74 6578 7420 7465 7874  63"/>.<text text
-00007a40: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00007a50: 783d 2231 3238 3422 2079 3d22 2d32 3436  x="1284" y="-246
-00007a60: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-00007a70: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-00007a80: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
-00007a90: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
-00007aa0: 3022 3e41 3037 3c2f 7465 7874 3e0a 3c74  0">A07</text>.<t
-00007ab0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00007ac0: 2273 7461 7274 2220 783d 2231 3136 3222  "start" x="1162"
-00007ad0: 2079 3d22 2d32 3334 2e34 2220 666f 6e74   y="-234.4" font
-00007ae0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-00007af0: 6572 6966 2220 7465 7874 2d64 6563 6f72  erif" text-decor
-00007b00: 6174 696f 6e3d 2275 6e64 6572 6c69 6e65  ation="underline
-00007b10: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
-00007b20: 3030 223e 4869 6e77 6569 733a 3c2f 7465  00">Hinweis:</te
-00007b30: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-00007b40: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00007b50: 2231 3136 3222 2079 3d22 2d32 3232 2e34  "1162" y="-222.4
-00007b60: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00007b70: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00007b80: 2d73 697a 653d 2231 322e 3030 223e 436c  -size="12.00">Cl
-00007b90: 7573 7465 723a 2041 626c 6568 6e75 6e67  uster: Ablehnung
-00007ba0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00007bb0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00007bc0: 2220 783d 2231 3136 3222 2079 3d22 2d32  " x="1162" y="-2
-00007bd0: 3130 2e34 2220 666f 6e74 2d66 616d 696c  10.4" font-famil
-00007be0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00007bf0: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00007c00: 223e 4c69 6566 6572 656e 6465 207a 756d  ">Lieferende zum
-00007c10: 2041 626d 656c 6465 6461 7475 6d20 7775   Abmeldedatum wu
-00007c20: 7264 6520 6265 7265 6974 733c 2f74 6578  rde bereits</tex
-00007c30: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00007c40: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00007c50: 3131 3632 2220 793d 222d 3139 382e 3422  1162" y="-198.4"
-00007c60: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00007c70: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00007c80: 7369 7a65 3d22 3132 2e30 3022 3e62 6573  size="12.00">bes
-00007c90: 7426 2332 3238 3b74 6967 743c 2f74 6578  t&#228;tigt</tex
-00007ca0: 743e 0a3c 2f67 3e0a 3c21 2d2d 2031 3226  t>.</g>.<!-- 12&
-00007cb0: 2334 353b 2667 743b 4130 3720 2d2d 3e0a  #45;&gt;A07 -->.
-00007cc0: 3c67 2069 643d 2265 6467 6532 3422 2063  <g id="edge24" c
-00007cd0: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
-00007ce0: 746c 653e 3132 2d26 6774 3b41 3037 3c2f  tle>12-&gt;A07</
-00007cf0: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
-00007d00: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
-00007d10: 2262 6c61 636b 2220 643d 224d 3133 3831  "black" d="M1381
-00007d20: 2e36 322c 2d33 3431 2e38 3343 3133 3636  .62,-341.83C1366
-00007d30: 2e33 312c 2d33 3230 2e34 3220 3133 3437  .31,-320.42 1347
-00007d40: 2e38 312c 2d32 3934 2e35 3520 3133 3332  .81,-294.55 1332
-00007d50: 2e32 352c 2d32 3732 2e38 222f 3e0a 3c70  .25,-272.8"/>.<p
-00007d60: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
-00007d70: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
-00007d80: 6b22 2070 6f69 6e74 733d 2231 3333 352e  k" points="1335.
-00007d90: 312c 2d32 3730 2e37 3620 3133 3236 2e34  1,-270.76 1326.4
-00007da0: 342c 2d32 3634 2e36 3720 3133 3239 2e34  4,-264.67 1329.4
-00007db0: 312c 2d32 3734 2e38 3420 3133 3335 2e31  1,-274.84 1335.1
-00007dc0: 2c2d 3237 302e 3736 222f 3e0a 3c74 6578  ,-270.76"/>.<tex
-00007dd0: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
-00007de0: 6964 646c 6522 2078 3d22 3133 3832 2e35  iddle" x="1382.5
-00007df0: 2220 793d 222d 3331 322e 3822 2066 6f6e  " y="-312.8" fon
-00007e00: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00007e10: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00007e20: 3d22 3134 2e30 3022 3e4e 6569 6e3c 2f74  ="14.00">Nein</t
-00007e30: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2031  ext>.</g>.<!-- 1
-00007e40: 3320 2d2d 3e0a 3c67 2069 643d 226e 6f64  3 -->.<g id="nod
-00007e50: 6532 3122 2063 6c61 7373 3d22 6e6f 6465  e21" class="node
-00007e60: 223e 0a3c 7469 746c 653e 3133 3c2f 7469  ">.<title>13</ti
-00007e70: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
-00007e80: 2223 3761 6162 3861 2220 7374 726f 6b65  "#7aab8a" stroke
-00007e90: 3d22 626c 6163 6b22 2064 3d22 4d31 3931  ="black" d="M191
-00007ea0: 322c 2d32 3931 4331 3931 322c 2d32 3931  2,-291C1912,-291
-00007eb0: 2031 3437 392c 2d32 3931 2031 3437 392c   1479,-291 1479,
-00007ec0: 2d32 3931 2031 3437 332c 2d32 3931 2031  -291 1473,-291 1
-00007ed0: 3436 372c 2d32 3835 2031 3436 372c 2d32  467,-285 1467,-2
-00007ee0: 3739 2031 3436 372c 2d32 3739 2031 3436  79 1467,-279 146
-00007ef0: 372c 2d31 3733 2031 3436 372c 2d31 3733  7,-173 1467,-173
-00007f00: 2031 3436 372c 2d31 3637 2031 3437 332c   1467,-167 1473,
-00007f10: 2d31 3631 2031 3437 392c 2d31 3631 2031  -161 1479,-161 1
-00007f20: 3437 392c 2d31 3631 2031 3931 322c 2d31  479,-161 1912,-1
-00007f30: 3631 2031 3931 322c 2d31 3631 2031 3931  61 1912,-161 191
-00007f40: 382c 2d31 3631 2031 3932 342c 2d31 3637  8,-161 1924,-167
-00007f50: 2031 3932 342c 2d31 3733 2031 3932 342c   1924,-173 1924,
-00007f60: 2d31 3733 2031 3932 342c 2d32 3739 2031  -173 1924,-279 1
-00007f70: 3932 342c 2d32 3739 2031 3932 342c 2d32  924,-279 1924,-2
-00007f80: 3835 2031 3931 382c 2d32 3931 2031 3931  85 1918,-291 191
-00007f90: 322c 2d32 3931 222f 3e0a 3c74 6578 7420  2,-291"/>.<text 
-00007fa0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
-00007fb0: 7274 2220 783d 2231 3438 3122 2079 3d22  rt" x="1481" y="
-00007fc0: 2d32 3731 2e38 2220 666f 6e74 2d66 616d  -271.8" font-fam
-00007fd0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-00007fe0: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
-00007ff0: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
-00008000: 3134 2e30 3022 3e31 333a 203c 2f74 6578  14.00">13: </tex
-00008010: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00008020: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00008030: 3135 3131 2220 793d 222d 3237 312e 3822  1511" y="-271.8"
-00008040: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00008050: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00008060: 7369 7a65 3d22 3134 2e30 3022 3e4c 6965  size="14.00">Lie
-00008070: 6774 2069 6e20 6465 7220 6265 7265 6974  gt in der bereit
-00008080: 7320 6265 7374 2623 3232 383b 7469 6774  s best&#228;tigt
-00008090: 656e 2041 626d 656c 6475 6e67 2065 696e  en Abmeldung ein
-000080a0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-000080b0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-000080c0: 2220 783d 2231 3438 3122 2079 3d22 2d32  " x="1481" y="-2
-000080d0: 3537 2e38 2220 666f 6e74 2d66 616d 696c  57.8" font-famil
-000080e0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-000080f0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00008100: 223e 5472 616e 7361 6b74 696f 6e73 6772  ">Transaktionsgr
-00008110: 756e 6420 766f 722c 2061 7573 2077 656c  und vor, aus wel
-00008120: 6368 656d 206e 6963 6874 2068 6572 766f  chem nicht hervo
-00008130: 7267 6568 742c 2064 6173 733c 2f74 6578  rgeht, dass</tex
-00008140: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
-00008150: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
-00008160: 3134 3831 2220 793d 222d 3234 332e 3822  1481" y="-243.8"
-00008170: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00008180: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00008190: 7369 7a65 3d22 3134 2e30 3022 3e64 6572  size="14.00">der
-000081a0: 2041 6e73 6368 6c75 7373 6e75 747a 6572   Anschlussnutzer
-000081b0: 2061 7573 6765 7a6f 6765 6e20 6973 743f   ausgezogen ist?
-000081c0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-000081d0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-000081e0: 2220 783d 2231 3438 3122 2079 3d22 2d32  " x="1481" y="-2
-000081f0: 3239 2e38 2220 666f 6e74 2d66 616d 696c  29.8" font-famil
-00008200: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00008210: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
-00008220: 223e 4461 7320 6973 7420 6265 6920 6465  ">Das ist bei de
-00008230: 6e20 666f 6c67 656e 6465 6e20 5472 616e  n folgenden Tran
-00008240: 7361 6b74 696f 6e73 6772 2623 3235 323b  saktionsgr&#252;
-00008250: 6e64 656e 2064 6572 2046 616c 6c3a 3c2f  nden der Fall:</
-00008260: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00008270: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00008280: 783d 2231 3438 3122 2079 3d22 2d32 3135  x="1481" y="-215
-00008290: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
-000082a0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
-000082b0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-000082c0: 2623 3631 3539 393b 2045 696e 2d2f 4175  &#61599; Ein-/Au
-000082d0: 737a 7567 2028 556d 7a75 6729 3c2f 7465  szug (Umzug)</te
-000082e0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-000082f0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00008300: 2231 3438 3122 2079 3d22 2d32 3031 2e38  "1481" y="-201.8
-00008310: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00008320: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00008330: 2d73 697a 653d 2231 342e 3030 223e 2623  -size="14.00">&#
-00008340: 3631 3539 393b 2041 7573 7a75 6720 7765  61599; Auszug we
-00008350: 6765 6e20 5374 696c 6c6c 6567 756e 673c  gen Stilllegung<
-00008360: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00008370: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00008380: 2078 3d22 3134 3831 2220 793d 222d 3138   x="1481" y="-18
-00008390: 372e 3822 2066 6f6e 742d 6661 6d69 6c79  7.8" font-family
-000083a0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
-000083b0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
-000083c0: 3e26 2336 3135 3939 3b20 4175 6668 6562  >&#61599; Aufheb
-000083d0: 756e 6720 6569 6e65 7220 7a75 6b26 2332  ung einer zuk&#2
-000083e0: 3532 3b6e 6674 6967 656e 205a 756f 7264  52;nftigen Zuord
-000083f0: 6e75 6e67 2077 6567 656e 3c2f 7465 7874  nung wegen</text
-00008400: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00008410: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00008420: 3438 3122 2079 3d22 2d31 3733 2e38 2220  481" y="-173.8" 
-00008430: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00008440: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00008450: 697a 653d 2231 342e 3030 223e 5374 696c  ize="14.00">Stil
-00008460: 6c6c 6567 756e 673c 2f74 6578 743e 0a3c  llegung</text>.<
-00008470: 2f67 3e0a 3c21 2d2d 2031 3226 2334 353b  /g>.<!-- 12&#45;
-00008480: 2667 743b 3133 202d 2d3e 0a3c 6720 6964  &gt;13 -->.<g id
-00008490: 3d22 6564 6765 3235 2220 636c 6173 733d  ="edge25" class=
-000084a0: 2265 6467 6522 3e0a 3c74 6974 6c65 3e31  "edge">.<title>1
-000084b0: 322d 2667 743b 3133 3c2f 7469 746c 653e  2-&gt;13</title>
-000084c0: 0a3c 7061 7468 2066 696c 6c3d 226e 6f6e  .<path fill="non
-000084d0: 6522 2073 7472 6f6b 653d 2262 6c61 636b  e" stroke="black
-000084e0: 2220 643d 224d 3134 3930 2e32 312c 2d33  " d="M1490.21,-3
-000084f0: 3431 2e36 3243 3135 3134 2e39 312c 2d33  41.62C1514.91,-3
-00008500: 3237 2e38 3320 3135 3432 2e38 392c 2d33  27.83 1542.89,-3
-00008510: 3132 2e32 2031 3537 302e 3037 2c2d 3239  12.2 1570.07,-29
-00008520: 372e 3033 222f 3e0a 3c70 6f6c 7967 6f6e  7.03"/>.<polygon
-00008530: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
-00008540: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
-00008550: 6e74 733d 2231 3537 312e 3639 2c2d 3330  nts="1571.69,-30
-00008560: 302e 3133 2031 3537 382e 3732 2c2d 3239  0.13 1578.72,-29
-00008570: 322e 3220 3135 3638 2e32 382c 2d32 3934  2.2 1568.28,-294
-00008580: 2e30 3220 3135 3731 2e36 392c 2d33 3030  .02 1571.69,-300
-00008590: 2e31 3322 2f3e 0a3c 7465 7874 2074 6578  .13"/>.<text tex
-000085a0: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-000085b0: 2220 783d 2231 3535 322e 3522 2079 3d22  " x="1552.5" y="
-000085c0: 2d33 3132 2e38 2220 666f 6e74 2d66 616d  -312.8" font-fam
-000085d0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-000085e0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
-000085f0: 3030 223e 4a61 3c2f 7465 7874 3e0a 3c2f  00">Ja</text>.</
-00008600: 673e 0a3c 212d 2d20 4130 3820 2d2d 3e0a  g>.<!-- A08 -->.
-00008610: 3c67 2069 643d 226e 6f64 6532 3222 2063  <g id="node22" c
-00008620: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
-00008630: 746c 653e 4130 383c 2f74 6974 6c65 3e0a  tle>A08</title>.
-00008640: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2223  <polygon fill="#
-00008650: 6363 6139 6162 2220 7374 726f 6b65 3d22  cca9ab" stroke="
-00008660: 626c 6163 6b22 2070 6f69 6e74 733d 2231  black" points="1
-00008670: 3637 342c 2d39 3220 3133 3935 2c2d 3932  674,-92 1395,-92
-00008680: 2031 3339 352c 2d31 3820 3136 3734 2c2d   1395,-18 1674,-
-00008690: 3138 2031 3637 342c 2d39 3222 2f3e 0a3c  18 1674,-92"/>.<
-000086a0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-000086b0: 3d22 7374 6172 7422 2078 3d22 3135 3139  ="start" x="1519
-000086c0: 2220 793d 222d 3735 2e38 2220 666f 6e74  " y="-75.8" font
-000086d0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
-000086e0: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
-000086f0: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
-00008700: 7a65 3d22 3134 2e30 3022 3e41 3038 3c2f  ze="14.00">A08</
-00008710: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
-00008720: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
-00008730: 783d 2231 3430 3722 2079 3d22 2d36 332e  x="1407" y="-63.
-00008740: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
-00008750: 5469 6d65 732c 7365 7269 6622 2074 6578  Times,serif" tex
-00008760: 742d 6465 636f 7261 7469 6f6e 3d22 756e  t-decoration="un
-00008770: 6465 726c 696e 6522 2066 6f6e 742d 7369  derline" font-si
-00008780: 7a65 3d22 3132 2e30 3022 3e48 696e 7765  ze="12.00">Hinwe
-00008790: 6973 3a3c 2f74 6578 743e 0a3c 7465 7874  is:</text>.<text
-000087a0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-000087b0: 6172 7422 2078 3d22 3134 3037 2220 793d  art" x="1407" y=
-000087c0: 222d 3531 2e34 2220 666f 6e74 2d66 616d  "-51.4" font-fam
-000087d0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
-000087e0: 2220 666f 6e74 2d73 697a 653d 2231 322e  " font-size="12.
-000087f0: 3030 223e 436c 7573 7465 723a 2041 626c  00">Cluster: Abl
-00008800: 6568 6e75 6e67 3c2f 7465 7874 3e0a 3c74  ehnung</text>.<t
-00008810: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00008820: 2273 7461 7274 2220 783d 2231 3430 3722  "start" x="1407"
-00008830: 2079 3d22 2d33 392e 3422 2066 6f6e 742d   y="-39.4" font-
-00008840: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
-00008850: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
-00008860: 3132 2e30 3022 3e4c 6965 6665 7265 6e64  12.00">Lieferend
-00008870: 6520 7a75 6d20 4162 6d65 6c64 6564 6174  e zum Abmeldedat
-00008880: 756d 2077 7572 6465 2061 7573 3c2f 7465  um wurde aus</te
-00008890: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
-000088a0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-000088b0: 2231 3430 3722 2079 3d22 2d32 372e 3422  "1407" y="-27.4"
-000088c0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-000088d0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-000088e0: 7369 7a65 3d22 3132 2e30 3022 3e67 6c65  size="12.00">gle
-000088f0: 6963 6865 6d20 4772 756e 6420 6265 7265  ichem Grund bere
-00008900: 6974 7320 6265 7374 2623 3232 383b 7469  its best&#228;ti
-00008910: 6774 2e3c 2f74 6578 743e 0a3c 2f67 3e0a  gt.</text>.</g>.
-00008920: 3c21 2d2d 2031 3326 2334 353b 2667 743b  <!-- 13&#45;&gt;
-00008930: 4130 3820 2d2d 3e0a 3c67 2069 643d 2265  A08 -->.<g id="e
-00008940: 6467 6532 3622 2063 6c61 7373 3d22 6564  dge26" class="ed
-00008950: 6765 223e 0a3c 7469 746c 653e 3133 2d26  ge">.<title>13-&
-00008960: 6774 3b41 3038 3c2f 7469 746c 653e 0a3c  gt;A08</title>.<
-00008970: 7061 7468 2066 696c 6c3d 226e 6f6e 6522  path fill="none"
-00008980: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
-00008990: 643d 224d 3136 3334 2e31 372c 2d31 3630  d="M1634.17,-160
-000089a0: 2e36 3343 3136 3135 2e30 362c 2d31 3430  .63C1615.06,-140
-000089b0: 2e35 3720 3135 3934 2e34 322c 2d31 3138  .57 1594.42,-118
-000089c0: 2e39 2031 3537 362e 392c 2d31 3030 2e35  .9 1576.9,-100.5
-000089d0: 3122 2f3e 0a3c 706f 6c79 676f 6e20 6669  1"/>.<polygon fi
-000089e0: 6c6c 3d22 626c 6163 6b22 2073 7472 6f6b  ll="black" strok
-000089f0: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
-00008a00: 3d22 3135 3739 2e35 372c 2d39 382e 3234  ="1579.57,-98.24
-00008a10: 2031 3537 302e 3134 2c2d 3933 2e34 3120   1570.14,-93.41 
-00008a20: 3135 3734 2e35 2c2d 3130 332e 3036 2031  1574.5,-103.06 1
-00008a30: 3537 392e 3537 2c2d 3938 2e32 3422 2f3e  579.57,-98.24"/>
-00008a40: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00008a50: 6f72 3d22 6d69 6464 6c65 2220 783d 2231  or="middle" x="1
-00008a60: 3633 312e 3522 2079 3d22 2d31 3331 2e38  631.5" y="-131.8
-00008a70: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
-00008a80: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
-00008a90: 2d73 697a 653d 2231 342e 3030 223e 4e65  -size="14.00">Ne
-00008aa0: 696e 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  in</text>.</g>.<
-00008ab0: 212d 2d20 4130 3920 2d2d 3e0a 3c67 2069  !-- A09 -->.<g i
-00008ac0: 643d 226e 6f64 6532 3322 2063 6c61 7373  d="node23" class
-00008ad0: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
-00008ae0: 4130 393c 2f74 6974 6c65 3e0a 3c70 6f6c  A09</title>.<pol
-00008af0: 7967 6f6e 2066 696c 6c3d 2223 6363 6139  ygon fill="#cca9
-00008b00: 6162 2220 7374 726f 6b65 3d22 626c 6163  ab" stroke="blac
-00008b10: 6b22 2070 6f69 6e74 733d 2232 3032 302e  k" points="2020.
-00008b20: 352c 2d31 3130 2031 3639 322e 352c 2d31  5,-110 1692.5,-1
-00008b30: 3130 2031 3639 322e 352c 3020 3230 3230  10 1692.5,0 2020
-00008b40: 2e35 2c30 2032 3032 302e 352c 2d31 3130  .5,0 2020.5,-110
-00008b50: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
-00008b60: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
-00008b70: 2231 3834 3122 2079 3d22 2d39 332e 3822  "1841" y="-93.8"
-00008b80: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00008b90: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00008ba0: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
-00008bb0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
-00008bc0: 4130 393c 2f74 6578 743e 0a3c 7465 7874  A09</text>.<text
-00008bd0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
-00008be0: 6172 7422 2078 3d22 3137 3034 2e35 2220  art" x="1704.5" 
-00008bf0: 793d 222d 3831 2e34 2220 666f 6e74 2d66  y="-81.4" font-f
-00008c00: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00008c10: 6966 2220 7465 7874 2d64 6563 6f72 6174  if" text-decorat
-00008c20: 696f 6e3d 2275 6e64 6572 6c69 6e65 2220  ion="underline" 
-00008c30: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00008c40: 223e 4869 6e77 6569 733a 3c2f 7465 7874  ">Hinweis:</text
-00008c50: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
-00008c60: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
-00008c70: 3730 342e 3522 2079 3d22 2d36 392e 3422  704.5" y="-69.4"
-00008c80: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
-00008c90: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
-00008ca0: 7369 7a65 3d22 3132 2e30 3022 3e43 6c75  size="12.00">Clu
-00008cb0: 7374 6572 3a20 5a75 7374 696d 6d75 6e67  ster: Zustimmung
-00008cc0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
-00008cd0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
-00008ce0: 2220 783d 2231 3730 342e 3522 2079 3d22  " x="1704.5" y="
-00008cf0: 2d35 372e 3422 2066 6f6e 742d 6661 6d69  -57.4" font-fami
-00008d00: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
-00008d10: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
-00008d20: 3022 3e45 726e 6575 7465 2042 6573 7426  0">Erneute Best&
-00008d30: 2332 3238 3b74 6967 756e 6720 6465 7220  #228;tigung der 
-00008d40: 4162 6d65 6c64 756e 6720 6175 6667 7275  Abmeldung aufgru
-00008d50: 6e64 2064 6572 3c2f 7465 7874 3e0a 3c74  nd der</text>.<t
-00008d60: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
-00008d70: 2273 7461 7274 2220 783d 2231 3730 342e  "start" x="1704.
-00008d80: 3522 2079 3d22 2d34 352e 3422 2066 6f6e  5" y="-45.4" fon
-00008d90: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00008da0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00008db0: 3d22 3132 2e30 3022 3e49 6e66 6f72 6d61  ="12.00">Informa
-00008dc0: 7469 6f6e 2c20 6461 7373 2064 6572 2041  tion, dass der A
-00008dd0: 6e73 6368 6c75 7373 6e75 747a 6572 206e  nschlussnutzer n
-00008de0: 6963 6874 206d 6568 723c 2f74 6578 743e  icht mehr</text>
-00008df0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
-00008e00: 6f72 3d22 7374 6172 7422 2078 3d22 3137  or="start" x="17
-00008e10: 3034 2e35 2220 793d 222d 3333 2e34 2220  04.5" y="-33.4" 
-00008e20: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
-00008e30: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
-00008e40: 697a 653d 2231 322e 3030 223e 616e 2064  ize="12.00">an d
-00008e50: 6572 204d 6172 6b74 6c6f 6b61 7469 6f6e  er Marktlokation
-00008e60: 2076 6f72 6861 6e64 656e 2069 7374 2e3c   vorhanden ist.<
-00008e70: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
-00008e80: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
-00008e90: 2078 3d22 3137 3034 2e35 2220 793d 222d   x="1704.5" y="-
-00008ea0: 3231 2e34 2220 666f 6e74 2d66 616d 696c  21.4" font-famil
-00008eb0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
-00008ec0: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
-00008ed0: 223e 4869 6e77 6569 733a 2044 6173 2062  ">Hinweis: Das b
-00008ee0: 6973 6865 7220 6265 7374 2623 3232 383b  isher best&#228;
-00008ef0: 7469 6774 6520 4269 6c61 6e7a 6965 7275  tigte Bilanzieru
-00008f00: 6e67 7365 6e64 653c 2f74 6578 743e 0a3c  ngsende</text>.<
-00008f10: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
-00008f20: 3d22 7374 6172 7422 2078 3d22 3137 3034  ="start" x="1704
-00008f30: 2e35 2220 793d 222d 392e 3422 2066 6f6e  .5" y="-9.4" fon
-00008f40: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
-00008f50: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
-00008f60: 3d22 3132 2e30 3022 3e62 6c65 6962 7420  ="12.00">bleibt 
-00008f70: 756e 7665 7226 2332 3238 3b6e 6465 7274  unver&#228;ndert
-00008f80: 2062 6573 7465 6865 6e2e 3c2f 7465 7874   bestehen.</text
-00008f90: 3e0a 3c2f 673e 0a3c 212d 2d20 3133 2623  >.</g>.<!-- 13&#
-00008fa0: 3435 3b26 6774 3b41 3039 202d 2d3e 0a3c  45;&gt;A09 -->.<
-00008fb0: 6720 6964 3d22 6564 6765 3237 2220 636c  g id="edge27" cl
-00008fc0: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
-00008fd0: 6c65 3e31 332d 2667 743b 4130 393c 2f74  le>13-&gt;A09</t
-00008fe0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
-00008ff0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
-00009000: 626c 6163 6b22 2064 3d22 4d31 3735 362e  black" d="M1756.
-00009010: 3833 2c2d 3136 302e 3633 4331 3737 302e  83,-160.63C1770.
-00009020: 3035 2c2d 3134 362e 3735 2031 3738 342c  05,-146.75 1784,
-00009030: 2d31 3332 2e31 2031 3739 372e 3135 2c2d  -132.1 1797.15,-
-00009040: 3131 382e 3322 2f3e 0a3c 706f 6c79 676f  118.3"/>.<polygo
-00009050: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
-00009060: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
-00009070: 696e 7473 3d22 3137 3939 2e33 382c 2d31  ints="1799.38,-1
-00009080: 3231 2e30 3420 3138 3033 2e37 342c 2d31  21.04 1803.74,-1
-00009090: 3131 2e33 3820 3137 3934 2e33 312c 2d31  11.38 1794.31,-1
-000090a0: 3136 2e32 3120 3137 3939 2e33 382c 2d31  16.21 1799.38,-1
-000090b0: 3231 2e30 3422 2f3e 0a3c 7465 7874 2074  21.04"/>.<text t
-000090c0: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
-000090d0: 6c65 2220 783d 2231 3739 322e 3522 2079  le" x="1792.5" y
-000090e0: 3d22 2d31 3331 2e38 2220 666f 6e74 2d66  ="-131.8" font-f
-000090f0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
-00009100: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
-00009110: 342e 3030 223e 4a61 3c2f 7465 7874 3e0a  4.00">Ja</text>.
-00009120: 3c2f 673e 0a3c 2f67 3e0a 3c2f 7376 673e  </g>.</g>.</svg>
-00009130: 0a20 203c 2f67 3e0a 3c2f 7376 673e 0a    .  </g>.</svg>.
+000000f0: 0a20 203c 673e 0a20 2020 203c 7376 6720  .  <g>.    <svg 
+00000100: 7665 7273 696f 6e3d 2231 2e31 2220 7769  version="1.1" wi
+00000110: 6474 683d 2232 3834 302e 3070 7822 2076  dth="2840.0px" v
+00000120: 6965 7742 6f78 3d22 3020 3020 3238 3430  iewBox="0 0 2840
+00000130: 2e30 2032 3036 322e 3636 3636 3636 3636  .0 2062.66666666
+00000140: 3636 3636 3522 2068 6569 6768 743d 2232  66665" height="2
+00000150: 3036 322e 3636 3636 3636 3636 3636 3636  062.666666666666
+00000160: 3570 7822 3e0a 2020 3c70 6f6c 7967 6f6e  5px">.  <polygon
+00000170: 2066 696c 6c3d 2223 6633 6631 6636 2220   fill="#f3f1f6" 
+00000180: 706f 696e 7473 3d22 302c 3020 3238 3430  points="0,0 2840
+00000190: 2e30 2c30 2032 3834 302e 302c 3230 3632  .0,0 2840.0,2062
+000001a0: 2e36 3636 3636 3636 3636 3636 3635 2030  .6666666666665 0
+000001b0: 2c32 3036 322e 3636 3636 3636 3636 3636  ,2062.6666666666
+000001c0: 3636 3522 2f3e 3c67 3e0a 2020 2020 3c67  665"/><g>.    <g
+000001d0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000001e0: 736c 6174 6528 3539 352e 3534 3533 3339  slate(595.545339
+000001f0: 3334 3832 3631 382c 2032 3036 2e32 3636  3482618, 206.266
+00000200: 3636 3636 3636 3636 3636 2920 7363 616c  6666666666) scal
+00000210: 6528 3120 3129 2074 7261 6e73 6c61 7465  e(1 1) translate
+00000220: 2830 2c20 3029 2073 6361 6c65 2839 2e33  (0, 0) scale(9.3
+00000230: 3238 3634 3839 3538 3539 3034 3338 2039  28648958590438 9
+00000240: 2e33 3238 3634 3839 3538 3539 3034 3338  .328648958590438
+00000250: 2920 223e 3c73 6f64 6970 6f64 693a 6e61  ) "><sodipodi:na
+00000260: 6d65 6476 6965 7720 786d 6c6e 733a 736f  medview xmlns:so
+00000270: 6469 706f 6469 3d22 6874 7470 3a2f 2f73  dipodi="http://s
+00000280: 6f64 6970 6f64 692e 736f 7572 6365 666f  odipodi.sourcefo
+00000290: 7267 652e 6e65 742f 4454 442f 736f 6469  rge.net/DTD/sodi
+000002a0: 706f 6469 2d30 2e64 7464 2220 786d 6c6e  podi-0.dtd" xmln
+000002b0: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
+000002c0: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
+000002d0: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
+000002e0: 6e6b 7363 6170 6522 2069 643d 226e 616d  nkscape" id="nam
+000002f0: 6564 7669 6577 3722 2070 6167 6563 6f6c  edview7" pagecol
+00000300: 6f72 3d22 2366 6666 6666 6622 2062 6f72  or="#ffffff" bor
+00000310: 6465 7263 6f6c 6f72 3d22 2339 3939 3939  dercolor="#99999
+00000320: 3922 2062 6f72 6465 726f 7061 6369 7479  9" borderopacity
+00000330: 3d22 3122 2069 6e6b 7363 6170 653a 7061  ="1" inkscape:pa
+00000340: 6765 7368 6164 6f77 3d22 3022 2069 6e6b  geshadow="0" ink
+00000350: 7363 6170 653a 7061 6765 6f70 6163 6974  scape:pageopacit
+00000360: 793d 2230 2220 696e 6b73 6361 7065 3a70  y="0" inkscape:p
+00000370: 6167 6563 6865 636b 6572 626f 6172 643d  agecheckerboard=
+00000380: 2230 2220 696e 6b73 6361 7065 3a64 6f63  "0" inkscape:doc
+00000390: 756d 656e 742d 756e 6974 733d 226d 6d22  ument-units="mm"
+000003a0: 2073 686f 7767 7269 643d 2266 616c 7365   showgrid="false
+000003b0: 2220 6669 742d 6d61 7267 696e 2d74 6f70  " fit-margin-top
+000003c0: 3d22 3022 2066 6974 2d6d 6172 6769 6e2d  ="0" fit-margin-
+000003d0: 6c65 6674 3d22 3022 2066 6974 2d6d 6172  left="0" fit-mar
+000003e0: 6769 6e2d 7269 6768 743d 2230 2220 6669  gin-right="0" fi
+000003f0: 742d 6d61 7267 696e 2d62 6f74 746f 6d3d  t-margin-bottom=
+00000400: 2230 2220 696e 6b73 6361 7065 3a7a 6f6f  "0" inkscape:zoo
+00000410: 6d3d 2230 2e36 3430 3532 3332 3922 2069  m="0.64052329" i
+00000420: 6e6b 7363 6170 653a 6378 3d22 3133 302e  nkscape:cx="130.
+00000430: 3336 3231 3622 2069 6e6b 7363 6170 653a  36216" inkscape:
+00000440: 6379 3d22 3431 322e 3136 3322 2069 6e6b  cy="412.163" ink
+00000450: 7363 6170 653a 7769 6e64 6f77 2d77 6964  scape:window-wid
+00000460: 7468 3d22 3135 3132 2220 696e 6b73 6361  th="1512" inksca
+00000470: 7065 3a77 696e 646f 772d 6865 6967 6874  pe:window-height
+00000480: 3d22 3931 3622 2069 6e6b 7363 6170 653a  ="916" inkscape:
+00000490: 7769 6e64 6f77 2d78 3d22 3338 3430 2220  window-x="3840" 
+000004a0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+000004b0: 793d 2231 3336 2220 696e 6b73 6361 7065  y="136" inkscape
+000004c0: 3a77 696e 646f 772d 6d61 7869 6d69 7a65  :window-maximize
+000004d0: 643d 2230 2220 696e 6b73 6361 7065 3a63  d="0" inkscape:c
+000004e0: 7572 7265 6e74 2d6c 6179 6572 3d22 6c61  urrent-layer="la
+000004f0: 7965 7231 222f 3e0a 2020 3c64 6566 7320  yer1"/>.  <defs 
+00000500: 6964 3d22 6465 6673 3222 3e0a 2020 2020  id="defs2">.    
+00000510: 3c63 6c69 7050 6174 6820 636c 6970 5061  <clipPath clipPa
+00000520: 7468 556e 6974 733d 2275 7365 7253 7061  thUnits="userSpa
+00000530: 6365 4f6e 5573 6522 2069 643d 2263 6c69  ceOnUse" id="cli
+00000540: 7050 6174 6832 3322 3e0a 2020 2020 2020  pPath23">.      
+00000550: 3c70 6174 6820 643d 224d 2030 2c35 3638  <path d="M 0,568
+00000560: 2e31 3536 2048 2035 3739 2e32 3336 2056  .156 H 579.236 V
+00000570: 2030 2048 2030 205a 2220 6964 3d22 7061   0 H 0 Z" id="pa
+00000580: 7468 3231 222f 3e0a 2020 2020 3c2f 636c  th21"/>.    </cl
+00000590: 6970 5061 7468 3e0a 2020 3c2f 6465 6673  ipPath>.  </defs
+000005a0: 3e0a 2020 3c67 2078 6d6c 6e73 3a69 6e6b  >.  <g xmlns:ink
+000005b0: 7363 6170 653d 2268 7474 703a 2f2f 7777  scape="http://ww
+000005c0: 772e 696e 6b73 6361 7065 2e6f 7267 2f6e  w.inkscape.org/n
+000005d0: 616d 6573 7061 6365 732f 696e 6b73 6361  amespaces/inksca
+000005e0: 7065 2220 696e 6b73 6361 7065 3a6c 6162  pe" inkscape:lab
+000005f0: 656c 3d22 4c61 7965 7220 3122 2069 6e6b  el="Layer 1" ink
+00000600: 7363 6170 653a 6772 6f75 706d 6f64 653d  scape:groupmode=
+00000610: 226c 6179 6572 2220 6964 3d22 6c61 7965  "layer" id="laye
+00000620: 7231 2220 7472 616e 7366 6f72 6d3d 2274  r1" transform="t
+00000630: 7261 6e73 6c61 7465 282d 3136 2e35 3431  ranslate(-16.541
+00000640: 3933 372c 2d35 352e 3330 3532 3637 2922  937,-55.305267)"
+00000650: 3e0a 2020 2020 3c67 2069 643d 2267 3139  >.    <g id="g19
+00000660: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
+00000670: 2823 636c 6970 5061 7468 3233 2922 2074  (#clipPath23)" t
+00000680: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00000690: 2830 2e33 3532 3737 3737 372c 302c 302c  (0.35277777,0,0,
+000006a0: 2d30 2e33 3532 3737 3737 372c 302e 3031  -0.35277777,0.01
+000006b0: 3031 3730 3233 2c32 3433 2e37 3336 3735  017023,243.73675
+000006c0: 2922 2073 7479 6c65 3d22 6f70 6163 6974  )" style="opacit
+000006d0: 793a 302e 3222 3e0a 2020 2020 2020 3c67  y:0.2">.      <g
+000006e0: 2069 643d 2267 3235 2220 7472 616e 7366   id="g25" transf
+000006f0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2831  orm="translate(1
+00000700: 3232 2e34 3434 2c33 322e 3731 3935 2922  22.444,32.7195)"
+00000710: 3e0a 2020 2020 2020 2020 3c70 6174 6820  >.        <path 
+00000720: 643d 226d 2030 2c30 2068 202d 3536 2e31  d="m 0,0 h -56.1
+00000730: 3034 2063 202d 3131 2c30 202d 3139 2e38  04 c -11,0 -19.8
+00000740: 3938 2c39 2e31 3233 202d 3139 2e34 3633  98,9.123 -19.463
+00000750: 2c32 302e 3131 3520 3130 2e35 3934 2c32  ,20.115 10.594,2
+00000760: 3637 2e31 3931 2032 3331 2e32 3737 2c34  67.191 231.277,4
+00000770: 3831 2e33 3032 2035 3031 2e30 3239 2c34  81.302 501.029,4
+00000780: 3831 2e33 3032 2076 202d 3536 2e30 3220  81.302 v -56.02 
+00000790: 6320 302c 2d31 302e 3938 202d 382e 3638  c 0,-10.98 -8.68
+000007a0: 382c 2d31 392e 3839 3220 2d31 392e 3635  8,-19.892 -19.65
+000007b0: 382c 2d32 302e 3339 3320 4320 3138 302e  8,-20.393 C 180.
+000007c0: 3239 2c34 3134 2e36 3937 2030 2c32 3238  29,414.697 0,228
+000007d0: 2e30 3035 2030 2c30 2220 7374 796c 653d  .005 0,0" style=
+000007e0: 2266 696c 6c3a 2336 6561 6438 333b 6669  "fill:#6ead83;fi
+000007f0: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00000800: 6c2d 7275 6c65 3a6e 6f6e 7a65 726f 3b73  l-rule:nonzero;s
+00000810: 7472 6f6b 653a 6e6f 6e65 2220 6964 3d22  troke:none" id="
+00000820: 7061 7468 3237 222f 3e0a 2020 2020 2020  path27"/>.      
+00000830: 3c2f 673e 0a20 2020 2020 203c 6720 6964  </g>.      <g id
+00000840: 3d22 6732 3922 2074 7261 6e73 666f 726d  ="g29" transform
+00000850: 3d22 7472 616e 736c 6174 6528 3237 332e  ="translate(273.
+00000860: 3738 3238 2c33 322e 3731 3935 2922 3e0a  7828,32.7195)">.
+00000870: 2020 2020 2020 2020 3c70 6174 6820 643d          <path d=
+00000880: 226d 2030 2c30 2068 202d 3535 2e39 3236  "m 0,0 h -55.926
+00000890: 2063 202d 3131 2e32 3238 2c30 202d 3230   c -11.228,0 -20
+000008a0: 2e30 3931 2c39 2e34 3832 202d 3139 2e34  .091,9.482 -19.4
+000008b0: 3335 2c32 302e 3639 2031 302e 3734 342c  35,20.69 10.744,
+000008c0: 3138 332e 3433 3920 3136 332e 3338 392c  183.439 163.389,
+000008d0: 3332 392e 3338 3820 3334 392e 3438 352c  329.388 349.485,
+000008e0: 3332 392e 3338 3820 7620 2d35 362e 3236  329.388 v -56.26
+000008f0: 3320 6320 302c 2d31 302e 3730 3920 2d38  3 c 0,-10.709 -8
+00000900: 2e32 3733 2c2d 3139 2e36 3137 202d 3138  .273,-19.617 -18
+00000910: 2e39 3537 2c2d 3230 2e33 3520 4320 3131  .957,-20.35 C 11
+00000920: 322e 3831 392c 3236 332e 3639 3620 302c  2.819,263.696 0,
+00000930: 3134 342e 3737 3420 302c 3022 2073 7479  144.774 0,0" sty
+00000940: 6c65 3d22 6669 6c6c 3a23 3665 6164 3833  le="fill:#6ead83
+00000950: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00000960: 6669 6c6c 2d72 756c 653a 6e6f 6e7a 6572  fill-rule:nonzer
+00000970: 6f3b 7374 726f 6b65 3a6e 6f6e 6522 2069  o;stroke:none" i
+00000980: 643d 2270 6174 6833 3122 2f3e 0a20 2020  d="path31"/>.   
+00000990: 2020 203c 2f67 3e0a 2020 2020 2020 3c67     </g>.      <g
+000009a0: 2069 643d 2267 3333 2220 7472 616e 7366   id="g33" transf
+000009b0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2834  orm="translate(4
+000009c0: 3235 2e37 3636 372c 3332 2e37 3139 3529  25.7667,32.7195)
+000009d0: 223e 0a20 2020 2020 2020 203c 7061 7468  ">.        <path
+000009e0: 2064 3d22 6d20 302c 3020 6820 2d35 352e   d="m 0,0 h -55.
+000009f0: 3434 3520 6320 2d31 312e 3635 332c 3020  445 c -11.653,0 
+00000a00: 2d32 302e 3630 342c 3130 2e31 3720 2d31  -20.604,10.17 -1
+00000a10: 392e 3333 342c 3231 2e37 3533 2031 302e  9.334,21.753 10.
+00000a20: 3836 362c 3939 2e30 3332 2039 352e 3033  866,99.032 95.03
+00000a30: 312c 3137 362e 3334 3120 3139 362e 3931  1,176.341 196.91
+00000a40: 392c 3137 362e 3334 3120 7620 2d35 372e  9,176.341 v -57.
+00000a50: 3031 3120 6320 302c 2d31 302e 3034 3620  011 c 0,-10.046 
+00000a60: 2d37 2e32 3833 2c2d 3138 2e37 3535 202d  -7.283,-18.755 -
+00000a70: 3137 2e32 3239 2c2d 3230 2e31 3635 2043  17.229,-20.165 C
+00000a80: 2034 352e 3638 382c 3131 322e 3532 3220   45.688,112.522 
+00000a90: 302c 3631 2e34 3937 2030 2c30 2220 7374  0,61.497 0,0" st
+00000aa0: 796c 653d 2266 696c 6c3a 2336 6561 6438  yle="fill:#6ead8
+00000ab0: 333b 6669 6c6c 2d6f 7061 6369 7479 3a31  3;fill-opacity:1
+00000ac0: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00000ad0: 726f 3b73 7472 6f6b 653a 6e6f 6e65 2220  ro;stroke:none" 
+00000ae0: 6964 3d22 7061 7468 3335 222f 3e0a 2020  id="path35"/>.  
+00000af0: 2020 2020 3c2f 673e 0a20 2020 203c 2f67      </g>.    </g
+00000b00: 3e0a 2020 3c2f 673e 0a3c 2f67 3e0a 2020  >.  </g>.</g>.  
+00000b10: 2020 3c73 7667 2077 6964 7468 3d22 3231    <svg width="21
+00000b20: 3330 7074 2220 6865 6967 6874 3d22 3135  30pt" height="15
+00000b30: 3437 7074 2220 7669 6577 426f 783d 2230  47pt" viewBox="0
+00000b40: 2e30 3020 302e 3030 2032 3132 392e 3530  .00 0.00 2129.50
+00000b50: 2031 3534 372e 3030 223e 0a3c 6720 6964   1547.00">.<g id
+00000b60: 3d22 6772 6170 6830 2220 636c 6173 733d  ="graph0" class=
+00000b70: 2267 7261 7068 2220 7472 616e 7366 6f72  "graph" transfor
+00000b80: 6d3d 2273 6361 6c65 2831 2031 2920 726f  m="scale(1 1) ro
+00000b90: 7461 7465 2830 2920 7472 616e 736c 6174  tate(0) translat
+00000ba0: 6528 3420 3135 3433 2922 3e0a 3c74 6974  e(4 1543)">.<tit
+00000bb0: 6c65 3e44 3c2f 7469 746c 653e 0a3c 7465  le>D</title>.<te
+00000bc0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00000bd0: 7374 6172 7422 2078 3d22 3931 362e 3735  start" x="916.75
+00000be0: 2220 793d 222d 3135 3231 2e36 2220 666f  " y="-1521.6" fo
+00000bf0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00000c00: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+00000c10: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
+00000c20: 7369 7a65 3d22 3138 2e30 3022 3e36 2e32  size="18.00">6.2
+00000c30: 2041 443a 204c 6965 6665 7265 6e64 6520   AD: Lieferende 
+00000c40: 4c46 2061 6e20 4e42 3c2f 7465 7874 3e0a  LF an NB</text>.
+00000c50: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00000c60: 723d 2273 7461 7274 2220 783d 2239 3133  r="start" x="913
+00000c70: 2e37 3522 2079 3d22 2d31 3439 312e 3222  .75" y="-1491.2"
+00000c80: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00000c90: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00000ca0: 7765 6967 6874 3d22 626f 6c64 2220 666f  weight="bold" fo
+00000cb0: 6e74 2d73 697a 653d 2231 362e 3030 223e  nt-size="16.00">
+00000cc0: 362e 322e 3120 455f 3034 3031 5f41 626d  6.2.1 E_0401_Abm
+00000cd0: 656c 6475 6e67 2070 7226 2332 3532 3b66  eldung pr&#252;f
+00000ce0: 656e 3c2f 7465 7874 3e0a 3c21 2d2d 2053  en</text>.<!-- S
+00000cf0: 7461 7274 202d 2d3e 0a3c 6720 6964 3d22  tart -->.<g id="
+00000d00: 6e6f 6465 3122 2063 6c61 7373 3d22 6e6f  node1" class="no
+00000d10: 6465 223e 0a3c 7469 746c 653e 5374 6172  de">.<title>Star
+00000d20: 743c 2f74 6974 6c65 3e0a 3c70 6f6c 7967  t</title>.<polyg
+00000d30: 6f6e 2066 696c 6c3d 2223 3761 3864 6131  on fill="#7a8da1
+00000d40: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00000d50: 2070 6f69 6e74 733d 2231 3432 342c 2d31   points="1424,-1
+00000d60: 3434 3120 3132 3633 2c2d 3134 3431 2031  441 1263,-1441 1
+00000d70: 3236 332c 2d31 3339 3720 3134 3234 2c2d  263,-1397 1424,-
+00000d80: 3133 3937 2031 3432 342c 2d31 3434 3122  1397 1424,-1441"
+00000d90: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00000da0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00000db0: 3133 3135 2220 793d 222d 3134 3231 2e38  1315" y="-1421.8
+00000dc0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00000dd0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00000de0: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00000df0: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00000e00: 3e45 5f30 3430 313c 2f74 6578 743e 0a3c  >E_0401</text>.<
+00000e10: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00000e20: 3d22 7374 6172 7422 2078 3d22 3132 3737  ="start" x="1277
+00000e30: 2220 793d 222d 3134 3039 2e34 2220 666f  " y="-1409.4" fo
+00000e40: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00000e50: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+00000e60: 6768 743d 2262 6f6c 6422 2074 6578 742d  ght="bold" text-
+00000e70: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00000e80: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00000e90: 3d22 3132 2e30 3022 3e50 7226 2332 3532  ="12.00">Pr&#252
+00000ea0: 3b66 656e 6465 2052 6f6c 6c65 3a3c 2f74  ;fende Rolle:</t
+00000eb0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00000ec0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00000ed0: 3d22 3133 3833 2220 793d 222d 3134 3039  ="1383" y="-1409
+00000ee0: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00000ef0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00000f00: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
+00000f10: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
+00000f20: 3022 3e20 4e42 3c2f 7465 7874 3e0a 3c2f  0"> NB</text>.</
+00000f30: 673e 0a3c 212d 2d20 3120 2d2d 3e0a 3c67  g>.<!-- 1 -->.<g
+00000f40: 2069 643d 226e 6f64 6532 2220 636c 6173   id="node2" clas
+00000f50: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
+00000f60: 3e31 3c2f 7469 746c 653e 0a3c 7061 7468  >1</title>.<path
+00000f70: 2066 696c 6c3d 2223 3761 6162 3861 2220   fill="#7aab8a" 
+00000f80: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
+00000f90: 3d22 4d31 3537 302e 352c 2d31 3336 3043  ="M1570.5,-1360C
+00000fa0: 3135 3730 2e35 2c2d 3133 3630 2031 3131  1570.5,-1360 111
+00000fb0: 362e 352c 2d31 3336 3020 3131 3136 2e35  6.5,-1360 1116.5
+00000fc0: 2c2d 3133 3630 2031 3131 302e 352c 2d31  ,-1360 1110.5,-1
+00000fd0: 3336 3020 3131 3034 2e35 2c2d 3133 3534  360 1104.5,-1354
+00000fe0: 2031 3130 342e 352c 2d31 3334 3820 3131   1104.5,-1348 11
+00000ff0: 3034 2e35 2c2d 3133 3438 2031 3130 342e  04.5,-1348 1104.
+00001000: 352c 2d31 3235 3620 3131 3034 2e35 2c2d  5,-1256 1104.5,-
+00001010: 3132 3536 2031 3130 342e 352c 2d31 3235  1256 1104.5,-125
+00001020: 3020 3131 3130 2e35 2c2d 3132 3434 2031  0 1110.5,-1244 1
+00001030: 3131 362e 352c 2d31 3234 3420 3131 3136  116.5,-1244 1116
+00001040: 2e35 2c2d 3132 3434 2031 3537 302e 352c  .5,-1244 1570.5,
+00001050: 2d31 3234 3420 3135 3730 2e35 2c2d 3132  -1244 1570.5,-12
+00001060: 3434 2031 3537 362e 352c 2d31 3234 3420  44 1576.5,-1244 
+00001070: 3135 3832 2e35 2c2d 3132 3530 2031 3538  1582.5,-1250 158
+00001080: 322e 352c 2d31 3235 3620 3135 3832 2e35  2.5,-1256 1582.5
+00001090: 2c2d 3132 3536 2031 3538 322e 352c 2d31  ,-1256 1582.5,-1
+000010a0: 3334 3820 3135 3832 2e35 2c2d 3133 3438  348 1582.5,-1348
+000010b0: 2031 3538 322e 352c 2d31 3335 3420 3135   1582.5,-1354 15
+000010c0: 3736 2e35 2c2d 3133 3630 2031 3537 302e  76.5,-1360 1570.
+000010d0: 352c 2d31 3336 3022 2f3e 0a3c 7465 7874  5,-1360"/>.<text
+000010e0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+000010f0: 6172 7422 2078 3d22 3131 3138 2e35 2220  art" x="1118.5" 
+00001100: 793d 222d 3133 3430 2e38 2220 666f 6e74  y="-1340.8" font
+00001110: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00001120: 6572 6966 2220 666f 6e74 2d77 6569 6768  erif" font-weigh
+00001130: 743d 2262 6f6c 6422 2066 6f6e 742d 7369  t="bold" font-si
+00001140: 7a65 3d22 3134 2e30 3022 3e31 3a20 3c2f  ze="14.00">1: </
+00001150: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00001160: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00001170: 783d 2231 3133 382e 3522 2079 3d22 2d31  x="1138.5" y="-1
+00001180: 3334 302e 3822 2066 6f6e 742d 6661 6d69  340.8" font-fami
+00001190: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+000011a0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+000011b0: 3022 3e4c 6965 6774 2065 696e 2054 7261  0">Liegt ein Tra
+000011c0: 6e73 616b 7469 6f6e 7367 7275 6e64 2076  nsaktionsgrund v
+000011d0: 6f72 2c20 6465 7220 6569 6e65 2041 626d  or, der eine Abm
+000011e0: 656c 6475 6e67 206e 7572 2069 6e3c 2f74  eldung nur in</t
+000011f0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00001200: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00001210: 3d22 3131 3138 2e35 2220 793d 222d 3133  ="1118.5" y="-13
+00001220: 3236 2e38 2220 666f 6e74 2d66 616d 696c  26.8" font-famil
+00001230: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00001240: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00001250: 223e 6469 6520 5a75 6b75 6e66 7420 7a75  ">die Zukunft zu
+00001260: 6c26 2332 3238 3b73 7374 3f3c 2f74 6578  l&#228;sst?</tex
+00001270: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00001280: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00001290: 3131 3138 2e35 2220 793d 222d 3133 3132  1118.5" y="-1312
+000012a0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+000012b0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+000012c0: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+000012d0: 4461 7320 6973 7420 6265 6920 6465 6e20  Das ist bei den 
+000012e0: 666f 6c67 656e 6465 6e20 5472 616e 7361  folgenden Transa
+000012f0: 6b74 696f 6e73 6772 2623 3235 323b 6e64  ktionsgr&#252;nd
+00001300: 656e 2064 6572 2046 616c 6c3a 3c2f 7465  en der Fall:</te
+00001310: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00001320: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00001330: 2231 3131 382e 3522 2079 3d22 2d31 3239  "1118.5" y="-129
+00001340: 382e 3822 2066 6f6e 742d 6661 6d69 6c79  8.8" font-family
+00001350: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00001360: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00001370: 3e26 2336 3135 3939 3b20 5765 6368 7365  >&#61599; Wechse
+00001380: 6c3c 2f74 6578 743e 0a3c 7465 7874 2074  l</text>.<text t
+00001390: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+000013a0: 7422 2078 3d22 3131 3138 2e35 2220 793d  t" x="1118.5" y=
+000013b0: 222d 3132 3834 2e38 2220 666f 6e74 2d66  "-1284.8" font-f
+000013c0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+000013d0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+000013e0: 342e 3030 223e 2623 3631 3539 393b 2045  4.00">&#61599; E
+000013f0: 6e64 6520 6465 7220 4553 5620 6f68 6e65  nde der ESV ohne
+00001400: 2046 6f6c 6765 6c69 6566 6572 756e 673c   Folgelieferung<
+00001410: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00001420: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00001430: 2078 3d22 3131 3138 2e35 2220 793d 222d   x="1118.5" y="-
+00001440: 3132 3730 2e38 2220 666f 6e74 2d66 616d  1270.8" font-fam
+00001450: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00001460: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00001470: 3030 223e 2623 3631 3539 393b 2041 7566  00">&#61599; Auf
+00001480: 6865 6275 6e67 2065 696e 6572 207a 756b  hebung einer zuk
+00001490: 2623 3235 323b 6e66 7469 6765 6e20 5a75  &#252;nftigen Zu
+000014a0: 6f72 646e 756e 6720 7765 6765 6e3c 2f74  ordnung wegen</t
+000014b0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+000014c0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000014d0: 3d22 3131 3138 2e35 2220 793d 222d 3132  ="1118.5" y="-12
+000014e0: 3536 2e38 2220 666f 6e74 2d66 616d 696c  56.8" font-famil
+000014f0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00001500: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00001510: 223e 6175 6667 6568 6f62 656e 656d 2056  ">aufgehobenem V
+00001520: 6572 7472 6167 7376 6572 6826 2332 3238  ertragsverh&#228
+00001530: 3b6c 746e 6973 3c2f 7465 7874 3e0a 3c2f  ;ltnis</text>.</
+00001540: 673e 0a3c 212d 2d20 5374 6172 7426 2334  g>.<!-- Start&#4
+00001550: 353b 2667 743b 3120 2d2d 3e0a 3c67 2069  5;&gt;1 -->.<g i
+00001560: 643d 2265 6467 6531 2220 636c 6173 733d  d="edge1" class=
+00001570: 2265 6467 6522 3e0a 3c74 6974 6c65 3e53  "edge">.<title>S
+00001580: 7461 7274 2d26 6774 3b31 3c2f 7469 746c  tart-&gt;1</titl
+00001590: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
+000015a0: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+000015b0: 636b 2220 643d 224d 3133 3433 2e35 2c2d  ck" d="M1343.5,-
+000015c0: 3133 3936 2e36 3443 3133 3433 2e35 2c2d  1396.64C1343.5,-
+000015d0: 3133 3839 2e32 3520 3133 3433 2e35 2c2d  1389.25 1343.5,-
+000015e0: 3133 3830 2e35 3220 3133 3433 2e35 2c2d  1380.52 1343.5,-
+000015f0: 3133 3731 2e34 3222 2f3e 0a3c 706f 6c79  1371.42"/>.<poly
+00001600: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
+00001610: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00001620: 706f 696e 7473 3d22 3133 3437 2c2d 3133  points="1347,-13
+00001630: 3731 2e37 2031 3334 332e 352c 2d31 3336  71.7 1343.5,-136
+00001640: 312e 3720 3133 3430 2c2d 3133 3731 2e37  1.7 1340,-1371.7
+00001650: 2031 3334 372c 2d31 3337 312e 3722 2f3e   1347,-1371.7"/>
+00001660: 0a3c 2f67 3e0a 3c21 2d2d 2032 202d 2d3e  .</g>.<!-- 2 -->
+00001670: 0a3c 6720 6964 3d22 6e6f 6465 3322 2063  .<g id="node3" c
+00001680: 6c61 7373 3d22 6e6f 6465 223e 0a3c 7469  lass="node">.<ti
+00001690: 746c 653e 323c 2f74 6974 6c65 3e0a 3c70  tle>2</title>.<p
+000016a0: 6174 6820 6669 6c6c 3d22 2337 6161 6238  ath fill="#7aab8
+000016b0: 6122 2073 7472 6f6b 653d 2262 6c61 636b  a" stroke="black
+000016c0: 2220 643d 224d 3133 3334 2e35 2c2d 3131  " d="M1334.5,-11
+000016d0: 3933 4331 3333 342e 352c 2d31 3139 3320  93C1334.5,-1193 
+000016e0: 3838 382e 352c 2d31 3139 3320 3838 382e  888.5,-1193 888.
+000016f0: 352c 2d31 3139 3320 3838 322e 352c 2d31  5,-1193 882.5,-1
+00001700: 3139 3320 3837 362e 352c 2d31 3138 3720  193 876.5,-1187 
+00001710: 3837 362e 352c 2d31 3138 3120 3837 362e  876.5,-1181 876.
+00001720: 352c 2d31 3138 3120 3837 362e 352c 2d31  5,-1181 876.5,-1
+00001730: 3037 3520 3837 362e 352c 2d31 3037 3520  075 876.5,-1075 
+00001740: 3837 362e 352c 2d31 3036 3920 3838 322e  876.5,-1069 882.
+00001750: 352c 2d31 3036 3320 3838 382e 352c 2d31  5,-1063 888.5,-1
+00001760: 3036 3320 3838 382e 352c 2d31 3036 3320  063 888.5,-1063 
+00001770: 3133 3334 2e35 2c2d 3130 3633 2031 3333  1334.5,-1063 133
+00001780: 342e 352c 2d31 3036 3320 3133 3430 2e35  4.5,-1063 1340.5
+00001790: 2c2d 3130 3633 2031 3334 362e 352c 2d31  ,-1063 1346.5,-1
+000017a0: 3036 3920 3133 3436 2e35 2c2d 3130 3735  069 1346.5,-1075
+000017b0: 2031 3334 362e 352c 2d31 3037 3520 3133   1346.5,-1075 13
+000017c0: 3436 2e35 2c2d 3131 3831 2031 3334 362e  46.5,-1181 1346.
+000017d0: 352c 2d31 3138 3120 3133 3436 2e35 2c2d  5,-1181 1346.5,-
+000017e0: 3131 3837 2031 3334 302e 352c 2d31 3139  1187 1340.5,-119
+000017f0: 3320 3133 3334 2e35 2c2d 3131 3933 222f  3 1334.5,-1193"/
+00001800: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00001810: 686f 723d 2273 7461 7274 2220 783d 2238  hor="start" x="8
+00001820: 3930 2e35 2220 793d 222d 3131 3733 2e38  90.5" y="-1173.8
+00001830: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00001840: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00001850: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00001860: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00001870: 3e32 3a20 3c2f 7465 7874 3e0a 3c74 6578  >2: </text>.<tex
+00001880: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00001890: 7461 7274 2220 783d 2239 3130 2e35 2220  tart" x="910.5" 
+000018a0: 793d 222d 3131 3733 2e38 2220 666f 6e74  y="-1173.8" font
+000018b0: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+000018c0: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+000018d0: 2231 342e 3030 223e 4c69 6567 7420 6569  "14.00">Liegt ei
+000018e0: 6e20 5472 616e 7361 6b74 696f 6e73 6772  n Transaktionsgr
+000018f0: 756e 6420 766f 722c 2077 656c 6368 6572  und vor, welcher
+00001900: 206d 6974 7465 696c 742c 2064 6173 7320   mitteilt, dass 
+00001910: 6465 723c 2f74 6578 743e 0a3c 7465 7874  der</text>.<text
+00001920: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00001930: 6172 7422 2078 3d22 3839 302e 3522 2079  art" x="890.5" y
+00001940: 3d22 2d31 3135 392e 3822 2066 6f6e 742d  ="-1159.8" font-
+00001950: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00001960: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00001970: 3134 2e30 3022 3e4b 756e 6465 2076 6f72  14.00">Kunde vor
+00001980: 204c 6965 6665 7262 6567 696e 6e20 6175   Lieferbeginn au
+00001990: 7367 657a 6f67 656e 2069 7374 2c20 627a  sgezogen ist, bz
+000019a0: 772e 2064 6965 3c2f 7465 7874 3e0a 3c74  w. die</text>.<t
+000019b0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+000019c0: 2273 7461 7274 2220 783d 2238 3930 2e35  "start" x="890.5
+000019d0: 2220 793d 222d 3131 3435 2e38 2220 666f  " y="-1145.8" fo
+000019e0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000019f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00001a00: 653d 2231 342e 3030 223e 4d61 726b 746c  e="14.00">Marktl
+00001a10: 6f6b 6174 696f 6e20 766f 7220 4c69 6566  okation vor Lief
+00001a20: 6572 6265 6769 6e6e 2073 7469 6c6c 6765  erbeginn stillge
+00001a30: 6c65 6774 2077 7572 6465 3f3c 2f74 6578  legt wurde?</tex
+00001a40: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00001a50: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00001a60: 3839 302e 3522 2079 3d22 2d31 3133 312e  890.5" y="-1131.
+00001a70: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00001a80: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00001a90: 742d 7369 7a65 3d22 3134 2e30 3022 3e44  t-size="14.00">D
+00001aa0: 6173 2069 7374 2062 6569 2064 656e 2066  as ist bei den f
+00001ab0: 6f6c 6765 6e64 656e 2054 7261 6e73 616b  olgenden Transak
+00001ac0: 7469 6f6e 7367 7226 2332 3532 3b6e 6465  tionsgr&#252;nde
+00001ad0: 6e20 6465 7220 4661 6c6c 3a3c 2f74 6578  n der Fall:</tex
+00001ae0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+00001af0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00001b00: 3839 302e 3522 2079 3d22 2d31 3131 372e  890.5" y="-1117.
+00001b10: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00001b20: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00001b30: 742d 7369 7a65 3d22 3134 2e30 3022 3e26  t-size="14.00">&
+00001b40: 2336 3135 3939 3b20 4175 6668 6562 756e  #61599; Aufhebun
+00001b50: 6720 6569 6e65 7220 7a75 6b26 2332 3532  g einer zuk&#252
+00001b60: 3b6e 6674 6967 656e 205a 756f 7264 6e75  ;nftigen Zuordnu
+00001b70: 6e67 2077 6567 656e 2041 7573 7a75 673c  ng wegen Auszug<
+00001b80: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00001b90: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00001ba0: 2078 3d22 3839 302e 3522 2079 3d22 2d31   x="890.5" y="-1
+00001bb0: 3130 332e 3822 2066 6f6e 742d 6661 6d69  103.8" font-fami
+00001bc0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00001bd0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00001be0: 3022 3e64 6573 204b 756e 6465 6e3c 2f74  0">des Kunden</t
+00001bf0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00001c00: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00001c10: 3d22 3839 302e 3522 2079 3d22 2d31 3038  ="890.5" y="-108
+00001c20: 392e 3822 2066 6f6e 742d 6661 6d69 6c79  9.8" font-family
+00001c30: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00001c40: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00001c50: 3e26 2336 3135 3939 3b20 4175 6668 6562  >&#61599; Aufheb
+00001c60: 756e 6720 6569 6e65 7220 7a75 6b26 2332  ung einer zuk&#2
+00001c70: 3532 3b6e 6674 6967 656e 205a 756f 7264  52;nftigen Zuord
+00001c80: 6e75 6e67 2077 6567 656e 3c2f 7465 7874  nung wegen</text
+00001c90: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00001ca0: 686f 723d 2273 7461 7274 2220 783d 2238  hor="start" x="8
+00001cb0: 3930 2e35 2220 793d 222d 3130 3735 2e38  90.5" y="-1075.8
+00001cc0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00001cd0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00001ce0: 2d73 697a 653d 2231 342e 3030 223e 5374  -size="14.00">St
+00001cf0: 696c 6c6c 6567 756e 673c 2f74 6578 743e  illlegung</text>
+00001d00: 0a3c 2f67 3e0a 3c21 2d2d 2031 2623 3435  .</g>.<!-- 1&#45
+00001d10: 3b26 6774 3b32 202d 2d3e 0a3c 6720 6964  ;&gt;2 -->.<g id
+00001d20: 3d22 6564 6765 3322 2063 6c61 7373 3d22  ="edge3" class="
+00001d30: 6564 6765 223e 0a3c 7469 746c 653e 312d  edge">.<title>1-
+00001d40: 2667 743b 323c 2f74 6974 6c65 3e0a 3c70  &gt;2</title>.<p
+00001d50: 6174 6820 6669 6c6c 3d22 6e6f 6e65 2220  ath fill="none" 
+00001d60: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
+00001d70: 3d22 4d31 3236 362e 3235 2c2d 3132 3433  ="M1266.25,-1243
+00001d80: 2e37 3343 3132 3437 2e34 372c 2d31 3232  .73C1247.47,-122
+00001d90: 392e 3831 2031 3232 372e 3137 2c2d 3132  9.81 1227.17,-12
+00001da0: 3134 2e37 3520 3132 3037 2e36 332c 2d31  14.75 1207.63,-1
+00001db0: 3230 302e 3237 222f 3e0a 3c70 6f6c 7967  200.27"/>.<polyg
+00001dc0: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00001dd0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00001de0: 6f69 6e74 733d 2231 3230 392e 3736 2c2d  oints="1209.76,-
+00001df0: 3131 3937 2e34 3920 3131 3939 2e36 342c  1197.49 1199.64,
+00001e00: 2d31 3139 342e 3334 2031 3230 352e 3539  -1194.34 1205.59
+00001e10: 2c2d 3132 3033 2e31 3120 3132 3039 2e37  ,-1203.11 1209.7
+00001e20: 362c 2d31 3139 372e 3439 222f 3e0a 3c74  6,-1197.49"/>.<t
+00001e30: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00001e40: 226d 6964 646c 6522 2078 3d22 3132 3537  "middle" x="1257
+00001e50: 2e35 2220 793d 222d 3132 3134 2e38 2220  .5" y="-1214.8" 
+00001e60: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00001e70: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00001e80: 697a 653d 2231 342e 3030 223e 4e65 696e  ize="14.00">Nein
+00001e90: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00001ea0: 2d20 3420 2d2d 3e0a 3c67 2069 643d 226e  - 4 -->.<g id="n
+00001eb0: 6f64 6536 2220 636c 6173 733d 226e 6f64  ode6" class="nod
+00001ec0: 6522 3e0a 3c74 6974 6c65 3e34 3c2f 7469  e">.<title>4</ti
+00001ed0: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00001ee0: 2223 3761 6162 3861 2220 7374 726f 6b65  "#7aab8a" stroke
+00001ef0: 3d22 626c 6163 6b22 2064 3d22 4d31 3737  ="black" d="M177
+00001f00: 362c 2d31 3135 3143 3137 3736 2c2d 3131  6,-1151C1776,-11
+00001f10: 3531 2031 3337 372c 2d31 3135 3120 3133  51 1377,-1151 13
+00001f20: 3737 2c2d 3131 3531 2031 3337 312c 2d31  77,-1151 1371,-1
+00001f30: 3135 3120 3133 3635 2c2d 3131 3435 2031  151 1365,-1145 1
+00001f40: 3336 352c 2d31 3133 3920 3133 3635 2c2d  365,-1139 1365,-
+00001f50: 3131 3339 2031 3336 352c 2d31 3131 3720  1139 1365,-1117 
+00001f60: 3133 3635 2c2d 3131 3137 2031 3336 352c  1365,-1117 1365,
+00001f70: 2d31 3131 3120 3133 3731 2c2d 3131 3035  -1111 1371,-1105
+00001f80: 2031 3337 372c 2d31 3130 3520 3133 3737   1377,-1105 1377
+00001f90: 2c2d 3131 3035 2031 3737 362c 2d31 3130  ,-1105 1776,-110
+00001fa0: 3520 3137 3736 2c2d 3131 3035 2031 3738  5 1776,-1105 178
+00001fb0: 322c 2d31 3130 3520 3137 3838 2c2d 3131  2,-1105 1788,-11
+00001fc0: 3131 2031 3738 382c 2d31 3131 3720 3137  11 1788,-1117 17
+00001fd0: 3838 2c2d 3131 3137 2031 3738 382c 2d31  88,-1117 1788,-1
+00001fe0: 3133 3920 3137 3838 2c2d 3131 3339 2031  139 1788,-1139 1
+00001ff0: 3738 382c 2d31 3134 3520 3137 3832 2c2d  788,-1145 1782,-
+00002000: 3131 3531 2031 3737 362c 2d31 3135 3122  1151 1776,-1151"
+00002010: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00002020: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00002030: 3133 3739 2220 793d 222d 3131 3331 2e38  1379" y="-1131.8
+00002040: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00002050: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00002060: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00002070: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00002080: 3e34 3a20 3c2f 7465 7874 3e0a 3c74 6578  >4: </text>.<tex
+00002090: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+000020a0: 7461 7274 2220 783d 2231 3339 3922 2079  tart" x="1399" y
+000020b0: 3d22 2d31 3133 312e 3822 2066 6f6e 742d  ="-1131.8" font-
+000020c0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000020d0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+000020e0: 3134 2e30 3022 3e4c 6965 6774 2064 6173  14.00">Liegt das
+000020f0: 2045 696e 6761 6e67 7364 6174 756d 206d   Eingangsdatum m
+00002100: 696e 6465 7374 656e 7320 3620 5754 2076  indestens 6 WT v
+00002110: 6f72 2064 656d 3c2f 7465 7874 3e0a 3c74  or dem</text>.<t
+00002120: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00002130: 2273 7461 7274 2220 783d 2231 3337 3922  "start" x="1379"
+00002140: 2079 3d22 2d31 3131 372e 3822 2066 6f6e   y="-1117.8" fon
+00002150: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00002160: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00002170: 3d22 3134 2e30 3022 3e41 626d 656c 6465  ="14.00">Abmelde
+00002180: 6461 7475 6d3f 3c2f 7465 7874 3e0a 3c2f  datum?</text>.</
+00002190: 673e 0a3c 212d 2d20 3126 2334 353b 2667  g>.<!-- 1&#45;&g
+000021a0: 743b 3420 2d2d 3e0a 3c67 2069 643d 2265  t;4 -->.<g id="e
+000021b0: 6467 6532 2220 636c 6173 733d 2265 6467  dge2" class="edg
+000021c0: 6522 3e0a 3c74 6974 6c65 3e31 2d26 6774  e">.<title>1-&gt
+000021d0: 3b34 3c2f 7469 746c 653e 0a3c 7061 7468  ;4</title>.<path
+000021e0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+000021f0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+00002200: 3134 3231 2e30 392c 2d31 3234 332e 3733  1421.09,-1243.73
+00002210: 4331 3436 302c 2d31 3231 3520 3135 3035  C1460,-1215 1505
+00002220: 2e34 372c 2d31 3138 312e 3434 2031 3533  .47,-1181.44 153
+00002230: 372e 3133 2c2d 3131 3538 2e30 3622 2f3e  7.13,-1158.06"/>
+00002240: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00002250: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+00002260: 6c61 636b 2220 706f 696e 7473 3d22 3135  lack" points="15
+00002270: 3338 2e39 2c2d 3131 3631 2e31 3120 3135  38.9,-1161.11 15
+00002280: 3434 2e38 362c 2d31 3135 322e 3335 2031  44.86,-1152.35 1
+00002290: 3533 342e 3734 2c2d 3131 3535 2e34 3820  534.74,-1155.48 
+000022a0: 3135 3338 2e39 2c2d 3131 3631 2e31 3122  1538.9,-1161.11"
+000022b0: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+000022c0: 6368 6f72 3d22 6d69 6464 6c65 2220 783d  chor="middle" x=
+000022d0: 2231 3436 362e 3522 2079 3d22 2d31 3231  "1466.5" y="-121
+000022e0: 342e 3822 2066 6f6e 742d 6661 6d69 6c79  4.8" font-family
+000022f0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00002300: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00002310: 3e4a 613c 2f74 6578 743e 0a3c 2f67 3e0a  >Ja</text>.</g>.
+00002320: 3c21 2d2d 2033 202d 2d3e 0a3c 6720 6964  <!-- 3 -->.<g id
+00002330: 3d22 6e6f 6465 3422 2063 6c61 7373 3d22  ="node4" class="
+00002340: 6e6f 6465 223e 0a3c 7469 746c 653e 333c  node">.<title>3<
+00002350: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
+00002360: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
+00002370: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+00002380: 3133 3336 2c2d 3939 3843 3133 3336 2c2d  1336,-998C1336,-
+00002390: 3939 3820 3839 392c 2d39 3938 2038 3939  998 899,-998 899
+000023a0: 2c2d 3939 3820 3839 332c 2d39 3938 2038  ,-998 893,-998 8
+000023b0: 3837 2c2d 3939 3220 3838 372c 2d39 3836  87,-992 887,-986
+000023c0: 2038 3837 2c2d 3938 3620 3838 372c 2d39   887,-986 887,-9
+000023d0: 3634 2038 3837 2c2d 3936 3420 3838 372c  64 887,-964 887,
+000023e0: 2d39 3538 2038 3933 2c2d 3935 3220 3839  -958 893,-952 89
+000023f0: 392c 2d39 3532 2038 3939 2c2d 3935 3220  9,-952 899,-952 
+00002400: 3133 3336 2c2d 3935 3220 3133 3336 2c2d  1336,-952 1336,-
+00002410: 3935 3220 3133 3432 2c2d 3935 3220 3133  952 1342,-952 13
+00002420: 3438 2c2d 3935 3820 3133 3438 2c2d 3936  48,-958 1348,-96
+00002430: 3420 3133 3438 2c2d 3936 3420 3133 3438  4 1348,-964 1348
+00002440: 2c2d 3938 3620 3133 3438 2c2d 3938 3620  ,-986 1348,-986 
+00002450: 3133 3438 2c2d 3939 3220 3133 3432 2c2d  1348,-992 1342,-
+00002460: 3939 3820 3133 3336 2c2d 3939 3822 2f3e  998 1336,-998"/>
+00002470: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00002480: 6f72 3d22 7374 6172 7422 2078 3d22 3930  or="start" x="90
+00002490: 3122 2079 3d22 2d39 3738 2e38 2220 666f  1" y="-978.8" fo
+000024a0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000024b0: 2c73 6572 6966 2220 666f 6e74 2d77 6569  ,serif" font-wei
+000024c0: 6768 743d 2262 6f6c 6422 2066 6f6e 742d  ght="bold" font-
+000024d0: 7369 7a65 3d22 3134 2e30 3022 3e33 3a20  size="14.00">3: 
+000024e0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+000024f0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00002500: 2220 783d 2239 3231 2220 793d 222d 3937  " x="921" y="-97
+00002510: 382e 3822 2066 6f6e 742d 6661 6d69 6c79  8.8" font-family
+00002520: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00002530: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00002540: 3e4c 6965 6774 2064 6173 2041 626d 656c  >Liegt das Abmel
+00002550: 6465 6461 7475 6d20 6d69 6e64 6573 7465  dedatum mindeste
+00002560: 6e73 2065 696e 656e 2054 6167 206e 6163  ns einen Tag nac
+00002570: 6820 6465 6d3c 2f74 6578 743e 0a3c 7465  h dem</text>.<te
+00002580: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00002590: 7374 6172 7422 2078 3d22 3930 3122 2079  start" x="901" y
+000025a0: 3d22 2d39 3634 2e38 2220 666f 6e74 2d66  ="-964.8" font-f
+000025b0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+000025c0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+000025d0: 342e 3030 223e 4569 6e67 616e 6773 6461  4.00">Eingangsda
+000025e0: 7475 6d20 6465 7220 4162 6d65 6c64 756e  tum der Abmeldun
+000025f0: 673f 3c2f 7465 7874 3e0a 3c2f 673e 0a3c  g?</text>.</g>.<
+00002600: 212d 2d20 3226 2334 353b 2667 743b 3320  !-- 2&#45;&gt;3 
+00002610: 2d2d 3e0a 3c67 2069 643d 2265 6467 6534  -->.<g id="edge4
+00002620: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
+00002630: 3c74 6974 6c65 3e32 2d26 6774 3b33 3c2f  <title>2-&gt;3</
+00002640: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+00002650: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00002660: 2262 6c61 636b 2220 643d 224d 3131 3134  "black" d="M1114
+00002670: 2e30 362c 2d31 3036 322e 3532 4331 3131  .06,-1062.52C111
+00002680: 342e 3739 2c2d 3130 3434 2e32 3620 3131  4.79,-1044.26 11
+00002690: 3135 2e35 352c 2d31 3032 352e 3131 2031  15.55,-1025.11 1
+000026a0: 3131 362e 3137 2c2d 3130 3039 2e34 3822  116.17,-1009.48"
+000026b0: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
+000026c0: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+000026d0: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+000026e0: 3131 3139 2e36 352c 2d31 3030 392e 3934  1119.65,-1009.94
+000026f0: 2031 3131 362e 3535 2c2d 3939 392e 3820   1116.55,-999.8 
+00002700: 3131 3132 2e36 362c 2d31 3030 392e 3636  1112.66,-1009.66
+00002710: 2031 3131 392e 3635 2c2d 3130 3039 2e39   1119.65,-1009.9
+00002720: 3422 2f3e 0a3c 7465 7874 2074 6578 742d  4"/>.<text text-
+00002730: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
+00002740: 783d 2231 3132 312e 3522 2079 3d22 2d31  x="1121.5" y="-1
+00002750: 3033 332e 3822 2066 6f6e 742d 6661 6d69  033.8" font-fami
+00002760: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00002770: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00002780: 3022 3e4a 613c 2f74 6578 743e 0a3c 2f67  0">Ja</text>.</g
+00002790: 3e0a 3c21 2d2d 2036 202d 2d3e 0a3c 6720  >.<!-- 6 -->.<g 
+000027a0: 6964 3d22 6e6f 6465 3922 2063 6c61 7373  id="node9" class
+000027b0: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
+000027c0: 363c 2f74 6974 6c65 3e0a 3c70 6174 6820  6</title>.<path 
+000027d0: 6669 6c6c 3d22 2337 6161 6238 6122 2073  fill="#7aab8a" s
+000027e0: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
+000027f0: 224d 3835 372c 2d31 3030 3543 3835 372c  "M857,-1005C857,
+00002800: 2d31 3030 3520 3433 362c 2d31 3030 3520  -1005 436,-1005 
+00002810: 3433 362c 2d31 3030 3520 3433 302c 2d31  436,-1005 430,-1
+00002820: 3030 3520 3432 342c 2d39 3939 2034 3234  005 424,-999 424
+00002830: 2c2d 3939 3320 3432 342c 2d39 3933 2034  ,-993 424,-993 4
+00002840: 3234 2c2d 3935 3720 3432 342c 2d39 3537  24,-957 424,-957
+00002850: 2034 3234 2c2d 3935 3120 3433 302c 2d39   424,-951 430,-9
+00002860: 3435 2034 3336 2c2d 3934 3520 3433 362c  45 436,-945 436,
+00002870: 2d39 3435 2038 3537 2c2d 3934 3520 3835  -945 857,-945 85
+00002880: 372c 2d39 3435 2038 3633 2c2d 3934 3520  7,-945 863,-945 
+00002890: 3836 392c 2d39 3531 2038 3639 2c2d 3935  869,-951 869,-95
+000028a0: 3720 3836 392c 2d39 3537 2038 3639 2c2d  7 869,-957 869,-
+000028b0: 3939 3320 3836 392c 2d39 3933 2038 3639  993 869,-993 869
+000028c0: 2c2d 3939 3920 3836 332c 2d31 3030 3520  ,-999 863,-1005 
+000028d0: 3835 372c 2d31 3030 3522 2f3e 0a3c 7465  857,-1005"/>.<te
+000028e0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000028f0: 7374 6172 7422 2078 3d22 3433 3822 2079  start" x="438" y
+00002900: 3d22 2d39 3835 2e38 2220 666f 6e74 2d66  ="-985.8" font-f
+00002910: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00002920: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
+00002930: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
+00002940: 3d22 3134 2e30 3022 3e36 3a20 3c2f 7465  ="14.00">6: </te
+00002950: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00002960: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00002970: 2234 3538 2220 793d 222d 3938 352e 3822  "458" y="-985.8"
+00002980: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00002990: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+000029a0: 7369 7a65 3d22 3134 2e30 3022 3e48 616e  size="14.00">Han
+000029b0: 6465 6c74 2065 7320 7369 6368 2075 6d20  delt es sich um 
+000029c0: 6569 6e65 204d 6172 6b74 6c6f 6b61 7469  eine Marktlokati
+000029d0: 6f6e 2c20 6465 7265 6e20 4d65 7373 2d3c  on, deren Mess-<
+000029e0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+000029f0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00002a00: 2078 3d22 3433 3822 2079 3d22 2d39 3731   x="438" y="-971
+00002a10: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00002a20: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00002a30: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00002a40: 6c6f 6b61 7469 6f6e 656e 2076 6f6c 6c73  lokationen volls
+00002a50: 7426 2332 3238 3b6e 6469 6720 6d69 7420  t&#228;ndig mit 
+00002a60: 694d 5320 6175 7367 6573 7461 7474 6574  iMS ausgestattet
+00002a70: 2073 696e 6420 6f64 6572 2f75 6e64 3c2f   sind oder/und</
+00002a80: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00002a90: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00002aa0: 783d 2234 3338 2220 793d 222d 3935 372e  x="438" y="-957.
+00002ab0: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00002ac0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00002ad0: 742d 7369 7a65 3d22 3134 2e30 3022 3e64  t-size="14.00">d
+00002ae0: 6572 656e 2050 726f 676e 6f73 6567 7275  eren Prognosegru
+00002af0: 6e64 6c61 6765 2061 7566 2042 6173 6973  ndlage auf Basis
+00002b00: 2076 6f6e 2057 6572 7465 6e20 6572 666f   von Werten erfo
+00002b10: 6c67 743f 3c2f 7465 7874 3e0a 3c2f 673e  lgt?</text>.</g>
+00002b20: 0a3c 212d 2d20 3226 2334 353b 2667 743b  .<!-- 2&#45;&gt;
+00002b30: 3620 2d2d 3e0a 3c67 2069 643d 2265 6467  6 -->.<g id="edg
+00002b40: 6535 2220 636c 6173 733d 2265 6467 6522  e5" class="edge"
+00002b50: 3e0a 3c74 6974 6c65 3e32 2d26 6774 3b36  >.<title>2-&gt;6
+00002b60: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+00002b70: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00002b80: 653d 2262 6c61 636b 2220 643d 224d 3931  e="black" d="M91
+00002b90: 322e 3935 2c2d 3130 3632 2e35 3243 3835  2.95,-1062.52C85
+00002ba0: 362e 3034 2c2d 3130 3434 2e30 3420 3739  6.04,-1044.04 79
+00002bb0: 362e 3335 2c2d 3130 3234 2e36 3620 3734  6.35,-1024.66 74
+00002bc0: 372e 3933 2c2d 3130 3038 2e39 3422 2f3e  7.93,-1008.94"/>
+00002bd0: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00002be0: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+00002bf0: 6c61 636b 2220 706f 696e 7473 3d22 3734  lack" points="74
+00002c00: 392e 3137 2c2d 3130 3035 2e36 3620 3733  9.17,-1005.66 73
+00002c10: 382e 3538 2c2d 3130 3035 2e39 2037 3437  8.58,-1005.9 747
+00002c20: 2e30 312c 2d31 3031 322e 3332 2037 3439  .01,-1012.32 749
+00002c30: 2e31 372c 2d31 3030 352e 3636 222f 3e0a  .17,-1005.66"/>.
+00002c40: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00002c50: 723d 226d 6964 646c 6522 2078 3d22 3836  r="middle" x="86
+00002c60: 372e 3522 2079 3d22 2d31 3033 332e 3822  7.5" y="-1033.8"
+00002c70: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00002c80: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00002c90: 7369 7a65 3d22 3134 2e30 3022 3e4e 6569  size="14.00">Nei
+00002ca0: 6e3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  n</text>.</g>.<!
+00002cb0: 2d2d 2041 3031 202d 2d3e 0a3c 6720 6964  -- A01 -->.<g id
+00002cc0: 3d22 6e6f 6465 3522 2063 6c61 7373 3d22  ="node5" class="
+00002cd0: 6e6f 6465 223e 0a3c 7469 746c 653e 4130  node">.<title>A0
+00002ce0: 313c 2f74 6974 6c65 3e0a 3c70 6f6c 7967  1</title>.<polyg
+00002cf0: 6f6e 2066 696c 6c3d 2223 6366 6239 3836  on fill="#cfb986
+00002d00: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00002d10: 2070 6f69 6e74 733d 2231 3235 392c 2d38   points="1259,-8
+00002d20: 3837 2039 3534 2c2d 3838 3720 3935 342c  87 954,-887 954,
+00002d30: 2d38 3031 2031 3235 392c 2d38 3031 2031  -801 1259,-801 1
+00002d40: 3235 392c 2d38 3837 222f 3e0a 3c74 6578  259,-887"/>.<tex
+00002d50: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00002d60: 7461 7274 2220 783d 2231 3039 3122 2079  tart" x="1091" y
+00002d70: 3d22 2d38 3730 2e38 2220 666f 6e74 2d66  ="-870.8" font-f
+00002d80: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00002d90: 6966 2220 666f 6e74 2d77 6569 6768 743d  if" font-weight=
+00002da0: 2262 6f6c 6422 2066 6f6e 742d 7369 7a65  "bold" font-size
+00002db0: 3d22 3134 2e30 3022 3e41 3031 3c2f 7465  ="14.00">A01</te
+00002dc0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00002dd0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00002de0: 2239 3636 2220 793d 222d 3835 382e 3422  "966" y="-858.4"
+00002df0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00002e00: 6d65 732c 7365 7269 6622 2074 6578 742d  mes,serif" text-
+00002e10: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00002e20: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00002e30: 3d22 3132 2e30 3022 3e48 696e 7765 6973  ="12.00">Hinweis
+00002e40: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00002e50: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00002e60: 7422 2078 3d22 3936 3622 2079 3d22 2d38  t" x="966" y="-8
+00002e70: 3436 2e34 2220 666f 6e74 2d66 616d 696c  46.4" font-famil
+00002e80: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00002e90: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
+00002ea0: 223e 436c 7573 7465 723a 2041 626c 6568  ">Cluster: Ableh
+00002eb0: 6e75 6e67 3c2f 7465 7874 3e0a 3c74 6578  nung</text>.<tex
+00002ec0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00002ed0: 7461 7274 2220 783d 2239 3636 2220 793d  tart" x="966" y=
+00002ee0: 222d 3833 342e 3422 2066 6f6e 742d 6661  "-834.4" font-fa
+00002ef0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00002f00: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
+00002f10: 2e30 3022 3e46 7269 7374 2623 3235 323b  .00">Frist&#252;
+00002f20: 6265 7273 6368 7265 6974 756e 6720 6265  berschreitung be
+00002f30: 6920 4175 6668 6562 756e 6720 6569 6e65  i Aufhebung eine
+00002f40: 7220 7a75 2d3c 2f74 6578 743e 0a3c 7465  r zu-</text>.<te
+00002f50: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00002f60: 7374 6172 7422 2078 3d22 3936 3622 2079  start" x="966" y
+00002f70: 3d22 2d38 3232 2e34 2220 666f 6e74 2d66  ="-822.4" font-f
+00002f80: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00002f90: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00002fa0: 322e 3030 223e 6b26 2332 3532 3b6e 6674  2.00">k&#252;nft
+00002fb0: 6967 656e 205a 756f 7264 6e75 6e67 2077  igen Zuordnung w
+00002fc0: 6567 656e 2041 7573 7a75 6720 6f64 6572  egen Auszug oder
+00002fd0: 2053 7469 6c6c 2d3c 2f74 6578 743e 0a3c   Still-</text>.<
+00002fe0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00002ff0: 3d22 7374 6172 7422 2078 3d22 3936 3622  ="start" x="966"
+00003000: 2079 3d22 2d38 3130 2e34 2220 666f 6e74   y="-810.4" font
+00003010: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00003020: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00003030: 2231 322e 3030 223e 6c65 6775 6e67 2e3c  "12.00">legung.<
+00003040: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+00003050: 2033 2623 3435 3b26 6774 3b41 3031 202d   3&#45;&gt;A01 -
+00003060: 2d3e 0a3c 6720 6964 3d22 6564 6765 3622  ->.<g id="edge6"
+00003070: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
+00003080: 7469 746c 653e 332d 2667 743b 4130 313c  title>3-&gt;A01<
+00003090: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
+000030a0: 6c6c 3d22 6e6f 6e65 2220 7374 726f 6b65  ll="none" stroke
+000030b0: 3d22 626c 6163 6b22 2064 3d22 4d31 3131  ="black" d="M111
+000030c0: 352e 3538 2c2d 3935 312e 3533 4331 3131  5.58,-951.53C111
+000030d0: 342e 3334 2c2d 3933 362e 3838 2031 3131  4.34,-936.88 111
+000030e0: 322e 3635 2c2d 3931 372e 3132 2031 3131  2.65,-917.12 111
+000030f0: 312e 3037 2c2d 3839 382e 3539 222f 3e0a  1.07,-898.59"/>.
+00003100: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
+00003110: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
+00003120: 6163 6b22 2070 6f69 6e74 733d 2231 3131  ack" points="111
+00003130: 342e 3537 2c2d 3839 382e 3434 2031 3131  4.57,-898.44 111
+00003140: 302e 3233 2c2d 3838 382e 3738 2031 3130  0.23,-888.78 110
+00003150: 372e 362c 2d38 3939 2e30 3420 3131 3134  7.6,-899.04 1114
+00003160: 2e35 372c 2d38 3938 2e34 3422 2f3e 0a3c  .57,-898.44"/>.<
+00003170: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00003180: 3d22 6d69 6464 6c65 2220 783d 2231 3132  ="middle" x="112
+00003190: 392e 3522 2079 3d22 2d39 3038 2e38 2220  9.5" y="-908.8" 
+000031a0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+000031b0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+000031c0: 697a 653d 2231 342e 3030 223e 4e65 696e  ize="14.00">Nein
+000031d0: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+000031e0: 2d20 3920 2d2d 3e0a 3c67 2069 643d 226e  - 9 -->.<g id="n
+000031f0: 6f64 6531 3422 2063 6c61 7373 3d22 6e6f  ode14" class="no
+00003200: 6465 223e 0a3c 7469 746c 653e 393c 2f74  de">.<title>9</t
+00003210: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
+00003220: 3d22 2337 6161 6238 6122 2073 7472 6f6b  ="#7aab8a" strok
+00003230: 653d 2262 6c61 636b 2220 643d 224d 3138  e="black" d="M18
+00003240: 3133 2c2d 3837 3443 3138 3133 2c2d 3837  13,-874C1813,-87
+00003250: 3420 3133 3630 2c2d 3837 3420 3133 3630  4 1360,-874 1360
+00003260: 2c2d 3837 3420 3133 3534 2c2d 3837 3420  ,-874 1354,-874 
+00003270: 3133 3438 2c2d 3836 3820 3133 3438 2c2d  1348,-868 1348,-
+00003280: 3836 3220 3133 3438 2c2d 3836 3220 3133  862 1348,-862 13
+00003290: 3438 2c2d 3832 3620 3133 3438 2c2d 3832  48,-826 1348,-82
+000032a0: 3620 3133 3438 2c2d 3832 3020 3133 3534  6 1348,-820 1354
+000032b0: 2c2d 3831 3420 3133 3630 2c2d 3831 3420  ,-814 1360,-814 
+000032c0: 3133 3630 2c2d 3831 3420 3138 3133 2c2d  1360,-814 1813,-
+000032d0: 3831 3420 3138 3133 2c2d 3831 3420 3138  814 1813,-814 18
+000032e0: 3139 2c2d 3831 3420 3138 3235 2c2d 3832  19,-814 1825,-82
+000032f0: 3020 3138 3235 2c2d 3832 3620 3138 3235  0 1825,-826 1825
+00003300: 2c2d 3832 3620 3138 3235 2c2d 3836 3220  ,-826 1825,-862 
+00003310: 3138 3235 2c2d 3836 3220 3138 3235 2c2d  1825,-862 1825,-
+00003320: 3836 3820 3138 3139 2c2d 3837 3420 3138  868 1819,-874 18
+00003330: 3133 2c2d 3837 3422 2f3e 0a3c 7465 7874  13,-874"/>.<text
+00003340: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00003350: 6172 7422 2078 3d22 3133 3632 2220 793d  art" x="1362" y=
+00003360: 222d 3835 342e 3822 2066 6f6e 742d 6661  "-854.8" font-fa
+00003370: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00003380: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+00003390: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+000033a0: 2231 342e 3030 223e 393a 203c 2f74 6578  "14.00">9: </tex
+000033b0: 743e 0a3c 7465 7874 2074 6578 742d 616e  t>.<text text-an
+000033c0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+000033d0: 3133 3832 2220 793d 222d 3835 342e 3822  1382" y="-854.8"
+000033e0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+000033f0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00003400: 7369 7a65 3d22 3134 2e30 3022 3e45 7266  size="14.00">Erf
+00003410: 6f6c 6774 2064 6965 2041 7566 6865 6275  olgt die Aufhebu
+00003420: 6e67 2065 696e 6572 207a 756b 2623 3235  ng einer zuk&#25
+00003430: 323b 6e66 7469 6765 6e20 5a75 6f72 646e  2;nftigen Zuordn
+00003440: 756e 6720 7a75 2064 656d 3c2f 7465 7874  ung zu dem</text
+00003450: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00003460: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+00003470: 3336 3222 2079 3d22 2d38 3430 2e38 2220  362" y="-840.8" 
+00003480: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00003490: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+000034a0: 697a 653d 2231 342e 3030 223e 676c 6569  ize="14.00">glei
+000034b0: 6368 656e 2044 6174 756d 2028 5a65 6974  chen Datum (Zeit
+000034c0: 7075 6e6b 7429 2c20 7765 6c63 6865 7220  punkt), welcher 
+000034d0: 6465 6d20 4c69 6566 6572 616e 7465 6e20  dem Lieferanten 
+000034e0: 696d 3c2f 7465 7874 3e0a 3c74 6578 7420  im</text>.<text 
+000034f0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00003500: 7274 2220 783d 2231 3336 3222 2079 3d22  rt" x="1362" y="
+00003510: 2d38 3236 2e38 2220 666f 6e74 2d66 616d  -826.8" font-fam
+00003520: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00003530: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00003540: 3030 223e 4c69 6566 6572 6265 6769 6e6e  00">Lieferbeginn
+00003550: 2062 6573 7426 2332 3238 3b74 6967 7420   best&#228;tigt 
+00003560: 7775 7264 653f 3c2f 7465 7874 3e0a 3c2f  wurde?</text>.</
+00003570: 673e 0a3c 212d 2d20 3326 2334 353b 2667  g>.<!-- 3&#45;&g
+00003580: 743b 3920 2d2d 3e0a 3c67 2069 643d 2265  t;9 -->.<g id="e
+00003590: 6467 6537 2220 636c 6173 733d 2265 6467  dge7" class="edg
+000035a0: 6522 3e0a 3c74 6974 6c65 3e33 2d26 6774  e">.<title>3-&gt
+000035b0: 3b39 3c2f 7469 746c 653e 0a3c 7061 7468  ;9</title>.<path
+000035c0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+000035d0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+000035e0: 3131 3939 2e31 392c 2d39 3531 2e35 3343  1199.19,-951.53C
+000035f0: 3132 3733 2e36 322c 2d39 3331 2e30 3620  1273.62,-931.06 
+00003600: 3133 3834 2e34 312c 2d39 3030 2e35 3920  1384.41,-900.59 
+00003610: 3134 3638 2e34 352c 2d38 3737 2e34 3722  1468.45,-877.47"
+00003620: 2f3e 0a3c 706f 6c79 676f 6e20 6669 6c6c  />.<polygon fill
+00003630: 3d22 626c 6163 6b22 2073 7472 6f6b 653d  ="black" stroke=
+00003640: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+00003650: 3134 3639 2e31 372c 2d38 3830 2e39 2031  1469.17,-880.9 1
+00003660: 3437 372e 3838 2c2d 3837 342e 3838 2031  477.88,-874.88 1
+00003670: 3436 372e 3331 2c2d 3837 342e 3135 2031  467.31,-874.15 1
+00003680: 3436 392e 3137 2c2d 3838 302e 3922 2f3e  469.17,-880.9"/>
+00003690: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+000036a0: 6f72 3d22 6d69 6464 6c65 2220 783d 2231  or="middle" x="1
+000036b0: 3337 322e 3522 2079 3d22 2d39 3038 2e38  372.5" y="-908.8
+000036c0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+000036d0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+000036e0: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
+000036f0: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00003700: 2d20 4130 3220 2d2d 3e0a 3c67 2069 643d  - A02 -->.<g id=
+00003710: 226e 6f64 6537 2220 636c 6173 733d 226e  "node7" class="n
+00003720: 6f64 6522 3e0a 3c74 6974 6c65 3e41 3032  ode">.<title>A02
+00003730: 3c2f 7469 746c 653e 0a3c 706f 6c79 676f  </title>.<polygo
+00003740: 6e20 6669 6c6c 3d22 2363 6662 3938 3622  n fill="#cfb986"
+00003750: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00003760: 706f 696e 7473 3d22 3231 3231 2e35 2c2d  points="2121.5,-
+00003770: 3130 3132 2031 3739 392e 352c 2d31 3031  1012 1799.5,-101
+00003780: 3220 3137 3939 2e35 2c2d 3933 3820 3231  2 1799.5,-938 21
+00003790: 3231 2e35 2c2d 3933 3820 3231 3231 2e35  21.5,-938 2121.5
+000037a0: 2c2d 3130 3132 222f 3e0a 3c74 6578 7420  ,-1012"/>.<text 
+000037b0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+000037c0: 7274 2220 783d 2231 3934 3522 2079 3d22  rt" x="1945" y="
+000037d0: 2d39 3935 2e38 2220 666f 6e74 2d66 616d  -995.8" font-fam
+000037e0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+000037f0: 2220 666f 6e74 2d77 6569 6768 743d 2262  " font-weight="b
+00003800: 6f6c 6422 2066 6f6e 742d 7369 7a65 3d22  old" font-size="
+00003810: 3134 2e30 3022 3e41 3032 3c2f 7465 7874  14.00">A02</text
+00003820: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00003830: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+00003840: 3831 312e 3522 2079 3d22 2d39 3833 2e34  811.5" y="-983.4
+00003850: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00003860: 696d 6573 2c73 6572 6966 2220 7465 7874  imes,serif" text
+00003870: 2d64 6563 6f72 6174 696f 6e3d 2275 6e64  -decoration="und
+00003880: 6572 6c69 6e65 2220 666f 6e74 2d73 697a  erline" font-siz
+00003890: 653d 2231 322e 3030 223e 4869 6e77 6569  e="12.00">Hinwei
+000038a0: 733a 3c2f 7465 7874 3e0a 3c74 6578 7420  s:</text>.<text 
+000038b0: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+000038c0: 7274 2220 783d 2231 3831 312e 3522 2079  rt" x="1811.5" y
+000038d0: 3d22 2d39 3731 2e34 2220 666f 6e74 2d66  ="-971.4" font-f
+000038e0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+000038f0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00003900: 322e 3030 223e 436c 7573 7465 723a 2041  2.00">Cluster: A
+00003910: 626c 6568 6e75 6e67 3c2f 7465 7874 3e0a  blehnung</text>.
+00003920: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00003930: 723d 2273 7461 7274 2220 783d 2231 3831  r="start" x="181
+00003940: 312e 3522 2079 3d22 2d39 3539 2e34 2220  1.5" y="-959.4" 
+00003950: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00003960: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00003970: 697a 653d 2231 322e 3030 223e 4672 6973  ize="12.00">Fris
+00003980: 7426 2332 3532 3b62 6572 7363 6872 6569  t&#252;berschrei
+00003990: 7475 6e67 2062 6569 2054 7261 6e73 616b  tung bei Transak
+000039a0: 7469 6f6e 7367 7226 2332 3532 3b6e 6465  tionsgr&#252;nde
+000039b0: 6e20 6626 2332 3532 3b72 3c2f 7465 7874  n f&#252;r</text
+000039c0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+000039d0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+000039e0: 3831 312e 3522 2079 3d22 2d39 3437 2e34  811.5" y="-947.4
+000039f0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00003a00: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00003a10: 2d73 697a 653d 2231 322e 3030 223e 6569  -size="12.00">ei
+00003a20: 6e65 2041 626d 656c 6475 6e67 2069 6e20  ne Abmeldung in 
+00003a30: 6465 7220 5a75 6b75 6e66 742e 3c2f 7465  der Zukunft.</te
+00003a40: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3426  xt>.</g>.<!-- 4&
+00003a50: 2334 353b 2667 743b 4130 3220 2d2d 3e0a  #45;&gt;A02 -->.
+00003a60: 3c67 2069 643d 2265 6467 6538 2220 636c  <g id="edge8" cl
+00003a70: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00003a80: 6c65 3e34 2d26 6774 3b41 3032 3c2f 7469  le>4-&gt;A02</ti
+00003a90: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00003aa0: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00003ab0: 6c61 636b 2220 643d 224d 3136 3333 2e35  lack" d="M1633.5
+00003ac0: 372c 2d31 3130 342e 3536 4331 3639 322e  7,-1104.56C1692.
+00003ad0: 3432 2c2d 3130 3831 2e34 3220 3137 3835  42,-1081.42 1785
+00003ae0: 2e34 352c 2d31 3034 342e 3833 2031 3835  .45,-1044.83 185
+00003af0: 372e 3235 2c2d 3130 3136 2e36 222f 3e0a  7.25,-1016.6"/>.
+00003b00: 3c70 6f6c 7967 6f6e 2066 696c 6c3d 2262  <polygon fill="b
+00003b10: 6c61 636b 2220 7374 726f 6b65 3d22 626c  lack" stroke="bl
+00003b20: 6163 6b22 2070 6f69 6e74 733d 2231 3835  ack" points="185
+00003b30: 382e 3235 2c2d 3130 3139 2e39 3720 3138  8.25,-1019.97 18
+00003b40: 3636 2e32 382c 2d31 3031 332e 3035 2031  66.28,-1013.05 1
+00003b50: 3835 352e 3639 2c2d 3130 3133 2e34 3520  855.69,-1013.45 
+00003b60: 3138 3538 2e32 352c 2d31 3031 392e 3937  1858.25,-1019.97
+00003b70: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+00003b80: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
+00003b90: 3d22 3138 3330 2e35 2220 793d 222d 3130  ="1830.5" y="-10
+00003ba0: 3333 2e38 2220 666f 6e74 2d66 616d 696c  33.8" font-famil
+00003bb0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00003bc0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00003bd0: 223e 4e65 696e 3c2f 7465 7874 3e0a 3c2f  ">Nein</text>.</
+00003be0: 673e 0a3c 212d 2d20 3520 2d2d 3e0a 3c67  g>.<!-- 5 -->.<g
+00003bf0: 2069 643d 226e 6f64 6538 2220 636c 6173   id="node8" clas
+00003c00: 733d 226e 6f64 6522 3e0a 3c74 6974 6c65  s="node">.<title
+00003c10: 3e35 3c2f 7469 746c 653e 0a3c 7061 7468  >5</title>.<path
+00003c20: 2066 696c 6c3d 2223 3761 6162 3861 2220   fill="#7aab8a" 
+00003c30: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
+00003c40: 3d22 4d31 3736 392e 352c 2d31 3031 3243  ="M1769.5,-1012C
+00003c50: 3137 3639 2e35 2c2d 3130 3132 2031 3337  1769.5,-1012 137
+00003c60: 392e 352c 2d31 3031 3220 3133 3739 2e35  9.5,-1012 1379.5
+00003c70: 2c2d 3130 3132 2031 3337 332e 352c 2d31  ,-1012 1373.5,-1
+00003c80: 3031 3220 3133 3637 2e35 2c2d 3130 3036  012 1367.5,-1006
+00003c90: 2031 3336 372e 352c 2d31 3030 3020 3133   1367.5,-1000 13
+00003ca0: 3637 2e35 2c2d 3130 3030 2031 3336 372e  67.5,-1000 1367.
+00003cb0: 352c 2d39 3530 2031 3336 372e 352c 2d39  5,-950 1367.5,-9
+00003cc0: 3530 2031 3336 372e 352c 2d39 3434 2031  50 1367.5,-944 1
+00003cd0: 3337 332e 352c 2d39 3338 2031 3337 392e  373.5,-938 1379.
+00003ce0: 352c 2d39 3338 2031 3337 392e 352c 2d39  5,-938 1379.5,-9
+00003cf0: 3338 2031 3736 392e 352c 2d39 3338 2031  38 1769.5,-938 1
+00003d00: 3736 392e 352c 2d39 3338 2031 3737 352e  769.5,-938 1775.
+00003d10: 352c 2d39 3338 2031 3738 312e 352c 2d39  5,-938 1781.5,-9
+00003d20: 3434 2031 3738 312e 352c 2d39 3530 2031  44 1781.5,-950 1
+00003d30: 3738 312e 352c 2d39 3530 2031 3738 312e  781.5,-950 1781.
+00003d40: 352c 2d31 3030 3020 3137 3831 2e35 2c2d  5,-1000 1781.5,-
+00003d50: 3130 3030 2031 3738 312e 352c 2d31 3030  1000 1781.5,-100
+00003d60: 3620 3137 3735 2e35 2c2d 3130 3132 2031  6 1775.5,-1012 1
+00003d70: 3736 392e 352c 2d31 3031 3222 2f3e 0a3c  769.5,-1012"/>.<
+00003d80: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00003d90: 3d22 7374 6172 7422 2078 3d22 3133 3831  ="start" x="1381
+00003da0: 2e35 2220 793d 222d 3939 322e 3822 2066  .5" y="-992.8" f
+00003db0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00003dc0: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
+00003dd0: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
+00003de0: 2d73 697a 653d 2231 342e 3030 223e 353a  -size="14.00">5:
+00003df0: 203c 2f74 6578 743e 0a3c 7465 7874 2074   </text>.<text t
+00003e00: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00003e10: 7422 2078 3d22 3134 3031 2e35 2220 793d  t" x="1401.5" y=
+00003e20: 222d 3939 322e 3822 2066 6f6e 742d 6661  "-992.8" font-fa
+00003e30: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00003e40: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+00003e50: 2e30 3022 3e4c 6965 6774 2064 6572 2054  .00">Liegt der T
+00003e60: 7261 6e73 616b 7469 6f6e 7367 7275 6e64  ransaktionsgrund
+00003e70: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+00003e80: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+00003e90: 2220 783d 2231 3338 312e 3522 2079 3d22  " x="1381.5" y="
+00003ea0: 2d39 3738 2e38 2220 666f 6e74 2d66 616d  -978.8" font-fam
+00003eb0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00003ec0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00003ed0: 3030 223e 2623 3832 3236 3b20 4175 6668  00">&#8226; Aufh
+00003ee0: 6562 756e 6720 6569 6e65 7220 7a75 6b26  ebung einer zuk&
+00003ef0: 2332 3532 3b6e 6674 6967 656e 205a 756f  #252;nftigen Zuo
+00003f00: 7264 6e75 6e67 2077 6567 656e 2061 7566  rdnung wegen auf
+00003f10: 2d3c 2f74 6578 743e 0a3c 7465 7874 2074  -</text>.<text t
+00003f20: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00003f30: 7422 2078 3d22 3133 3831 2e35 2220 793d  t" x="1381.5" y=
+00003f40: 222d 3936 342e 3822 2066 6f6e 742d 6661  "-964.8" font-fa
+00003f50: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00003f60: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+00003f70: 2e30 3022 3e67 6568 6f62 656e 656d 2056  .00">gehobenem V
+00003f80: 6572 7472 6167 7376 6572 6826 2332 3238  ertragsverh&#228
+00003f90: 3b6c 746e 6973 3c2f 7465 7874 3e0a 3c74  ;ltnis</text>.<t
+00003fa0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00003fb0: 2273 7461 7274 2220 783d 2231 3338 312e  "start" x="1381.
+00003fc0: 3522 2079 3d22 2d39 3530 2e38 2220 666f  5" y="-950.8" fo
+00003fd0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00003fe0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00003ff0: 653d 2231 342e 3030 223e 766f 723f 3c2f  e="14.00">vor?</
+00004000: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
+00004010: 3426 2334 353b 2667 743b 3520 2d2d 3e0a  4&#45;&gt;5 -->.
+00004020: 3c67 2069 643d 2265 6467 6539 2220 636c  <g id="edge9" cl
+00004030: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00004040: 6c65 3e34 2d26 6774 3b35 3c2f 7469 746c  le>4-&gt;5</titl
+00004050: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
+00004060: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+00004070: 636b 2220 643d 224d 3135 3736 2e32 2c2d  ck" d="M1576.2,-
+00004080: 3131 3034 2e37 3243 3135 3735 2e39 322c  1104.72C1575.92,
+00004090: 2d31 3038 332e 3437 2031 3537 352e 3439  -1083.47 1575.49
+000040a0: 2c2d 3130 3530 2e37 3820 3135 3735 2e31  ,-1050.78 1575.1
+000040b0: 332c 2d31 3032 332e 3636 222f 3e0a 3c70  3,-1023.66"/>.<p
+000040c0: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
+000040d0: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
+000040e0: 6b22 2070 6f69 6e74 733d 2231 3537 382e  k" points="1578.
+000040f0: 3633 2c2d 3130 3233 2e39 2031 3537 352c  63,-1023.9 1575,
+00004100: 2d31 3031 332e 3935 2031 3537 312e 3634  -1013.95 1571.64
+00004110: 2c2d 3130 3233 2e39 3920 3135 3738 2e36  ,-1023.99 1578.6
+00004120: 332c 2d31 3032 332e 3922 2f3e 0a3c 7465  3,-1023.9"/>.<te
+00004130: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00004140: 6d69 6464 6c65 2220 783d 2231 3538 312e  middle" x="1581.
+00004150: 3522 2079 3d22 2d31 3033 332e 3822 2066  5" y="-1033.8" f
+00004160: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00004170: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00004180: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
+00004190: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2035  ext>.</g>.<!-- 5
+000041a0: 2623 3435 3b26 6774 3b39 202d 2d3e 0a3c  &#45;&gt;9 -->.<
+000041b0: 6720 6964 3d22 6564 6765 3130 2220 636c  g id="edge10" cl
+000041c0: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+000041d0: 6c65 3e35 2d26 6774 3b39 3c2f 7469 746c  le>5-&gt;9</titl
+000041e0: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
+000041f0: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+00004200: 636b 2220 643d 224d 3135 3737 2e38 372c  ck" d="M1577.87,
+00004210: 2d39 3337 2e37 3243 3135 3739 2e33 382c  -937.72C1579.38,
+00004220: 2d39 3231 2e35 2031 3538 312e 3137 2c2d  -921.5 1581.17,-
+00004230: 3930 322e 3320 3135 3832 2e37 322c 2d38  902.3 1582.72,-8
+00004240: 3835 2e36 222f 3e0a 3c70 6f6c 7967 6f6e  85.6"/>.<polygon
+00004250: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00004260: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+00004270: 6e74 733d 2231 3538 362e 3137 2c2d 3838  nts="1586.17,-88
+00004280: 362e 3238 2031 3538 332e 3632 2c2d 3837  6.28 1583.62,-87
+00004290: 3620 3135 3739 2e32 2c2d 3838 352e 3634  6 1579.2,-885.64
+000042a0: 2031 3538 362e 3137 2c2d 3838 362e 3238   1586.17,-886.28
+000042b0: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+000042c0: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
+000042d0: 3d22 3135 3837 2e35 2220 793d 222d 3930  ="1587.5" y="-90
+000042e0: 382e 3822 2066 6f6e 742d 6661 6d69 6c79  8.8" font-family
+000042f0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00004300: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00004310: 3e4a 613c 2f74 6578 743e 0a3c 2f67 3e0a  >Ja</text>.</g>.
+00004320: 3c21 2d2d 2031 3020 2d2d 3e0a 3c67 2069  <!-- 10 -->.<g i
+00004330: 643d 226e 6f64 6531 3622 2063 6c61 7373  d="node16" class
+00004340: 3d22 6e6f 6465 223e 0a3c 7469 746c 653e  ="node">.<title>
+00004350: 3130 3c2f 7469 746c 653e 0a3c 7061 7468  10</title>.<path
+00004360: 2066 696c 6c3d 2223 3761 6162 3861 2220   fill="#7aab8a" 
+00004370: 7374 726f 6b65 3d22 626c 6163 6b22 2064  stroke="black" d
+00004380: 3d22 4d31 3336 352e 352c 2d37 3530 4331  ="M1365.5,-750C1
+00004390: 3336 352e 352c 2d37 3530 2039 3231 2e35  365.5,-750 921.5
+000043a0: 2c2d 3735 3020 3932 312e 352c 2d37 3530  ,-750 921.5,-750
+000043b0: 2039 3135 2e35 2c2d 3735 3020 3930 392e   915.5,-750 909.
+000043c0: 352c 2d37 3434 2039 3039 2e35 2c2d 3733  5,-744 909.5,-73
+000043d0: 3820 3930 392e 352c 2d37 3338 2039 3039  8 909.5,-738 909
+000043e0: 2e35 2c2d 3539 3020 3930 392e 352c 2d35  .5,-590 909.5,-5
+000043f0: 3930 2039 3039 2e35 2c2d 3538 3420 3931  90 909.5,-584 91
+00004400: 352e 352c 2d35 3738 2039 3231 2e35 2c2d  5.5,-578 921.5,-
+00004410: 3537 3820 3932 312e 352c 2d35 3738 2031  578 921.5,-578 1
+00004420: 3336 352e 352c 2d35 3738 2031 3336 352e  365.5,-578 1365.
+00004430: 352c 2d35 3738 2031 3337 312e 352c 2d35  5,-578 1371.5,-5
+00004440: 3738 2031 3337 372e 352c 2d35 3834 2031  78 1377.5,-584 1
+00004450: 3337 372e 352c 2d35 3930 2031 3337 372e  377.5,-590 1377.
+00004460: 352c 2d35 3930 2031 3337 372e 352c 2d37  5,-590 1377.5,-7
+00004470: 3338 2031 3337 372e 352c 2d37 3338 2031  38 1377.5,-738 1
+00004480: 3337 372e 352c 2d37 3434 2031 3337 312e  377.5,-744 1371.
+00004490: 352c 2d37 3530 2031 3336 352e 352c 2d37  5,-750 1365.5,-7
+000044a0: 3530 222f 3e0a 3c74 6578 7420 7465 7874  50"/>.<text text
+000044b0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+000044c0: 783d 2239 3233 2e35 2220 793d 222d 3733  x="923.5" y="-73
+000044d0: 302e 3822 2066 6f6e 742d 6661 6d69 6c79  0.8" font-family
+000044e0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+000044f0: 6f6e 742d 7765 6967 6874 3d22 626f 6c64  ont-weight="bold
+00004500: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00004510: 3030 223e 3130 3a20 3c2f 7465 7874 3e0a  00">10: </text>.
+00004520: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00004530: 723d 2273 7461 7274 2220 783d 2239 3533  r="start" x="953
+00004540: 2e35 2220 793d 222d 3733 302e 3822 2066  .5" y="-730.8" f
+00004550: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00004560: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00004570: 7a65 3d22 3134 2e30 3022 3e57 7572 6465  ze="14.00">Wurde
+00004580: 2064 6965 205a 756f 7264 6e75 6e67 2064   die Zuordnung d
+00004590: 6573 2061 6e66 7261 6765 6e64 656e 204c  es anfragenden L
+000045a0: 6965 6665 7261 6e74 656e 207a 7572 3c2f  ieferanten zur</
+000045b0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+000045c0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+000045d0: 783d 2239 3233 2e35 2220 793d 222d 3731  x="923.5" y="-71
+000045e0: 362e 3822 2066 6f6e 742d 6661 6d69 6c79  6.8" font-family
+000045f0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00004600: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00004610: 3e4d 6172 6b74 6c6f 6b61 7469 6f6e 207a  >Marktlokation z
+00004620: 756d 2069 6465 6e74 6973 6368 656e 2041  um identischen A
+00004630: 626d 656c 6465 6461 7475 6d20 6265 7265  bmeldedatum bere
+00004640: 6974 7320 6475 7263 683c 2f74 6578 743e  its durch</text>
+00004650: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00004660: 6f72 3d22 7374 6172 7422 2078 3d22 3932  or="start" x="92
+00004670: 332e 3522 2079 3d22 2d37 3032 2e38 2220  3.5" y="-702.8" 
+00004680: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00004690: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+000046a0: 697a 653d 2231 342e 3030 223e 6569 6e65  ize="14.00">eine
+000046b0: 2042 6573 7426 2332 3238 3b74 6967 756e   Best&#228;tigun
+000046c0: 6720 696e 2064 656e 2066 6f6c 6765 6e64  g in den folgend
+000046d0: 656e 2050 726f 7a65 7373 7363 6872 6974  en Prozessschrit
+000046e0: 7465 6e20 6265 656e 6465 743f 3c2f 7465  ten beendet?</te
+000046f0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00004700: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00004710: 2239 3233 2e35 2220 793d 222d 3638 382e  "923.5" y="-688.
+00004720: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00004730: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00004740: 742d 7369 7a65 3d22 3134 2e30 3022 3e46  t-size="14.00">F
+00004750: 616c 6c3a 3c2f 7465 7874 3e0a 3c74 6578  all:</text>.<tex
+00004760: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00004770: 7461 7274 2220 783d 2239 3233 2e35 2220  tart" x="923.5" 
+00004780: 793d 222d 3637 342e 3822 2066 6f6e 742d  y="-674.8" font-
+00004790: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000047a0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+000047b0: 3134 2e30 3022 3e26 2336 3135 3939 3b20  14.00">&#61599; 
+000047c0: 5344 3a20 4c69 6566 6572 656e 6465 2076  SD: Lieferende v
+000047d0: 6f6e 204c 4620 616e 204e 422c 2050 726f  on LF an NB, Pro
+000047e0: 7a65 7373 7363 6872 6974 7420 3220 2241  zessschritt 2 "A
+000047f0: 6e74 776f 7274 3c2f 7465 7874 3e0a 3c74  ntwort</text>.<t
+00004800: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00004810: 2273 7461 7274 2220 783d 2239 3233 2e35  "start" x="923.5
+00004820: 2220 793d 222d 3636 302e 3822 2066 6f6e  " y="-660.8" fon
+00004830: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00004840: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00004850: 3d22 3134 2e30 3022 3e61 7566 2041 626d  ="14.00">auf Abm
+00004860: 656c 6475 6e67 223c 2f74 6578 743e 0a3c  eldung"</text>.<
+00004870: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00004880: 3d22 7374 6172 7422 2078 3d22 3932 332e  ="start" x="923.
+00004890: 3522 2079 3d22 2d36 3436 2e38 2220 666f  5" y="-646.8" fo
+000048a0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000048b0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+000048c0: 653d 2231 342e 3030 223e 2623 3631 3539  e="14.00">&#6159
+000048d0: 393b 2053 443a 204c 6965 6665 7265 6e64  9; SD: Lieferend
+000048e0: 6520 766f 6e20 4e42 2061 6e20 4c46 2c20  e von NB an LF, 
+000048f0: 5072 6f7a 6573 7373 6368 7269 7474 2032  Prozessschritt 2
+00004900: 2022 416e 7477 6f72 743c 2f74 6578 743e   "Antwort</text>
+00004910: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00004920: 6f72 3d22 7374 6172 7422 2078 3d22 3932  or="start" x="92
+00004930: 332e 3522 2079 3d22 2d36 3332 2e38 2220  3.5" y="-632.8" 
+00004940: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00004950: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00004960: 697a 653d 2231 342e 3030 223e 6175 6620  ize="14.00">auf 
+00004970: 4162 6d65 6c64 756e 6722 3c2f 7465 7874  Abmeldung"</text
+00004980: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00004990: 686f 723d 2273 7461 7274 2220 783d 2239  hor="start" x="9
+000049a0: 3233 2e35 2220 793d 222d 3631 382e 3822  23.5" y="-618.8"
+000049b0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+000049c0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+000049d0: 7369 7a65 3d22 3134 2e30 3022 3e26 2336  size="14.00">&#6
+000049e0: 3135 3939 3b20 5344 3a20 4c69 6566 6572  1599; SD: Liefer
+000049f0: 6265 6769 6e6e 2c20 5072 6f7a 6573 7373  beginn, Prozesss
+00004a00: 6368 7269 7474 2034 2022 4265 616e 7477  chritt 4 "Beantw
+00004a10: 6f72 7475 6e67 2064 6572 3c2f 7465 7874  ortung der</text
+00004a20: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00004a30: 686f 723d 2273 7461 7274 2220 783d 2239  hor="start" x="9
+00004a40: 3233 2e35 2220 793d 222d 3630 342e 3822  23.5" y="-604.8"
+00004a50: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00004a60: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+00004a70: 7369 7a65 3d22 3134 2e30 3022 3e41 626d  size="14.00">Abm
+00004a80: 656c 6465 616e 6672 6167 6522 206f 6465  eldeanfrage" ode
+00004a90: 7220 6469 6520 4265 7374 2623 3232 383b  r die Best&#228;
+00004aa0: 7469 6775 6e67 2065 7266 6f6c 6774 2064  tigung erfolgt d
+00004ab0: 7572 6368 3c2f 7465 7874 3e0a 3c74 6578  urch</text>.<tex
+00004ac0: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00004ad0: 7461 7274 2220 783d 2239 3233 2e35 2220  tart" x="923.5" 
+00004ae0: 793d 222d 3539 302e 3822 2066 6f6e 742d  y="-590.8" font-
+00004af0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00004b00: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00004b10: 3134 2e30 3022 3e64 6965 2046 7269 7374  14.00">die Frist
+00004b20: 7665 7273 7472 6569 6368 756e 673c 2f74  verstreichung</t
+00004b30: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2035  ext>.</g>.<!-- 5
+00004b40: 2623 3435 3b26 6774 3b31 3020 2d2d 3e0a  &#45;&gt;10 -->.
+00004b50: 3c67 2069 643d 2265 6467 6531 3122 2063  <g id="edge11" c
+00004b60: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
+00004b70: 746c 653e 352d 2667 743b 3130 3c2f 7469  tle>5-&gt;10</ti
+00004b80: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00004b90: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00004ba0: 6c61 636b 2220 643d 224d 3133 3637 2e32  lack" d="M1367.2
+00004bb0: 352c 2d39 3430 2e39 3243 3133 3436 2e32  5,-940.92C1346.2
+00004bc0: 322c 2d39 3334 2e38 3320 3133 3239 2e30  2,-934.83 1329.0
+00004bd0: 382c 2d39 3237 2e38 3620 3133 3139 2e35  8,-927.86 1319.5
+00004be0: 2c2d 3932 3020 3132 3735 2e30 322c 2d38  ,-920 1275.02,-8
+00004bf0: 3833 2e34 3920 3132 3939 2e37 352c 2d38  83.49 1299.75,-8
+00004c00: 3439 2e33 3220 3132 3638 2e35 2c2d 3830  49.32 1268.5,-80
+00004c10: 3120 3132 3539 2e32 2c2d 3738 362e 3632  1 1259.2,-786.62
+00004c20: 2031 3234 382e 3334 2c2d 3737 322e 3331   1248.34,-772.31
+00004c30: 2031 3233 362e 3937 2c2d 3735 382e 3639   1236.97,-758.69
+00004c40: 222f 3e0a 3c70 6f6c 7967 6f6e 2066 696c  "/>.<polygon fil
+00004c50: 6c3d 2262 6c61 636b 2220 7374 726f 6b65  l="black" stroke
+00004c60: 3d22 626c 6163 6b22 2070 6f69 6e74 733d  ="black" points=
+00004c70: 2231 3233 392e 3936 2c2d 3735 362e 3820  "1239.96,-756.8 
+00004c80: 3132 3330 2e38 322c 2d37 3531 2e34 3520  1230.82,-751.45 
+00004c90: 3132 3334 2e36 322c 2d37 3631 2e33 3320  1234.62,-761.33 
+00004ca0: 3132 3339 2e39 362c 2d37 3536 2e38 222f  1239.96,-756.8"/
+00004cb0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00004cc0: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
+00004cd0: 3133 3130 2e35 2220 793d 222d 3834 302e  1310.5" y="-840.
+00004ce0: 3322 2066 6f6e 742d 6661 6d69 6c79 3d22  3" font-family="
+00004cf0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00004d00: 742d 7369 7a65 3d22 3134 2e30 3022 3e4e  t-size="14.00">N
+00004d10: 6569 6e3c 2f74 6578 743e 0a3c 2f67 3e0a  ein</text>.</g>.
+00004d20: 3c21 2d2d 2037 202d 2d3e 0a3c 6720 6964  <!-- 7 -->.<g id
+00004d30: 3d22 6e6f 6465 3130 2220 636c 6173 733d  ="node10" class=
+00004d40: 226e 6f64 6522 3e0a 3c74 6974 6c65 3e37  "node">.<title>7
+00004d50: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+00004d60: 696c 6c3d 2223 3761 6162 3861 2220 7374  ill="#7aab8a" st
+00004d70: 726f 6b65 3d22 626c 6163 6b22 2064 3d22  roke="black" d="
+00004d80: 4d34 3439 2c2d 3836 3743 3434 392c 2d38  M449,-867C449,-8
+00004d90: 3637 2031 322c 2d38 3637 2031 322c 2d38  67 12,-867 12,-8
+00004da0: 3637 2036 2c2d 3836 3720 302c 2d38 3631  67 6,-867 0,-861
+00004db0: 2030 2c2d 3835 3520 302c 2d38 3535 2030   0,-855 0,-855 0
+00004dc0: 2c2d 3833 3320 302c 2d38 3333 2030 2c2d  ,-833 0,-833 0,-
+00004dd0: 3832 3720 362c 2d38 3231 2031 322c 2d38  827 6,-821 12,-8
+00004de0: 3231 2031 322c 2d38 3231 2034 3439 2c2d  21 12,-821 449,-
+00004df0: 3832 3120 3434 392c 2d38 3231 2034 3535  821 449,-821 455
+00004e00: 2c2d 3832 3120 3436 312c 2d38 3237 2034  ,-821 461,-827 4
+00004e10: 3631 2c2d 3833 3320 3436 312c 2d38 3333  61,-833 461,-833
+00004e20: 2034 3631 2c2d 3835 3520 3436 312c 2d38   461,-855 461,-8
+00004e30: 3535 2034 3631 2c2d 3836 3120 3435 352c  55 461,-861 455,
+00004e40: 2d38 3637 2034 3439 2c2d 3836 3722 2f3e  -867 449,-867"/>
+00004e50: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00004e60: 6f72 3d22 7374 6172 7422 2078 3d22 3134  or="start" x="14
+00004e70: 2220 793d 222d 3834 372e 3822 2066 6f6e  " y="-847.8" fon
+00004e80: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00004e90: 7365 7269 6622 2066 6f6e 742d 7765 6967  serif" font-weig
+00004ea0: 6874 3d22 626f 6c64 2220 666f 6e74 2d73  ht="bold" font-s
+00004eb0: 697a 653d 2231 342e 3030 223e 373a 203c  ize="14.00">7: <
+00004ec0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00004ed0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00004ee0: 2078 3d22 3334 2220 793d 222d 3834 372e   x="34" y="-847.
+00004ef0: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00004f00: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00004f10: 742d 7369 7a65 3d22 3134 2e30 3022 3e4c  t-size="14.00">L
+00004f20: 6965 6774 2064 6173 2041 626d 656c 6465  iegt das Abmelde
+00004f30: 6461 7475 6d20 6d69 6e64 6573 7465 6e73  datum mindestens
+00004f40: 2065 696e 656e 2054 6167 206e 6163 6820   einen Tag nach 
+00004f50: 6465 6d3c 2f74 6578 743e 0a3c 7465 7874  dem</text>.<text
+00004f60: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00004f70: 6172 7422 2078 3d22 3134 2220 793d 222d  art" x="14" y="-
+00004f80: 3833 332e 3822 2066 6f6e 742d 6661 6d69  833.8" font-fami
+00004f90: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00004fa0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00004fb0: 3022 3e45 696e 6761 6e67 7364 6174 756d  0">Eingangsdatum
+00004fc0: 2064 6572 2041 626d 656c 6475 6e67 3f3c   der Abmeldung?<
+00004fd0: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+00004fe0: 2036 2623 3435 3b26 6774 3b37 202d 2d3e   6&#45;&gt;7 -->
+00004ff0: 0a3c 6720 6964 3d22 6564 6765 3132 2220  .<g id="edge12" 
+00005000: 636c 6173 733d 2265 6467 6522 3e0a 3c74  class="edge">.<t
+00005010: 6974 6c65 3e36 2d26 6774 3b37 3c2f 7469  itle>6-&gt;7</ti
+00005020: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00005030: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00005040: 6c61 636b 2220 643d 224d 3535 312e 3538  lack" d="M551.58
+00005050: 2c2d 3934 342e 3537 4334 3739 2e38 382c  ,-944.57C479.88,
+00005060: 2d39 3232 2e33 3320 3338 322e 3432 2c2d  -922.33 382.42,-
+00005070: 3839 322e 3131 2033 3133 2e37 342c 2d38  892.11 313.74,-8
+00005080: 3730 2e38 3122 2f3e 0a3c 706f 6c79 676f  70.81"/>.<polygo
+00005090: 6e20 6669 6c6c 3d22 626c 6163 6b22 2073  n fill="black" s
+000050a0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
+000050b0: 696e 7473 3d22 3331 352e 3031 2c2d 3836  ints="315.01,-86
+000050c0: 372e 3534 2033 3034 2e34 322c 2d38 3637  7.54 304.42,-867
+000050d0: 2e39 3220 3331 322e 3934 2c2d 3837 342e  .92 312.94,-874.
+000050e0: 3233 2033 3135 2e30 312c 2d38 3637 2e35  23 315.01,-867.5
+000050f0: 3422 2f3e 0a3c 7465 7874 2074 6578 742d  4"/>.<text text-
+00005100: 616e 6368 6f72 3d22 6d69 6464 6c65 2220  anchor="middle" 
+00005110: 783d 2234 3730 2e35 2220 793d 222d 3930  x="470.5" y="-90
+00005120: 382e 3822 2066 6f6e 742d 6661 6d69 6c79  8.8" font-family
+00005130: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00005140: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00005150: 3e4a 613c 2f74 6578 743e 0a3c 2f67 3e0a  >Ja</text>.</g>.
+00005160: 3c21 2d2d 2038 202d 2d3e 0a3c 6720 6964  <!-- 8 -->.<g id
+00005170: 3d22 6e6f 6465 3132 2220 636c 6173 733d  ="node12" class=
+00005180: 226e 6f64 6522 3e0a 3c74 6974 6c65 3e38  "node">.<title>8
+00005190: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+000051a0: 696c 6c3d 2223 3761 6162 3861 2220 7374  ill="#7aab8a" st
+000051b0: 726f 6b65 3d22 626c 6163 6b22 2064 3d22  roke="black" d="
+000051c0: 4d39 3234 2c2d 3836 3743 3932 342c 2d38  M924,-867C924,-8
+000051d0: 3637 2034 3931 2c2d 3836 3720 3439 312c  67 491,-867 491,
+000051e0: 2d38 3637 2034 3835 2c2d 3836 3720 3437  -867 485,-867 47
+000051f0: 392c 2d38 3631 2034 3739 2c2d 3835 3520  9,-861 479,-855 
+00005200: 3437 392c 2d38 3535 2034 3739 2c2d 3833  479,-855 479,-83
+00005210: 3320 3437 392c 2d38 3333 2034 3739 2c2d  3 479,-833 479,-
+00005220: 3832 3720 3438 352c 2d38 3231 2034 3931  827 485,-821 491
+00005230: 2c2d 3832 3120 3439 312c 2d38 3231 2039  ,-821 491,-821 9
+00005240: 3234 2c2d 3832 3120 3932 342c 2d38 3231  24,-821 924,-821
+00005250: 2039 3330 2c2d 3832 3120 3933 362c 2d38   930,-821 936,-8
+00005260: 3237 2039 3336 2c2d 3833 3320 3933 362c  27 936,-833 936,
+00005270: 2d38 3333 2039 3336 2c2d 3835 3520 3933  -833 936,-855 93
+00005280: 362c 2d38 3535 2039 3336 2c2d 3836 3120  6,-855 936,-861 
+00005290: 3933 302c 2d38 3637 2039 3234 2c2d 3836  930,-867 924,-86
+000052a0: 3722 2f3e 0a3c 7465 7874 2074 6578 742d  7"/>.<text text-
+000052b0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000052c0: 3d22 3439 3322 2079 3d22 2d38 3437 2e38  ="493" y="-847.8
+000052d0: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+000052e0: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+000052f0: 2d77 6569 6768 743d 2262 6f6c 6422 2066  -weight="bold" f
+00005300: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00005310: 3e38 3a20 3c2f 7465 7874 3e0a 3c74 6578  >8: </text>.<tex
+00005320: 7420 7465 7874 2d61 6e63 686f 723d 2273  t text-anchor="s
+00005330: 7461 7274 2220 783d 2235 3133 2220 793d  tart" x="513" y=
+00005340: 222d 3834 372e 3822 2066 6f6e 742d 6661  "-847.8" font-fa
+00005350: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00005360: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+00005370: 2e30 3022 3e4c 6965 6774 2064 6173 2045  .00">Liegt das E
+00005380: 696e 6761 6e67 7364 6174 756d 2064 6572  ingangsdatum der
+00005390: 2041 626d 656c 6475 6e67 206d 6568 7220   Abmeldung mehr 
+000053a0: 616c 7320 7365 6368 733c 2f74 6578 743e  als sechs</text>
+000053b0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+000053c0: 6f72 3d22 7374 6172 7422 2078 3d22 3439  or="start" x="49
+000053d0: 3322 2079 3d22 2d38 3333 2e38 2220 666f  3" y="-833.8" fo
+000053e0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+000053f0: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00005400: 653d 2231 342e 3030 223e 576f 6368 656e  e="14.00">Wochen
+00005410: 206e 6163 6820 6465 6d20 4162 6d65 6c64   nach dem Abmeld
+00005420: 6564 6174 756d 2064 6572 2041 626d 656c  edatum der Abmel
+00005430: 6475 6e67 3f3c 2f74 6578 743e 0a3c 2f67  dung?</text>.</g
+00005440: 3e0a 3c21 2d2d 2036 2623 3435 3b26 6774  >.<!-- 6&#45;&gt
+00005450: 3b38 202d 2d3e 0a3c 6720 6964 3d22 6564  ;8 -->.<g id="ed
+00005460: 6765 3133 2220 636c 6173 733d 2265 6467  ge13" class="edg
+00005470: 6522 3e0a 3c74 6974 6c65 3e36 2d26 6774  e">.<title>6-&gt
+00005480: 3b38 3c2f 7469 746c 653e 0a3c 7061 7468  ;8</title>.<path
+00005490: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+000054a0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+000054b0: 3636 302e 3334 2c2d 3934 342e 3733 4336  660.34,-944.73C6
+000054c0: 3639 2e38 2c2d 3932 342e 3732 2036 3832  69.8,-924.72 682
+000054d0: 2e33 342c 2d38 3938 2e32 2036 3932 2e31  .34,-898.2 692.1
+000054e0: 322c 2d38 3737 2e35 3322 2f3e 0a3c 706f  2,-877.53"/>.<po
+000054f0: 6c79 676f 6e20 6669 6c6c 3d22 626c 6163  lygon fill="blac
+00005500: 6b22 2073 7472 6f6b 653d 2262 6c61 636b  k" stroke="black
+00005510: 2220 706f 696e 7473 3d22 3639 352e 3138  " points="695.18
+00005520: 2c2d 3837 392e 3233 2036 3936 2e33 2c2d  ,-879.23 696.3,-
+00005530: 3836 382e 3720 3638 382e 3836 2c2d 3837  868.7 688.86,-87
+00005540: 362e 3234 2036 3935 2e31 382c 2d38 3739  6.24 695.18,-879
+00005550: 2e32 3322 2f3e 0a3c 7465 7874 2074 6578  .23"/>.<text tex
+00005560: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
+00005570: 2220 783d 2236 3936 2e35 2220 793d 222d  " x="696.5" y="-
+00005580: 3930 382e 3822 2066 6f6e 742d 6661 6d69  908.8" font-fami
+00005590: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+000055a0: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+000055b0: 3022 3e4e 6569 6e3c 2f74 6578 743e 0a3c  0">Nein</text>.<
+000055c0: 2f67 3e0a 3c21 2d2d 2041 3033 202d 2d3e  /g>.<!-- A03 -->
+000055d0: 0a3c 6720 6964 3d22 6e6f 6465 3131 2220  .<g id="node11" 
+000055e0: 636c 6173 733d 226e 6f64 6522 3e0a 3c74  class="node">.<t
+000055f0: 6974 6c65 3e41 3033 3c2f 7469 746c 653e  itle>A03</title>
+00005600: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00005610: 2363 6662 3938 3622 2073 7472 6f6b 653d  #cfb986" stroke=
+00005620: 2262 6c61 636b 2220 706f 696e 7473 3d22  "black" points="
+00005630: 3338 322c 2d37 3031 2037 392c 2d37 3031  382,-701 79,-701
+00005640: 2037 392c 2d36 3237 2033 3832 2c2d 3632   79,-627 382,-62
+00005650: 3720 3338 322c 2d37 3031 222f 3e0a 3c74  7 382,-701"/>.<t
+00005660: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00005670: 2273 7461 7274 2220 783d 2232 3135 2220  "start" x="215" 
+00005680: 793d 222d 3638 342e 3822 2066 6f6e 742d  y="-684.8" font-
+00005690: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000056a0: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+000056b0: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+000056c0: 653d 2231 342e 3030 223e 4130 333c 2f74  e="14.00">A03</t
+000056d0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+000056e0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000056f0: 3d22 3931 2220 793d 222d 3637 322e 3422  ="91" y="-672.4"
+00005700: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+00005710: 6d65 732c 7365 7269 6622 2074 6578 742d  mes,serif" text-
+00005720: 6465 636f 7261 7469 6f6e 3d22 756e 6465  decoration="unde
+00005730: 726c 696e 6522 2066 6f6e 742d 7369 7a65  rline" font-size
+00005740: 3d22 3132 2e30 3022 3e48 696e 7765 6973  ="12.00">Hinweis
+00005750: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00005760: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00005770: 7422 2078 3d22 3931 2220 793d 222d 3636  t" x="91" y="-66
+00005780: 302e 3422 2066 6f6e 742d 6661 6d69 6c79  0.4" font-family
+00005790: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+000057a0: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+000057b0: 3e43 6c75 7374 6572 3a20 4162 6c65 686e  >Cluster: Ablehn
+000057c0: 756e 673c 2f74 6578 743e 0a3c 7465 7874  ung</text>.<text
+000057d0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+000057e0: 6172 7422 2078 3d22 3931 2220 793d 222d  art" x="91" y="-
+000057f0: 3634 382e 3422 2066 6f6e 742d 6661 6d69  648.4" font-fami
+00005800: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00005810: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
+00005820: 3022 3e45 696e 6761 6e67 7366 7269 7374  0">Eingangsfrist
+00005830: 2062 6569 2069 4d53 2f6b 4d45 206d 6974   bei iMS/kME mit
+00005840: 2052 4c4d 206e 6963 6874 2065 696e 2d3c   RLM nicht ein-<
+00005850: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00005860: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00005870: 2078 3d22 3931 2220 793d 222d 3633 362e   x="91" y="-636.
+00005880: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00005890: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+000058a0: 742d 7369 7a65 3d22 3132 2e30 3022 3e67  t-size="12.00">g
+000058b0: 6568 616c 7465 6e2e 3c2f 7465 7874 3e0a  ehalten.</text>.
+000058c0: 3c2f 673e 0a3c 212d 2d20 3726 2334 353b  </g>.<!-- 7&#45;
+000058d0: 2667 743b 4130 3320 2d2d 3e0a 3c67 2069  &gt;A03 -->.<g i
+000058e0: 643d 2265 6467 6531 3422 2063 6c61 7373  d="edge14" class
+000058f0: 3d22 6564 6765 223e 0a3c 7469 746c 653e  ="edge">.<title>
+00005900: 372d 2667 743b 4130 333c 2f74 6974 6c65  7-&gt;A03</title
+00005910: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
+00005920: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00005930: 6b22 2064 3d22 4d32 3330 2e35 2c2d 3832  k" d="M230.5,-82
+00005940: 302e 3832 4332 3330 2e35 2c2d 3739 332e  0.82C230.5,-793.
+00005950: 3934 2032 3330 2e35 2c2d 3734 372e 3920  94 230.5,-747.9 
+00005960: 3233 302e 352c 2d37 3132 2e38 3222 2f3e  230.5,-712.82"/>
+00005970: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00005980: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+00005990: 6c61 636b 2220 706f 696e 7473 3d22 3233  lack" points="23
+000059a0: 342c 2d37 3132 2e39 2032 3330 2e35 2c2d  4,-712.9 230.5,-
+000059b0: 3730 322e 3920 3232 372c 2d37 3132 2e39  702.9 227,-712.9
+000059c0: 2032 3334 2c2d 3731 322e 3922 2f3e 0a3c   234,-712.9"/>.<
+000059d0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+000059e0: 3d22 6d69 6464 6c65 2220 783d 2232 3437  ="middle" x="247
+000059f0: 2e35 2220 793d 222d 3737 312e 3822 2066  .5" y="-771.8" f
+00005a00: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00005a10: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00005a20: 7a65 3d22 3134 2e30 3022 3e4e 6569 6e3c  ze="14.00">Nein<
+00005a30: 2f74 6578 743e 0a3c 2f67 3e0a 3c21 2d2d  /text>.</g>.<!--
+00005a40: 2037 2623 3435 3b26 6774 3b31 3020 2d2d   7&#45;&gt;10 --
+00005a50: 3e0a 3c67 2069 643d 2265 6467 6531 3522  >.<g id="edge15"
+00005a60: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
+00005a70: 7469 746c 653e 372d 2667 743b 3130 3c2f  title>7-&gt;10</
+00005a80: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+00005a90: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+00005aa0: 2262 6c61 636b 2220 643d 224d 3334 332e  "black" d="M343.
+00005ab0: 3439 2c2d 3832 302e 3534 4333 3833 2e31  49,-820.54C383.1
+00005ac0: 392c 2d38 3133 2e33 3420 3432 382e 3139  9,-813.34 428.19
+00005ad0: 2c2d 3830 352e 3936 2034 3639 2e35 2c2d  ,-805.96 469.5,-
+00005ae0: 3830 3120 3539 312e 3535 2c2d 3738 362e  801 591.55,-786.
+00005af0: 3334 2036 3234 2e32 312c 2d38 3033 2e30  34 624.21,-803.0
+00005b00: 3220 3734 352e 352c 2d37 3833 2038 3031  2 745.5,-783 801
+00005b10: 2e33 342c 2d37 3733 2e37 3820 3831 342e  .34,-773.78 814.
+00005b20: 3132 2c2d 3736 352e 3639 2038 3638 2e35  12,-765.69 868.5
+00005b30: 2c2d 3735 3020 3837 382e 3238 2c2d 3734  ,-750 878.28,-74
+00005b40: 372e 3138 2038 3838 2e32 352c 2d37 3434  7.18 888.25,-744
+00005b50: 2e32 3620 3839 382e 3332 2c2d 3734 312e  .26 898.32,-741.
+00005b60: 3239 222f 3e0a 3c70 6f6c 7967 6f6e 2066  29"/>.<polygon f
+00005b70: 696c 6c3d 2262 6c61 636b 2220 7374 726f  ill="black" stro
+00005b80: 6b65 3d22 626c 6163 6b22 2070 6f69 6e74  ke="black" point
+00005b90: 733d 2238 3939 2e32 322c 2d37 3434 2e36  s="899.22,-744.6
+00005ba0: 3820 3930 372e 3832 2c2d 3733 382e 3438  8 907.82,-738.48
+00005bb0: 2038 3937 2e32 332c 2d37 3337 2e39 3620   897.23,-737.96 
+00005bc0: 3839 392e 3232 2c2d 3734 342e 3638 222f  899.22,-744.68"/
+00005bd0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00005be0: 686f 723d 226d 6964 646c 6522 2078 3d22  hor="middle" x="
+00005bf0: 3831 362e 3522 2079 3d22 2d37 3731 2e38  816.5" y="-771.8
+00005c00: 2220 666f 6e74 2d66 616d 696c 793d 2254  " font-family="T
+00005c10: 696d 6573 2c73 6572 6966 2220 666f 6e74  imes,serif" font
+00005c20: 2d73 697a 653d 2231 342e 3030 223e 4a61  -size="14.00">Ja
+00005c30: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00005c40: 2d20 4130 3420 2d2d 3e0a 3c67 2069 643d  - A04 -->.<g id=
+00005c50: 226e 6f64 6531 3322 2063 6c61 7373 3d22  "node13" class="
+00005c60: 6e6f 6465 223e 0a3c 7469 746c 653e 4130  node">.<title>A0
+00005c70: 343c 2f74 6974 6c65 3e0a 3c70 6f6c 7967  4</title>.<polyg
+00005c80: 6f6e 2066 696c 6c3d 2223 6366 6239 3836  on fill="#cfb986
+00005c90: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00005ca0: 2070 6f69 6e74 733d 2238 3539 2e35 2c2d   points="859.5,-
+00005cb0: 3730 3120 3535 352e 352c 2d37 3031 2035  701 555.5,-701 5
+00005cc0: 3535 2e35 2c2d 3632 3720 3835 392e 352c  55.5,-627 859.5,
+00005cd0: 2d36 3237 2038 3539 2e35 2c2d 3730 3122  -627 859.5,-701"
+00005ce0: 2f3e 0a3c 7465 7874 2074 6578 742d 616e  />.<text text-an
+00005cf0: 6368 6f72 3d22 7374 6172 7422 2078 3d22  chor="start" x="
+00005d00: 3639 3222 2079 3d22 2d36 3834 2e38 2220  692" y="-684.8" 
+00005d10: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00005d20: 6573 2c73 6572 6966 2220 666f 6e74 2d77  es,serif" font-w
+00005d30: 6569 6768 743d 2262 6f6c 6422 2066 6f6e  eight="bold" fon
+00005d40: 742d 7369 7a65 3d22 3134 2e30 3022 3e41  t-size="14.00">A
+00005d50: 3034 3c2f 7465 7874 3e0a 3c74 6578 7420  04</text>.<text 
+00005d60: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00005d70: 7274 2220 783d 2235 3637 2e35 2220 793d  rt" x="567.5" y=
+00005d80: 222d 3637 322e 3422 2066 6f6e 742d 6661  "-672.4" font-fa
+00005d90: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00005da0: 6622 2074 6578 742d 6465 636f 7261 7469  f" text-decorati
+00005db0: 6f6e 3d22 756e 6465 726c 696e 6522 2066  on="underline" f
+00005dc0: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00005dd0: 3e48 696e 7765 6973 3a3c 2f74 6578 743e  >Hinweis:</text>
+00005de0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00005df0: 6f72 3d22 7374 6172 7422 2078 3d22 3536  or="start" x="56
+00005e00: 372e 3522 2079 3d22 2d36 3630 2e34 2220  7.5" y="-660.4" 
+00005e10: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00005e20: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00005e30: 697a 653d 2231 322e 3030 223e 436c 7573  ize="12.00">Clus
+00005e40: 7465 723a 2041 626c 6568 6e75 6e67 3c2f  ter: Ablehnung</
+00005e50: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00005e60: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00005e70: 783d 2235 3637 2e35 2220 793d 222d 3634  x="567.5" y="-64
+00005e80: 382e 3422 2066 6f6e 742d 6661 6d69 6c79  8.4" font-family
+00005e90: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00005ea0: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00005eb0: 3e46 7269 7374 2623 3235 323b 6265 7273  >Frist&#252;bers
+00005ec0: 6368 7265 6974 756e 6720 6265 6920 6b4d  chreitung bei kM
+00005ed0: 4520 6f68 6e65 2052 4c4d 2f6d 4d45 2f3c  E ohne RLM/mME/<
+00005ee0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00005ef0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00005f00: 2078 3d22 3536 372e 3522 2079 3d22 2d36   x="567.5" y="-6
+00005f10: 3336 2e34 2220 666f 6e74 2d66 616d 696c  36.4" font-famil
+00005f20: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00005f30: 666f 6e74 2d73 697a 653d 2231 322e 3030  font-size="12.00
+00005f40: 223e 5061 7573 6368 616c 616e 6c61 6765  ">Pauschalanlage
+00005f50: 2e3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  .</text>.</g>.<!
+00005f60: 2d2d 2038 2623 3435 3b26 6774 3b41 3034  -- 8&#45;&gt;A04
+00005f70: 202d 2d3e 0a3c 6720 6964 3d22 6564 6765   -->.<g id="edge
+00005f80: 3136 2220 636c 6173 733d 2265 6467 6522  16" class="edge"
+00005f90: 3e0a 3c74 6974 6c65 3e38 2d26 6774 3b41  >.<title>8-&gt;A
+00005fa0: 3034 3c2f 7469 746c 653e 0a3c 7061 7468  04</title>.<path
+00005fb0: 2066 696c 6c3d 226e 6f6e 6522 2073 7472   fill="none" str
+00005fc0: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+00005fd0: 3730 372e 352c 2d38 3230 2e38 3243 3730  707.5,-820.82C70
+00005fe0: 372e 352c 2d37 3933 2e39 3420 3730 372e  7.5,-793.94 707.
+00005ff0: 352c 2d37 3437 2e39 2037 3037 2e35 2c2d  5,-747.9 707.5,-
+00006000: 3731 322e 3832 222f 3e0a 3c70 6f6c 7967  712.82"/>.<polyg
+00006010: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00006020: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00006030: 6f69 6e74 733d 2237 3131 2c2d 3731 322e  oints="711,-712.
+00006040: 3920 3730 372e 352c 2d37 3032 2e39 2037  9 707.5,-702.9 7
+00006050: 3034 2c2d 3731 322e 3920 3731 312c 2d37  04,-712.9 711,-7
+00006060: 3132 2e39 222f 3e0a 3c74 6578 7420 7465  12.9"/>.<text te
+00006070: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00006080: 6522 2078 3d22 3732 342e 3522 2079 3d22  e" x="724.5" y="
+00006090: 2d37 3731 2e38 2220 666f 6e74 2d66 616d  -771.8" font-fam
+000060a0: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+000060b0: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+000060c0: 3030 223e 4e65 696e 3c2f 7465 7874 3e0a  00">Nein</text>.
+000060d0: 3c2f 673e 0a3c 212d 2d20 3826 2334 353b  </g>.<!-- 8&#45;
+000060e0: 2667 743b 3130 202d 2d3e 0a3c 6720 6964  &gt;10 -->.<g id
+000060f0: 3d22 6564 6765 3137 2220 636c 6173 733d  ="edge17" class=
+00006100: 2265 6467 6522 3e0a 3c74 6974 6c65 3e38  "edge">.<title>8
+00006110: 2d26 6774 3b31 303c 2f74 6974 6c65 3e0a  -&gt;10</title>.
+00006120: 3c70 6174 6820 6669 6c6c 3d22 6e6f 6e65  <path fill="none
+00006130: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00006140: 2064 3d22 4d38 3438 2e33 352c 2d38 3230   d="M848.35,-820
+00006150: 2e35 3243 3838 382e 3136 2c2d 3831 312e  .52C888.16,-811.
+00006160: 3535 2039 3330 2e38 362c 2d37 3939 2e33  55 930.86,-799.3
+00006170: 3420 3936 382e 352c 2d37 3833 2039 3835  4 968.5,-783 985
+00006180: 2e37 382c 2d37 3735 2e35 2031 3030 332e  .78,-775.5 1003.
+00006190: 3138 2c2d 3736 362e 3235 2031 3031 392e  18,-766.25 1019.
+000061a0: 3935 2c2d 3735 362e 3236 222f 3e0a 3c70  95,-756.26"/>.<p
+000061b0: 6f6c 7967 6f6e 2066 696c 6c3d 2262 6c61  olygon fill="bla
+000061c0: 636b 2220 7374 726f 6b65 3d22 626c 6163  ck" stroke="blac
+000061d0: 6b22 2070 6f69 6e74 733d 2231 3032 312e  k" points="1021.
+000061e0: 3733 2c2d 3735 392e 3237 2031 3032 382e  73,-759.27 1028.
+000061f0: 3435 2c2d 3735 312e 3039 2031 3031 382e  45,-751.09 1018.
+00006200: 3039 2c2d 3735 332e 3239 2031 3032 312e  09,-753.29 1021.
+00006210: 3733 2c2d 3735 392e 3237 222f 3e0a 3c74  73,-759.27"/>.<t
+00006220: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00006230: 226d 6964 646c 6522 2078 3d22 3130 3030  "middle" x="1000
+00006240: 2e35 2220 793d 222d 3737 312e 3822 2066  .5" y="-771.8" f
+00006250: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00006260: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00006270: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
+00006280: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
+00006290: 3035 202d 2d3e 0a3c 6720 6964 3d22 6e6f  05 -->.<g id="no
+000062a0: 6465 3135 2220 636c 6173 733d 226e 6f64  de15" class="nod
+000062b0: 6522 3e0a 3c74 6974 6c65 3e41 3035 3c2f  e">.<title>A05</
+000062c0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
+000062d0: 6669 6c6c 3d22 2363 6662 3938 3622 2073  fill="#cfb986" s
+000062e0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
+000062f0: 696e 7473 3d22 3137 3436 2e35 2c2d 3730  ints="1746.5,-70
+00006300: 3720 3134 3236 2e35 2c2d 3730 3720 3134  7 1426.5,-707 14
+00006310: 3236 2e35 2c2d 3632 3120 3137 3436 2e35  26.5,-621 1746.5
+00006320: 2c2d 3632 3120 3137 3436 2e35 2c2d 3730  ,-621 1746.5,-70
+00006330: 3722 2f3e 0a3c 7465 7874 2074 6578 742d  7"/>.<text text-
+00006340: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00006350: 3d22 3135 3731 2220 793d 222d 3639 302e  ="1571" y="-690.
+00006360: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00006370: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00006380: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+00006390: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+000063a0: 223e 4130 353c 2f74 6578 743e 0a3c 7465  ">A05</text>.<te
+000063b0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000063c0: 7374 6172 7422 2078 3d22 3134 3338 2e35  start" x="1438.5
+000063d0: 2220 793d 222d 3637 382e 3422 2066 6f6e  " y="-678.4" fon
+000063e0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+000063f0: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
+00006400: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
+00006410: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
+00006420: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
+00006430: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00006440: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00006450: 3d22 3134 3338 2e35 2220 793d 222d 3636  ="1438.5" y="-66
+00006460: 362e 3422 2066 6f6e 742d 6661 6d69 6c79  6.4" font-family
+00006470: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00006480: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00006490: 3e43 6c75 7374 6572 3a20 4162 6c65 686e  >Cluster: Ablehn
+000064a0: 756e 673c 2f74 6578 743e 0a3c 7465 7874  ung</text>.<text
+000064b0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+000064c0: 6172 7422 2078 3d22 3134 3338 2e35 2220  art" x="1438.5" 
+000064d0: 793d 222d 3635 342e 3422 2066 6f6e 742d  y="-654.4" font-
+000064e0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000064f0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00006500: 3132 2e30 3022 3e44 6965 2041 7566 6865  12.00">Die Aufhe
+00006510: 6275 6e67 2065 696e 6572 207a 756b 2623  bung einer zuk&#
+00006520: 3235 323b 6e66 7469 6765 6e20 5a75 6f72  252;nftigen Zuor
+00006530: 646e 756e 673c 2f74 6578 743e 0a3c 7465  dnung</text>.<te
+00006540: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00006550: 7374 6172 7422 2078 3d22 3134 3338 2e35  start" x="1438.5
+00006560: 2220 793d 222d 3634 322e 3422 2066 6f6e  " y="-642.4" fon
+00006570: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00006580: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00006590: 3d22 3132 2e30 3022 3e6d 7573 7320 7a75  ="12.00">muss zu
+000065a0: 6d20 4461 7475 6d20 285a 6569 7470 756e  m Datum (Zeitpun
+000065b0: 6b74 2920 616e 6765 6765 6265 6e20 7765  kt) angegeben we
+000065c0: 7264 656e 2c3c 2f74 6578 743e 0a3c 7465  rden,</text>.<te
+000065d0: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+000065e0: 7374 6172 7422 2078 3d22 3134 3338 2e35  start" x="1438.5
+000065f0: 2220 793d 222d 3633 302e 3422 2066 6f6e  " y="-630.4" fon
+00006600: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00006610: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00006620: 3d22 3132 2e30 3022 3e77 6965 2069 6d20  ="12.00">wie im 
+00006630: 4c69 6566 6572 6265 6769 6e6e 2062 6573  Lieferbeginn bes
+00006640: 7426 2332 3238 3b74 6967 742e 3c2f 7465  t&#228;tigt.</te
+00006650: 7874 3e0a 3c2f 673e 0a3c 212d 2d20 3926  xt>.</g>.<!-- 9&
+00006660: 2334 353b 2667 743b 4130 3520 2d2d 3e0a  #45;&gt;A05 -->.
+00006670: 3c67 2069 643d 2265 6467 6531 3822 2063  <g id="edge18" c
+00006680: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
+00006690: 746c 653e 392d 2667 743b 4130 353c 2f74  tle>9-&gt;A05</t
+000066a0: 6974 6c65 3e0a 3c70 6174 6820 6669 6c6c  itle>.<path fill
+000066b0: 3d22 6e6f 6e65 2220 7374 726f 6b65 3d22  ="none" stroke="
+000066c0: 626c 6163 6b22 2064 3d22 4d31 3538 362e  black" d="M1586.
+000066d0: 352c 2d38 3133 2e36 3143 3135 3836 2e35  5,-813.61C1586.5
+000066e0: 2c2d 3738 372e 3834 2031 3538 362e 352c  ,-787.84 1586.5,
+000066f0: 2d37 3439 2e37 3320 3135 3836 2e35 2c2d  -749.73 1586.5,-
+00006700: 3731 382e 3536 222f 3e0a 3c70 6f6c 7967  718.56"/>.<polyg
+00006710: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+00006720: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+00006730: 6f69 6e74 733d 2231 3539 302c 2d37 3138  oints="1590,-718
+00006740: 2e39 3420 3135 3836 2e35 2c2d 3730 382e  .94 1586.5,-708.
+00006750: 3934 2031 3538 332c 2d37 3138 2e39 3420  94 1583,-718.94 
+00006760: 3135 3930 2c2d 3731 382e 3934 222f 3e0a  1590,-718.94"/>.
+00006770: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+00006780: 723d 226d 6964 646c 6522 2078 3d22 3136  r="middle" x="16
+00006790: 3033 2e35 2220 793d 222d 3737 312e 3822  03.5" y="-771.8"
+000067a0: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+000067b0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+000067c0: 7369 7a65 3d22 3134 2e30 3022 3e4e 6569  size="14.00">Nei
+000067d0: 6e3c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  n</text>.</g>.<!
+000067e0: 2d2d 2039 2623 3435 3b26 6774 3b31 3020  -- 9&#45;&gt;10 
+000067f0: 2d2d 3e0a 3c67 2069 643d 2265 6467 6531  -->.<g id="edge1
+00006800: 3922 2063 6c61 7373 3d22 6564 6765 223e  9" class="edge">
+00006810: 0a3c 7469 746c 653e 392d 2667 743b 3130  .<title>9-&gt;10
+00006820: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+00006830: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+00006840: 653d 2262 6c61 636b 2220 643d 224d 3135  e="black" d="M15
+00006850: 3133 2e33 352c 2d38 3133 2e36 3143 3134  13.35,-813.61C14
+00006860: 3732 2e36 382c 2d37 3937 2e32 3720 3134  72.68,-797.27 14
+00006870: 3139 2e36 372c 2d37 3735 2e39 3720 3133  19.67,-775.97 13
+00006880: 3636 2e35 352c 2d37 3534 2e36 3222 2f3e  66.55,-754.62"/>
+00006890: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+000068a0: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+000068b0: 6c61 636b 2220 706f 696e 7473 3d22 3133  lack" points="13
+000068c0: 3637 2e39 312c 2d37 3531 2e34 2031 3335  67.91,-751.4 135
+000068d0: 372e 3333 2c2d 3735 302e 3932 2031 3336  7.33,-750.92 136
+000068e0: 352e 332c 2d37 3537 2e38 3920 3133 3637  5.3,-757.89 1367
+000068f0: 2e39 312c 2d37 3531 2e34 222f 3e0a 3c74  .91,-751.4"/>.<t
+00006900: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00006910: 226d 6964 646c 6522 2078 3d22 3134 3337  "middle" x="1437
+00006920: 2e35 2220 793d 222d 3737 312e 3822 2066  .5" y="-771.8" f
+00006930: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00006940: 732c 7365 7269 6622 2066 6f6e 742d 7369  s,serif" font-si
+00006950: 7a65 3d22 3134 2e30 3022 3e4a 613c 2f74  ze="14.00">Ja</t
+00006960: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2041  ext>.</g>.<!-- A
+00006970: 3036 202d 2d3e 0a3c 6720 6964 3d22 6e6f  06 -->.<g id="no
+00006980: 6465 3137 2220 636c 6173 733d 226e 6f64  de17" class="nod
+00006990: 6522 3e0a 3c74 6974 6c65 3e41 3036 3c2f  e">.<title>A06</
+000069a0: 7469 746c 653e 0a3c 706f 6c79 676f 6e20  title>.<polygon 
+000069b0: 6669 6c6c 3d22 2363 6662 3938 3622 2073  fill="#cfb986" s
+000069c0: 7472 6f6b 653d 2262 6c61 636b 2220 706f  troke="black" po
+000069d0: 696e 7473 3d22 3131 3536 2c2d 3431 3720  ints="1156,-417 
+000069e0: 3936 332c 2d34 3137 2039 3633 2c2d 3335  963,-417 963,-35
+000069f0: 3520 3131 3536 2c2d 3335 3520 3131 3536  5 1156,-355 1156
+00006a00: 2c2d 3431 3722 2f3e 0a3c 7465 7874 2074  ,-417"/>.<text t
+00006a10: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00006a20: 7422 2078 3d22 3130 3434 2220 793d 222d  t" x="1044" y="-
+00006a30: 3430 302e 3822 2066 6f6e 742d 6661 6d69  400.8" font-fami
+00006a40: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00006a50: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
+00006a60: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
+00006a70: 342e 3030 223e 4130 363c 2f74 6578 743e  4.00">A06</text>
+00006a80: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00006a90: 6f72 3d22 7374 6172 7422 2078 3d22 3937  or="start" x="97
+00006aa0: 3522 2079 3d22 2d33 3838 2e34 2220 666f  5" y="-388.4" fo
+00006ab0: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00006ac0: 2c73 6572 6966 2220 7465 7874 2d64 6563  ,serif" text-dec
+00006ad0: 6f72 6174 696f 6e3d 2275 6e64 6572 6c69  oration="underli
+00006ae0: 6e65 2220 666f 6e74 2d73 697a 653d 2231  ne" font-size="1
+00006af0: 322e 3030 223e 4869 6e77 6569 733a 3c2f  2.00">Hinweis:</
+00006b00: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00006b10: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00006b20: 783d 2239 3735 2220 793d 222d 3337 362e  x="975" y="-376.
+00006b30: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00006b40: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00006b50: 742d 7369 7a65 3d22 3132 2e30 3022 3e43  t-size="12.00">C
+00006b60: 6c75 7374 6572 3a20 5a75 7374 696d 6d75  luster: Zustimmu
+00006b70: 6e67 3c2f 7465 7874 3e0a 3c74 6578 7420  ng</text>.<text 
+00006b80: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00006b90: 7274 2220 783d 2239 3735 2220 793d 222d  rt" x="975" y="-
+00006ba0: 3336 342e 3422 2066 6f6e 742d 6661 6d69  364.4" font-fami
+00006bb0: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00006bc0: 2066 6f6e 742d 7369 7a65 3d22 3132 2e30   font-size="12.0
+00006bd0: 3022 3e42 6573 7426 2332 3238 3b74 6967  0">Best&#228;tig
+00006be0: 756e 6720 6465 7220 4162 6d65 6c64 756e  ung der Abmeldun
+00006bf0: 673c 2f74 6578 743e 0a3c 2f67 3e0a 3c21  g</text>.</g>.<!
+00006c00: 2d2d 2031 3026 2334 353b 2667 743b 4130  -- 10&#45;&gt;A0
+00006c10: 3620 2d2d 3e0a 3c67 2069 643d 2265 6467  6 -->.<g id="edg
+00006c20: 6532 3122 2063 6c61 7373 3d22 6564 6765  e21" class="edge
+00006c30: 223e 0a3c 7469 746c 653e 3130 2d26 6774  ">.<title>10-&gt
+00006c40: 3b41 3036 3c2f 7469 746c 653e 0a3c 7061  ;A06</title>.<pa
+00006c50: 7468 2066 696c 6c3d 226e 6f6e 6522 2073  th fill="none" s
+00006c60: 7472 6f6b 653d 2262 6c61 636b 2220 643d  troke="black" d=
+00006c70: 224d 3130 3839 2e31 332c 2d35 3737 2e36  "M1089.13,-577.6
+00006c80: 3943 3130 3830 2e38 392c 2d35 3631 2e34  9C1080.89,-561.4
+00006c90: 2031 3037 332e 3439 2c2d 3534 342e 3038   1073.49,-544.08
+00006ca0: 2031 3036 382e 352c 2d35 3237 2031 3035   1068.5,-527 105
+00006cb0: 392e 3135 2c2d 3439 342e 3938 2031 3035  9.15,-494.98 105
+00006cc0: 372e 3233 2c2d 3435 372e 3136 2031 3035  7.23,-457.16 105
+00006cd0: 372e 3436 2c2d 3432 382e 3922 2f3e 0a3c  7.46,-428.9"/>.<
+00006ce0: 706f 6c79 676f 6e20 6669 6c6c 3d22 626c  polygon fill="bl
+00006cf0: 6163 6b22 2073 7472 6f6b 653d 2262 6c61  ack" stroke="bla
+00006d00: 636b 2220 706f 696e 7473 3d22 3130 3630  ck" points="1060
+00006d10: 2e39 362c 2d34 3239 2031 3035 372e 3635  .96,-429 1057.65
+00006d20: 2c2d 3431 382e 3934 2031 3035 332e 3936  ,-418.94 1053.96
+00006d30: 2c2d 3432 382e 3837 2031 3036 302e 3936  ,-428.87 1060.96
+00006d40: 2c2d 3432 3922 2f3e 0a3c 7465 7874 2074  ,-429"/>.<text t
+00006d50: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
+00006d60: 6c65 2220 783d 2231 3038 352e 3522 2079  le" x="1085.5" y
+00006d70: 3d22 2d35 3030 2e33 2220 666f 6e74 2d66  ="-500.3" font-f
+00006d80: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00006d90: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00006da0: 342e 3030 223e 4e65 696e 3c2f 7465 7874  4.00">Nein</text
+00006db0: 3e0a 3c2f 673e 0a3c 212d 2d20 3131 202d  >.</g>.<!-- 11 -
+00006dc0: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3138  ->.<g id="node18
+00006dd0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
+00006de0: 3c74 6974 6c65 3e31 313c 2f74 6974 6c65  <title>11</title
+00006df0: 3e0a 3c70 6174 6820 6669 6c6c 3d22 2337  >.<path fill="#7
+00006e00: 6161 6238 6122 2073 7472 6f6b 653d 2262  aab8a" stroke="b
+00006e10: 6c61 636b 2220 643d 224d 3136 3033 2e35  lack" d="M1603.5
+00006e20: 2c2d 3532 3743 3136 3033 2e35 2c2d 3532  ,-527C1603.5,-52
+00006e30: 3720 3131 3233 2e35 2c2d 3532 3720 3131  7 1123.5,-527 11
+00006e40: 3233 2e35 2c2d 3532 3720 3131 3137 2e35  23.5,-527 1117.5
+00006e50: 2c2d 3532 3720 3131 3131 2e35 2c2d 3532  ,-527 1111.5,-52
+00006e60: 3120 3131 3131 2e35 2c2d 3531 3520 3131  1 1111.5,-515 11
+00006e70: 3131 2e35 2c2d 3531 3520 3131 3131 2e35  11.5,-515 1111.5
+00006e80: 2c2d 3439 3320 3131 3131 2e35 2c2d 3439  ,-493 1111.5,-49
+00006e90: 3320 3131 3131 2e35 2c2d 3438 3720 3131  3 1111.5,-487 11
+00006ea0: 3137 2e35 2c2d 3438 3120 3131 3233 2e35  17.5,-481 1123.5
+00006eb0: 2c2d 3438 3120 3131 3233 2e35 2c2d 3438  ,-481 1123.5,-48
+00006ec0: 3120 3136 3033 2e35 2c2d 3438 3120 3136  1 1603.5,-481 16
+00006ed0: 3033 2e35 2c2d 3438 3120 3136 3039 2e35  03.5,-481 1609.5
+00006ee0: 2c2d 3438 3120 3136 3135 2e35 2c2d 3438  ,-481 1615.5,-48
+00006ef0: 3720 3136 3135 2e35 2c2d 3439 3320 3136  7 1615.5,-493 16
+00006f00: 3135 2e35 2c2d 3439 3320 3136 3135 2e35  15.5,-493 1615.5
+00006f10: 2c2d 3531 3520 3136 3135 2e35 2c2d 3531  ,-515 1615.5,-51
+00006f20: 3520 3136 3135 2e35 2c2d 3532 3120 3136  5 1615.5,-521 16
+00006f30: 3039 2e35 2c2d 3532 3720 3136 3033 2e35  09.5,-527 1603.5
+00006f40: 2c2d 3532 3722 2f3e 0a3c 7465 7874 2074  ,-527"/>.<text t
+00006f50: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00006f60: 7422 2078 3d22 3131 3235 2e35 2220 793d  t" x="1125.5" y=
+00006f70: 222d 3530 372e 3822 2066 6f6e 742d 6661  "-507.8" font-fa
+00006f80: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00006f90: 6622 2066 6f6e 742d 7765 6967 6874 3d22  f" font-weight="
+00006fa0: 626f 6c64 2220 666f 6e74 2d73 697a 653d  bold" font-size=
+00006fb0: 2231 342e 3030 223e 3131 3a20 3c2f 7465  "14.00">11: </te
+00006fc0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00006fd0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00006fe0: 2231 3135 352e 3522 2079 3d22 2d35 3037  "1155.5" y="-507
+00006ff0: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00007000: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00007010: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00007020: 4973 7420 6465 7220 616e 6672 6167 656e  Ist der anfragen
+00007030: 6465 204c 4620 616d 2046 6f6c 6765 7461  de LF am Folgeta
+00007040: 6720 6465 7320 4162 6d65 6c64 756e 6773  g des Abmeldungs
+00007050: 6461 7475 6d20 6465 723c 2f74 6578 743e  datum der</text>
+00007060: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00007070: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
+00007080: 3235 2e35 2220 793d 222d 3439 332e 3822  25.5" y="-493.8"
+00007090: 2066 6f6e 742d 6661 6d69 6c79 3d22 5469   font-family="Ti
+000070a0: 6d65 732c 7365 7269 6622 2066 6f6e 742d  mes,serif" font-
+000070b0: 7369 7a65 3d22 3134 2e30 3022 3e4d 6172  size="14.00">Mar
+000070c0: 6b74 6c6f 6b61 7469 6f6e 206e 6f63 6820  ktlokation noch 
+000070d0: 7a75 6765 6f72 646e 6574 3f3c 2f74 6578  zugeordnet?</tex
+000070e0: 743e 0a3c 2f67 3e0a 3c21 2d2d 2031 3026  t>.</g>.<!-- 10&
+000070f0: 2334 353b 2667 743b 3131 202d 2d3e 0a3c  #45;&gt;11 -->.<
+00007100: 6720 6964 3d22 6564 6765 3230 2220 636c  g id="edge20" cl
+00007110: 6173 733d 2265 6467 6522 3e0a 3c74 6974  ass="edge">.<tit
+00007120: 6c65 3e31 302d 2667 743b 3131 3c2f 7469  le>10-&gt;11</ti
+00007130: 746c 653e 0a3c 7061 7468 2066 696c 6c3d  tle>.<path fill=
+00007140: 226e 6f6e 6522 2073 7472 6f6b 653d 2262  "none" stroke="b
+00007150: 6c61 636b 2220 643d 224d 3132 3632 2e35  lack" d="M1262.5
+00007160: 312c 2d35 3737 2e35 3343 3132 3834 2e33  1,-577.53C1284.3
+00007170: 382c 2d35 3631 2e38 3220 3133 3035 2e37  8,-561.82 1305.7
+00007180: 372c 2d35 3436 2e34 3620 3133 3233 2e32  7,-546.46 1323.2
+00007190: 2c2d 3533 332e 3935 222f 3e0a 3c70 6f6c  ,-533.95"/>.<pol
+000071a0: 7967 6f6e 2066 696c 6c3d 2262 6c61 636b  ygon fill="black
+000071b0: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+000071c0: 2070 6f69 6e74 733d 2231 3332 352e 3134   points="1325.14
+000071d0: 2c2d 3533 362e 3836 2031 3333 312e 3232  ,-536.86 1331.22
+000071e0: 2c2d 3532 382e 3139 2031 3332 312e 3035  ,-528.19 1321.05
+000071f0: 2c2d 3533 312e 3138 2031 3332 352e 3134  ,-531.18 1325.14
+00007200: 2c2d 3533 362e 3836 222f 3e0a 3c74 6578  ,-536.86"/>.<tex
+00007210: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
+00007220: 6964 646c 6522 2078 3d22 3133 3130 2e35  iddle" x="1310.5
+00007230: 2220 793d 222d 3534 382e 3822 2066 6f6e  " y="-548.8" fon
+00007240: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00007250: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00007260: 3d22 3134 2e30 3022 3e4a 613c 2f74 6578  ="14.00">Ja</tex
+00007270: 743e 0a3c 2f67 3e0a 3c21 2d2d 2031 3126  t>.</g>.<!-- 11&
+00007280: 2334 353b 2667 743b 4130 3620 2d2d 3e0a  #45;&gt;A06 -->.
+00007290: 3c67 2069 643d 2265 6467 6532 3322 2063  <g id="edge23" c
+000072a0: 6c61 7373 3d22 6564 6765 223e 0a3c 7469  lass="edge">.<ti
+000072b0: 746c 653e 3131 2d26 6774 3b41 3036 3c2f  tle>11-&gt;A06</
+000072c0: 7469 746c 653e 0a3c 7061 7468 2066 696c  title>.<path fil
+000072d0: 6c3d 226e 6f6e 6522 2073 7472 6f6b 653d  l="none" stroke=
+000072e0: 2262 6c61 636b 2220 643d 224d 3133 3031  "black" d="M1301
+000072f0: 2e33 332c 2d34 3830 2e36 3643 3132 3632  .33,-480.66C1262
+00007300: 2e32 322c 2d34 3636 2e34 3620 3132 3130  .22,-466.46 1210
+00007310: 2e37 372c 2d34 3437 2e35 3220 3131 3635  .77,-447.52 1165
+00007320: 2e35 2c2d 3433 3020 3131 3538 2e35 392c  .5,-430 1158.59,
+00007330: 2d34 3237 2e33 3320 3131 3531 2e34 352c  -427.33 1151.45,
+00007340: 2d34 3234 2e35 3220 3131 3434 2e32 392c  -424.52 1144.29,
+00007350: 2d34 3231 2e36 3822 2f3e 0a3c 706f 6c79  -421.68"/>.<poly
+00007360: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
+00007370: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00007380: 706f 696e 7473 3d22 3131 3435 2e37 392c  points="1145.79,
+00007390: 2d34 3138 2e35 3120 3131 3335 2e32 2c2d  -418.51 1135.2,-
+000073a0: 3431 382e 3035 2031 3134 332e 322c 2d34  418.05 1143.2,-4
+000073b0: 3235 2e30 3120 3131 3435 2e37 392c 2d34  25.01 1145.79,-4
+000073c0: 3138 2e35 3122 2f3e 0a3c 7465 7874 2074  18.51"/>.<text t
+000073d0: 6578 742d 616e 6368 6f72 3d22 6d69 6464  ext-anchor="midd
+000073e0: 6c65 2220 783d 2231 3235 382e 3522 2079  le" x="1258.5" y
+000073f0: 3d22 2d34 3531 2e38 2220 666f 6e74 2d66  ="-451.8" font-f
+00007400: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00007410: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00007420: 342e 3030 223e 4a61 3c2f 7465 7874 3e0a  4.00">Ja</text>.
+00007430: 3c2f 673e 0a3c 212d 2d20 3132 202d 2d3e  </g>.<!-- 12 -->
+00007440: 0a3c 6720 6964 3d22 6e6f 6465 3139 2220  .<g id="node19" 
+00007450: 636c 6173 733d 226e 6f64 6522 3e0a 3c74  class="node">.<t
+00007460: 6974 6c65 3e31 323c 2f74 6974 6c65 3e0a  itle>12</title>.
+00007470: 3c70 6174 6820 6669 6c6c 3d22 2337 6161  <path fill="#7aa
+00007480: 6238 6122 2073 7472 6f6b 653d 2262 6c61  b8a" stroke="bla
+00007490: 636b 2220 643d 224d 3136 3339 2c2d 3433  ck" d="M1639,-43
+000074a0: 3043 3136 3339 2c2d 3433 3020 3131 3836  0C1639,-430 1186
+000074b0: 2c2d 3433 3020 3131 3836 2c2d 3433 3020  ,-430 1186,-430 
+000074c0: 3131 3830 2c2d 3433 3020 3131 3734 2c2d  1180,-430 1174,-
+000074d0: 3432 3420 3131 3734 2c2d 3431 3820 3131  424 1174,-418 11
+000074e0: 3734 2c2d 3431 3820 3131 3734 2c2d 3335  74,-418 1174,-35
+000074f0: 3420 3131 3734 2c2d 3335 3420 3131 3734  4 1174,-354 1174
+00007500: 2c2d 3334 3820 3131 3830 2c2d 3334 3220  ,-348 1180,-342 
+00007510: 3131 3836 2c2d 3334 3220 3131 3836 2c2d  1186,-342 1186,-
+00007520: 3334 3220 3136 3339 2c2d 3334 3220 3136  342 1639,-342 16
+00007530: 3339 2c2d 3334 3220 3136 3435 2c2d 3334  39,-342 1645,-34
+00007540: 3220 3136 3531 2c2d 3334 3820 3136 3531  2 1651,-348 1651
+00007550: 2c2d 3335 3420 3136 3531 2c2d 3335 3420  ,-354 1651,-354 
+00007560: 3136 3531 2c2d 3431 3820 3136 3531 2c2d  1651,-418 1651,-
+00007570: 3431 3820 3136 3531 2c2d 3432 3420 3136  418 1651,-424 16
+00007580: 3435 2c2d 3433 3020 3136 3339 2c2d 3433  45,-430 1639,-43
+00007590: 3022 2f3e 0a3c 7465 7874 2074 6578 742d  0"/>.<text text-
+000075a0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000075b0: 3d22 3131 3838 2220 793d 222d 3431 302e  ="1188" y="-410.
+000075c0: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+000075d0: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+000075e0: 742d 7765 6967 6874 3d22 626f 6c64 2220  t-weight="bold" 
+000075f0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00007600: 223e 3132 3a20 3c2f 7465 7874 3e0a 3c74  ">12: </text>.<t
+00007610: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00007620: 2273 7461 7274 2220 783d 2231 3231 3822  "start" x="1218"
+00007630: 2079 3d22 2d34 3130 2e38 2220 666f 6e74   y="-410.8" font
+00007640: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00007650: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+00007660: 2231 342e 3030 223e 4c69 6567 7420 6569  "14.00">Liegt ei
+00007670: 6e20 5472 616e 7361 6b74 696f 6e73 6772  n Transaktionsgr
+00007680: 756e 6420 766f 722c 2061 7573 2077 656c  und vor, aus wel
+00007690: 6368 656d 2068 6572 766f 7267 6568 742c  chem hervorgeht,
+000076a0: 3c2f 7465 7874 3e0a 3c74 6578 7420 7465  </text>.<text te
+000076b0: 7874 2d61 6e63 686f 723d 2273 7461 7274  xt-anchor="start
+000076c0: 2220 783d 2231 3138 3822 2079 3d22 2d33  " x="1188" y="-3
+000076d0: 3936 2e38 2220 666f 6e74 2d66 616d 696c  96.8" font-famil
+000076e0: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+000076f0: 666f 6e74 2d73 697a 653d 2231 342e 3030  font-size="14.00
+00007700: 223e 6461 7373 2064 6572 2041 6e73 6368  ">dass der Ansch
+00007710: 6c75 7373 6e75 747a 6572 2061 7573 6765  lussnutzer ausge
+00007720: 7a6f 6765 6e20 6973 743f 3c2f 7465 7874  zogen ist?</text
+00007730: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00007740: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+00007750: 3138 3822 2079 3d22 2d33 3832 2e38 2220  188" y="-382.8" 
+00007760: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00007770: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00007780: 697a 653d 2231 342e 3030 223e 4461 7320  ize="14.00">Das 
+00007790: 6973 7420 6265 6920 6465 6e20 666f 6c67  ist bei den folg
+000077a0: 656e 6465 6e20 5472 616e 7361 6b74 696f  enden Transaktio
+000077b0: 6e73 6772 2623 3235 323b 6e64 656e 2064  nsgr&#252;nden d
+000077c0: 6572 2046 616c 6c3a 3c2f 7465 7874 3e0a  er Fall:</text>.
+000077d0: 3c74 6578 7420 7465 7874 2d61 6e63 686f  <text text-ancho
+000077e0: 723d 2273 7461 7274 2220 783d 2231 3138  r="start" x="118
+000077f0: 3822 2079 3d22 2d33 3638 2e38 2220 666f  8" y="-368.8" fo
+00007800: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00007810: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00007820: 653d 2231 342e 3030 223e 2623 3631 3539  e="14.00">&#6159
+00007830: 393b 2045 696e 2d2f 4175 737a 7567 2028  9; Ein-/Auszug (
+00007840: 556d 7a75 6729 3c2f 7465 7874 3e0a 3c74  Umzug)</text>.<t
+00007850: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00007860: 2273 7461 7274 2220 783d 2231 3138 3822  "start" x="1188"
+00007870: 2079 3d22 2d33 3534 2e38 2220 666f 6e74   y="-354.8" font
+00007880: 2d66 616d 696c 793d 2254 696d 6573 2c73  -family="Times,s
+00007890: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
+000078a0: 2231 342e 3030 223e 2623 3631 3539 393b  "14.00">&#61599;
+000078b0: 2041 7573 7a75 6720 7765 6765 6e20 5374   Auszug wegen St
+000078c0: 696c 6c6c 6567 756e 673c 2f74 6578 743e  illlegung</text>
+000078d0: 0a3c 2f67 3e0a 3c21 2d2d 2031 3126 2334  .</g>.<!-- 11&#4
+000078e0: 353b 2667 743b 3132 202d 2d3e 0a3c 6720  5;&gt;12 -->.<g 
+000078f0: 6964 3d22 6564 6765 3232 2220 636c 6173  id="edge22" clas
+00007900: 733d 2265 6467 6522 3e0a 3c74 6974 6c65  s="edge">.<title
+00007910: 3e31 312d 2667 743b 3132 3c2f 7469 746c  >11-&gt;12</titl
+00007920: 653e 0a3c 7061 7468 2066 696c 6c3d 226e  e>.<path fill="n
+00007930: 6f6e 6522 2073 7472 6f6b 653d 2262 6c61  one" stroke="bla
+00007940: 636b 2220 643d 224d 3133 3732 2e39 352c  ck" d="M1372.95,
+00007950: 2d34 3830 2e36 3343 3133 3737 2e37 332c  -480.63C1377.73,
+00007960: 2d34 3639 2e33 2031 3338 332e 3737 2c2d  -469.3 1383.77,-
+00007970: 3435 352e 3031 2031 3338 392e 3638 2c2d  455.01 1389.68,-
+00007980: 3434 312e 3032 222f 3e0a 3c70 6f6c 7967  441.02"/>.<polyg
+00007990: 6f6e 2066 696c 6c3d 2262 6c61 636b 2220  on fill="black" 
+000079a0: 7374 726f 6b65 3d22 626c 6163 6b22 2070  stroke="black" p
+000079b0: 6f69 6e74 733d 2231 3339 322e 3839 2c2d  oints="1392.89,-
+000079c0: 3434 322e 3431 2031 3339 332e 3536 2c2d  442.41 1393.56,-
+000079d0: 3433 312e 3834 2031 3338 362e 3435 2c2d  431.84 1386.45,-
+000079e0: 3433 392e 3639 2031 3339 322e 3839 2c2d  439.69 1392.89,-
+000079f0: 3434 322e 3431 222f 3e0a 3c74 6578 7420  442.41"/>.<text 
+00007a00: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
+00007a10: 646c 6522 2078 3d22 3134 3033 2e35 2220  dle" x="1403.5" 
+00007a20: 793d 222d 3435 312e 3822 2066 6f6e 742d  y="-451.8" font-
+00007a30: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+00007a40: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+00007a50: 3134 2e30 3022 3e4e 6569 6e3c 2f74 6578  14.00">Nein</tex
+00007a60: 743e 0a3c 2f67 3e0a 3c21 2d2d 2041 3037  t>.</g>.<!-- A07
+00007a70: 202d 2d3e 0a3c 6720 6964 3d22 6e6f 6465   -->.<g id="node
+00007a80: 3230 2220 636c 6173 733d 226e 6f64 6522  20" class="node"
+00007a90: 3e0a 3c74 6974 6c65 3e41 3037 3c2f 7469  >.<title>A07</ti
+00007aa0: 746c 653e 0a3c 706f 6c79 676f 6e20 6669  tle>.<polygon fi
+00007ab0: 6c6c 3d22 2363 6662 3938 3622 2073 7472  ll="#cfb986" str
+00007ac0: 6f6b 653d 2262 6c61 636b 2220 706f 696e  oke="black" poin
+00007ad0: 7473 3d22 3134 3439 2c2d 3236 3320 3131  ts="1449,-263 11
+00007ae0: 3530 2c2d 3236 3320 3131 3530 2c2d 3138  50,-263 1150,-18
+00007af0: 3920 3134 3439 2c2d 3138 3920 3134 3439  9 1449,-189 1449
+00007b00: 2c2d 3236 3322 2f3e 0a3c 7465 7874 2074  ,-263"/>.<text t
+00007b10: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00007b20: 7422 2078 3d22 3132 3834 2220 793d 222d  t" x="1284" y="-
+00007b30: 3234 362e 3822 2066 6f6e 742d 6661 6d69  246.8" font-fami
+00007b40: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00007b50: 2066 6f6e 742d 7765 6967 6874 3d22 626f   font-weight="bo
+00007b60: 6c64 2220 666f 6e74 2d73 697a 653d 2231  ld" font-size="1
+00007b70: 342e 3030 223e 4130 373c 2f74 6578 743e  4.00">A07</text>
+00007b80: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00007b90: 6f72 3d22 7374 6172 7422 2078 3d22 3131  or="start" x="11
+00007ba0: 3632 2220 793d 222d 3233 342e 3422 2066  62" y="-234.4" f
+00007bb0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+00007bc0: 732c 7365 7269 6622 2074 6578 742d 6465  s,serif" text-de
+00007bd0: 636f 7261 7469 6f6e 3d22 756e 6465 726c  coration="underl
+00007be0: 696e 6522 2066 6f6e 742d 7369 7a65 3d22  ine" font-size="
+00007bf0: 3132 2e30 3022 3e48 696e 7765 6973 3a3c  12.00">Hinweis:<
+00007c00: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00007c10: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00007c20: 2078 3d22 3131 3632 2220 793d 222d 3232   x="1162" y="-22
+00007c30: 322e 3422 2066 6f6e 742d 6661 6d69 6c79  2.4" font-family
+00007c40: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00007c50: 6f6e 742d 7369 7a65 3d22 3132 2e30 3022  ont-size="12.00"
+00007c60: 3e43 6c75 7374 6572 3a20 4162 6c65 686e  >Cluster: Ablehn
+00007c70: 756e 673c 2f74 6578 743e 0a3c 7465 7874  ung</text>.<text
+00007c80: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00007c90: 6172 7422 2078 3d22 3131 3632 2220 793d  art" x="1162" y=
+00007ca0: 222d 3231 302e 3422 2066 6f6e 742d 6661  "-210.4" font-fa
+00007cb0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00007cc0: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
+00007cd0: 2e30 3022 3e4c 6965 6665 7265 6e64 6520  .00">Lieferende 
+00007ce0: 7a75 6d20 4162 6d65 6c64 6564 6174 756d  zum Abmeldedatum
+00007cf0: 2077 7572 6465 2062 6572 6569 7473 3c2f   wurde bereits</
+00007d00: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00007d10: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00007d20: 783d 2231 3136 3222 2079 3d22 2d31 3938  x="1162" y="-198
+00007d30: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00007d40: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00007d50: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
+00007d60: 6265 7374 2623 3232 383b 7469 6774 3c2f  best&#228;tigt</
+00007d70: 7465 7874 3e0a 3c2f 673e 0a3c 212d 2d20  text>.</g>.<!-- 
+00007d80: 3132 2623 3435 3b26 6774 3b41 3037 202d  12&#45;&gt;A07 -
+00007d90: 2d3e 0a3c 6720 6964 3d22 6564 6765 3234  ->.<g id="edge24
+00007da0: 2220 636c 6173 733d 2265 6467 6522 3e0a  " class="edge">.
+00007db0: 3c74 6974 6c65 3e31 322d 2667 743b 4130  <title>12-&gt;A0
+00007dc0: 373c 2f74 6974 6c65 3e0a 3c70 6174 6820  7</title>.<path 
+00007dd0: 6669 6c6c 3d22 6e6f 6e65 2220 7374 726f  fill="none" stro
+00007de0: 6b65 3d22 626c 6163 6b22 2064 3d22 4d31  ke="black" d="M1
+00007df0: 3338 312e 3632 2c2d 3334 312e 3833 4331  381.62,-341.83C1
+00007e00: 3336 362e 3331 2c2d 3332 302e 3432 2031  366.31,-320.42 1
+00007e10: 3334 372e 3831 2c2d 3239 342e 3535 2031  347.81,-294.55 1
+00007e20: 3333 322e 3235 2c2d 3237 322e 3822 2f3e  332.25,-272.8"/>
+00007e30: 0a3c 706f 6c79 676f 6e20 6669 6c6c 3d22  .<polygon fill="
+00007e40: 626c 6163 6b22 2073 7472 6f6b 653d 2262  black" stroke="b
+00007e50: 6c61 636b 2220 706f 696e 7473 3d22 3133  lack" points="13
+00007e60: 3335 2e31 2c2d 3237 302e 3736 2031 3332  35.1,-270.76 132
+00007e70: 362e 3434 2c2d 3236 342e 3637 2031 3332  6.44,-264.67 132
+00007e80: 392e 3431 2c2d 3237 342e 3834 2031 3333  9.41,-274.84 133
+00007e90: 352e 312c 2d32 3730 2e37 3622 2f3e 0a3c  5.1,-270.76"/>.<
+00007ea0: 7465 7874 2074 6578 742d 616e 6368 6f72  text text-anchor
+00007eb0: 3d22 6d69 6464 6c65 2220 783d 2231 3338  ="middle" x="138
+00007ec0: 322e 3522 2079 3d22 2d33 3132 2e38 2220  2.5" y="-312.8" 
+00007ed0: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00007ee0: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00007ef0: 697a 653d 2231 342e 3030 223e 4e65 696e  ize="14.00">Nein
+00007f00: 3c2f 7465 7874 3e0a 3c2f 673e 0a3c 212d  </text>.</g>.<!-
+00007f10: 2d20 3133 202d 2d3e 0a3c 6720 6964 3d22  - 13 -->.<g id="
+00007f20: 6e6f 6465 3231 2220 636c 6173 733d 226e  node21" class="n
+00007f30: 6f64 6522 3e0a 3c74 6974 6c65 3e31 333c  ode">.<title>13<
+00007f40: 2f74 6974 6c65 3e0a 3c70 6174 6820 6669  /title>.<path fi
+00007f50: 6c6c 3d22 2337 6161 6238 6122 2073 7472  ll="#7aab8a" str
+00007f60: 6f6b 653d 2262 6c61 636b 2220 643d 224d  oke="black" d="M
+00007f70: 3139 3132 2c2d 3239 3143 3139 3132 2c2d  1912,-291C1912,-
+00007f80: 3239 3120 3134 3739 2c2d 3239 3120 3134  291 1479,-291 14
+00007f90: 3739 2c2d 3239 3120 3134 3733 2c2d 3239  79,-291 1473,-29
+00007fa0: 3120 3134 3637 2c2d 3238 3520 3134 3637  1 1467,-285 1467
+00007fb0: 2c2d 3237 3920 3134 3637 2c2d 3237 3920  ,-279 1467,-279 
+00007fc0: 3134 3637 2c2d 3137 3320 3134 3637 2c2d  1467,-173 1467,-
+00007fd0: 3137 3320 3134 3637 2c2d 3136 3720 3134  173 1467,-167 14
+00007fe0: 3733 2c2d 3136 3120 3134 3739 2c2d 3136  73,-161 1479,-16
+00007ff0: 3120 3134 3739 2c2d 3136 3120 3139 3132  1 1479,-161 1912
+00008000: 2c2d 3136 3120 3139 3132 2c2d 3136 3120  ,-161 1912,-161 
+00008010: 3139 3138 2c2d 3136 3120 3139 3234 2c2d  1918,-161 1924,-
+00008020: 3136 3720 3139 3234 2c2d 3137 3320 3139  167 1924,-173 19
+00008030: 3234 2c2d 3137 3320 3139 3234 2c2d 3237  24,-173 1924,-27
+00008040: 3920 3139 3234 2c2d 3237 3920 3139 3234  9 1924,-279 1924
+00008050: 2c2d 3238 3520 3139 3138 2c2d 3239 3120  ,-285 1918,-291 
+00008060: 3139 3132 2c2d 3239 3122 2f3e 0a3c 7465  1912,-291"/>.<te
+00008070: 7874 2074 6578 742d 616e 6368 6f72 3d22  xt text-anchor="
+00008080: 7374 6172 7422 2078 3d22 3134 3831 2220  start" x="1481" 
+00008090: 793d 222d 3237 312e 3822 2066 6f6e 742d  y="-271.8" font-
+000080a0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000080b0: 7269 6622 2066 6f6e 742d 7765 6967 6874  rif" font-weight
+000080c0: 3d22 626f 6c64 2220 666f 6e74 2d73 697a  ="bold" font-siz
+000080d0: 653d 2231 342e 3030 223e 3133 3a20 3c2f  e="14.00">13: </
+000080e0: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+000080f0: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00008100: 783d 2231 3531 3122 2079 3d22 2d32 3731  x="1511" y="-271
+00008110: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00008120: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00008130: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00008140: 4c69 6567 7420 696e 2064 6572 2062 6572  Liegt in der ber
+00008150: 6569 7473 2062 6573 7426 2332 3238 3b74  eits best&#228;t
+00008160: 6967 7465 6e20 4162 6d65 6c64 756e 6720  igten Abmeldung 
+00008170: 6569 6e3c 2f74 6578 743e 0a3c 7465 7874  ein</text>.<text
+00008180: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00008190: 6172 7422 2078 3d22 3134 3831 2220 793d  art" x="1481" y=
+000081a0: 222d 3235 372e 3822 2066 6f6e 742d 6661  "-257.8" font-fa
+000081b0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+000081c0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+000081d0: 2e30 3022 3e54 7261 6e73 616b 7469 6f6e  .00">Transaktion
+000081e0: 7367 7275 6e64 2076 6f72 2c20 6175 7320  sgrund vor, aus 
+000081f0: 7765 6c63 6865 6d20 6e69 6368 7420 6865  welchem nicht he
+00008200: 7276 6f72 6765 6874 2c20 6461 7373 3c2f  rvorgeht, dass</
+00008210: 7465 7874 3e0a 3c74 6578 7420 7465 7874  text>.<text text
+00008220: 2d61 6e63 686f 723d 2273 7461 7274 2220  -anchor="start" 
+00008230: 783d 2231 3438 3122 2079 3d22 2d32 3433  x="1481" y="-243
+00008240: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00008250: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00008260: 6e74 2d73 697a 653d 2231 342e 3030 223e  nt-size="14.00">
+00008270: 6465 7220 416e 7363 686c 7573 736e 7574  der Anschlussnut
+00008280: 7a65 7220 6175 7367 657a 6f67 656e 2069  zer ausgezogen i
+00008290: 7374 3f3c 2f74 6578 743e 0a3c 7465 7874  st?</text>.<text
+000082a0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+000082b0: 6172 7422 2078 3d22 3134 3831 2220 793d  art" x="1481" y=
+000082c0: 222d 3232 392e 3822 2066 6f6e 742d 6661  "-229.8" font-fa
+000082d0: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+000082e0: 6622 2066 6f6e 742d 7369 7a65 3d22 3134  f" font-size="14
+000082f0: 2e30 3022 3e44 6173 2069 7374 2062 6569  .00">Das ist bei
+00008300: 2064 656e 2066 6f6c 6765 6e64 656e 2054   den folgenden T
+00008310: 7261 6e73 616b 7469 6f6e 7367 7226 2332  ransaktionsgr&#2
+00008320: 3532 3b6e 6465 6e20 6465 7220 4661 6c6c  52;nden der Fall
+00008330: 3a3c 2f74 6578 743e 0a3c 7465 7874 2074  :</text>.<text t
+00008340: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00008350: 7422 2078 3d22 3134 3831 2220 793d 222d  t" x="1481" y="-
+00008360: 3231 352e 3822 2066 6f6e 742d 6661 6d69  215.8" font-fami
+00008370: 6c79 3d22 5469 6d65 732c 7365 7269 6622  ly="Times,serif"
+00008380: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00008390: 3022 3e26 2336 3135 3939 3b20 4569 6e2d  0">&#61599; Ein-
+000083a0: 2f41 7573 7a75 6720 2855 6d7a 7567 293c  /Auszug (Umzug)<
+000083b0: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+000083c0: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+000083d0: 2078 3d22 3134 3831 2220 793d 222d 3230   x="1481" y="-20
+000083e0: 312e 3822 2066 6f6e 742d 6661 6d69 6c79  1.8" font-family
+000083f0: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00008400: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00008410: 3e26 2336 3135 3939 3b20 4175 737a 7567  >&#61599; Auszug
+00008420: 2077 6567 656e 2053 7469 6c6c 6c65 6775   wegen Stilllegu
+00008430: 6e67 3c2f 7465 7874 3e0a 3c74 6578 7420  ng</text>.<text 
+00008440: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00008450: 7274 2220 783d 2231 3438 3122 2079 3d22  rt" x="1481" y="
+00008460: 2d31 3837 2e38 2220 666f 6e74 2d66 616d  -187.8" font-fam
+00008470: 696c 793d 2254 696d 6573 2c73 6572 6966  ily="Times,serif
+00008480: 2220 666f 6e74 2d73 697a 653d 2231 342e  " font-size="14.
+00008490: 3030 223e 2623 3631 3539 393b 2041 7566  00">&#61599; Auf
+000084a0: 6865 6275 6e67 2065 696e 6572 207a 756b  hebung einer zuk
+000084b0: 2623 3235 323b 6e66 7469 6765 6e20 5a75  &#252;nftigen Zu
+000084c0: 6f72 646e 756e 6720 7765 6765 6e3c 2f74  ordnung wegen</t
+000084d0: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+000084e0: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+000084f0: 3d22 3134 3831 2220 793d 222d 3137 332e  ="1481" y="-173.
+00008500: 3822 2066 6f6e 742d 6661 6d69 6c79 3d22  8" font-family="
+00008510: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00008520: 742d 7369 7a65 3d22 3134 2e30 3022 3e53  t-size="14.00">S
+00008530: 7469 6c6c 6c65 6775 6e67 3c2f 7465 7874  tilllegung</text
+00008540: 3e0a 3c2f 673e 0a3c 212d 2d20 3132 2623  >.</g>.<!-- 12&#
+00008550: 3435 3b26 6774 3b31 3320 2d2d 3e0a 3c67  45;&gt;13 -->.<g
+00008560: 2069 643d 2265 6467 6532 3522 2063 6c61   id="edge25" cla
+00008570: 7373 3d22 6564 6765 223e 0a3c 7469 746c  ss="edge">.<titl
+00008580: 653e 3132 2d26 6774 3b31 333c 2f74 6974  e>12-&gt;13</tit
+00008590: 6c65 3e0a 3c70 6174 6820 6669 6c6c 3d22  le>.<path fill="
+000085a0: 6e6f 6e65 2220 7374 726f 6b65 3d22 626c  none" stroke="bl
+000085b0: 6163 6b22 2064 3d22 4d31 3439 302e 3231  ack" d="M1490.21
+000085c0: 2c2d 3334 312e 3632 4331 3531 342e 3931  ,-341.62C1514.91
+000085d0: 2c2d 3332 372e 3833 2031 3534 322e 3839  ,-327.83 1542.89
+000085e0: 2c2d 3331 322e 3220 3135 3730 2e30 372c  ,-312.2 1570.07,
+000085f0: 2d32 3937 2e30 3322 2f3e 0a3c 706f 6c79  -297.03"/>.<poly
+00008600: 676f 6e20 6669 6c6c 3d22 626c 6163 6b22  gon fill="black"
+00008610: 2073 7472 6f6b 653d 2262 6c61 636b 2220   stroke="black" 
+00008620: 706f 696e 7473 3d22 3135 3731 2e36 392c  points="1571.69,
+00008630: 2d33 3030 2e31 3320 3135 3738 2e37 322c  -300.13 1578.72,
+00008640: 2d32 3932 2e32 2031 3536 382e 3238 2c2d  -292.2 1568.28,-
+00008650: 3239 342e 3032 2031 3537 312e 3639 2c2d  294.02 1571.69,-
+00008660: 3330 302e 3133 222f 3e0a 3c74 6578 7420  300.13"/>.<text 
+00008670: 7465 7874 2d61 6e63 686f 723d 226d 6964  text-anchor="mid
+00008680: 646c 6522 2078 3d22 3135 3532 2e35 2220  dle" x="1552.5" 
+00008690: 793d 222d 3331 322e 3822 2066 6f6e 742d  y="-312.8" font-
+000086a0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000086b0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+000086c0: 3134 2e30 3022 3e4a 613c 2f74 6578 743e  14.00">Ja</text>
+000086d0: 0a3c 2f67 3e0a 3c21 2d2d 2041 3038 202d  .</g>.<!-- A08 -
+000086e0: 2d3e 0a3c 6720 6964 3d22 6e6f 6465 3232  ->.<g id="node22
+000086f0: 2220 636c 6173 733d 226e 6f64 6522 3e0a  " class="node">.
+00008700: 3c74 6974 6c65 3e41 3038 3c2f 7469 746c  <title>A08</titl
+00008710: 653e 0a3c 706f 6c79 676f 6e20 6669 6c6c  e>.<polygon fill
+00008720: 3d22 2363 6662 3938 3622 2073 7472 6f6b  ="#cfb986" strok
+00008730: 653d 2262 6c61 636b 2220 706f 696e 7473  e="black" points
+00008740: 3d22 3136 3734 2c2d 3932 2031 3339 352c  ="1674,-92 1395,
+00008750: 2d39 3220 3133 3935 2c2d 3138 2031 3637  -92 1395,-18 167
+00008760: 342c 2d31 3820 3136 3734 2c2d 3932 222f  4,-18 1674,-92"/
+00008770: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00008780: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+00008790: 3531 3922 2079 3d22 2d37 352e 3822 2066  519" y="-75.8" f
+000087a0: 6f6e 742d 6661 6d69 6c79 3d22 5469 6d65  ont-family="Time
+000087b0: 732c 7365 7269 6622 2066 6f6e 742d 7765  s,serif" font-we
+000087c0: 6967 6874 3d22 626f 6c64 2220 666f 6e74  ight="bold" font
+000087d0: 2d73 697a 653d 2231 342e 3030 223e 4130  -size="14.00">A0
+000087e0: 383c 2f74 6578 743e 0a3c 7465 7874 2074  8</text>.<text t
+000087f0: 6578 742d 616e 6368 6f72 3d22 7374 6172  ext-anchor="star
+00008800: 7422 2078 3d22 3134 3037 2220 793d 222d  t" x="1407" y="-
+00008810: 3633 2e34 2220 666f 6e74 2d66 616d 696c  63.4" font-famil
+00008820: 793d 2254 696d 6573 2c73 6572 6966 2220  y="Times,serif" 
+00008830: 7465 7874 2d64 6563 6f72 6174 696f 6e3d  text-decoration=
+00008840: 2275 6e64 6572 6c69 6e65 2220 666f 6e74  "underline" font
+00008850: 2d73 697a 653d 2231 322e 3030 223e 4869  -size="12.00">Hi
+00008860: 6e77 6569 733a 3c2f 7465 7874 3e0a 3c74  nweis:</text>.<t
+00008870: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00008880: 2273 7461 7274 2220 783d 2231 3430 3722  "start" x="1407"
+00008890: 2079 3d22 2d35 312e 3422 2066 6f6e 742d   y="-51.4" font-
+000088a0: 6661 6d69 6c79 3d22 5469 6d65 732c 7365  family="Times,se
+000088b0: 7269 6622 2066 6f6e 742d 7369 7a65 3d22  rif" font-size="
+000088c0: 3132 2e30 3022 3e43 6c75 7374 6572 3a20  12.00">Cluster: 
+000088d0: 4162 6c65 686e 756e 673c 2f74 6578 743e  Ablehnung</text>
+000088e0: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+000088f0: 6f72 3d22 7374 6172 7422 2078 3d22 3134  or="start" x="14
+00008900: 3037 2220 793d 222d 3339 2e34 2220 666f  07" y="-39.4" fo
+00008910: 6e74 2d66 616d 696c 793d 2254 696d 6573  nt-family="Times
+00008920: 2c73 6572 6966 2220 666f 6e74 2d73 697a  ,serif" font-siz
+00008930: 653d 2231 322e 3030 223e 4c69 6566 6572  e="12.00">Liefer
+00008940: 656e 6465 207a 756d 2041 626d 656c 6465  ende zum Abmelde
+00008950: 6461 7475 6d20 7775 7264 6520 6175 733c  datum wurde aus<
+00008960: 2f74 6578 743e 0a3c 7465 7874 2074 6578  /text>.<text tex
+00008970: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00008980: 2078 3d22 3134 3037 2220 793d 222d 3237   x="1407" y="-27
+00008990: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+000089a0: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+000089b0: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
+000089c0: 676c 6569 6368 656d 2047 7275 6e64 2062  gleichem Grund b
+000089d0: 6572 6569 7473 2062 6573 7426 2332 3238  ereits best&#228
+000089e0: 3b74 6967 742e 3c2f 7465 7874 3e0a 3c2f  ;tigt.</text>.</
+000089f0: 673e 0a3c 212d 2d20 3133 2623 3435 3b26  g>.<!-- 13&#45;&
+00008a00: 6774 3b41 3038 202d 2d3e 0a3c 6720 6964  gt;A08 -->.<g id
+00008a10: 3d22 6564 6765 3236 2220 636c 6173 733d  ="edge26" class=
+00008a20: 2265 6467 6522 3e0a 3c74 6974 6c65 3e31  "edge">.<title>1
+00008a30: 332d 2667 743b 4130 383c 2f74 6974 6c65  3-&gt;A08</title
+00008a40: 3e0a 3c70 6174 6820 6669 6c6c 3d22 6e6f  >.<path fill="no
+00008a50: 6e65 2220 7374 726f 6b65 3d22 626c 6163  ne" stroke="blac
+00008a60: 6b22 2064 3d22 4d31 3633 342e 3137 2c2d  k" d="M1634.17,-
+00008a70: 3136 302e 3633 4331 3631 352e 3036 2c2d  160.63C1615.06,-
+00008a80: 3134 302e 3537 2031 3539 342e 3432 2c2d  140.57 1594.42,-
+00008a90: 3131 382e 3920 3135 3736 2e39 2c2d 3130  118.9 1576.9,-10
+00008aa0: 302e 3531 222f 3e0a 3c70 6f6c 7967 6f6e  0.51"/>.<polygon
+00008ab0: 2066 696c 6c3d 2262 6c61 636b 2220 7374   fill="black" st
+00008ac0: 726f 6b65 3d22 626c 6163 6b22 2070 6f69  roke="black" poi
+00008ad0: 6e74 733d 2231 3537 392e 3537 2c2d 3938  nts="1579.57,-98
+00008ae0: 2e32 3420 3135 3730 2e31 342c 2d39 332e  .24 1570.14,-93.
+00008af0: 3431 2031 3537 342e 352c 2d31 3033 2e30  41 1574.5,-103.0
+00008b00: 3620 3135 3739 2e35 372c 2d39 382e 3234  6 1579.57,-98.24
+00008b10: 222f 3e0a 3c74 6578 7420 7465 7874 2d61  "/>.<text text-a
+00008b20: 6e63 686f 723d 226d 6964 646c 6522 2078  nchor="middle" x
+00008b30: 3d22 3136 3331 2e35 2220 793d 222d 3133  ="1631.5" y="-13
+00008b40: 312e 3822 2066 6f6e 742d 6661 6d69 6c79  1.8" font-family
+00008b50: 3d22 5469 6d65 732c 7365 7269 6622 2066  ="Times,serif" f
+00008b60: 6f6e 742d 7369 7a65 3d22 3134 2e30 3022  ont-size="14.00"
+00008b70: 3e4e 6569 6e3c 2f74 6578 743e 0a3c 2f67  >Nein</text>.</g
+00008b80: 3e0a 3c21 2d2d 2041 3039 202d 2d3e 0a3c  >.<!-- A09 -->.<
+00008b90: 6720 6964 3d22 6e6f 6465 3233 2220 636c  g id="node23" cl
+00008ba0: 6173 733d 226e 6f64 6522 3e0a 3c74 6974  ass="node">.<tit
+00008bb0: 6c65 3e41 3039 3c2f 7469 746c 653e 0a3c  le>A09</title>.<
+00008bc0: 706f 6c79 676f 6e20 6669 6c6c 3d22 2363  polygon fill="#c
+00008bd0: 6662 3938 3622 2073 7472 6f6b 653d 2262  fb986" stroke="b
+00008be0: 6c61 636b 2220 706f 696e 7473 3d22 3230  lack" points="20
+00008bf0: 3230 2e35 2c2d 3131 3020 3136 3932 2e35  20.5,-110 1692.5
+00008c00: 2c2d 3131 3020 3136 3932 2e35 2c30 2032  ,-110 1692.5,0 2
+00008c10: 3032 302e 352c 3020 3230 3230 2e35 2c2d  020.5,0 2020.5,-
+00008c20: 3131 3022 2f3e 0a3c 7465 7874 2074 6578  110"/>.<text tex
+00008c30: 742d 616e 6368 6f72 3d22 7374 6172 7422  t-anchor="start"
+00008c40: 2078 3d22 3138 3431 2220 793d 222d 3933   x="1841" y="-93
+00008c50: 2e38 2220 666f 6e74 2d66 616d 696c 793d  .8" font-family=
+00008c60: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00008c70: 6e74 2d77 6569 6768 743d 2262 6f6c 6422  nt-weight="bold"
+00008c80: 2066 6f6e 742d 7369 7a65 3d22 3134 2e30   font-size="14.0
+00008c90: 3022 3e41 3039 3c2f 7465 7874 3e0a 3c74  0">A09</text>.<t
+00008ca0: 6578 7420 7465 7874 2d61 6e63 686f 723d  ext text-anchor=
+00008cb0: 2273 7461 7274 2220 783d 2231 3730 342e  "start" x="1704.
+00008cc0: 3522 2079 3d22 2d38 312e 3422 2066 6f6e  5" y="-81.4" fon
+00008cd0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+00008ce0: 7365 7269 6622 2074 6578 742d 6465 636f  serif" text-deco
+00008cf0: 7261 7469 6f6e 3d22 756e 6465 726c 696e  ration="underlin
+00008d00: 6522 2066 6f6e 742d 7369 7a65 3d22 3132  e" font-size="12
+00008d10: 2e30 3022 3e48 696e 7765 6973 3a3c 2f74  .00">Hinweis:</t
+00008d20: 6578 743e 0a3c 7465 7874 2074 6578 742d  ext>.<text text-
+00008d30: 616e 6368 6f72 3d22 7374 6172 7422 2078  anchor="start" x
+00008d40: 3d22 3137 3034 2e35 2220 793d 222d 3639  ="1704.5" y="-69
+00008d50: 2e34 2220 666f 6e74 2d66 616d 696c 793d  .4" font-family=
+00008d60: 2254 696d 6573 2c73 6572 6966 2220 666f  "Times,serif" fo
+00008d70: 6e74 2d73 697a 653d 2231 322e 3030 223e  nt-size="12.00">
+00008d80: 436c 7573 7465 723a 205a 7573 7469 6d6d  Cluster: Zustimm
+00008d90: 756e 673c 2f74 6578 743e 0a3c 7465 7874  ung</text>.<text
+00008da0: 2074 6578 742d 616e 6368 6f72 3d22 7374   text-anchor="st
+00008db0: 6172 7422 2078 3d22 3137 3034 2e35 2220  art" x="1704.5" 
+00008dc0: 793d 222d 3537 2e34 2220 666f 6e74 2d66  y="-57.4" font-f
+00008dd0: 616d 696c 793d 2254 696d 6573 2c73 6572  amily="Times,ser
+00008de0: 6966 2220 666f 6e74 2d73 697a 653d 2231  if" font-size="1
+00008df0: 322e 3030 223e 4572 6e65 7574 6520 4265  2.00">Erneute Be
+00008e00: 7374 2623 3232 383b 7469 6775 6e67 2064  st&#228;tigung d
+00008e10: 6572 2041 626d 656c 6475 6e67 2061 7566  er Abmeldung auf
+00008e20: 6772 756e 6420 6465 723c 2f74 6578 743e  grund der</text>
+00008e30: 0a3c 7465 7874 2074 6578 742d 616e 6368  .<text text-anch
+00008e40: 6f72 3d22 7374 6172 7422 2078 3d22 3137  or="start" x="17
+00008e50: 3034 2e35 2220 793d 222d 3435 2e34 2220  04.5" y="-45.4" 
+00008e60: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00008e70: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00008e80: 697a 653d 2231 322e 3030 223e 496e 666f  ize="12.00">Info
+00008e90: 726d 6174 696f 6e2c 2064 6173 7320 6465  rmation, dass de
+00008ea0: 7220 416e 7363 686c 7573 736e 7574 7a65  r Anschlussnutze
+00008eb0: 7220 6e69 6368 7420 6d65 6872 3c2f 7465  r nicht mehr</te
+00008ec0: 7874 3e0a 3c74 6578 7420 7465 7874 2d61  xt>.<text text-a
+00008ed0: 6e63 686f 723d 2273 7461 7274 2220 783d  nchor="start" x=
+00008ee0: 2231 3730 342e 3522 2079 3d22 2d33 332e  "1704.5" y="-33.
+00008ef0: 3422 2066 6f6e 742d 6661 6d69 6c79 3d22  4" font-family="
+00008f00: 5469 6d65 732c 7365 7269 6622 2066 6f6e  Times,serif" fon
+00008f10: 742d 7369 7a65 3d22 3132 2e30 3022 3e61  t-size="12.00">a
+00008f20: 6e20 6465 7220 4d61 726b 746c 6f6b 6174  n der Marktlokat
+00008f30: 696f 6e20 766f 7268 616e 6465 6e20 6973  ion vorhanden is
+00008f40: 742e 3c2f 7465 7874 3e0a 3c74 6578 7420  t.</text>.<text 
+00008f50: 7465 7874 2d61 6e63 686f 723d 2273 7461  text-anchor="sta
+00008f60: 7274 2220 783d 2231 3730 342e 3522 2079  rt" x="1704.5" y
+00008f70: 3d22 2d32 312e 3422 2066 6f6e 742d 6661  ="-21.4" font-fa
+00008f80: 6d69 6c79 3d22 5469 6d65 732c 7365 7269  mily="Times,seri
+00008f90: 6622 2066 6f6e 742d 7369 7a65 3d22 3132  f" font-size="12
+00008fa0: 2e30 3022 3e48 696e 7765 6973 3a20 4461  .00">Hinweis: Da
+00008fb0: 7320 6269 7368 6572 2062 6573 7426 2332  s bisher best&#2
+00008fc0: 3238 3b74 6967 7465 2042 696c 616e 7a69  28;tigte Bilanzi
+00008fd0: 6572 756e 6773 656e 6465 3c2f 7465 7874  erungsende</text
+00008fe0: 3e0a 3c74 6578 7420 7465 7874 2d61 6e63  >.<text text-anc
+00008ff0: 686f 723d 2273 7461 7274 2220 783d 2231  hor="start" x="1
+00009000: 3730 342e 3522 2079 3d22 2d39 2e34 2220  704.5" y="-9.4" 
+00009010: 666f 6e74 2d66 616d 696c 793d 2254 696d  font-family="Tim
+00009020: 6573 2c73 6572 6966 2220 666f 6e74 2d73  es,serif" font-s
+00009030: 697a 653d 2231 322e 3030 223e 626c 6569  ize="12.00">blei
+00009040: 6274 2075 6e76 6572 2623 3232 383b 6e64  bt unver&#228;nd
+00009050: 6572 7420 6265 7374 6568 656e 2e3c 2f74  ert bestehen.</t
+00009060: 6578 743e 0a3c 2f67 3e0a 3c21 2d2d 2031  ext>.</g>.<!-- 1
+00009070: 3326 2334 353b 2667 743b 4130 3920 2d2d  3&#45;&gt;A09 --
+00009080: 3e0a 3c67 2069 643d 2265 6467 6532 3722  >.<g id="edge27"
+00009090: 2063 6c61 7373 3d22 6564 6765 223e 0a3c   class="edge">.<
+000090a0: 7469 746c 653e 3133 2d26 6774 3b41 3039  title>13-&gt;A09
+000090b0: 3c2f 7469 746c 653e 0a3c 7061 7468 2066  </title>.<path f
+000090c0: 696c 6c3d 226e 6f6e 6522 2073 7472 6f6b  ill="none" strok
+000090d0: 653d 2262 6c61 636b 2220 643d 224d 3137  e="black" d="M17
+000090e0: 3536 2e38 332c 2d31 3630 2e36 3343 3137  56.83,-160.63C17
+000090f0: 3730 2e30 352c 2d31 3436 2e37 3520 3137  70.05,-146.75 17
+00009100: 3834 2c2d 3133 322e 3120 3137 3937 2e31  84,-132.1 1797.1
+00009110: 352c 2d31 3138 2e33 222f 3e0a 3c70 6f6c  5,-118.3"/>.<pol
+00009120: 7967 6f6e 2066 696c 6c3d 2262 6c61 636b  ygon fill="black
+00009130: 2220 7374 726f 6b65 3d22 626c 6163 6b22  " stroke="black"
+00009140: 2070 6f69 6e74 733d 2231 3739 392e 3338   points="1799.38
+00009150: 2c2d 3132 312e 3034 2031 3830 332e 3734  ,-121.04 1803.74
+00009160: 2c2d 3131 312e 3338 2031 3739 342e 3331  ,-111.38 1794.31
+00009170: 2c2d 3131 362e 3231 2031 3739 392e 3338  ,-116.21 1799.38
+00009180: 2c2d 3132 312e 3034 222f 3e0a 3c74 6578  ,-121.04"/>.<tex
+00009190: 7420 7465 7874 2d61 6e63 686f 723d 226d  t text-anchor="m
+000091a0: 6964 646c 6522 2078 3d22 3137 3932 2e35  iddle" x="1792.5
+000091b0: 2220 793d 222d 3133 312e 3822 2066 6f6e  " y="-131.8" fon
+000091c0: 742d 6661 6d69 6c79 3d22 5469 6d65 732c  t-family="Times,
+000091d0: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+000091e0: 3d22 3134 2e30 3022 3e4a 613c 2f74 6578  ="14.00">Ja</tex
+000091f0: 743e 0a3c 2f67 3e0a 3c2f 673e 0a3c 2f73  t>.</g>.</g>.</s
+00009200: 7667 3e0a 2020 3c2f 673e 0a3c 2f73 7667  vg>.  </g>.</svg
+00009210: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
```

### Comparing `ebdtable2graph-0.1.8/unittests/test_ebd_table_models.py` & `ebdtable2graph-0.1.9/unittests/test_ebd_table_models.py`

 * *Files identical despite different names*

### Comparing `ebdtable2graph-0.1.8/unittests/test_table_to_graph.py` & `ebdtable2graph-0.1.9/unittests/test_table_to_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from ebdtable2graph import (
     convert_graph_to_plantuml,
     convert_plantuml_to_svg_kroki,
     convert_table_to_digraph,
     convert_table_to_graph,
 )
-from ebdtable2graph.add_watermark import add_watermark
 from ebdtable2graph.graph_conversion import get_all_edges, get_all_nodes
 from ebdtable2graph.graphviz import convert_dot_to_svg_kroki, convert_graph_to_dot
 from ebdtable2graph.models import EbdGraph, EbdGraphMetaData
 from ebdtable2graph.models.ebd_graph import (
     DecisionNode,
     EbdGraphEdge,
     EbdGraphNode,
@@ -180,34 +179,74 @@
         svg_code = convert_dot_to_svg_kroki(dot_code)  # Raises an error if conversion fails
         os.makedirs(Path(__file__).parent / "output", exist_ok=True)
         with open(
             Path(__file__).parent / "output" / f"{ebd_graph.metadata.ebd_code}.dot.svg", "w+", encoding="utf-8"
         ) as svg_file:
             svg_file.write(svg_code)
 
-    def test_table_to_digraph_dot_with_watermark(self):
+    @pytest.mark.parametrize(
+        "add_background",
+        [
+            pytest.param(
+                True,
+            ),
+            pytest.param(
+                False,
+            ),
+        ],
+    )
+    def test_table_to_digraph_dot_with_watermark(self, add_background):
         ebd_graph = convert_table_to_graph(table_e0003)
         dot_code = convert_graph_to_dot(ebd_graph)
-        svg_code = convert_dot_to_svg_kroki(dot_code, add_watermark=False)  # Raises an error if conversion fails
+        svg_code = convert_dot_to_svg_kroki(
+            dot_code, add_watermark=False, add_background=False
+        )  # Raises an error if conversion fails
         os.makedirs(Path(__file__).parent / "output", exist_ok=True)
 
         with open(
             Path(__file__).parent / "output" / f"{ebd_graph.metadata.ebd_code}_without_watermark.dot.svg",
             "w+",
             encoding="utf-8",
         ) as svg_file:
             svg_file.write(svg_code)
 
-        svg_without_watermark = svg_code.encode("utf-8")
+        svg_code_with_watermark = convert_dot_to_svg_kroki(
+            dot_code, add_watermark=True, add_background=add_background
+        )  # Raises an error if conversion fails
+
+        file_path2 = (
+            Path(__file__).parent
+            / "output"
+            / f"{ebd_graph.metadata.ebd_code}_with_watermark_background_is_{add_background}.dot.svg"
+        )
+        with open(file_path2, "w", encoding="utf-8") as ebd_svg:
+            ebd_svg.write(svg_code_with_watermark)
+
+    def test_table_to_digraph_dot_with_background(self):
+        ebd_graph = convert_table_to_graph(table_e0003)
+        dot_code = convert_graph_to_dot(ebd_graph)
+        svg_code = convert_dot_to_svg_kroki(
+            dot_code, add_watermark=False, add_background=False
+        )  # Raises an error if conversion fails
+        os.makedirs(Path(__file__).parent / "output", exist_ok=True)
+
+        with open(
+            Path(__file__).parent / "output" / f"{ebd_graph.metadata.ebd_code}_without_watermark.dot.svg",
+            "w+",
+            encoding="utf-8",
+        ) as svg_file:
+            svg_file.write(svg_code)
 
-        svg_with_watermark = add_watermark(svg_without_watermark)
+        svg_code = convert_dot_to_svg_kroki(
+            dot_code, add_watermark=False, add_background=True
+        )  # Raises an error if conversion fails
 
-        file_path2 = Path(__file__).parent / "output" / f"{ebd_graph.metadata.ebd_code}_with_watermark.dot.svg"
+        file_path2 = Path(__file__).parent / "output" / f"{ebd_graph.metadata.ebd_code}_with_background.dot.svg"
         with open(file_path2, "w", encoding="utf-8") as ebd_svg:
-            ebd_svg.write(svg_with_watermark.decode())
+            ebd_svg.write(svg_code)
 
     def test_table_e0401_too_complex_for_plantuml(self):
         """
         Test the conversion pipeline for E_0401. In this case the plantuml conversion should fail because the graph is
         too complex for this implementation.
         """
         with pytest.raises(AssertionError) as exc:
```

