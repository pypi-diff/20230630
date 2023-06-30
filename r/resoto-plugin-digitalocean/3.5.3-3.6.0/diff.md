# Comparing `tmp/resoto-plugin-digitalocean-3.5.3.tar.gz` & `tmp/resoto-plugin-digitalocean-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.5.3.tar", last modified: Wed Jun 21 14:23:34 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.6.0.tar", last modified: Fri Jun 30 19:22:29 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.5.3.tar` & `resoto-plugin-digitalocean-3.6.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43858 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:52.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:23:33.000000 resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.994874 resoto-plugin-digitalocean-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:33.998874 resoto-plugin-digitalocean-3.5.3/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/neighbor_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25525 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 14:19:43.000000 resoto-plugin-digitalocean-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.942439 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43858 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.946439 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:01.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.946439 resoto-plugin-digitalocean-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/neighbor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25525 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.5.3/PKG-INFO` & `resoto-plugin-digitalocean-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -14,11 +14,11 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-digitalocean
 DigitalOcean Collector Plugin for Resoto
```

### Comparing `resoto-plugin-digitalocean-3.5.3/pyproject.toml` & `resoto-plugin-digitalocean-3.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean"
 description = "Resoto DigitalOcean Collector Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,23 +23,23 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
-dev = [
+test = [
     "mypy",
     "tzlocal",
 ]
 
 [project.entry-points."resoto.plugins"]
 digitalocean_collector = "resoto_plugin_digitalocean:DigitalOceanCollectorPlugin"
```

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/config.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -14,11 +14,11 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: test
 
 # resoto-plugin-digitalocean
 DigitalOcean Collector Plugin for Resoto
```

### Comparing `resoto-plugin-digitalocean-3.5.3/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.6.0/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.3/test/test_collector.py` & `resoto-plugin-digitalocean-3.6.0/test/test_collector.py`

 * *Files identical despite different names*

