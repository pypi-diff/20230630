# Comparing `tmp/resoto-plugin-scarf-3.5.3.tar.gz` & `tmp/resoto-plugin-scarf-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-scarf-3.5.3.tar", last modified: Wed Jun 21 14:25:58 2023, max compression
+gzip compressed data, was "resoto-plugin-scarf-3.6.0.tar", last modified: Fri Jun 30 19:25:06 2023, max compression
```

## Comparing `resoto-plugin-scarf-3.5.3.tar` & `resoto-plugin-scarf-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:24:24.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 14:25:58.000000 resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:58.333928 resoto-plugin-scarf-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-21 14:23:18.000000 resoto-plugin-scarf-3.5.3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:25:06.963646 resoto-plugin-scarf-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-30 19:25:06.963646 resoto-plugin-scarf-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:25:06.963646 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:25:06.963646 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:22:40.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 19:25:06.000000 resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:25:06.967646 resoto-plugin-scarf-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:25:06.963646 resoto-plugin-scarf-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-30 19:21:04.000000 resoto-plugin-scarf-3.6.0/test/test_config.py
```

### Comparing `resoto-plugin-scarf-3.5.3/PKG-INFO` & `resoto-plugin-scarf-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Scarf Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-scarf-3.5.3/README.md` & `resoto-plugin-scarf-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.3/pyproject.toml` & `resoto-plugin-scarf-3.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-scarf"
 description = "Resoto Scarf Collector Plugin"
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
     "requests",
 ]
 
 [project.entry-points."resoto.plugins"]
 scarf = "resoto_plugin_scarf:ScarfCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/__init__.py` & `resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/resources.py` & `resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.3/resoto_plugin_scarf/scarf.py` & `resoto-plugin-scarf-3.6.0/resoto_plugin_scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-scarf-3.5.3/resoto_plugin_scarf.egg-info/PKG-INFO` & `resoto-plugin-scarf-3.6.0/resoto_plugin_scarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-scarf
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto Scarf Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/scarf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

