# Comparing `tmp/griffon-0.2.8.tar.gz` & `tmp/griffon-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.8.tar", last modified: Wed Jun 28 11:45:57 2023, max compression
+gzip compressed data, was "griffon-0.2.9.tar", last modified: Thu Jun 29 11:32:10 2023, max compression
```

## Comparing `griffon-0.2.8.tar` & `griffon-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.841769 griffon-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-28 11:45:42.000000 griffon-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-28 11:45:57.841769 griffon-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-28 11:45:42.000000 griffon-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    26911 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    51297 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.841769 griffon-0.2.8/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.841769 griffon-0.2.8/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-28 11:45:42.000000 griffon-0.2.8/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.837769 griffon-0.2.8/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-28 11:45:57.000000 griffon-0.2.8/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-28 11:45:42.000000 griffon-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:45:57.841769 griffon-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-28 11:45:42.000000 griffon-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:45:57.841769 griffon-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-28 11:45:42.000000 griffon-0.2.8/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.770885 griffon-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 11:31:52.000000 griffon-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-29 11:32:10.770885 griffon-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-29 11:31:52.000000 griffon-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52387 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35899 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-29 11:31:52.000000 griffon-0.2.9/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.766885 griffon-0.2.9/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 11:32:10.000000 griffon-0.2.9/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-29 11:31:52.000000 griffon-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:32:10.770885 griffon-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-29 11:31:52.000000 griffon-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:32:10.770885 griffon-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-29 11:31:52.000000 griffon-0.2.9/tests/test_unit.py
```

### Comparing `griffon-0.2.8/LICENSE` & `griffon-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/PKG-INFO` & `griffon-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.8/README.md` & `griffon-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/__init__.py` & `griffon-0.2.9/griffon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
```

### Comparing `griffon-0.2.8/griffon/autocomplete/__init__.py` & `griffon-0.2.9/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/cli.py` & `griffon-0.2.9/griffon/cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/configure.py` & `griffon-0.2.9/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/docs.py` & `griffon-0.2.9/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/entities/__init__.py` & `griffon-0.2.9/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.9/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/entities/corgi.py` & `griffon-0.2.9/griffon/commands/entities/corgi.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/entities/helpers.py` & `griffon-0.2.9/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/entities/osidb.py` & `griffon-0.2.9/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugin_commands.py` & `griffon-0.2.9/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugins/bugzilla.py` & `griffon-0.2.9/griffon/commands/plugins/bugzilla.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.9/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.9/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugins/osv.py` & `griffon-0.2.9/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/plugins/semgrep.py` & `griffon-0.2.9/griffon/commands/plugins/semgrep.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/process.py` & `griffon-0.2.9/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/commands/queries.py` & `griffon-0.2.9/griffon/commands/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,22 @@
 )
 from griffon.commands.entities.helpers import query_params_options
 from griffon.commands.reports import (
     generate_affects_report,
     generate_entity_report,
     generate_license_report,
 )
-from griffon.output import console, cprint, raw_json_transform
+from griffon.output import (
+    console,
+    cprint,
+    generate_affects,
+    generate_normalised_results,
+    generate_result_tree,
+    raw_json_transform,
+)
 from griffon.services import QueryService, core_queries  # , exp
 
 logger = logging.getLogger("griffon")
 
 query_service = QueryService()
 
 
@@ -378,26 +385,28 @@
         if ctx.params["sfm2_flaw_id"]:
             console.no_color = True
             console.highlighter = None
             operation_status.stop()
 
             # generate affects
             output = raw_json_transform(q, True)
-            ordered_results = sorted(output["results"], key=lambda d: d["product_stream"])
-            affects = []
-            product_versions = sorted(
-                list(set([item["product_version"] for item in ordered_results]))
+
+            exclude_products = []
+            if get_config_option(ctx.obj["PROFILE"], "exclude"):
+                exclude_products = get_config_option(ctx.obj["PROFILE"], "exclude").split("\n")
+            exclude_components = []
+            if get_config_option(ctx.obj["PROFILE"], "exclude_components"):
+                exclude_components = get_config_option(
+                    ctx.obj["PROFILE"], "exclude_components"
+                ).split("\n")
+            normalised_results = generate_normalised_results(
+                output, exclude_products, exclude_components
             )
-            for pv in product_versions:
-                names = [item["name"] for item in ordered_results if pv == item["product_version"]]
-                names = list(set(names))
-                for name in names:
-                    affects.append(
-                        {"product_version": pv, "component_name": name, "operation": "add"}
-                    )
+            result_tree = generate_result_tree(normalised_results)
+            affects = generate_affects(ctx, result_tree, exclude_components, "add", format="json")
 
             # attempt to import sfm2client module
             try:
                 import sfm2client
             except ImportError:
                 logger.warning("sfm2client library not found, cannot compare with flaw affects")
                 ctx.exit()
```

### Comparing `griffon-0.2.8/griffon/commands/reports.py` & `griffon-0.2.9/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/output.py` & `griffon-0.2.9/griffon/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,123 @@
                 item["ofuri"],
                 item["manifest_link"],
                 no_wrap=no_wrap,
             )
     ctx.exit()
 
 
+def generate_normalised_results(output, exclude_products, exclude_components):
+    normalised_results = list()
+    if "results" in output:
+        for item in output["results"]:
+            for ps in item["product_streams"]:
+                if ps["product_versions"][0]["name"] not in exclude_products:
+                    if not any([match in item["name"] for match in exclude_components]):
+                        c = {
+                            "product_version": ps["product_versions"][0]["name"],
+                            "product_stream": ps.get("name"),
+                            "namespace": item.get("namespace"),
+                            "name": item.get("name"),
+                            "nvr": item.get("nvr"),
+                            "type": item.get("type"),
+                            "arch": item.get("arch"),
+                            "version": item.get("version"),
+                            "related_url": item.get("related_url"),
+                            "purl": item.get("purl"),
+                            "sources": item.get("sources"),
+                            "upstreams": item.get("upstreams"),
+                        }
+                        if "software_build" in item:
+                            c["build_source_url"] = item["software_build"].get("source")
+                        normalised_results.append(c)
+    return normalised_results
+
+
+def generate_result_tree(normalised_results):
+    product_versions = sorted(list(set([item["product_version"] for item in normalised_results])))
+    result_tree = {}
+    for pv in product_versions:
+        result_tree[pv] = {}
+        product_streams = sorted(
+            list(
+                set(
+                    [
+                        item["product_stream"]
+                        for item in normalised_results
+                        if item["product_version"] == pv
+                    ]
+                )
+            )
+        )
+        for ps in product_streams:
+            result_tree[pv][ps] = {}
+            component_names = sorted(
+                list(
+                    set(
+                        [
+                            item["name"]
+                            for item in normalised_results
+                            if item["product_stream"] == ps
+                        ]
+                    )
+                )
+            )
+            for cn in component_names:
+                result_tree[pv][ps][cn] = {}
+                nvrs = [
+                    item
+                    for item in normalised_results
+                    if item["product_stream"] == ps and item["name"] == cn
+                ]
+
+                for nvr in nvrs:
+                    result_tree[pv][ps][cn][nvr["nvr"]] = nvr
+    return result_tree
+
+
+def generate_affects(
+    ctx, result_tree, exclude_components, flaw_operation, format="text", no_wrap=False
+):
+    search_component_name = ctx.params["component_name"]
+    for pv in result_tree.keys():
+        component_names = set()
+        for ps in result_tree[pv].keys():
+            for component_name in result_tree[pv][ps].keys():
+                for nvr in result_tree[pv][ps][component_name].keys():
+                    source_names = [
+                        source["name"]
+                        for source in result_tree[pv][ps][component_name][nvr]["sources"]
+                        if source["namespace"] == "REDHAT"
+                    ]
+                component_names.update(source_names)
+        # we should only show component name if both {component name} and {component name-container} exists # noqa
+        if (
+            search_component_name in component_names
+            and f"{search_component_name}-container" in component_names
+        ):
+            component_names.remove(f"{search_component_name}-container")
+        if format == "text":
+            for cn in component_names:
+                # ensure {component name} is not in profile exclude components enum
+                if not any([match in cn for match in exclude_components]):
+                    console.print(
+                        f"{pv}/{cn}={flaw_operation}",
+                        no_wrap=no_wrap,
+                    )
+        else:
+            affects = []
+            for cn in component_names:
+                # ensure {component name} is not in profile exclude components enum
+                if not any([match in cn for match in exclude_components]):
+                    affects.append(
+                        {"product_version": pv, "component_name": cn, "operation": flaw_operation}
+                    )
+            return affects
+
+
 def text_output_products_contain_component(
     ctx, output, exclude_products, exclude_components, no_wrap=False
 ):
     search_component_name = ctx.params["component_name"]
 
     # handle single component
     if ctx.params["purl"]:
@@ -174,107 +283,33 @@
     if "results" in output and output["count"] > 0:
         console.highlighter = None
 
         # order at the end
         # ordered_results = sorted(output["results"], key=lambda d: d["product_stream"])
 
         # first flatten the tree
-        normalised_results = list()
-        if "results" in output:
-            for item in output["results"]:
-                for ps in item["product_streams"]:
-                    if ps["product_versions"][0]["name"] not in exclude_products:
-                        if not any([match in item["name"] for match in exclude_components]):
-                            c = {
-                                "product_version": ps["product_versions"][0]["name"],
-                                "product_stream": ps.get("name"),
-                                "namespace": item.get("namespace"),
-                                "name": item.get("name"),
-                                "nvr": item.get("nvr"),
-                                "type": item.get("type"),
-                                "arch": item.get("arch"),
-                                "version": item.get("version"),
-                                "related_url": item.get("related_url"),
-                                "purl": item.get("purl"),
-                                "sources": item.get("sources"),
-                                "upstreams": item.get("upstreams"),
-                            }
-                            if "software_build" in item:
-                                c["build_source_url"] = item["software_build"].get("source")
-                            normalised_results.append(c)
-        product_versions = sorted(
-            list(set([item["product_version"] for item in normalised_results]))
+        normalised_results = generate_normalised_results(
+            output, exclude_products, exclude_components
         )
-        result_tree = {}
-        for pv in product_versions:
-            result_tree[pv] = {}
-            product_streams = sorted(
-                list(
-                    set(
-                        [
-                            item["product_stream"]
-                            for item in normalised_results
-                            if item["product_version"] == pv
-                        ]
-                    )
-                )
-            )
-            for ps in product_streams:
-                result_tree[pv][ps] = {}
-                component_names = sorted(
-                    list(
-                        set(
-                            [
-                                item["name"]
-                                for item in normalised_results
-                                if item["product_stream"] == ps
-                            ]
-                        )
-                    )
-                )
-                for cn in component_names:
-                    result_tree[pv][ps][cn] = {}
-                    nvrs = [
-                        item
-                        for item in normalised_results
-                        if item["product_stream"] == ps and item["name"] == cn
-                    ]
-
-                    for nvr in nvrs:
-                        result_tree[pv][ps][cn][nvr["nvr"]] = nvr
+        result_tree = generate_result_tree(normalised_results)
 
         # TODO - MAVEN component type will require special handling
         if ctx.params["affect_mode"]:
             console.no_color = True
             console.highlighter = None
 
             flaw_mode = ctx.params["flaw_mode"]
             flaw_operation = "dry_run"
             if flaw_mode == "add":
                 flaw_operation = "new"
             if flaw_mode == "update":
                 flaw_operation = "update"
 
-            for pv in result_tree.keys():
-                component_names = set()
-                for ps in result_tree[pv].keys():
-                    component_names.update(result_tree[pv][ps].keys())
-                # we should only show component name if both {component name} and {component name-container} exists # noqa
-                if (
-                    search_component_name in component_names
-                    and f"{search_component_name}-container" in component_names
-                ):
-                    component_names.remove(f"{search_component_name}-container")
-                for cn in component_names:
-                    # ensure {component name} is not in profile exclude components enum
-                    if not any([match in cn for match in exclude_components]):
-                        console.print(
-                            f"{pv}/{cn}={flaw_operation}",
-                            no_wrap=no_wrap,
-                        )
+            generate_affects(ctx, result_tree, exclude_components, flaw_operation, no_wrap=False)
+
         else:
             if ctx.obj["VERBOSE"] == 0:  # product_version X component_name
                 for pv in result_tree.keys():
                     component_names = set()
                     for ps in result_tree[pv].keys():
                         component_names.update(result_tree[pv][ps].keys())
                     # we should only show component name if both {component name} and {component name-container} exists # noqa
```

### Comparing `griffon-0.2.8/griffon/services/__init__.py` & `griffon-0.2.9/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/services/core_process.py` & `griffon-0.2.9/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/services/core_queries.py` & `griffon-0.2.9/griffon/services/core_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         self.search_upstreams = self.params.get("search_upstreams")
         self.filter_rh_naming = self.params.get("filter_rh_naming")
         self.no_community = self.params.get("no_community")
 
     def execute(self) -> List[Dict[str, Any]]:
         results = []
         params = {
-            "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,sources.nvr,sources.purl,sources.name,sources.download_url,sources.related_url,upstreams.nvr,upstreams.purl,upstreams.name,upstreams.download_url,upstreams.related_url,release,version,arch,product_streams.product_versions,product_streams.name,product_streams.ofuri",  # noqa
+            "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,sources.nvr,sources.purl,sources.name,sources.namespace,sources.download_url,sources.related_url,upstreams.nvr,upstreams.purl,upstreams.name,upstreams.download_url,upstreams.related_url,release,version,arch,product_streams.product_versions,product_streams.name,product_streams.ofuri",  # noqa
         }
 
         if self.search_latest:
             params["latest_components_by_streams"] = "True"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
```

### Comparing `griffon-0.2.8/griffon/services/core_reports.py` & `griffon-0.2.9/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon/static/default_griffonrc` & `griffon-0.2.9/griffon/static/default_griffonrc`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/griffon.egg-info/PKG-INFO` & `griffon-0.2.9/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.8
+Version: 0.2.9
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.8/griffon.egg-info/SOURCES.txt` & `griffon-0.2.9/griffon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/pyproject.toml` & `griffon-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/setup.py` & `griffon-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_cli.py` & `griffon-0.2.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_entities.py` & `griffon-0.2.9/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_manage.py` & `griffon-0.2.9/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_plugins.py` & `griffon-0.2.9/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_process.py` & `griffon-0.2.9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_queries.py` & `griffon-0.2.9/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_reports.py` & `griffon-0.2.9/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.8/tests/test_unit.py` & `griffon-0.2.9/tests/test_unit.py`

 * *Files identical despite different names*

