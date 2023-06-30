# Comparing `tmp/broker-0.3.2.tar.gz` & `tmp/broker-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broker-0.3.2.tar", last modified: Wed May 17 15:53:27 2023, max compression
+gzip compressed data, was "broker-0.3.3.tar", last modified: Fri Jun 30 12:42:20 2023, max compression
```

## Comparing `broker-0.3.2.tar` & `broker-0.3.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.159932 broker-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.163932 broker-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 15:53:11.000000 broker-0.3.2/.github/workflows/update_broker_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 15:53:11.000000 broker-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-17 15:53:11.000000 broker-0.3.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-17 15:53:11.000000 broker-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 15:53:11.000000 broker-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-17 15:53:27.171933 broker-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-17 15:53:11.000000 broker-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 15:53:11.000000 broker-0.3.2/broker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/binds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:11.000000 broker-0.3.2/broker/binds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-17 15:53:11.000000 broker-0.3.2/broker/binds/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-17 15:53:11.000000 broker-0.3.2/broker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-17 15:53:11.000000 broker-0.3.2/broker/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 15:53:11.000000 broker-0.3.2/broker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-17 15:53:11.000000 broker-0.3.2/broker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-17 15:53:11.000000 broker-0.3.2/broker/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-17 15:53:11.000000 broker-0.3.2/broker/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29309 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 15:53:11.000000 broker-0.3.2/broker/providers/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-17 15:53:11.000000 broker-0.3.2/broker/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-17 15:53:11.000000 broker-0.3.2/broker/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/broker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:53:17.000000 broker-0.3.2/broker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 15:53:27.000000 broker-0.3.2/broker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-17 15:53:11.000000 broker-0.3.2/broker_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 15:53:11.000000 broker-0.3.2/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 15:53:11.000000 broker-0.3.2/logs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 15:53:11.000000 broker-0.3.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 15:53:27.171933 broker-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 15:53:11.000000 broker-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 15:53:11.000000 broker-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.167932 broker-0.3.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/ansible_tower/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_children.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_jobs.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/ansible_tower/fake_workflows.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/args_file.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/args_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/broker_args.json
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/broker_args.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.163932 broker-0.3.2/tests/data/cli_scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/cli_scenarios/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/cli_scenarios/satlab/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/data/container/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/container/fake_containers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/container/fake_images.json
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-17 15:53:11.000000 broker-0.3.2/tests/data/fake_inventory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 15:53:11.000000 broker-0.3.2/tests/functional/test_satlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:53:27.171933 broker-0.3.2/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-17 15:53:11.000000 broker-0.3.2/tests/providers/test_ansible_tower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-17 15:53:11.000000 broker-0.3.2/tests/providers/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 15:53:11.000000 broker-0.3.2/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.829252 broker-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-30 12:42:01.000000 broker-0.3.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-30 12:42:01.000000 broker-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 12:42:01.000000 broker-0.3.3/.github/workflows/update_broker_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-30 12:42:01.000000 broker-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 12:42:01.000000 broker-0.3.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-06-30 12:42:01.000000 broker-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 12:42:01.000000 broker-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-30 12:42:20.837252 broker-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-30 12:42:01.000000 broker-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 12:42:01.000000 broker-0.3.3/broker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/broker/binds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:01.000000 broker-0.3.3/broker/binds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-30 12:42:01.000000 broker-0.3.3/broker/binds/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-06-30 12:42:01.000000 broker-0.3.3/broker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-30 12:42:01.000000 broker-0.3.3/broker/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-30 12:42:01.000000 broker-0.3.3/broker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-06-30 12:42:01.000000 broker-0.3.3/broker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-30 12:42:01.000000 broker-0.3.3/broker/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-30 12:42:01.000000 broker-0.3.3/broker/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/broker/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-30 12:42:01.000000 broker-0.3.3/broker/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29317 2023-06-30 12:42:01.000000 broker-0.3.3/broker/providers/ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-30 12:42:01.000000 broker-0.3.3/broker/providers/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-30 12:42:01.000000 broker-0.3.3/broker/providers/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-30 12:42:01.000000 broker-0.3.3/broker/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-30 12:42:01.000000 broker-0.3.3/broker/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/broker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:42:11.000000 broker-0.3.3/broker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 12:42:20.000000 broker-0.3.3/broker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-30 12:42:01.000000 broker-0.3.3/broker_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-30 12:42:01.000000 broker-0.3.3/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:42:01.000000 broker-0.3.3/logs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 12:42:01.000000 broker-0.3.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-30 12:42:20.837252 broker-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 12:42:01.000000 broker-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 12:42:01.000000 broker-0.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/data/ansible_tower/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/ansible_tower/fake_children.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/ansible_tower/fake_jobs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/ansible_tower/fake_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/args_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/args_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/broker_args.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/broker_args.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.833252 broker-0.3.3/tests/data/cli_scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/data/cli_scenarios/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/containers/checkout_ch-d_ubi8_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/containers/execute_ch-d_ubi8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/data/cli_scenarios/satlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/checkout_latest_rhel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/checkout_latest_sat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/checkout_rhel78.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/checkout_sat_69.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/execute_templates_list.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/cli_scenarios/satlab/execute_test_workflow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/data/container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/container/fake_containers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/container/fake_images.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-30 12:42:01.000000 broker-0.3.3/tests/data/fake_inventory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-30 12:42:01.000000 broker-0.3.3/tests/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-30 12:42:01.000000 broker-0.3.3/tests/functional/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-30 12:42:01.000000 broker-0.3.3/tests/functional/test_satlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:42:20.837252 broker-0.3.3/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-30 12:42:01.000000 broker-0.3.3/tests/providers/test_ansible_tower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-30 12:42:01.000000 broker-0.3.3/tests/providers/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-30 12:42:01.000000 broker-0.3.3/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-30 12:42:01.000000 broker-0.3.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-30 12:42:01.000000 broker-0.3.3/tests/test_settings.py
```

### Comparing `broker-0.3.2/.github/workflows/codeql-analysis.yml` & `broker-0.3.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/.github/workflows/python-publish.yml` & `broker-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/.github/workflows/update_broker_image.yml` & `broker-0.3.3/.github/workflows/update_broker_image.yml`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/.gitignore` & `broker-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/LICENSE` & `broker-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/PKG-INFO` & `broker-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.2
+Version: 0.3.3
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.2/README.md` & `broker-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/binds/containers.py` & `broker-0.3.3/broker/binds/containers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/broker.py` & `broker-0.3.3/broker/broker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 from logzero import logger
 from broker.providers import PROVIDERS, PROVIDER_ACTIONS, _provider_imports
 from broker.hosts import Host
 from broker import exceptions, helpers
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 # load all the provider class so they are registered
@@ -18,14 +19,15 @@
 
 
 class mp_decorator:
     """This decorator wraps Broker methods to enable multiprocessing
 
     The decorated method is expected to return an itearable.
     """
+
     MAX_WORKERS = None
     """ If set to integer, the count of workers will be limited to that amount.
      If set to None, the max workers count of the EXECUTOR will match the count of items."""
 
     EXECUTOR = ThreadPoolExecutor
 
     def __init__(self, func=None):
@@ -207,15 +209,19 @@
         if isinstance(hosts, dict):
             # flatten the lists of hosts from the values of the dict
             hosts = [host for host_list in hosts.values() for host in host_list]
         else:
             if not isinstance(hosts, list):
                 hosts = [hosts]
             if in_context:
-                hosts = [host for host in hosts if not getattr(host, '_skip_context_checkin', False)]
+                hosts = [
+                    host
+                    for host in hosts
+                    if not getattr(host, "_skip_context_checkin", False)
+                ]
         if not hosts:
             logger.debug("Checkin called with no hosts, taking no action")
             return
 
         with ThreadPoolExecutor(max_workers=1 if sequential else None) as workers:
             completed_checkins = as_completed(
                 # reversing over a copy of the list to avoid skipping
@@ -264,17 +270,15 @@
         if not isinstance(hosts, list):
             hosts = [hosts]
 
         if not hosts:
             logger.debug("Extend called with no hosts, taking no action")
             return
 
-        with ThreadPoolExecutor(
-            max_workers=1 if sequential else len(hosts)
-        ) as workers:
+        with ThreadPoolExecutor(max_workers=1 if sequential else len(hosts)) as workers:
             completed_extends = as_completed(
                 workers.submit(self._extend, _host) for _host in hosts
             )
             for completed in completed_extends:
                 _host = completed.result()
                 logger.info(f"Completed extend for {_host.hostname or _host.name}")
 
@@ -319,14 +323,73 @@
         """Reconstruct one or more hosts from the local inventory
 
         :param filter: A broker-spec filter string
         """
         inv_hosts = helpers.load_inventory(filter=filter)
         return [self.reconstruct_host(inv_host) for inv_host in inv_hosts]
 
+    @classmethod
+    @contextmanager
+    def multi_manager(cls, **multi_dict):
+        """Given a mapping of names to Broker argument dictionaries:
+        create multiple Broker instances, check them out in parallel, yield, then checkin.
+
+        Example:
+            with Broker.multi_mode(
+                rhel7={
+                    "host_class": ContentHost,
+                    "workflow": "deploy_base_rhel",
+                    "deploy_rhel_version": "7",
+                },
+                rhel8={
+                    "host_class": ContentHost,
+                    "workflow": "deploy_base_rhel",
+                    "deploy_rhel_version": "8",
+                }
+            ) as host_dict:
+                pass
+
+        All are checked out at the same time. The user is presented with the hosts in
+        a dictionary by argument name e.g. host_dict["rhel7"] is a ContentHost object
+        """
+        # create all the broker instances and perform checkouts in parallel
+        broker_instances = {name: cls(**kwargs) for name, kwargs in multi_dict.items()}
+        with ThreadPoolExecutor(max_workers=len(broker_instances)) as workers:
+            completed_checkouts = as_completed(
+                workers.submit(broker.checkout) for broker in broker_instances.values()
+            )
+            for completed in completed_checkouts:
+                completed.result()
+        all_hosts = []
+        for broker_inst in broker_instances.values():
+            all_hosts.extend(broker_inst._hosts)
+        # run setup on all hosts in parallel
+        with ThreadPoolExecutor(max_workers=len(all_hosts)) as workers:
+            completed_setups = as_completed(
+                workers.submit(host.setup) for host in all_hosts
+            )
+            for completed in completed_setups:
+                completed.result()
+        # yield control to the user
+        yield {name: broker._hosts for name, broker in broker_instances.items()}
+        # teardown all hosts in parallel
+        with ThreadPoolExecutor(max_workers=len(all_hosts)) as workers:
+            completed_teardowns = as_completed(
+                workers.submit(host.teardown) for host in all_hosts
+            )
+            for completed in completed_teardowns:
+                completed.result()
+        # checkin all hosts in parallel
+        with ThreadPoolExecutor(max_workers=len(broker_instances)) as workers:
+            completed_checkins = as_completed(
+                workers.submit(broker.checkin) for broker in broker_instances.values()
+            )
+            for completed in completed_checkins:
+                completed.result()
+
     def __repr__(self):
         inner = ", ".join(
             f"{k}={v}"
             for k, v in self.__dict__.items()
             if not k.startswith("_") and not callable(v)
         )
         return f"{self.__class__.__name__}({inner})"
```

### Comparing `broker-0.3.2/broker/commands.py` & `broker-0.3.3/broker/commands.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/exceptions.py` & `broker-0.3.3/broker/exceptions.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/helpers.py` & `broker-0.3.3/broker/helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/hosts.py` & `broker-0.3.3/broker/hosts.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/logger.py` & `broker-0.3.3/broker/logger.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/providers/__init__.py` & `broker-0.3.3/broker/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/providers/ansible_tower.py` & `broker-0.3.3/broker/providers/ansible_tower.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,16 @@
         prov_inv = broker_args.pop("tower_inventory", None)
         if isinstance(prov_inv, str):
             logger.debug(f"prov_inv: {prov_inv}")
             prov_inv = self._translate_inventory(prov_inv)
         if prov_inv:
             logger.debug(f"prov_inv: {prov_inv}")
             broker_args["inventory"] = prov_inv
-        caller_host._prov_inst.release(
-            broker_args.get("source_vm", caller_host.name), broker_args
-        )
+        source_vm = broker_args.pop("source_vm", caller_host.name)
+        caller_host._prov_inst.release(source_vm, broker_args)
 
     def _set_attributes(self, host_inst, broker_args=None, misc_attrs=None):
         host_inst.__dict__.update(
             {
                 "release": self._host_release,
                 "_prov_inst": self,
                 "_broker_provider": "AnsibleTower",
```

### Comparing `broker-0.3.2/broker/providers/container.py` & `broker-0.3.3/broker/providers/container.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/providers/test_provider.py` & `broker-0.3.3/broker/providers/test_provider.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/session.py` & `broker-0.3.3/broker/session.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker/settings.py` & `broker-0.3.3/broker/settings.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker.egg-info/PKG-INFO` & `broker-0.3.3/broker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broker
-Version: 0.3.2
+Version: 0.3.3
 Summary: The infrastructure middleman.
 Home-page: https://github.com/SatelliteQE/broker
 Author: Jacob J Callahan
 Author-email: jacob.callahan05@gmail.com
 License: GNU General Public License v3
 Keywords: broker,AnsibleTower
 Platform: UNKNOWN
```

### Comparing `broker-0.3.2/broker.egg-info/SOURCES.txt` & `broker-0.3.3/broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/broker_settings.yaml.example` & `broker-0.3.3/broker_settings.yaml.example`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,17 @@
             host_password: "<plain text password>"
     runtime: 'docker'
     # name used to prefix container names, used to distinguish yourself
     # if not set, then your local username will be used
     # name_prefix: test
     results_limit: 50
     auto_map_ports: False
+Beaker:
+    hub_url:
+    max_job_wait: 24h
 TestProvider:
     instances:
         - test1:
             foo: "bar"
             default: True
         - test2:
             foo: "baz"
```

### Comparing `broker-0.3.2/setup.cfg` & `broker-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/data/ansible_tower/fake_children.json` & `broker-0.3.3/tests/data/ansible_tower/fake_children.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/data/ansible_tower/fake_jobs.json` & `broker-0.3.3/tests/data/ansible_tower/fake_jobs.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/data/container/fake_containers.json` & `broker-0.3.3/tests/data/container/fake_containers.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/data/container/fake_images.json` & `broker-0.3.3/tests/data/container/fake_images.json`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/data/fake_inventory.yaml` & `broker-0.3.3/tests/data/fake_inventory.yaml`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/functional/README.md` & `broker-0.3.3/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/functional/test_containers.py` & `broker-0.3.3/tests/functional/test_satlab.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 import pytest
 from click.testing import CliRunner
 from broker import Broker
 from broker.commands import cli
-from broker.providers.container import Container
+from broker.providers.ansible_tower import AnsibleTower
 from broker.settings import inventory_path
 
-SCENARIO_DIR = Path("tests/data/cli_scenarios/containers")
+SCENARIO_DIR = Path("tests/data/cli_scenarios/satlab")
 
 
 @pytest.fixture(scope="module", autouse=True)
 def skip_if_not_configured():
     try:
-        Container()
+        AnsibleTower()
     except Exception as err:
-        pytest.skip(f"Container is not configured correctly: {err}")
+        pytest.skip(f"AnsibleTower is not configured correctly: {err}")
 
 
 @pytest.fixture(scope="module")
 def temp_inventory():
     """Temporarily move the local inventory, then move it back when done"""
     backup_path = inventory_path.rename(f"{inventory_path.absolute()}.bak")
     yield
     CliRunner().invoke(
-        cli, ["checkin", "--all", "--filter", "_broker_provider<Container"]
+        cli, ["checkin", "--all", "--filter", "_broker_provider<AnsibleTower"]
     )
     inventory_path.unlink()
     backup_path.rename(inventory_path)
 
 
-# ----- CLI Scenario Tests -----
-
 @pytest.mark.parametrize(
     "args_file", [f for f in SCENARIO_DIR.iterdir() if f.name.startswith("checkout_")]
 )
 def test_checkout_scenarios(args_file, temp_inventory):
     result = CliRunner().invoke(cli, ["checkout", "--args-file", args_file])
     assert result.exit_code == 0
 
@@ -45,77 +43,75 @@
 )
 def test_execute_scenarios(args_file):
     result = CliRunner().invoke(cli, ["execute", "--args-file", args_file])
     assert result.exit_code == 0
 
 
 def test_inventory_sync():
-    result = CliRunner().invoke(cli, ["inventory", "--sync", "Container"])
+    result = CliRunner().invoke(cli, ["inventory", "--sync", "AnsibleTower"])
     assert result.exit_code == 0
 
 
-def test_containerhosts_list():
-    result = CliRunner().invoke(cli, ["providers", "Container", "--container-hosts"])
+def test_workflows_list():
+    result = CliRunner().invoke(cli, ["providers", "AnsibleTower", "--workflows"])
     assert result.exit_code == 0
 
 
-def test_containerhost_query():
+def test_workflow_query():
     result = CliRunner().invoke(
-        cli, ["providers", "Container", "--container-host", "ubi8:latest"]
+        cli, ["providers", "AnsibleTower", "--workflow", "list-templates"]
     )
     assert result.exit_code == 0
 
 
 # ----- Broker API Tests -----
 
-def test_container_e2e():
-    with Broker(container_host="ubi8:latest") as c_host:
-        assert c_host._cont_inst.top()['Processes']
-        res = c_host.execute("hostname")
-        assert res.stdout.strip() == c_host.hostname
+def test_tower_host():
+    with Broker(workflow="deploy-base-rhel") as r_host:
+        res = r_host.execute("hostname")
+        assert res.stdout.strip() == r_host.hostname
         loc_settings_path = Path("broker_settings.yaml")
         remote_dir = "/tmp/fake"
-        c_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
-        res = c_host.execute(f"ls {remote_dir}")
+        r_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
+        res = r_host.execute(f"ls {remote_dir}")
         assert str(loc_settings_path) in res.stdout
         with NamedTemporaryFile() as tmp:
-            c_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
-            data = c_host.session.sftp_read(
+            r_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
+            data = r_host.session.sftp_read(
                 f"{remote_dir}/{loc_settings_path.name}", return_data=True
             )
             assert (
                 loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
             ), "Local file is different from the received one"
             assert (
                 loc_settings_path.read_bytes() == data
             ), "Local file is different from the received one (return_data=True)"
             assert data == Path(tmp.file.name).read_bytes(), "Received files do not match"
         # test the tail_file context manager
         tailed_file = f"{remote_dir}/tail_me.txt"
-        c_host.execute(f"echo 'hello world' > {tailed_file}")
-        with c_host.session.tail_file(tailed_file) as tf:
-            c_host.execute(f"echo 'this is a new line' >> {tailed_file}")
+        r_host.execute(f"echo 'hello world' > {tailed_file}")
+        with r_host.session.tail_file(tailed_file) as tf:
+            r_host.execute(f"echo 'this is a new line' >> {tailed_file}")
         assert 'this is a new line' in tf.stdout
         assert 'hello world' not in tf.stdout
 
 
-def test_container_e2e_mp():
-    with Broker(container_host="ubi8:latest", _count=7) as c_hosts:
-        for c_host in c_hosts:
-            assert c_host._cont_inst.top()['Processes']
-            res = c_host.execute("hostname")
-            assert res.stdout.strip() == c_host.hostname
+def test_tower_host_mp():
+    with Broker(workflow="deploy-base-rhel", _count=3) as r_hosts:
+        for r_host in r_hosts:
+            res = r_host.execute("hostname")
+            assert res.stdout.strip() == r_host.hostname
             loc_settings_path = Path("broker_settings.yaml")
             remote_dir = "/tmp/fake"
-            c_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
-            res = c_host.execute(f"ls {remote_dir}")
+            r_host.session.sftp_write(loc_settings_path.name, f"{remote_dir}/")
+            res = r_host.execute(f"ls {remote_dir}")
             assert str(loc_settings_path) in res.stdout
             with NamedTemporaryFile() as tmp:
-                c_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
-                data = c_host.session.sftp_read(
+                r_host.session.sftp_read(f"{remote_dir}/{loc_settings_path.name}", tmp.file.name)
+                data = r_host.session.sftp_read(
                     f"{remote_dir}/{loc_settings_path.name}", return_data=True
                 )
                 assert (
                     loc_settings_path.read_bytes() == Path(tmp.file.name).read_bytes()
                 ), "Local file is different from the received one"
                 assert (
                     loc_settings_path.read_bytes() == data
```

### Comparing `broker-0.3.2/tests/providers/test_ansible_tower.py` & `broker-0.3.3/tests/providers/test_ansible_tower.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
     stubbing for:
      - root.load_session.get()
      - root.available_versions.v2.get()
      - v2.ping.get().version
      - v2.jobs.get(id=child_id).results.pop()
      - v2.workflow_job_templates.get(name=workflow).results.pop()
-     - v2.workflow_job_templates.get(name=workflow).results.pop()
      - wfjt.launch(payload={"extra_vars": str(kwargs).replace("--", "")})
      - job.wait_until_completed()
      - merge_dicts(artifacts, at_object.artifacts)
      - at_object.get_related("workflow_nodes").results
     """
 
     def __init__(self, **kwargs):
@@ -90,19 +89,28 @@
 
 def test_execute(tower_stub):
     job = tower_stub.execute(workflow="deploy-base-rhel")
     assert "workflow_nodes" in job.related
 
 
 def test_host_creation(tower_stub):
-    vmb = Broker()
+    bx = Broker()
     job = tower_stub.execute(workflow="deploy-base-rhel")
-    host = tower_stub.construct_host(job, vmb.host_classes)
-    assert isinstance(host, vmb.host_classes["host"])
+    host = tower_stub.construct_host(job, bx.host_classes)
+    assert isinstance(host, bx.host_classes["host"])
     assert host.hostname == "fake.host.test.com"
     assert host._broker_args["os_distribution_version"] == "7.8"
 
 
 def test_workflow_lookup_failure(tower_stub):
     with pytest.raises(Broker.ProviderError) as err:
         tower_stub.execute(workflow="this-does-not-exist")
     assert "Workflow not found by name: this-does-not-exist" in err.value.message
+
+
+def test_host_release_dual_params(tower_stub):
+    bx = Broker()
+    job = tower_stub.execute(workflow="deploy-base-rhel")
+    host = tower_stub.construct_host(job, bx.host_classes)
+    host._broker_args["source_vm"] = "fake-physical-host"
+    assert host._broker_args["source_vm"] == host.name
+    host.release()
```

### Comparing `broker-0.3.2/tests/providers/test_container.py` & `broker-0.3.3/tests/providers/test_container.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/test_helpers.py` & `broker-0.3.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `broker-0.3.2/tests/test_settings.py` & `broker-0.3.3/tests/test_settings.py`

 * *Files identical despite different names*

