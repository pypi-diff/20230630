# Comparing `tmp/dysweep-0.0.9.tar.gz` & `tmp/dysweep-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.9.tar", last modified: Sun Jun 18 12:24:51 2023, max compression
+gzip compressed data, was "dysweep-0.1.0.tar", last modified: Fri Jun 30 16:54:48 2023, max compression
```

## Comparing `dysweep-0.0.9.tar` & `dysweep-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 12:22:29.000000 dysweep-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 12:24:51.837873 dysweep-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-18 12:22:29.000000 dysweep-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:24:51.837873 dysweep-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-18 12:22:29.000000 dysweep-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 16:52:28.000000 dysweep-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-30 16:54:48.136932 dysweep-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-30 16:52:28.000000 dysweep-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22831 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 16:52:28.000000 dysweep-0.1.0/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:54:48.136932 dysweep-0.1.0/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 16:54:48.000000 dysweep-0.1.0/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:54:48.136932 dysweep-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-30 16:52:28.000000 dysweep-0.1.0/setup.py
```

### Comparing `dysweep-0.0.9/LICENSE` & `dysweep-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.9/PKG-INFO` & `dysweep-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.9
+Version: 0.1.0
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # Dysweep
```

### Comparing `dysweep-0.0.9/dysweep/utils.py` & `dysweep-0.1.0/dysweep/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,16 @@
                 )
             if isinstance(val, dict) or isinstance(val, list):
                 sanity_check_special_keys(val, current_path + [key])
     elif isinstance(conf, list):
         for idx, val in enumerate(conf):
             if isinstance(val, dict) or isinstance(val, list):
                 sanity_check_special_keys(val, current_path + [str(idx)])
+                
 # overwrite args recursively
-
-
 def upsert_config(args: th.Union[th.Dict, th.List],
                   sweep_config: th.Union[th.Dict, th.List, int, float, str],
                   current_path: th.Optional[th.List[str]] = None,
                   root_args: th.Optional[th.Union[th.Dict, th.List]] = None):
     # try and catch an exception and add "line" to the exception and then re-raise it
     if current_path is None:
         current_path = []
@@ -413,17 +412,14 @@
                     args[-1] = upsert_config(args[-1], val, current_path=current_path + [
                                              str(len(args) - 1)], root_args=root_args)
             else:
                 # a primitive type
                 args = sweep_config
 
         if len(current_path) == 0:
-            # print("Final config:")
-            # pprint(args)
-
             # Sanity check if any of the nested dicts contain special keys
             # If they do, then we need to throw an error
             # This is because we don't want to allow the user to specify
             # a sweep config that has a special key in it
             sanity_check_special_keys(args, current_path=current_path)
 
     except Exception as e:
@@ -435,17 +431,27 @@
                        str(current_path),)
             # update e so that it has the sweep_config
             # format sweep_config in a nice string using pprint
 
             e.args += ("Configuration to upsert: " +
                        json.dumps(sweep_config, indent=2),)
         raise e
-    # print("After upsert:")
-    # pprint(args)
-    # print("000000000000000-------000000000000000")
+    # Change all the __IDX__ arguments to a list
+    # if that is the case here
+    if isinstance(args, dict):
+        is_list_pretender = True
+        for key in args.keys():
+            if not key.startswith(IDX_INDICATOR):
+                is_list_pretender = False
+        if is_list_pretender:
+            all_list_items = [None for _ in range(len(args.keys()))]
+            for key in args.keys():
+                idx = int(key[len(IDX_INDICATOR):])
+                all_list_items[idx] = args[key]
+            args = all_list_items
     return args
 
 
 def standardize_sweep_config(sweep_config: dict):
     global remaining_bunch
     config_copy = {k: copy.deepcopy(v) if isinstance(
         v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
```

### Comparing `dysweep-0.0.9/dysweep/wandbX.py` & `dysweep-0.1.0/dysweep/wandbX.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from pprint import pprint
 import os
 from .utils import standardize_sweep_config, destandardize_sweep_config, upsert_config
 from wandb.sdk.wandb_run import Run, _run_decorator
 from wandb.sdk import wandb_config
 import warnings
 import copy
+from pprint import pprint
 
 METADATA_RUN_NAME_PREFIX = "HIERARCHICAL_SWEEP_"
 
 base_config: th.Optional[dict] = None
 compression: th.Optional[dict] = None
 
 
 def hierarchical_config(conf):
     if base_config is None or compression is None:
         return conf
-    # make a deep copy of the base config
+    # make a deep copy of the base config and upsert it with the current config
     return upsert_config(copy.deepcopy(base_config), destandardize_sweep_config(conf, compression))
 
 
 def sweep(
     base_config: dict,
     sweep_config: dict,
     entity: th.Optional[str] = None,
@@ -33,14 +34,23 @@
     base_config as an artifact. Then, compress the sweepConfiguration
     and turn it into a standard SweepConfig. Finally, pass the SweepConfig
     to wandb.sweep and return the sweep_id.
 
     I ended up with this implementation, because wandb has not yet released the
     Public API, so I had to use the artifacts capability for it to work.
     """
+    # import these three variables from .utils: 
+    # compression_mapping = {}
+    # value_compression_mapping = {}
+    # remaining_bunch = {}
+    from .utils import compression_mapping, value_compression_mapping, remaining_bunch
+    compression_mapping.clear()
+    value_compression_mapping.clear()
+    remaining_bunch.clear()
+    
     # (1) change the sweep_config to a standard sweep_config
     sweep_standard, compression = standardize_sweep_config(sweep_config)
     sweep_metadata = {'base_config': base_config, 'compression': compression}
     sweep_id = wandb.sweep(sweep_standard, entity=entity, project=project)
 
     # (2) create a run and save the base_config as an artifact
     wandb.init(entity=entity, project=project,
```

### Comparing `dysweep-0.0.9/dysweep.egg-info/PKG-INFO` & `dysweep-0.1.0/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.9
+Version: 0.1.0
 Summary: Use Weights and Biases Sweeps for Dynamic Configuration generation.
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # Dysweep
```

### Comparing `dysweep-0.0.9/setup.py` & `dysweep-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,20 @@
     license="Apache License 2.0",
     description="Use Weights and Biases Sweeps for Dynamic Configuration generation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hamid Kamkari",
     author_email="hamidrezakamkari@gmail.com",
     url="https://github.com/HamidrezaKmK/dysweep",
+    entry_points={
+        'console_scripts' : [
+            'dysweep_create = dysweep.console:create_sweep',
+            'dysweep_run_resume = dysweep.console:run_resume_sweep'
+        ]
+    },
     keywords=[
         "dynamic configurations",
         "large scale experiments",
         "deep learning",
         "sweeps",
         "hyperparameter tuning",
         "lazy evaluation"
```

