# Comparing `tmp/apm4py-0.1.8.tar.gz` & `tmp/apm4py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apm4py-0.1.8.tar", max compression
+gzip compressed data, was "apm4py-0.1.9.tar", max compression
```

## Comparing `apm4py-0.1.8.tar` & `apm4py-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11356 2023-06-30 16:02:03.613275 apm4py-0.1.8/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-30 18:57:46.267521 apm4py-0.1.8/README.md
--rw-r--r--   0        0        0     2470 2023-06-30 16:02:03.652836 apm4py-0.1.8/apm4py/__init__.py
--rw-r--r--   0        0        0       89 2023-06-30 18:57:46.397157 apm4py-0.1.8/apm4py/aggregation/__init__.py
--rw-r--r--   0        0        0    11018 2023-06-30 18:57:46.409848 apm4py-0.1.8/apm4py/aggregation/core.py
--rw-r--r--   0        0        0     3458 2023-06-30 18:57:46.415322 apm4py-0.1.8/apm4py/aggregation/groupings.py
--rw-r--r--   0        0        0     2842 2023-06-30 18:57:46.415662 apm4py-0.1.8/apm4py/aggregation/metrics.py
--rw-r--r--   0        0        0      113 2023-06-30 16:02:03.652469 apm4py-0.1.8/apm4py/aggregation/utils.py
--rw-r--r--   0        0        0     4732 2023-06-30 18:57:46.345756 apm4py-0.1.8/apm4py/api.py
--rw-r--r--   0        0        0     2594 2023-06-30 18:57:46.276978 apm4py-0.1.8/apm4py/cli.py
--rw-r--r--   0        0        0      893 2023-06-30 16:02:03.668554 apm4py-0.1.8/apm4py/decorators.py
--rw-r--r--   0        0        0     5408 2023-06-30 16:02:03.667510 apm4py-0.1.8/apm4py/filter.py
--rw-r--r--   0        0        0    23919 2023-06-30 18:57:46.385216 apm4py-0.1.8/apm4py/logs.py
--rw-r--r--   0        0        0     1019 2023-06-30 18:57:46.277064 apm4py-0.1.8/apm4py/process_mining_api.py
--rw-r--r--   0        0        0     3733 2023-06-30 18:57:46.277036 apm4py-0.1.8/apm4py/resources.py
--rw-r--r--   0        0        0      898 2023-06-30 16:02:03.668268 apm4py-0.1.8/apm4py/structures.py
--rw-r--r--   0        0        0     6711 2023-06-30 16:02:03.666158 apm4py-0.1.8/apm4py/utils.py
--rw-r--r--   0        0        0      394 2023-06-30 19:00:17.135994 apm4py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2275 1970-01-01 00:00:00.000000 apm4py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-30 16:02:03.613275 apm4py-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2076 2023-06-30 19:10:49.411441 apm4py-0.1.9/README.md
+-rw-r--r--   0        0        0     2470 2023-06-30 16:02:03.652836 apm4py-0.1.9/apm4py/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-30 18:57:46.397157 apm4py-0.1.9/apm4py/aggregation/__init__.py
+-rw-r--r--   0        0        0    11018 2023-06-30 18:57:46.409848 apm4py-0.1.9/apm4py/aggregation/core.py
+-rw-r--r--   0        0        0     3458 2023-06-30 18:57:46.415322 apm4py-0.1.9/apm4py/aggregation/groupings.py
+-rw-r--r--   0        0        0     2842 2023-06-30 18:57:46.415662 apm4py-0.1.9/apm4py/aggregation/metrics.py
+-rw-r--r--   0        0        0      113 2023-06-30 16:02:03.652469 apm4py-0.1.9/apm4py/aggregation/utils.py
+-rw-r--r--   0        0        0     4732 2023-06-30 18:57:46.345756 apm4py-0.1.9/apm4py/api.py
+-rw-r--r--   0        0        0     3383 2023-06-30 19:49:12.867227 apm4py-0.1.9/apm4py/cli.py
+-rw-r--r--   0        0        0      893 2023-06-30 16:02:03.668554 apm4py-0.1.9/apm4py/decorators.py
+-rw-r--r--   0        0        0     5408 2023-06-30 16:02:03.667510 apm4py-0.1.9/apm4py/filter.py
+-rw-r--r--   0        0        0    23919 2023-06-30 18:57:46.385216 apm4py-0.1.9/apm4py/logs.py
+-rw-r--r--   0        0        0     1019 2023-06-30 18:57:46.277064 apm4py-0.1.9/apm4py/process_mining_api.py
+-rw-r--r--   0        0        0     3733 2023-06-30 18:57:46.277036 apm4py-0.1.9/apm4py/resources.py
+-rw-r--r--   0        0        0      898 2023-06-30 16:02:03.668268 apm4py-0.1.9/apm4py/structures.py
+-rw-r--r--   0        0        0     6711 2023-06-30 16:02:03.666158 apm4py-0.1.9/apm4py/utils.py
+-rw-r--r--   0        0        0      413 2023-06-30 19:51:27.046960 apm4py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 apm4py-0.1.9/PKG-INFO
```

### Comparing `apm4py-0.1.8/LICENSE` & `apm4py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/README.md` & `apm4py-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,22 +32,28 @@
 * event log CSV has "event" in the file name
 * case attribute CSV has "case" in the file name
 * event log semantics json have "event" in the file name
 * case attribute log semantics json have "case" in the file name
 
 See ./tests/data/incident_management as an example.
 
-With that you can do 
-`poetry run apm --name "Incident Management" tests/data/incident_management`
+To install the CLI globally, use [pipx](https://pypa.github.io/pipx/installation/):
+```bash
+pipx install apm4py
+apm --name "Incident Management" tests/data/incident_management
+```
+
+It will prompt you for host settings on the first run and also supports having multiple profiles with different hosts. Similar as the aws-cli. Profiles are saved in `~/.apm/`.
+
 
-# Building and installing
+# Building and installing from source
 ```bash
 poetry install
 poetry build
-pip install /dist/apm4py-0.1.7-py3-none-any.whl
+pip install /dist/apm4py-0.X.Y-py3-none-any.whl
 ```
 
 
 # How to contribute
 
 See the details in [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `apm4py-0.1.8/apm4py/__init__.py` & `apm4py-0.1.9/apm4py/__init__.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/aggregation/core.py` & `apm4py-0.1.9/apm4py/aggregation/core.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/aggregation/groupings.py` & `apm4py-0.1.9/apm4py/aggregation/groupings.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/aggregation/metrics.py` & `apm4py-0.1.9/apm4py/aggregation/metrics.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/api.py` & `apm4py-0.1.9/apm4py/api.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/cli.py` & `apm4py-0.1.9/apm4py/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import glob
 import json
 import os
 from pathlib import Path
+import polars as pl
 import sys
 import typer
 from typing import Optional
 
 import apm4py
 
 app = typer.Typer()
@@ -13,14 +14,53 @@
 
 @app.command()
 def upload(
     data_folder: str = typer.Argument(help="Folder where data sets are stored"),
     name: Optional[str] = typer.Option(None, help="Name of the event log"),
     profile: str = typer.Option("default", help="Profile of the Process Mining host"),
 ):
+    profile_config = get_profile_config(profile)
+    api = apm4py.create_api(**profile_config)
+    event_file = get_file_by_pattern(data_folder, "*[eE]vent*.csv")
+    event_semantics = get_file_by_pattern(data_folder, "*[eE]vent*.json")
+    case_file = get_file_by_pattern(data_folder, "*[cC]ase*.csv")
+    case_semantics = get_file_by_pattern(data_folder, "*[cC]ase*.json")
+
+    name = name if name is not None else Path(event_file).stem
+    api.upload_event_log_file(
+        name=name,
+        event_file_path=event_file,
+        event_semantics_path=event_semantics,
+        case_file_path=case_file,
+        case_semantics_path=case_semantics,
+    )
+
+
+@app.command()
+def list_logs(
+    profile: str = typer.Option("default", help="Profile of the Process Mining host"),
+):
+    profile_config = get_profile_config(profile)
+    api = apm4py.create_api(**profile_config)
+    logs = api.list_logs()
+
+    if len(logs) > 0:
+        pl.Config.set_fmt_str_lengths(100)
+        print(
+            pl.from_dicts(logs)
+            .with_columns(pl.from_epoch("insertedAt", time_unit="ms"))
+            .select(["name", "insertedAt"])
+            .sort("insertedAt", descending=True)
+        )
+
+    else:
+        print("No logs available")
+
+
+def get_profile_config(profile: str):
     apm_dir = os.path.join(os.environ.get("HOME"), ".apm")
     apm_profile_path = os.path.join(os.environ.get("HOME"), ".apm", profile)
     if not os.path.exists(apm_profile_path):
         if not os.path.exists(apm_dir):
             os.mkdir(apm_dir)
 
         print(f"Profile {profile} does not exists. Please create a profile first.")
@@ -28,16 +68,17 @@
         if profile == "":
             profile = "default"
 
         host = typer.prompt("Hostname")
         scheme = typer.prompt("Scheme", default="https")
         port = typer.prompt("Port", default="auto")
         token = typer.prompt("API Token", default="None")
+        instance = typer.prompt("Instance", default=2)
 
-        profile_config = {"host": host, "scheme": scheme}
+        profile_config = {"host": host, "scheme": scheme, "instance": instance}
 
         if port != "auto":
             profile_config["port"] = port
 
         if token != "None":
             profile_config["token"] = token
 
@@ -45,28 +86,15 @@
         with open(apm_profile_path, "w") as profile_file:
             json.dump(profile_config, profile_file)
 
     else:
         with open(apm_profile_path, "r") as profile_file:
             profile_config = json.loads(profile_file.read())
 
-    api = apm4py.create_api(**profile_config)
-    event_file = get_file_by_pattern(data_folder, "*[eE]vent*.csv")
-    event_semantics = get_file_by_pattern(data_folder, "*[eE]vent*.json")
-    case_file = get_file_by_pattern(data_folder, "*[cC]ase*.csv")
-    case_semantics = get_file_by_pattern(data_folder, "*[cC]ase*.json")
-
-    name = name if name is not None else Path(event_file).stem
-    api.upload_event_log_file(
-        name=name,
-        event_file_path=event_file,
-        event_semantics_path=event_semantics,
-        case_file_path=case_file,
-        case_semantics_path=case_semantics,
-    )
+    return profile_config
 
 
 def get_file_by_pattern(dir: str, file_pattern: str) -> Optional[str]:
     files = glob.glob(os.path.join(dir, file_pattern))
     if len(files) == 0:
         return None
```

### Comparing `apm4py-0.1.8/apm4py/decorators.py` & `apm4py-0.1.9/apm4py/decorators.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/filter.py` & `apm4py-0.1.9/apm4py/filter.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/logs.py` & `apm4py-0.1.9/apm4py/logs.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/process_mining_api.py` & `apm4py-0.1.9/apm4py/process_mining_api.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/resources.py` & `apm4py-0.1.9/apm4py/resources.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/structures.py` & `apm4py-0.1.9/apm4py/structures.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/apm4py/utils.py` & `apm4py-0.1.9/apm4py/utils.py`

 * *Files identical despite different names*

### Comparing `apm4py-0.1.8/PKG-INFO` & `apm4py-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apm4py
-Version: 0.1.8
+Version: 0.1.9
 Summary: apm4py is a Python API for Appian Process Mining (APM)
 Author: Appian
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: polars (>=0.18.4,<0.19.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # apm4py
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg
 )](https://www.python.org/downloads/release/python-374/)
@@ -46,22 +47,28 @@
 * event log CSV has "event" in the file name
 * case attribute CSV has "case" in the file name
 * event log semantics json have "event" in the file name
 * case attribute log semantics json have "case" in the file name
 
 See ./tests/data/incident_management as an example.
 
-With that you can do 
-`poetry run apm --name "Incident Management" tests/data/incident_management`
+To install the CLI globally, use [pipx](https://pypa.github.io/pipx/installation/):
+```bash
+pipx install apm4py
+apm --name "Incident Management" tests/data/incident_management
+```
+
+It will prompt you for host settings on the first run and also supports having multiple profiles with different hosts. Similar as the aws-cli. Profiles are saved in `~/.apm/`.
+
 
-# Building and installing
+# Building and installing from source
 ```bash
 poetry install
 poetry build
-pip install /dist/apm4py-0.1.7-py3-none-any.whl
+pip install /dist/apm4py-0.X.Y-py3-none-any.whl
 ```
 
 
 # How to contribute
 
 See the details in [CONTRIBUTING.md](CONTRIBUTING.md).
```

