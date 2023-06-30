# Comparing `tmp/lbrlabs_pulumi_cockroach-0.0.1a1688146398.tar.gz` & `tmp/lbrlabs_pulumi_cockroach-0.0.1a1688147067.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_cockroach-0.0.1a1688146398.tar", last modified: Fri Jun 30 17:38:16 2023, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_cockroach-0.0.1a1688147067.tar", last modified: Fri Jun 30 17:49:25 2023, max compression
```

## Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398.tar` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/ca_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/cmek.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_cluster_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_connection_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_person_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/log_export_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/private_endpoint_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/private_endpoint_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/sql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/user_role_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-30 17:38:16.000000 lbrlabs_pulumi_cockroach-0.0.1a1688146398/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/ca_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/cmek.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_cluster_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_connection_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_person_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/log_export_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/private_endpoint_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/private_endpoint_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/user_role_grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:49:25.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-30 17:49:24.000000 lbrlabs_pulumi_cockroach-0.0.1a1688147067/setup.py
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/PKG-INFO` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs_pulumi_cockroach
-Version: 0.0.1a1688146398
+Version: 0.0.1a1688147067
 Summary: A Pulumi package to create and managed cockroach db resources in Pulumi programs.
 Home-page: https://lbrlabs.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-cockroach
 Description: 
         # Cockroach Resource Provider
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/README.md` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/__init__.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/_inputs.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/_inputs.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/_utilities.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/allow_list.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/allow_list.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/ca_cert.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/ca_cert.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/cluster.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/cluster.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/cmek.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/cmek.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/config/vars.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/config/vars.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/database.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/database.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/finalize_version_upgrade.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_cluster_cert.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_cluster_cert.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_cockroach_cluster.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_connection_string.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_connection_string.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_organization.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_organization.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/get_person_user.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/get_person_user.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/log_export_config.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/log_export_config.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/maintenance_window.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/metric_export_cloudwatch_config.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/metric_export_datadog_config.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/outputs.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/outputs.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/private_endpoint_connection.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/private_endpoint_connection.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/private_endpoint_services.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/private_endpoint_services.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/provider.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/sql_user.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/sql_user.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach/user_role_grants.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach/user_role_grants.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs-pulumi-cockroach
-Version: 0.0.1a1688146398
+Version: 0.0.1a1688147067
 Summary: A Pulumi package to create and managed cockroach db resources in Pulumi programs.
 Home-page: https://lbrlabs.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-cockroach
 Description: 
         # Cockroach Resource Provider
```

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/lbrlabs_pulumi_cockroach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_cockroach-0.0.1a1688146398/setup.py` & `lbrlabs_pulumi_cockroach-0.0.1a1688147067/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1a1688146398"
-PLUGIN_VERSION = "0.0.1-alpha.1688146398+99c5389c"
+VERSION = "0.0.1a1688147067"
+PLUGIN_VERSION = "0.0.1-alpha.1688147067+fd70bcbc"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cockroach', PLUGIN_VERSION, '--server', 'github://api.github.com/lbrlabs'])
         except OSError as error:
```

