# Comparing `tmp/dlrnapi_client-0.8.1.tar.gz` & `tmp/dlrnapi_client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlrnapi_client-0.8.1.tar", last modified: Wed Mar  4 10:59:45 2020, max compression
+gzip compressed data, was "dist/dlrnapi_client-0.9.1.tar", last modified: Fri Mar 27 10:56:13 2020, max compression
```

## Comparing `dlrnapi_client-0.8.1.tar` & `dlrnapi_client-0.9.1.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client/
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client/ansible/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      280 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/ansible/ansible.cfg.example
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    13698 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/ansible/dlrn_api.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1421 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/ansible/example_playbook.yaml
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client/apis/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      128 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/apis/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    47001 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/apis/default_api.py
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1030 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3848 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/agg_query.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6577 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/ci_agg_vote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8432 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/ci_vote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8215 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/metrics.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2830 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/model_import.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7405 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/params.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8472 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/params_1.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4635 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/params_2.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7659 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/params_3.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8617 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/promotion.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6860 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/promotion_query.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7117 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/models/repo.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1289 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    24054 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/api_client.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6887 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/configuration.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12684 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/rest.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    18890 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/dlrnapi_client/shell.py
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6830 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/PKG-INFO
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1722 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/SOURCES.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/dependency_links.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       55 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/entry_points.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/not-zip-safe
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       46 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/pbr.json
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       86 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/requires.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       15 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/dlrnapi_client.egg-info/top_level.txt
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/docs/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      869 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/CIVote.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    13471 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/DefaultApi.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      473 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Metrics.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      510 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/MetricsRequest.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      373 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/ModelImport.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1142 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Params.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1266 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Params1.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      595 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Params2.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      739 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Params3.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      570 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Promotion.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      745 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/Repo.md
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1854 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/docs/command-line.md
-drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/test/
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/__init__.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      671 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_agg_query.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      803 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_ci_agg_vote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      862 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_ci_vote.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4055 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_default_api.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1166 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_metrics.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      669 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_model_import.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      774 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_params.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      808 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_params_1.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      682 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_params_2.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      809 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_params_3.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      873 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_promotion.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      865 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_promotion_query.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      789 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test/test_repo.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      375 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/.zuul.yaml
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      419 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/AUTHORS
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1832 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/ChangeLog
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10142 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/LICENSE
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       16 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/MANIFEST.in
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4452 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/README.rst
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       96 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/requirements.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1304 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/setup.cfg
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      242 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/setup.py
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       95 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/test-requirements.txt
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      541 2020-03-04 10:59:18.000000 dlrnapi_client-0.8.1/tox.ini
--rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6830 2020-03-04 10:59:45.000000 dlrnapi_client-0.8.1/PKG-INFO
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client/
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client/ansible/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      280 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/ansible/ansible.cfg.example
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    15143 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/ansible/dlrn_api.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1421 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/ansible/example_playbook.yaml
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client/apis/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      128 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/apis/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    52303 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/apis/default_api.py
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1030 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     3848 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/agg_query.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6577 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/ci_agg_vote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8432 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/ci_vote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8215 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/metrics.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2830 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/model_import.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7405 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/params.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8472 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/params_1.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4635 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/params_2.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7659 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/params_3.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     8617 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/promotion.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6860 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/promotion_query.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7117 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/models/repo.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1289 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    24054 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/api_client.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     6887 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/configuration.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    12684 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/rest.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    20270 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/dlrnapi_client/shell.py
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7128 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/PKG-INFO
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1757 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       55 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/entry_points.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        1 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/not-zip-safe
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       46 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/pbr.json
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       86 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/requires.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       15 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/dlrnapi_client.egg-info/top_level.txt
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/docs/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      521 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/AggQuery.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      800 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/CIAggVote.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      869 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/CIVote.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    16619 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/DefaultApi.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      473 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Metrics.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      510 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/MetricsRequest.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      373 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/ModelImport.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1142 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Params.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1266 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Params1.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      595 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Params2.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      739 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Params3.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      570 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Promotion.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      745 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/Repo.md
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     2034 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/docs/command-line.md
+drwxr-xr-x   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/test/
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)        0 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/__init__.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      671 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_agg_query.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      803 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_ci_agg_vote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      862 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_ci_vote.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4055 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_default_api.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1166 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_metrics.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      669 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_model_import.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      774 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_params.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      808 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_params_1.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      682 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_params_2.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      809 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_params_3.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      873 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_promotion.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      865 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_promotion_query.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      789 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test/test_repo.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      450 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/.zuul.yaml
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      419 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/AUTHORS
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1932 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/ChangeLog
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)    10142 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/LICENSE
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       16 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/MANIFEST.in
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     4718 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/README.rst
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       96 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/requirements.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     1304 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/setup.cfg
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      242 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/setup.py
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)       95 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/test-requirements.txt
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)      541 2020-03-27 10:55:34.000000 dlrnapi_client-0.9.1/tox.ini
+-rw-r--r--   0 zuul-worker  (1001) zuul-worker  (1001)     7128 2020-03-27 10:56:13.000000 dlrnapi_client-0.9.1/PKG-INFO
```

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/ansible/dlrn_api.py` & `dlrnapi_client-0.9.1/dlrnapi_client/ansible/dlrn_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 description:
     - Ansible module to manage the DLRN API
 options:
     action:
         description:
             - Action to take
         choices: [repo-get, repo-use, repo-status, report-result, repo-promote,
-                  commit-import, promotion-get, build-metrics, agg-status]
+                  repo-promote-batch, commit-import, promotion-get,
+                  build-metrics, agg-status]
         required: true
     host:
         description:
             - URL for the DLRN API host
         required: true
     user:
         description:
@@ -129,16 +130,20 @@
     package_name:
         description:
             - If action is build-metrics, filter results for this package.
     component:
         description:
             - If action is repo-get, repo-use or promotion-get, filter on
               this component.
+    hash_pairs:
+        description:
+            - If action is repo-promote-batch, this is a list of commit_hash
+              and distro_hash pairs to be promoted using promote_name.
 requirements:
-    - "python >= 2.6"
+    - "python >= 2.7"
     - "python-dlrnapi_client"
 '''
 
 EXAMPLES = '''
 # Get the last repo tested by any CI
 - dlrn_api:
     action: repo-get
@@ -209,24 +214,37 @@
     host: http://dlrn.example.com:5000
     user: myuser
     password: mypasswd
     commit_hash: 3a9326f251b9a4162eb0dfa9f1c924ef47c2c55a
     distro_hash: 024e24f0cf4366c2290c22f24e42de714d1addd1
     promote_name: current-passed-ci
 
+# Do a batch promotion
+- dlrn_api:
+    action: repo-promote-batch
+    host: http://dlrn.example.com:5000
+    user: myuser
+    password: mypasswd
+    hash_pairs:
+        - commit_hash: 3a9326f251b9a4162eb0dfa9f1c924ef47c2c55a
+          distro_hash: 024e24f0cf4366c2290c22f24e42de714d1addd1
+        - commit_hash: 3a9326f251b9a4162eb0dfa9f1c924ef47c2c533
+          distro_hash: 024e24f0cf4366c2290c22f24e42de714d1addae
+    promote_name: current-passed-ci
+
 # Import a remote commit
 - dlrn_api:
     action: commit-import
     host: http://dlrn.example.com:5000
     user: myuser
     password: mypasswd
     repo_url: http://builder.example.com/3a9326f251b9a4162eb0_024e24f0
 '''
 auth_required_actions = ['repo-use', 'report-result', 'repo-promote',
-                         'commit-import']
+                         'repo-promote-batch', 'commit-import']
 
 
 class DLRNAPIWrapper(object):
     """Wrapper class
 
     It is meant to provide the options dict, and a parameter verification
     method
@@ -243,14 +261,15 @@
         self.info_url = params.get('info_url')
         self.timestamp = params.get('timestamp')
         self.notes = params.get('notes')
         self.promote_name = params.get('promote_name')
         self.repo_url = params.get('repo_url')
         self.component = params.get('component')
         self.agg_hash = params.get('agg_hash')
+        self.hash_pairs = params.get('hash_pairs')
 
     def check_options(self, action, module):
         if action == 'repo-use':
             if self.reporting_job_id is None:
                 module.fail_json(msg="Missing parameter reporting_job_id")
         elif action == 'report-result':
             if self.agg_hash is not None and\
@@ -276,14 +295,28 @@
         elif action == 'repo-promote':
             if self.commit_hash is None:
                 module.fail_json(msg="Missing parameter commit_hash")
             if self.distro_hash is None:
                 module.fail_json(msg="Missing parameter distro_hash")
             if self.promote_name is None:
                 module.fail_json(msg="Missing parameter promote_name")
+        elif action == 'repo-promote-batch':
+            if self.hash_pairs is None:
+                module.fail_json(msg="Missing parameter hash_pairs")
+            if self.promote_name is None:
+                module.fail_json(msg="Missing parameter promote_name")
+            # The hash_pairs format is different when passed to the client,
+            # so convert it here
+            hash_pairs = ''
+            for pair in self.hash_pairs[:-1]:
+                hash_pairs += '%s_%s,' % (pair['commit_hash'],
+                                          pair['distro_hash'])
+            hash_pairs += '%s_%s' % (self.hash_pairs[-1]['commit_hash'],
+                                     self.hash_pairs[-1]['distro_hash'])
+            self.hash_pairs = hash_pairs
         elif action == 'commit-import':
             if self.repo_url is None:
                 module.fail_json(msg="Missing parameter repo_url")
         elif action == 'promotion-get':
             if (self.commit_hash is not None and self.distro_hash is None):
                 module.fail_json(msg="Missing parameter distro_hash")
             if (self.distro_hash is not None and self.commit_hash is None):
@@ -294,21 +327,20 @@
             if self.end_date is None:
                 module.fail_json(msg="Missing end_date")
 
 
 def main():
     module = AnsibleModule(
         argument_spec=dict(
-            action=dict(required=True, choices=['repo-get', 'repo-use',
-                                                'repo-status', 'report-result',
-                                                'repo-promote',
-                                                'commit-import',
-                                                'promotion-get',
-                                                'build-metrics',
-                                                'agg-status']),
+            action=dict(required=True,
+                        choices=['repo-get', 'repo-use',
+                                 'repo-status', 'report-result',
+                                 'repo-promote', 'repo-promote-batch',
+                                 'commit-import', 'promotion-get',
+                                 'build-metrics', 'agg-status']),
             host=dict(required=True),
             user=dict(),
             password=dict(no_log=True),
             reporting_job_id=dict(),
             max_age=dict(default='0', type='int'),
             success=dict(type='bool'),
             job_id=dict(),
@@ -321,15 +353,16 @@
             notes=dict(),
             promote_name=dict(),
             repo_url=dict(),
             start_date=dict(),
             end_date=dict(),
             package_name=dict(),
             component=dict(),
-            agg_hash=dict()
+            agg_hash=dict(),
+            hash_pairs=dict(type='list')
         )
     )
 
     action = module.params['action']
     username = module.params['user']
     password = module.params['password']
     if action in auth_required_actions and (username is None or
```

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/ansible/example_playbook.yaml` & `dlrnapi_client-0.9.1/dlrnapi_client/ansible/example_playbook.yaml`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/apis/default_api.py` & `dlrnapi_client-0.9.1/dlrnapi_client/apis/default_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -420,14 +420,134 @@
                                             '_return_http_data_only'),
                                         _preload_content=params.get(
                                             '_preload_content', True),
                                         _request_timeout=params.get(
                                             '_request_timeout'),
                                         collection_formats=collection_formats)
 
+    def api_promote_batch_post(self, params, **kwargs):
+        """Atomically promote a list of repositories.
+
+        This is the equivalent of calling api_promote_post multiple times, one
+        with each commit/distro_hash combination. The only difference is that
+        the call is atomic, and when components are enabled, the aggregated
+        repo files are only updated once.
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.api_promote_batch_post(params,
+                                                callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param  list[Promotion] params: The JSON params to post (required)
+        :return: Promotion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.api_promote_batch_post_with_http_info(params, **kwargs)
+        else:
+            (data) = self.api_promote_batch_post_with_http_info(params,
+                                                                **kwargs)
+            return data
+
+    def api_promote_batch_post_with_http_info(self, params, **kwargs):
+        """Atomically promote a list of repositories.
+
+        This is the equivalent of calling api_promote_post multiple times, one
+        with each commit/distro_hash combination. The only difference is that
+        the call is atomic, and when components are enabled, the aggregated
+        repo files are only updated once.
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.api_promote_batch_post_with_http_info(params,
+                                                               callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param  list[Promotion] params: The JSON params to post (required)
+        :return: Promotion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['params']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method api_promote_post" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'params' is set
+        if ('params' not in params) or (params['params'] is None):
+            raise ValueError("Missing the required parameter `params` when "
+                             "calling `api_promote_post`")
+
+        collection_formats = {}
+
+        resource_path = '/api/promote-batch'.replace('{format}', 'json')
+        path_params = {}
+
+        query_params = {}
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'params' in params:
+            body_params = params['params']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/json'])
+
+        # Authentication setting
+        auth_settings = ['basicAuth']
+
+        return self.api_client.call_api(resource_path, 'POST',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type='Promotion',
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get(
+                                            '_return_http_data_only'),
+                                        _preload_content=params.get(
+                                            '_preload_content', True),
+                                        _request_timeout=params.get(
+                                            '_request_timeout'),
+                                        collection_formats=collection_formats)
+
     def api_remote_import_post(self, params, **kwargs):
         """Import a commit built by another instance.
 
         This API call mimics the behavior of the ``dlrn-remote`` command,
         with the only exception of not being able to specify a custom
         rdoinfo location.
```

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/__init__.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/agg_query.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/agg_query.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/ci_agg_vote.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/ci_agg_vote.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/ci_vote.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/ci_vote.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/metrics.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/metrics.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/model_import.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/model_import.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/params.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/params.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/params_1.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/params_1.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/params_2.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/params_2.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/params_3.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/params_3.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/promotion.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/promotion.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/promotion_query.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/promotion_query.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/models/repo.py` & `dlrnapi_client-0.9.1/dlrnapi_client/models/repo.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/__init__.py` & `dlrnapi_client-0.9.1/dlrnapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/api_client.py` & `dlrnapi_client-0.9.1/dlrnapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/configuration.py` & `dlrnapi_client-0.9.1/dlrnapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/rest.py` & `dlrnapi_client-0.9.1/dlrnapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client/shell.py` & `dlrnapi_client-0.9.1/dlrnapi_client/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,32 @@
     try:
         api_response = api_instance.api_promote_post(params)
         return api_response
     except ApiException as e:
         raise e
 
 
+def repo_promote_batch(api_instance, options):
+    params = list()
+    hash_pairs = options.hash_pairs.split(',')
+    for pair in hash_pairs:
+        commit_hash = pair.split('_')[0]
+        distro_hash = pair.split('_')[1]
+        param = dlrnapi_client.Promotion()
+        param.commit_hash = commit_hash
+        param.distro_hash = distro_hash
+        param.promote_name = options.promote_name
+        params.append(param)
+    try:
+        api_response = api_instance.api_promote_batch_post(params)
+        return api_response
+    except ApiException as e:
+        raise e
+
+
 def get_promotions(api_instance, options):
     params = dlrnapi_client.PromotionQuery()  # PromotionQuery
     if options.commit_hash:
         params.commit_hash = options.commit_hash
     if options.distro_hash:
         params.distro_hash = options.distro_hash
     if options.agg_hash:
@@ -191,14 +209,15 @@
 command_funcs = {
     'repo-get': get_last_tested_repo,
     'repo-use': post_last_tested_repo,
     'repo-status': repo_status,
     'agg-status': agg_status,
     'report-result': report_result,
     'repo-promote': repo_promote,
+    'repo-promote-batch': repo_promote_batch,
     'commit-import': import_commit,
     'promotion-get': get_promotions,
     'build-metrics': get_metrics_builds,
 }
 
 
 def main():
@@ -340,14 +359,26 @@
     parser_prom.add_argument('--commit-hash', type=str, required=True,
                              help='commit_hash of the repo to be promoted')
     parser_prom.add_argument('--distro-hash', type=str, required=True,
                              help='distro_hash of the repo to be promoted')
     parser_prom.add_argument('--promote-name', type=str, required=True,
                              help='Name to be used for the promotion')
 
+    # Subcommand repo-promote-batch
+    parser_prom = subparsers.add_parser('repo-promote-batch',
+                                        help='Promote multiple repositories '
+                                             'at the same time, as an atomic '
+                                             'operation.')
+    parser_prom.add_argument('--hash-pairs', type=str, required=True,
+                             help='commit_hash+distro_hash of the repos to '
+                                  'be promoted, specified as a comma-separated'
+                                  ' list of commit_distro hash pairs')
+    parser_prom.add_argument('--promote-name', type=str, required=True,
+                             help='Name to be used for the promotion')
+
     # Subcommand promotion-get
     parser_promget = subparsers.add_parser('promotion-get',
                                            help='Get information about '
                                                 'promotions')
     parser_promget.add_argument('--commit-hash', type=str, required=False,
                                 help='commit_hash of the repo to search '
                                      'promotions for. Requires --distro-hash '
```

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client.egg-info/PKG-INFO` & `dlrnapi_client-0.9.1/dlrnapi_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrnapi-client
-Version: 0.8.1
+Version: 0.9.1
 Summary: Client for DLRN REST API
 Home-page: http://www.rdoproject.org/
 Author: OpenStack
 Author-email: jpena@redhat.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/softwarefactory-project/dlrnapi_client/issues
 Project-URL: Source Code, https://github.com/softwarefactory-project/dlrnapi_client
@@ -18,15 +18,15 @@
         -  API version: 1.0.0
         -  Package version: 1.0.0
         -  Build package: io.swagger.codegen.languages.PythonClientCodegen
         
         Requirements.
         -------------
         
-        Python 2.7 and 3.4+
+        Python 2.7 or 3.6+
         
         Installation & Usage
         --------------------
         
         You can install directly from Github
         
         .. code:: sh
@@ -106,19 +106,21 @@
         
         ============ ============================ ============================== ===========
         Class        Method                       HTTP request                   Description
         ============ ============================ ============================== ===========
         *DefaultApi* `api_last_tested_repo_get`_  **GET** /api/last_tested_repo
         *DefaultApi* `api_last_tested_repo_post`_ **POST** /api/last_tested_repo
         *DefaultApi* `api_promote_post`_          **POST** /api/promote
+        *DefaultApi* `api_promote_batch_post`_    **POST** /api/promote-batch
         *DefaultApi* `api_promotions_get`_        **POST** /api/promotions
         *DefaultApi* `api_build_metrics_get`_     **GET** /api/metrics/builds
         *DefaultApi* `api_remote_import_post`_    **POST** /api/remote/import
         *DefaultApi* `api_repo_status_get`_       **GET** /api/repo_status
         *DefaultApi* `api_report_result_post`_    **POST**/api/report_result
+        *DefaultApi* `api_agg_status_get`_        **GET**/api/agg_status
         ============ ============================ ============================== ===========
         
         Documentation For Models
         ------------------------
         
         -  `CIVote`_
         -  `Import`_
@@ -154,19 +156,21 @@
         .. _Swagger Codegen: https://github.com/swagger-api/swagger-codegen
         .. _Setuptools: http://pypi.python.org/pypi/setuptools
         .. _installation procedure: #installation--usage
         .. _dlrnapi: docs/command-line.md
         .. _api_last_tested_repo_get: docs/DefaultApi.md#api_last_tested_repo_get
         .. _api_last_tested_repo_post: docs/DefaultApi.md#api_last_tested_repo_post
         .. _api_promote_post: docs/DefaultApi.md#api_promote_post
+        .. _api_promote_batch_post: docs/DefaultApi.md#api_promote_batch_post
         .. _api_promotions_get: docs/DefaultApi.md#api_promotions_get
         .. _api_build_metrics_get: docs/DefaultApi.md#api_build_metrics_get
         .. _api_remote_import_post: docs/DefaultApi.md#api_remote_import_post
         .. _api_repo_status_get: docs/DefaultApi.md#api_repo_status_get
         .. _api_report_result_post: docs/DefaultApi.md#api_report_result_post
+        .. _api_agg_status_get: docs/DefaultApi.md#api_agg_status_get
         .. _CIVote: docs/CIVote.md
         .. _Import: docs/ModelImport.md
         .. _Params: docs/Params.md
         .. _Params1: docs/Params1.md
         .. _Params2: docs/Params2.md
         .. _Params3: docs/Params3.md
         .. _Promotion: docs/Promotion.md
```

### Comparing `dlrnapi_client-0.8.1/dlrnapi_client.egg-info/SOURCES.txt` & `dlrnapi_client-0.9.1/dlrnapi_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 dlrnapi_client/models/params.py
 dlrnapi_client/models/params_1.py
 dlrnapi_client/models/params_2.py
 dlrnapi_client/models/params_3.py
 dlrnapi_client/models/promotion.py
 dlrnapi_client/models/promotion_query.py
 dlrnapi_client/models/repo.py
+docs/AggQuery.md
+docs/CIAggVote.md
 docs/CIVote.md
 docs/DefaultApi.md
 docs/Metrics.md
 docs/MetricsRequest.md
 docs/ModelImport.md
 docs/Params.md
 docs/Params1.md
```

### Comparing `dlrnapi_client-0.8.1/docs/CIVote.md` & `dlrnapi_client-0.9.1/docs/CIVote.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/DefaultApi.md` & `dlrnapi_client-0.9.1/docs/DefaultApi.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 All URIs are relative to <http://127.0.0.1:5000>
 
 Method |HTTP request |Description
 ------------- | ------------- | -------------
 [**api_last_tested_repo_get**](DefaultApi.md#api_last_tested_repo_get) |**GET** /api/last_tested_repo |
 [**api_last_tested_repo_post**](DefaultApi.md#api_last_tested_repo_post)|**POST** /api/last_tested_repo |
 [**api_promote_post**](DefaultApi.md#api_promote_post) | **POST** /api/promote |
+[**api_promote_batch_post**](DefaultApi.md#api_promote_batch_post) | **POST** /api/promote-batch |
 [**api_promotions_get**](DefaultApi.md#api_promotions_get) | **GET** /api/promotions |
 [**api_build_metrics_get**](DefaultApi.md#api_build_metrics_get)|**GET** /api/metrics/builds|
 [**api_remote_import_post**](DefaultApi.md#api_remote_import_post) |**POST** /api/remote/import |
 [**api_repo_status_get**](DefaultApi.md#api_repo_status_get)|**GET** /api/repo_status |
+[**api_agg_status_get**](DefaultApi.md#api_agg_status_get)|**GET** /api/agg_status |
 [**api_report_result_post**](DefaultApi.md#api_report_result_post)|**POST** /api/report_result|
 
 
 # **api_last_tested_repo_get**
 > Repo api_last_tested_repo_get(params)
 
 Get the last tested repo since a specific time.  If a ``job_id`` is specified, the order of precedence for the repo returned is:
@@ -185,14 +187,74 @@
 ### HTTP request headers
 
 -   **Content-Type**: application/json
 -   **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
+# **api_promote_batch_post**
+> Promotion api_promote_batch_post(params=params)
+
+Promote several repositories as an atomic operation. Note the API will refuse
+to promote using promote_name=\"consistent\" or \"current\", since those are
+reserved keywords for DLRN.
+
+### Example
+```python
+from __future__ import print_statement
+import time
+import dlrnapi_client
+from dlrnapi_client.rest import ApiException
+from pprint import pprint
+
+# Configure HTTP basic authorization: basicAuth
+dlrnapi_client.configuration.username = 'YOUR_USERNAME'
+dlrnapi_client.configuration.password = 'YOUR_PASSWORD'
+
+# create an instance of the API class
+api_instance = dlrnapi_client.DefaultApi()
+
+params = list()
+hash_pairs = options.hash_pairs.split(',')
+for pair in hash_pairs:
+    commit_hash = pair.split('_')[0]
+    distro_hash = pair.split('_')[1]
+    param = dlrnapi_client.Promotion()
+    param.commit_hash = commit_hash
+    param.distro_hash = distro_hash
+    param.promote_name = options.promote_name
+    params.append(param)
+try:
+    api_response = api_instance.api_promote_batch_post(params)
+    pprint(api_response)
+except ApiException as e:
+    raise e
+```
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+**params**|[list(**Promotion**)](Promotion.md)|The JSON params to post|\[optional\]
+
+### Return type
+
+[**Promotion**](Promotion.md)
+
+### Authorization
+
+[basicAuth](../README.md#basicAuth)
+
+### HTTP request headers
+
+-   **Content-Type**: application/json
+-   **Accept**: application/json
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **api_promotions_get**
 > list[Promotion] api_promotions_get(params)
 
 
 
 Get all the promotions, optionally for a specific repository or promotion name. 
 
@@ -369,14 +431,59 @@
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
+-   **Content-Type**: application/json
+-   **Accept**: application/json
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
+# **api_agg_status_get**
+> list\[CIAggVote\] api_agg_status_get(params=params)
+
+Get all the CI reports for a specific repo aggregate.
+
+### Example
+```python
+from __future__ import print_statement
+import time
+import dlrnapi_client
+from dlrnapi_client.rest import ApiException
+from pprint import pprint
+
+# create an instance of the API class
+api_instance = dlrnapi_client.DefaultApi()
+params = dlrnapi_client.AggQuery()  # AggQuery | The JSON params to post
+
+try:
+    api_response = api_instance.api_agg_status_get(params=params)
+    pprint(api_response)
+except ApiException as e:
+    print("Exception when calling DefaultApi->api_agg_status_get: %s\n" % e)
+```
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+**params**|[**AggQuery**](AggQuery.md)|The JSON params to post|\[optional\]
+
+### Return type
+
+[**list[CIAggVote]**](CIAggVote.md)
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
 -   **Content-Type**: application/json
 -   **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **api_report_result_post**
 > CIVote api_report_result_post(params=params)
```

### Comparing `dlrnapi_client-0.8.1/docs/Params.md` & `dlrnapi_client-0.9.1/docs/Params.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/Params1.md` & `dlrnapi_client-0.9.1/docs/Params1.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/Params2.md` & `dlrnapi_client-0.9.1/docs/Params2.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/Params3.md` & `dlrnapi_client-0.9.1/docs/Params3.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/Promotion.md` & `dlrnapi_client-0.9.1/docs/Promotion.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/Repo.md` & `dlrnapi_client-0.9.1/docs/Repo.md`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/docs/command-line.md` & `dlrnapi_client-0.9.1/docs/command-line.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Usage
 
 ## Parameters
 
 ```bash
 usage: dlrnapi [-h] --url URL [--username USERNAME] [--password PASSWORD]
-               {repo-get,repo-use,repo-status,agg-status,report-result,repo-promote,promotion-get,commit-import,build-metrics}
+               {repo-get,repo-use,repo-status,agg-status,report-result,repo-promote,repo-promote-batch,promotion-get,commit-import,build-metrics}
                ...
 
 optional arguments:
   -h, --help            show this help message and exit
   --url URL             URL to use
   --username USERNAME, -u USERNAME
                         username for authentication, defaults to
@@ -16,30 +16,32 @@
   --password PASSWORD, -p PASSWORD
                         password for authentication, defaults to
                         "DLRNAPI_PASSWORD" environment variable is set
 
 subcommands:
   available subcommands
 
-  {repo-get,repo-use,repo-status,agg-status,report-result,repo-promote,promotion-get,commit-import,build-metrics}
+  {repo-get,repo-use,repo-status,agg-status,report-result,repo-promote,repo-promote-batch,promotion-get,commit-import,build-metrics}
     repo-get            Get last tested repo
     repo-use            Get the last tested repo since a specific time
                         (optionally for a CI job), and add an "in progress"
                         entry in the CI job table for this.
     repo-status         Get all the CI reports for a specific repository.
     agg-status          Get all the CI reports for a specific aggregated
                         repository.
     report-result       Report the result of a CI job
     repo-promote        Promote a repository
+    repo-promote-batch  Promote multiple repositories at the same time, as an
+                        atomic operation.
     promotion-get       Get information about promotions
     commit-import       Import a commit built by another instance
     build-metrics       Fetch build metrics in a time period
 ```
 The **url** parameter is mandatory in all cases. **username** and **password**
-are required for the _repo-use_, _report-result_, _repo-promote_ and
-_commit-import_ subcommands.
+are required for the _repo-use_, _report-result_, _repo-promote_,
+_repo-promote-batch_ and _commit-import_ subcommands.
 
 For detailed usage information on each subcommand, run:
 
 ```bash
 $ dlrnapi <subcommand> -h
 ```
```

### Comparing `dlrnapi_client-0.8.1/test/test_agg_query.py` & `dlrnapi_client-0.9.1/test/test_agg_query.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_ci_agg_vote.py` & `dlrnapi_client-0.9.1/test/test_ci_agg_vote.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_ci_vote.py` & `dlrnapi_client-0.9.1/test/test_ci_vote.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_default_api.py` & `dlrnapi_client-0.9.1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_metrics.py` & `dlrnapi_client-0.9.1/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_model_import.py` & `dlrnapi_client-0.9.1/test/test_model_import.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_params.py` & `dlrnapi_client-0.9.1/test/test_params.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_params_1.py` & `dlrnapi_client-0.9.1/test/test_params_1.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_params_2.py` & `dlrnapi_client-0.9.1/test/test_params_2.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_params_3.py` & `dlrnapi_client-0.9.1/test/test_params_3.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_promotion.py` & `dlrnapi_client-0.9.1/test/test_promotion.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_promotion_query.py` & `dlrnapi_client-0.9.1/test/test_promotion_query.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/test/test_repo.py` & `dlrnapi_client-0.9.1/test/test_repo.py`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/ChangeLog` & `dlrnapi_client-0.9.1/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+0.9.1
+-----
+
+* Fix README.rst for pypi publishing
+
+0.9.0
+-----
+
+* Add support for batch promotions
+
 0.8.1
 -----
 
 * Support aggregate hash in Ansible module
 
 0.8.0
 -----
```

### Comparing `dlrnapi_client-0.8.1/LICENSE` & `dlrnapi_client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/README.rst` & `dlrnapi_client-0.9.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 -  API version: 1.0.0
 -  Package version: 1.0.0
 -  Build package: io.swagger.codegen.languages.PythonClientCodegen
 
 Requirements.
 -------------
 
-Python 2.7 and 3.4+
+Python 2.7 or 3.6+
 
 Installation & Usage
 --------------------
 
 You can install directly from Github
 
 .. code:: sh
@@ -96,19 +96,21 @@
 
 ============ ============================ ============================== ===========
 Class        Method                       HTTP request                   Description
 ============ ============================ ============================== ===========
 *DefaultApi* `api_last_tested_repo_get`_  **GET** /api/last_tested_repo
 *DefaultApi* `api_last_tested_repo_post`_ **POST** /api/last_tested_repo
 *DefaultApi* `api_promote_post`_          **POST** /api/promote
+*DefaultApi* `api_promote_batch_post`_    **POST** /api/promote-batch
 *DefaultApi* `api_promotions_get`_        **POST** /api/promotions
 *DefaultApi* `api_build_metrics_get`_     **GET** /api/metrics/builds
 *DefaultApi* `api_remote_import_post`_    **POST** /api/remote/import
 *DefaultApi* `api_repo_status_get`_       **GET** /api/repo_status
 *DefaultApi* `api_report_result_post`_    **POST**/api/report_result
+*DefaultApi* `api_agg_status_get`_        **GET**/api/agg_status
 ============ ============================ ============================== ===========
 
 Documentation For Models
 ------------------------
 
 -  `CIVote`_
 -  `Import`_
@@ -144,19 +146,21 @@
 .. _Swagger Codegen: https://github.com/swagger-api/swagger-codegen
 .. _Setuptools: http://pypi.python.org/pypi/setuptools
 .. _installation procedure: #installation--usage
 .. _dlrnapi: docs/command-line.md
 .. _api_last_tested_repo_get: docs/DefaultApi.md#api_last_tested_repo_get
 .. _api_last_tested_repo_post: docs/DefaultApi.md#api_last_tested_repo_post
 .. _api_promote_post: docs/DefaultApi.md#api_promote_post
+.. _api_promote_batch_post: docs/DefaultApi.md#api_promote_batch_post
 .. _api_promotions_get: docs/DefaultApi.md#api_promotions_get
 .. _api_build_metrics_get: docs/DefaultApi.md#api_build_metrics_get
 .. _api_remote_import_post: docs/DefaultApi.md#api_remote_import_post
 .. _api_repo_status_get: docs/DefaultApi.md#api_repo_status_get
 .. _api_report_result_post: docs/DefaultApi.md#api_report_result_post
+.. _api_agg_status_get: docs/DefaultApi.md#api_agg_status_get
 .. _CIVote: docs/CIVote.md
 .. _Import: docs/ModelImport.md
 .. _Params: docs/Params.md
 .. _Params1: docs/Params1.md
 .. _Params2: docs/Params2.md
 .. _Params3: docs/Params3.md
 .. _Promotion: docs/Promotion.md
```

### Comparing `dlrnapi_client-0.8.1/setup.cfg` & `dlrnapi_client-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/tox.ini` & `dlrnapi_client-0.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `dlrnapi_client-0.8.1/PKG-INFO` & `dlrnapi_client-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrnapi_client
-Version: 0.8.1
+Version: 0.9.1
 Summary: Client for DLRN REST API
 Home-page: http://www.rdoproject.org/
 Author: OpenStack
 Author-email: jpena@redhat.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/softwarefactory-project/dlrnapi_client/issues
 Project-URL: Source Code, https://github.com/softwarefactory-project/dlrnapi_client
@@ -18,15 +18,15 @@
         -  API version: 1.0.0
         -  Package version: 1.0.0
         -  Build package: io.swagger.codegen.languages.PythonClientCodegen
         
         Requirements.
         -------------
         
-        Python 2.7 and 3.4+
+        Python 2.7 or 3.6+
         
         Installation & Usage
         --------------------
         
         You can install directly from Github
         
         .. code:: sh
@@ -106,19 +106,21 @@
         
         ============ ============================ ============================== ===========
         Class        Method                       HTTP request                   Description
         ============ ============================ ============================== ===========
         *DefaultApi* `api_last_tested_repo_get`_  **GET** /api/last_tested_repo
         *DefaultApi* `api_last_tested_repo_post`_ **POST** /api/last_tested_repo
         *DefaultApi* `api_promote_post`_          **POST** /api/promote
+        *DefaultApi* `api_promote_batch_post`_    **POST** /api/promote-batch
         *DefaultApi* `api_promotions_get`_        **POST** /api/promotions
         *DefaultApi* `api_build_metrics_get`_     **GET** /api/metrics/builds
         *DefaultApi* `api_remote_import_post`_    **POST** /api/remote/import
         *DefaultApi* `api_repo_status_get`_       **GET** /api/repo_status
         *DefaultApi* `api_report_result_post`_    **POST**/api/report_result
+        *DefaultApi* `api_agg_status_get`_        **GET**/api/agg_status
         ============ ============================ ============================== ===========
         
         Documentation For Models
         ------------------------
         
         -  `CIVote`_
         -  `Import`_
@@ -154,19 +156,21 @@
         .. _Swagger Codegen: https://github.com/swagger-api/swagger-codegen
         .. _Setuptools: http://pypi.python.org/pypi/setuptools
         .. _installation procedure: #installation--usage
         .. _dlrnapi: docs/command-line.md
         .. _api_last_tested_repo_get: docs/DefaultApi.md#api_last_tested_repo_get
         .. _api_last_tested_repo_post: docs/DefaultApi.md#api_last_tested_repo_post
         .. _api_promote_post: docs/DefaultApi.md#api_promote_post
+        .. _api_promote_batch_post: docs/DefaultApi.md#api_promote_batch_post
         .. _api_promotions_get: docs/DefaultApi.md#api_promotions_get
         .. _api_build_metrics_get: docs/DefaultApi.md#api_build_metrics_get
         .. _api_remote_import_post: docs/DefaultApi.md#api_remote_import_post
         .. _api_repo_status_get: docs/DefaultApi.md#api_repo_status_get
         .. _api_report_result_post: docs/DefaultApi.md#api_report_result_post
+        .. _api_agg_status_get: docs/DefaultApi.md#api_agg_status_get
         .. _CIVote: docs/CIVote.md
         .. _Import: docs/ModelImport.md
         .. _Params: docs/Params.md
         .. _Params1: docs/Params1.md
         .. _Params2: docs/Params2.md
         .. _Params3: docs/Params3.md
         .. _Promotion: docs/Promotion.md
```

