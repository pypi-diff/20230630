# Comparing `tmp/happi-2.2.0.tar.gz` & `tmp/happi-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happi-2.2.0.tar", last modified: Tue May  9 00:02:29 2023, max compression
+gzip compressed data, was "happi-2.3.0.tar", last modified: Fri Jun 30 20:52:47 2023, max compression
```

## Comparing `happi-2.2.0.tar` & `happi-2.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.753220 happi-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-09 00:02:12.000000 happi-2.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-05-09 00:02:12.000000 happi-2.2.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-09 00:02:12.000000 happi-2.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-09 00:02:12.000000 happi-2.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.733220 happi-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-05-09 00:02:12.000000 happi-2.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-09 00:02:12.000000 happi-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.733220 happi-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-09 00:02:12.000000 happi-2.2.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-09 00:02:12.000000 happi-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      279 2023-05-09 00:02:12.000000 happi-2.2.0/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-09 00:02:12.000000 happi-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-09 00:02:12.000000 happi-2.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-05-09 00:02:12.000000 happi-2.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-09 00:02:12.000000 happi-2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-09 00:02:12.000000 happi-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-05-09 00:02:29.753220 happi-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-09 00:02:12.000000 happi-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.737220 happi-2.2.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/activate.sh
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/deactivate.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-09 00:02:12.000000 happi-2.2.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-05-09 00:02:12.000000 happi-2.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.737220 happi-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-09 00:02:12.000000 happi-2.2.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-05-09 00:02:12.000000 happi-2.2.0/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-05-09 00:02:12.000000 happi-2.2.0/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7422 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/client.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/containers.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    23277 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-09 00:02:12.000000 happi-2.2.0/docs/source/upcoming_release_notes/template-short.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      929 2023-05-09 00:02:12.000000 happi-2.2.0/examples/db.json
--rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-05-09 00:02:12.000000 happi-2.2.0/examples/launch_edl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.741220 happi-2.2.0/examples/qt/
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-09 00:02:12.000000 happi-2.2.0/examples/qt/listview.py
--rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-05-09 00:02:12.000000 happi-2.2.0/examples/qt/treeview.py
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-05-09 00:02:12.000000 happi-2.2.0/github_deploy_key_pcdshub_happi.enc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.745220 happi-2.2.0/happi/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-09 00:02:12.000000 happi-2.2.0/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 00:02:12.000000 happi-2.2.0/happi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:29.000000 happi-2.2.0/happi/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-09 00:02:12.000000 happi-2.2.0/happi/audit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi/backends/
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/json_db.py
--rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/multi_db.py
--rw-r--r--   0 runner    (1001) docker     (122)    15490 2023-05-09 00:02:12.000000 happi-2.2.0/happi/backends/qs_db.py
--rw-r--r--   0 runner    (1001) docker     (122)    38591 2023-05-09 00:02:12.000000 happi-2.2.0/happi/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    29883 2023-05-09 00:02:12.000000 happi-2.2.0/happi/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-05-09 00:02:12.000000 happi-2.2.0/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-09 00:02:12.000000 happi-2.2.0/happi/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-05-09 00:02:12.000000 happi-2.2.0/happi/item.py
--rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-05-09 00:02:12.000000 happi-2.2.0/happi/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     7221 2023-05-09 00:02:12.000000 happi-2.2.0/happi/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi/qt/
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-09 00:02:12.000000 happi-2.2.0/happi/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-05-09 00:02:12.000000 happi-2.2.0/happi/qt/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.753220 happi-2.2.0/happi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19157 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_audit.py
--rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)    24416 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    12850 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_happi_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     6602 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-09 00:02:12.000000 happi-2.2.0/happi/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-05-09 00:02:12.000000 happi-2.2.0/happi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-09 00:02:12.000000 happi-2.2.0/happi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:29.749220 happi-2.2.0/happi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-09 00:02:29.000000 happi-2.2.0/happi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-09 00:02:12.000000 happi-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-09 00:02:12.000000 happi-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 00:02:29.753220 happi-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.833547 happi-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-30 20:52:22.000000 happi-2.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-06-30 20:52:22.000000 happi-2.3.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-30 20:52:22.000000 happi-2.3.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-30 20:52:22.000000 happi-2.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.817547 happi-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-30 20:52:22.000000 happi-2.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-30 20:52:22.000000 happi-2.3.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.817547 happi-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-30 20:52:22.000000 happi-2.3.0/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-06-30 20:52:22.000000 happi-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-06-30 20:52:22.000000 happi-2.3.0/.landscape.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-06-30 20:52:22.000000 happi-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-30 20:52:22.000000 happi-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-06-30 20:52:22.000000 happi-2.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-30 20:52:22.000000 happi-2.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 20:52:22.000000 happi-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-06-30 20:52:47.833547 happi-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-30 20:52:22.000000 happi-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.821547 happi-2.3.0/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-30 20:52:22.000000 happi-2.3.0/conda-recipe/activate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-30 20:52:22.000000 happi-2.3.0/conda-recipe/deactivate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-30 20:52:22.000000 happi-2.3.0/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-30 20:52:22.000000 happi-2.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.821547 happi-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-06-30 20:52:22.000000 happi-2.3.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-06-30 20:52:22.000000 happi-2.3.0/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-06-30 20:52:22.000000 happi-2.3.0/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.821547 happi-2.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7422 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/client.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    24283 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.821547 happi-2.3.0/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-30 20:52:22.000000 happi-2.3.0/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-30 20:52:22.000000 happi-2.3.0/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.821547 happi-2.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-06-30 20:52:22.000000 happi-2.3.0/examples/db.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-06-30 20:52:22.000000 happi-2.3.0/examples/launch_edl.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.825547 happi-2.3.0/examples/qt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-30 20:52:22.000000 happi-2.3.0/examples/qt/listview.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-06-30 20:52:22.000000 happi-2.3.0/examples/qt/treeview.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.825547 happi-2.3.0/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-30 20:52:22.000000 happi-2.3.0/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-30 20:52:22.000000 happi-2.3.0/happi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-30 20:52:47.000000 happi-2.3.0/happi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-30 20:52:22.000000 happi-2.3.0/happi/audit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.829548 happi-2.3.0/happi/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10360 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/json_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/multi_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15490 2023-06-30 20:52:22.000000 happi-2.3.0/happi/backends/qs_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41731 2023-06-30 20:52:22.000000 happi-2.3.0/happi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30040 2023-06-30 20:52:22.000000 happi-2.3.0/happi/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-06-30 20:52:22.000000 happi-2.3.0/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-30 20:52:22.000000 happi-2.3.0/happi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-06-30 20:52:22.000000 happi-2.3.0/happi/item.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-06-30 20:52:22.000000 happi-2.3.0/happi/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7221 2023-06-30 20:52:22.000000 happi-2.3.0/happi/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.829548 happi-2.3.0/happi/qt/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-30 20:52:22.000000 happi-2.3.0/happi/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6352 2023-06-30 20:52:22.000000 happi-2.3.0/happi/qt/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.833547 happi-2.3.0/happi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19157 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_audit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24479 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12850 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_happi_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6602 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-30 20:52:22.000000 happi-2.3.0/happi/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-06-30 20:52:22.000000 happi-2.3.0/happi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-06-30 20:52:22.000000 happi-2.3.0/happi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:52:47.829548 happi-2.3.0/happi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-30 20:52:47.000000 happi-2.3.0/happi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-30 20:52:22.000000 happi-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-30 20:52:22.000000 happi-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 20:52:47.833547 happi-2.3.0/setup.cfg
```

### Comparing `happi-2.2.0/.flake8` & `happi-2.3.0/.flake8`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/.github/ISSUE_TEMPLATE.md` & `happi-2.3.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `happi-2.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/.github/workflows/standard.yml` & `happi-2.3.0/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/.gitignore` & `happi-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/.pre-commit-config.yaml` & `happi-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/CONTRIBUTING.rst` & `happi-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/LICENSE.md` & `happi-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/PKG-INFO` & `happi-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happi
-Version: 2.2.0
+Version: 2.3.0
 Summary: Happi Database Access for LCLS Beamline Devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,14 +45,15 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 <h1 align="center">HAPPI</h1>
 
 <div align="center">
   <strong>Heuristic Access to Positioning of Photon Instrumentation</strong>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: happi Version: 2.2.0 Summary: Happi Database Access
+Metadata-Version: 2.1 Name: happi Version: 2.3.0 Summary: Happi Database Access
 for LCLS Beamline Devices Author: SLAC National Accelerator Laboratory License:
 Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt of
 any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: (1)
 Redistributions of source code must retain the above copyright notice, this
@@ -30,16 +30,16 @@
 without imposing a separate written license agreement for such Enhancements,
 then you hereby grant the following license: a non-exclusive, royalty-free
 perpetual license to install, use, modify, prepare derivative works,
 incorporate into other computer software, distribute, and sublicense such
 Enhancements or derivative works thereof, in binary and source code form.
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.9
-Description-Content-Type: text/markdown Provides-Extra: test License-File:
-LICENSE.md License-File: AUTHORS.rst
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+doc License-File: LICENSE.md License-File: AUTHORS.rst
                               ****** HAPPI ******
            Heuristic Access to Positioning of Photon Instrumentation
   Motivation â¢ Features â¢ Installation â¢ Basic_Usage â¢ Documentation
 ## Motivation LCLS endstations deal with dynamic sets of instrumentation.
 Information like ports, triggers and aliases are all important for operation,
 but hard to manage when spread across a multitude of applications. **Happi**
 solves this problem by creating a single access point for all the metadata
```

### Comparing `happi-2.2.0/README.md` & `happi-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/conda-recipe/meta.yaml` & `happi-2.3.0/conda-recipe/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - setuptools_scm
   run:
   - python >=3.9
   - click
   - coloredlogs
   - entrypoints
   - jinja2
+  - platformdirs
   - prettytable
   - simplejson
   run-constrained:
   - psdm_qs_cli >=0.3.1
   - pymongo >=4.0.2
```

### Comparing `happi-2.2.0/docs/Makefile` & `happi-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/pre-release-notes.sh` & `happi-2.3.0/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/release_notes.py` & `happi-2.3.0/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/api.rst` & `happi-2.3.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/client.rst` & `happi-2.3.0/docs/source/client.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/conf.py` & `happi-2.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/containers.rst` & `happi-2.3.0/docs/source/containers.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/index.rst` & `happi-2.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/docs/source/releases.rst` & `happi-2.3.0/docs/source/releases.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,40 @@
 Release History
 ###############
 
 
+v2.3.0 (2023-06-30)
+===================
+
+Features
+--------
+- CLI command ``happi config edit`` - open config file in ``$EDITOR``
+- CLI command ``happi config init`` - create new config file with default options
+- CLI command ``happi config show`` - show location & contents of config file
+- Extend the config searching mechanism to check the platformdirs config directory.
+  The happi config file path is taken from the ``HAPPI_CFG`` environment variable,
+  but if the variable is not set then the following locations are searched in order
+  for files named ``.happi.cfg`` or ``happi.cfg``:
+
+  - The location specified by the ``XDG_CONFIG_HOME`` environment variable
+  - ``~/.config``
+  - (**new**) The location specified by ``platformdirs.user_config_dir("happi")``
+
+Maintenance
+-----------
+- Add dependency on `platformdirs <https://pypi.org/project/platformdirs/>`_.
+- Update build requirements to use pip-provided extras for documentation and test builds
+
+Contributors
+------------
+- tangkong
+- untzag
+
+
+
 v2.2.0 (2023-05-08)
 ===================
 
 Features
 --------
 - Adds a hook in ``happi.loader.from_container`` that runs the method
   ``post_happi_md`` on an instantiated object after the metadata
@@ -463,15 +492,15 @@
 
 
 v1.6.0 (2020-04-30)
 ===================
 
 -  LCLS-specific containers are moved out of happi, and into
    `pcdsdevices <https://github.com/pcdshub/pcdsdevices/tree/master/pcdsdevices/happi>`__
--  ``OphydItem`` is now the preferred “basic” ``ophyd.Device``
+-  ``OphydItem`` is now the preferred basic ``ophyd.Device``
    container, with the intention of fully deprecating ``Device`` to
    avoid naming confusion
 -  Minor internal fixes
 
 
 v1.5.0 (2020-04-06)
 ===================
@@ -504,21 +533,21 @@
 
 v1.4.0 (2020-03-13)
 ===================
 
 Enhancements
 ------------
 
--  Add an add command for cli, e.g. happi add to start an interactive
+-  Add an add command for cli, e.g. ``happi add`` to start an interactive
    device adder
--  Add an edit command for cli, e.g. happi edit im3l0 location=750
+-  Add an edit command for cli, e.g. ``happi edit im3l0 location=750``
    prefix=IM3L0:PPM
 -  Change search command syntax to be simpler (more like edit)
--  Add a load command for cli, e.g. happi load im3l0 im1l1 -> IPython
-   session plus other changes made in dev to “get it working”
+-  Add a load command for cli, e.g. ``happi load im3l0 im1l1`` -> IPython
+   session plus other changes made in dev to get it working
 -  Add two new Happi-aware Qt widgets: HappiDeviceListView &
    HappiDeviceTreeView
 
 Bug Fixes
 ---------
 
 -  Initialize database if it does not yet exists
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `happi-2.2.0/docs/source/upcoming_release_notes/template-full.rst` & `happi-2.3.0/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/examples/db.json` & `happi-2.3.0/examples/db.json`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/examples/launch_edl.py` & `happi-2.3.0/examples/launch_edl.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/examples/qt/listview.py` & `happi-2.3.0/examples/qt/listview.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/examples/qt/treeview.py` & `happi-2.3.0/examples/qt/treeview.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/audit.py` & `happi-2.3.0/happi/audit.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/backends/__init__.py` & `happi-2.3.0/happi/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/backends/core.py` & `happi-2.3.0/happi/backends/core.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/backends/json_db.py` & `happi-2.3.0/happi/backends/json_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     The happi information is kept in a single large dictionary that is stored
     using the ``simplejson`` package.
 
     Parameters
     ----------
     path : str
         Path to JSON file.
-    initialze : bool, optional
+    initialize : bool, optional
         Initialize a new empty JSON file to begin filling.
     cfg_path : str, optional
         Path to the happi config.
     """
 
     def __init__(
         self,
```

### Comparing `happi-2.2.0/happi/backends/mongo_db.py` & `happi-2.3.0/happi/backends/mongo_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/backends/multi_db.py` & `happi-2.3.0/happi/backends/multi_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/backends/qs_db.py` & `happi-2.3.0/happi/backends/qs_db.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/cli.py` & `happi-2.3.0/happi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 import inspect
 import io
 import json
 import logging
 import os
 # on import allows arrow key navigation in prompt
 import readline  # noqa
+import subprocess
 import sys
 import time
 from contextlib import contextmanager, redirect_stderr, redirect_stdout
 from cProfile import Profile
 from pathlib import Path
 
 import click
 import coloredlogs
+import platformdirs
 import prettytable
 
 import happi
 from happi.errors import SearchError
 
 from .audit import (checks, find_unfilled_mandatory_info,
                     find_unfilled_optional_info, verify_result)
@@ -34,14 +36,27 @@
 
 logger = logging.getLogger(__name__)
 
 version_msg = f'Happi: Version {happi.__version__} from {happi.__file__}'
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
+def get_happi_client_from_config(path):
+    # gather client
+    try:
+        client = happi.client.Client.from_config(path)
+        logger.debug("Happi client: %r" % client)
+        # insert items into context to be passed to subcommands
+        # User objects must be assigned to ctx.obj, which will be passed
+        # through to new context objects
+        return client
+    except OSError:
+        logger.debug("Happi configuration not found.")
+
+
 @click.group(
     help=('The happi command-line interface, used to view and manipulate '
           'device databases'),
     context_settings=CONTEXT_SETTINGS
 )
 @click.option('--path', type=click.Path(exists=True),
               help='Provide the path to happi configuration file. '
@@ -60,22 +75,15 @@
     else:
         shown_logger = logging.getLogger('happi')
         level = "INFO"
     coloredlogs.install(level=level, logger=shown_logger,
                         fmt='[%(asctime)s] - %(levelname)s -  %(message)s')
     logger.debug("Set logging level of %r to %r", shown_logger.name, level)
 
-    # gather client
-    client = happi.client.Client.from_config(cfg=path)
-    logger.debug("Happi client: %r" % client)
-
-    # insert items into context to be passed to subcommands
-    # User objects must be assigned to ctx.obj, which will be passed
-    # through to new context objects
-    ctx.obj = client
+    ctx.obj = path
 
     # Cleanup tasks related to loaded devices
     @ctx.call_on_close
     def device_cleanup():
         pyepics_cleanup()
         ophyd_cleanup()
 
@@ -102,15 +110,15 @@
     If 'field=' is omitted, it will assumed to be 'name'.
     You may include as many search criteria as you like; these will
     be combined with ANDs.
     """
     logger.debug("We're in the search block")
 
     final_results = search_parser(
-        client=ctx.obj,
+        client=get_happi_client_from_config(ctx.obj),
         use_glob=use_glob,
         search_criteria=search_criteria,
     )
     if not final_results:
         return []
 
     # Final processing for output
@@ -237,15 +245,15 @@
               help='Copy the fields from an existing container. '
               'Provide the name of the item to clone.')
 @click.pass_context
 def add(ctx, clone: str):
     """Add new entries or copy existing entries."""
     logger.debug(f'Starting interactive add, {clone}')
     # retrieve client
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
 
     registry = happi.containers.registry
     if clone:
         clone_source = client.find_item(name=clone)
         # Must use the same container if cloning
         response = registry.entry_for_class(clone_source.__class__)
     else:
@@ -304,15 +312,15 @@
 @happi_cli.command()
 @click.argument('name', type=str)
 @click.pass_context
 def delete(ctx, name: str):
     """
     Delete an existing entry.  Only accepts exact names
     """
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
     try:
         item = client.find_item(name=name)
     except SearchError as e:
         raise click.ClickException(f'Could not find item ({name}): {e}')
 
     item.show_info()
     if click.confirm('Are you sure you want to delete this entry? \n'
@@ -332,15 +340,15 @@
 def edit(ctx, name: str, edits: list[str]):
     """
     Change an existing entry.
 
     Applies EDITS of the form: field=value to the item of name NAME.
     """
     # retrieve client
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
 
     logger.debug('Starting edit block')
     try:
         item = client.find_item(name=name)
     except SearchError as e:
         raise click.ClickException(f'Could not find item {name!r}: {e}')
 
@@ -390,15 +398,15 @@
 @click.argument('item_names', nargs=-1)
 @click.pass_context
 def load(ctx, item_names: list[str]):
     """Open IPython terminal with ITEM_NAMES loaded."""
 
     logger.debug('Starting load block')
     # retrieve client
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
 
     devices = {}
     names = " ".join(item_names)
     names = names.split()
     if len(names) < 1:
         raise click.BadArgumentUsage('No item names given')
     logger.info(f'Creating shell with devices {item_names}')
@@ -425,15 +433,15 @@
 # translate exactly
 @happi_cli.command()
 @click.argument("json_data", nargs=-1)
 @click.pass_context
 def update(ctx, json_data: str):
     """Update happi db with JSON_DATA payload."""
     # retrieve client
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
     if len(json_data) < 1:
         raise click.BadArgumentUsage('No json data given')
 
     # parse input
     input_ = " ".join(json_data).strip()
     print(json_data)
     if input_ == "-":
@@ -468,15 +476,15 @@
     """
     Change the container of an item.
 
     Transfers item (NAME) to a new container (TARGET)
     """
     logger.debug('Starting transfer block')
     # retrive client
-    client = ctx.obj
+    client = get_happi_client_from_config(ctx.obj)
     # verify name and target both exist and are valid
     try:
         item = client.find_item(name=name)
     except SearchError as e:
         raise click.ClickException(str(e))
     registry = happi.containers.registry
     # This is slow if dictionary is large
@@ -542,15 +550,15 @@
     (wait_connected) to see the full time until the device is fully ready
     to go, presuming the device has a wait_for_connection method.
 
     Search terms are standard as in the same search terms as the search
     cli function. A blank search term means to load all the devices.
     """
     logger.debug('Starting benchmark block')
-    client: happi.Client = ctx.obj
+    client: happi.Client = get_happi_client_from_config(ctx.obj)
     full_stats = []
     logger.info('Collecting happi items...')
     start = time.monotonic()
     if search_criteria:
         items = search_parser(
             client=client,
             use_glob=use_glob,
@@ -732,15 +740,15 @@
 
     Search terms are standard as in the same search terms as the search
     cli function. A blank search term means to load all the devices.
     """
     logger.debug('Starting profile block')
     if profiler not in ('auto', 'pcdsutils', 'cprofile'):
         raise RuntimeError(f'Invalid profiler selection {profiler}')
-    client: happi.Client = ctx.obj
+    client: happi.Client = get_happi_client_from_config(ctx.obj)
     if profile_all:
         profile_database = True
         profile_import = True
         profile_object = True
     if not any((profile_database, profile_import, profile_object)):
         raise RuntimeError('No profile options selected!')
     if profiler == 'auto':
@@ -1003,15 +1011,15 @@
                     f'one check.  Matches: ({[ch.__name__ for ch in matches]})'
                 )
             check_list.append(matches[0])
     else:
         # take all checks
         check_list = checks
 
-    client: happi.Client = ctx.obj
+    client: happi.Client = get_happi_client_from_config(ctx.obj)
 
     results = search_parser(client, use_glob, search_criteria)
     logger.info(f'found {len(results)} items to verify')
     logger.info(f'running checks: {[f.__name__ for f in check_list]}')
 
     test_results = {'name': [], 'success': [], 'check': [], 'msg': []}
     f = io.StringIO()
@@ -1093,15 +1101,15 @@
     """
     Repair the database.
 
     Repairs all entries matching SEARCH_CRITERIA, repairs entire database otherwise.
     """
     logger.debug('starting repair block')
 
-    client: happi.Client = ctx.obj
+    client: happi.Client = get_happi_client_from_config(ctx.obj)
     if search_criteria:
         results = search_parser(client, use_glob, search_criteria)
     else:
         # run repair on all items
         results = search_parser(client, True, '*')
 
     for res in results:
@@ -1129,10 +1137,91 @@
         except KeyboardInterrupt:
             # Finish the current save if interrupted
             logger.warning('caught keyboard interrupt, finishing')
             res.item.save()
             break
 
 
+@click.group(help="Commands related to the happi config file.")
+def config():
+    pass
+
+
+@config.command(name="edit")
+def edit_config():
+    """Open happi configuration file for editing."""
+    config_filepath = happi.client.Client.find_config()
+    if sys.platform.startswith("win32"):
+        import shutil
+        editor = shutil.which(os.environ.get("EDITOR", "notepad.exe"))
+        subprocess.run([editor, config_filepath])
+    else:
+        subprocess.run([os.environ.get("EDITOR", "vi"), config_filepath])
+
+
+@config.command()
+@click.option("--overwrite/--no-overwrite", "overwrite", default=False,
+              help="Overwrite existing config.")
+@click.option("--backend", type=click.Choice(["json"], case_sensitive=False), default="json")
+def init(overwrite, backend):
+    """Create configuration file with default options."""
+
+    # find config_filepath
+    try:
+        config_filepath = Path(happi.client.Client.find_config())
+    except OSError:
+        config_filepath = Path(platformdirs.user_config_dir("happi")) / "happi.cfg"
+    else:
+        if not overwrite:
+            click.echo("Found existing config file at:")
+            click.echo(f"  {config_filepath}")
+            click.echo("Stopping! Use --overwrite to destroy this config file.")
+            return
+    click.echo("Creating new config file at:")
+    click.echo(f"  {config_filepath}")
+
+    # find database_filepath
+    database_filepath = Path(platformdirs.user_data_dir("happi")) / "db.json"
+    if database_filepath.exists():
+        click.echo("Using existing database file at:")
+    else:
+        click.echo("Creating new database file at:")
+
+    click.echo(f"  {database_filepath}")
+
+    # create config file
+    config_filepath.parent.mkdir(parents=True, exist_ok=True)
+    with open(config_filepath, "w") as f:
+        f.write("[DEFAULT]\n")
+        f.write(f"path={database_filepath}\n")
+
+    # create database file
+    database_filepath.parent.mkdir(parents=True, exist_ok=True)
+    database_filepath.touch(exist_ok=True)
+
+    click.echo("Done!")
+
+
+@config.command()
+def show():
+    """Show configuration file in current state."""
+    config_filepath = Path(happi.client.Client.find_config())
+    click.echo(f"File: {config_filepath}")
+
+    def draw_line():
+        try:
+            click.echo("-"*os.get_terminal_size()[0])
+        except OSError:
+            # non-interactive mode (piping results). No max width
+            click.echo("-"*79)
+
+    draw_line()
+    with open(config_filepath, "r") as f:
+        for line in f:
+            click.echo(line.strip())
+    draw_line()
+
+
 def main():
     """Execute the ``happi_cli`` with command line arguments"""
+    happi_cli.add_command(config)
     happi_cli()
```

### Comparing `happi-2.2.0/happi/client.py` & `happi-2.3.0/happi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import os
 import re
 import sys
 import time as ttime
 from collections.abc import Sequence
 from typing import Any, Optional
 
+import platformdirs
+
 from . import containers
 from .backends import BACKENDS, DEFAULT_BACKEND
 from .backends.core import _Backend
 from .errors import DatabaseError, EntryError, SearchError, TransferError
 from .item import HappiItem
 from .loader import from_container
 
@@ -890,22 +892,25 @@
         if os.environ.get('HAPPI_CFG', False):
             happi_cfg = os.environ.get('HAPPI_CFG')
             logger.debug("Found $HAPPI_CFG specification for Client "
                          "configuration at %s", happi_cfg)
             return happi_cfg
         # Search in the current directory and home directory
         else:
-            config_dir = (os.environ.get('XDG_CONFIG_HOME')
-                          or os.path.expanduser('~/.config'))
-            logger.debug('Searching for Happi config in %s', config_dir)
-            for path in ('.happi.cfg', 'happi.cfg'):
-                full_path = os.path.join(config_dir, path)
-                if os.path.exists(full_path):
-                    logger.debug("Found configuration file at %r", full_path)
-                    return full_path
+            config_dirs = [os.environ.get('XDG_CONFIG_HOME', "."),
+                           os.path.expanduser('~/.config'),
+                           platformdirs.user_config_dir("happi")]
+            for directory in config_dirs:
+                logger.debug('Searching for Happi config in %s', directory)
+                for path in ('.happi.cfg', 'happi.cfg'):
+                    full_path = os.path.join(directory, path)
+
+                    if os.path.exists(full_path):
+                        logger.debug("Found configuration file at %r", full_path)
+                        return full_path
         # If found nothing
         raise OSError("No happi configuration file found. Check HAPPI_CFG.")
 
     def choices_for_field(self, field):
         """
         List all choices for a given field.
```

### Comparing `happi-2.2.0/happi/containers.py` & `happi-2.3.0/happi/containers.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/errors.py` & `happi-2.3.0/happi/errors.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/item.py` & `happi-2.3.0/happi/item.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/loader.py` & `happi-2.3.0/happi/loader.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/prompt.py` & `happi-2.3.0/happi/prompt.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/qt/model.py` & `happi-2.3.0/happi/qt/model.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/conftest.py` & `happi-2.3.0/happi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_audit.py` & `happi-2.3.0/happi/tests/test_audit.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_backends.py` & `happi-2.3.0/happi/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_cli.py` & `happi-2.3.0/happi/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,31 +93,31 @@
     assert result.exit_code == 0
     assert result.exception is None
     assert 'Usage:' in result.output
     assert 'Options:' in result.output
     assert 'Commands:' in result.output
 
 
-def test_search(client: happi.client.Client):
+def test_search(client: happi.client.Client, happi_cfg: str):
     res = client.search_regex(beamline="TST")
 
-    with search.make_context('search', ['beamline=TST'], obj=client) as ctx:
+    with search.make_context('search', ['beamline=TST'], obj=happi_cfg) as ctx:
         res_cli = search.invoke(ctx)
 
     assert [r.item for r in res] == [r.item for r in res_cli]
 
 
 def test_search_with_name(
     client: happi.client.Client,
     runner: CliRunner,
     happi_cfg: str
 ):
     res = client.search_regex(name='TST_BASE_PIM2')
 
-    with search.make_context('search', ['TST_BASE_PIM2'], obj=client) as ctx:
+    with search.make_context('search', ['TST_BASE_PIM2'], obj=happi_cfg) as ctx:
         res_cli = search.invoke(ctx)
 
     assert [r.item for r in res] == [r.item for r in res_cli]
     # test duplicate search parameters
     bad_result = runner.invoke(happi_cli, ['--path', happi_cfg,
                                            'search', 'TST_BASE_PIM2',
                                            'name=TST_BASE_PIM2'])
@@ -132,30 +132,30 @@
 
     regex_result = runner.invoke(happi_cli, ['--path', happi_cfg, 'search',
                                  '--names', '--regex', r'tst_.*\d'])
 
     assert glob_result.output == regex_result.output
 
 
-def test_search_z(client: happi.client.Client):
+def test_search_z(happi_cfg: str, client: happi.client.Client):
     res = client.search_regex(z="6.0")
-    with search.make_context('search', ['z=6.0'], obj=client) as ctx:
+    with search.make_context('search', ['z=6.0'], obj=happi_cfg) as ctx:
         res_cli = search.invoke(ctx)
 
     assert [r.item for r in res] == [r.item for r in res_cli]
 
 
 def test_search_z_range(
     client: happi.client.Client,
     runner: CliRunner,
     happi_cfg: str
 ):
     res = client.search_range('z', 3.0, 6.0)
 
-    with search.make_context('search', ['z=3.0,6.0'], obj=client) as ctx:
+    with search.make_context('search', ['z=3.0,6.0'], obj=happi_cfg) as ctx:
         res_cli = search.invoke(ctx)
 
     assert [r.item for r in res] == [r.item for r in res_cli]
 
     # test range intersection
     result = runner.invoke(happi_cli, ['--path', happi_cfg, 'search',
                            '--names', 'z=3.0,6.1', 'y=9.0,12.0'])
@@ -204,21 +204,21 @@
     #                            'search', '--names', 'z=3'])
     # float_result = runner.invoke(happi_cli, ['--path', happi_cfg,
     #                              'search', '--names', 'z=3.0'])
     # assert int_result.output == ''
     # assert float_result.output == ''
 
 
-def test_both_range_and_regex_search(client: happi.client.Client):
+def test_both_range_and_regex_search(happi_cfg: str, client: happi.client.Client):
     # we're only interested in getting this entry (TST_BASE_PIM2)
     res = client.search_regex(z='6.0')
     # we're going to search for z=3,7 name=TST_BASE_PIM2
     # we should only get in return one entry, even though the z value found 2
     with search.make_context('search', ['name=TST_BASE_PIM2', 'z=3.0,7.0'],
-                             obj=client) as ctx:
+                             obj=happi_cfg) as ctx:
         res_cli = search.invoke(ctx)
 
     assert [r.item for r in res] == [r.item for r in res_cli]
 
 
 def test_search_json(runner: CliRunner, happi_cfg: str):
     expected_output = '''[
```

### Comparing `happi-2.2.0/happi/tests/test_client.py` & `happi-2.3.0/happi/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_happi_item.py` & `happi-2.3.0/happi/tests/test_happi_item.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_loader.py` & `happi-2.3.0/happi/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/tests/test_prompt.py` & `happi-2.3.0/happi/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/utils.py` & `happi-2.3.0/happi/utils.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi/version.py` & `happi-2.3.0/happi/version.py`

 * *Files identical despite different names*

### Comparing `happi-2.2.0/happi.egg-info/PKG-INFO` & `happi-2.3.0/happi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happi
-Version: 2.2.0
+Version: 2.3.0
 Summary: Happi Database Access for LCLS Beamline Devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,14 +45,15 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 <h1 align="center">HAPPI</h1>
 
 <div align="center">
   <strong>Heuristic Access to Positioning of Photon Instrumentation</strong>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: happi Version: 2.2.0 Summary: Happi Database Access
+Metadata-Version: 2.1 Name: happi Version: 2.3.0 Summary: Happi Database Access
 for LCLS Beamline Devices Author: SLAC National Accelerator Laboratory License:
 Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt of
 any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: (1)
 Redistributions of source code must retain the above copyright notice, this
@@ -30,16 +30,16 @@
 without imposing a separate written license agreement for such Enhancements,
 then you hereby grant the following license: a non-exclusive, royalty-free
 perpetual license to install, use, modify, prepare derivative works,
 incorporate into other computer software, distribute, and sublicense such
 Enhancements or derivative works thereof, in binary and source code form.
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.9
-Description-Content-Type: text/markdown Provides-Extra: test License-File:
-LICENSE.md License-File: AUTHORS.rst
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+doc License-File: LICENSE.md License-File: AUTHORS.rst
                               ****** HAPPI ******
            Heuristic Access to Positioning of Photon Instrumentation
   Motivation â¢ Features â¢ Installation â¢ Basic_Usage â¢ Documentation
 ## Motivation LCLS endstations deal with dynamic sets of instrumentation.
 Information like ports, triggers and aliases are all important for operation,
 but hard to manage when spread across a multitude of applications. **Happi**
 solves this problem by creating a single access point for all the metadata
```

### Comparing `happi-2.2.0/happi.egg-info/SOURCES.txt` & `happi-2.3.0/happi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .pre-commit-config.yaml
 AUTHORS.rst
 CONTRIBUTING.rst
 LICENSE.md
 MANIFEST.in
 README.md
 dev-requirements.txt
-github_deploy_key_pcdshub_happi.enc
+docs-requirements.txt
 pyproject.toml
 requirements.txt
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/standard.yml
 conda-recipe/activate.sh
 conda-recipe/deactivate.sh
```

### Comparing `happi-2.2.0/pyproject.toml` & `happi-2.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 zip_safe = false
 include_package_data = true
 
 [project.license]
 file = "LICENSE.md"
 
 [project.scripts]
-happi = "happi.cli:happi_cli"
+happi = "happi.cli:main"
 
 [tool.setuptools_scm]
 write_to = "happi/_version.py"
 
 [tool.flake8]
 exclude = "docs/*,versioneer.py"
 
@@ -38,7 +38,13 @@
 content-type = "text/markdown"
 
 [tool.setuptools.dynamic.dependencies]
 file = [ "requirements.txt",]
 
 [tool.setuptools.dynamic.optional-dependencies.test]
 file = "dev-requirements.txt"
+
+[tool.setuptools.dynamic.optional-dependencies.doc]
+file = "docs-requirements.txt"
+
+[tool.pytest.ini_options]
+addopts = "--cov=."
```

