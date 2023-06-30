# Comparing `tmp/influxdb3-python-cli-0.2.1.tar.gz` & `tmp/influxdb3-python-cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-cli-0.2.1.tar", last modified: Fri Jun 30 14:36:39 2023, max compression
+gzip compressed data, was "influxdb3-python-cli-0.2.2.tar", last modified: Fri Jun 30 14:58:29 2023, max compression
```

## Comparing `influxdb3-python-cli-0.2.1.tar` & `influxdb3-python-cli-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 14:36:39.000000 influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/config_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9564 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/influxdb_cli/influx3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:36:39.031549 influxdb3-python-cli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 14:36:27.000000 influxdb3-python-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:29.285176 influxdb3-python-cli-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:58:29.285176 influxdb3-python-cli-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:29.285176 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 14:58:29.000000 influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:29.285176 influxdb3-python-cli-0.2.2/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/influxdb_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/influxdb_cli/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9557 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/influxdb_cli/influx3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:58:29.285176 influxdb3-python-cli-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-30 14:58:14.000000 influxdb3-python-cli-0.2.2/setup.py
```

### Comparing `influxdb3-python-cli-0.2.1/LICENSE` & `influxdb3-python-cli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.1/PKG-INFO` & `influxdb3-python-cli-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.2 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.2.1/README.md` & `influxdb3-python-cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.1/influxdb3_python_cli.egg-info/PKG-INFO` & `influxdb3-python-cli-0.2.2/influxdb3_python_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Community Python client for InfluxDB 3.0 (CLI)
 Home-page: https://github.com/InfluxCommunity/influxdb-python-cli
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: influxdb3-python-cli Version: 0.2.2 Summary:
 Community Python client for InfluxDB 3.0 (CLI) Home-page: https://github.com/
 InfluxCommunity/influxdb-python-cli Author: InfluxData Author-email:
 contact@influxdata.com Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `influxdb3-python-cli-0.2.1/influxdb_cli/config_helper.py` & `influxdb3-python-cli-0.2.2/influxdb_cli/helper.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-cli-0.2.1/influxdb_cli/influx3.py` & `influxdb3-python-cli-0.2.2/influxdb_cli/influx3.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 import json
 from prompt_toolkit import PromptSession
 from prompt_toolkit.lexers import PygmentsLexer
 from pygments.lexers import SqlLexer
 from influxdb_client_3 import InfluxDBClient3
 import os
-from config_helper import config_helper
+from helper import config_helper
 
 _usage_string = """
 to write data use influxdb line protocol:
 > influx3 write testmes,tag1=tagvalue field1=0.0 <optional timestamp>
 
 to read data with sql:
 > influx3 sql select * from testmes where time > now() - interval'1 minute'
```

### Comparing `influxdb3-python-cli-0.2.1/setup.py` & `influxdb3-python-cli-0.2.2/setup.py`

 * *Files identical despite different names*

