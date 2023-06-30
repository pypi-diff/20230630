# Comparing `tmp/resoto-plugin-slack-3.5.3.tar.gz` & `tmp/resoto-plugin-slack-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-slack-3.5.3.tar", last modified: Wed Jun 21 14:18:48 2023, max compression
+gzip compressed data, was "resoto-plugin-slack-3.6.0.tar", last modified: Fri Jun 30 19:21:51 2023, max compression
```

## Comparing `resoto-plugin-slack-3.5.3.tar` & `resoto-plugin-slack-3.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:48.751801 resoto-plugin-slack-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 14:18:48.751801 resoto-plugin-slack-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:48.747801 resoto-plugin-slack-3.5.3/resoto_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:48.751801 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:17:09.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 14:18:48.000000 resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:18:48.751801 resoto-plugin-slack-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:48.751801 resoto-plugin-slack-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-21 14:16:00.000000 resoto-plugin-slack-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/resoto_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:50.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-slack-3.5.3/PKG-INFO` & `resoto-plugin-slack-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-slack-3.5.3/pyproject.toml` & `resoto-plugin-slack-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-slack"
 description = "Resoto Slack Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."resoto.plugins"]
 slack_bot = "resoto_plugin_slack:SlackBotPlugin"
 slack_collector = "resoto_plugin_slack:SlackCollectorPlugin"
```

### Comparing `resoto-plugin-slack-3.5.3/resoto_plugin_slack/__init__.py` & `resoto-plugin-slack-3.6.0/resoto_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.5.3/resoto_plugin_slack/resources.py` & `resoto-plugin-slack-3.6.0/resoto_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.5.3/resoto_plugin_slack.egg-info/PKG-INFO` & `resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

