# Comparing `tmp/experiment-launcher-2.2.tar.gz` & `tmp/experiment-launcher-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-launcher-2.2.tar", last modified: Thu Feb  2 14:52:55 2023, max compression
+gzip compressed data, was "experiment-launcher-2.3.tar", last modified: Fri Jun 30 13:48:03 2023, max compression
```

## Comparing `experiment-launcher-2.2.tar` & `experiment-launcher-2.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 carvalho  (1000) carvalho  (1000)        0 2023-02-02 14:52:55.349582 experiment-launcher-2.2/
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)     1063 2023-01-30 16:46:58.000000 experiment-launcher-2.2/LICENSE
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)       42 2023-01-30 16:46:58.000000 experiment-launcher-2.2/MANIFEST.in
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)      573 2023-02-02 14:52:55.349582 experiment-launcher-2.2/PKG-INFO
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)     5799 2023-01-30 16:46:58.000000 experiment-launcher-2.2/README.md
-drwxrwxr-x   0 carvalho  (1000) carvalho  (1000)        0 2023-02-02 14:52:55.349582 experiment-launcher-2.2/experiment_launcher/
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)      232 2023-02-02 14:16:07.000000 experiment-launcher-2.2/experiment_launcher/__init__.py
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)     1515 2023-02-02 14:22:39.000000 experiment-launcher-2.2/experiment_launcher/decorators.py
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)      447 2023-01-30 16:46:58.000000 experiment-launcher-2.2/experiment_launcher/exceptions.py
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)    17645 2023-02-02 14:15:23.000000 experiment-launcher-2.2/experiment_launcher/launcher.py
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)     3203 2023-02-02 14:26:13.000000 experiment-launcher-2.2/experiment_launcher/utils.py
-drwxrwxr-x   0 carvalho  (1000) carvalho  (1000)        0 2023-02-02 14:52:55.349582 experiment-launcher-2.2/experiment_launcher.egg-info/
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)      573 2023-02-02 14:52:55.000000 experiment-launcher-2.2/experiment_launcher.egg-info/PKG-INFO
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)      472 2023-02-02 14:52:55.000000 experiment-launcher-2.2/experiment_launcher.egg-info/SOURCES.txt
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)        1 2023-02-02 14:52:55.000000 experiment-launcher-2.2/experiment_launcher.egg-info/dependency_links.txt
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)        1 2023-01-30 16:47:56.000000 experiment-launcher-2.2/experiment_launcher.egg-info/not-zip-safe
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)       36 2023-02-02 14:52:55.000000 experiment-launcher-2.2/experiment_launcher.egg-info/requires.txt
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)       20 2023-02-02 14:52:55.000000 experiment-launcher-2.2/experiment_launcher.egg-info/top_level.txt
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)       36 2023-01-30 16:46:58.000000 experiment-launcher-2.2/requirements.txt
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)       38 2023-02-02 14:52:55.349582 experiment-launcher-2.2/setup.cfg
--rw-rw-r--   0 carvalho  (1000) carvalho  (1000)     1233 2023-01-30 16:46:58.000000 experiment-launcher-2.2/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-30 13:48:03.266129 experiment-launcher-2.3/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       42 2023-06-30 09:48:52.000000 experiment-launcher-2.3/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)      581 2023-06-30 13:48:03.266129 experiment-launcher-2.3/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5799 2023-06-30 09:48:52.000000 experiment-launcher-2.3/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-30 13:48:03.266129 experiment-launcher-2.3/experiment_launcher/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      232 2023-06-30 13:47:52.000000 experiment-launcher-2.3/experiment_launcher/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1628 2023-06-30 13:40:31.000000 experiment-launcher-2.3/experiment_launcher/decorators.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      447 2023-06-30 09:48:52.000000 experiment-launcher-2.3/experiment_launcher/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17645 2023-06-30 09:48:52.000000 experiment-launcher-2.3/experiment_launcher/launcher.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3186 2023-06-30 13:40:31.000000 experiment-launcher-2.3/experiment_launcher/utils.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-30 13:48:03.266129 experiment-launcher-2.3/experiment_launcher.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      581 2023-06-30 13:48:03.000000 experiment-launcher-2.3/experiment_launcher.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      464 2023-06-30 13:48:03.000000 experiment-launcher-2.3/experiment_launcher.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-30 13:48:03.000000 experiment-launcher-2.3/experiment_launcher.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-30 13:40:48.000000 experiment-launcher-2.3/experiment_launcher.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)       36 2023-06-30 13:48:03.000000 experiment-launcher-2.3/experiment_launcher.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       20 2023-06-30 13:48:03.000000 experiment-launcher-2.3/experiment_launcher.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       36 2023-06-30 09:48:52.000000 experiment-launcher-2.3/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-30 13:48:03.266129 experiment-launcher-2.3/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1233 2023-06-30 09:48:52.000000 experiment-launcher-2.3/setup.py
```

### Comparing `experiment-launcher-2.2/PKG-INFO` & `experiment-launcher-2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: experiment-launcher
-Version: 2.2
+Version: 2.3
 Summary: A Python toolkit for launching experiments.
 Home-page: https://git.ias.informatik.tu-darmstadt.de/common/experiment_launcher
 Author: Davide Tateo, Joao Carvalho
 Author-email: davide@robot-learning.de, joao@robot-learning.de
 License: MIT
+Description: experiment_launcher is a Python library used to run experiments. Supports Joblib and slurm jobs.
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
-
-experiment_launcher is a Python library used to run experiments. Supports Joblib and slurm jobs.
```

### Comparing `experiment-launcher-2.2/README.md` & `experiment-launcher-2.3/README.md`

 * *Files identical despite different names*

### Comparing `experiment-launcher-2.2/experiment_launcher/decorators.py` & `experiment-launcher-2.3/experiment_launcher/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 
     return wrapper
 
 
 single_experiment = partial(wrapper_single_experiment)
 single_experiment_flat = partial(wrapper_single_experiment, make_dirs_with_seed=False)
 single_experiment_yaml = partial(wrapper_single_experiment, save_args_yaml=True, use_logging=True, print_exp_args=False)
+single_experiment_flat_yaml = partial(wrapper_single_experiment, make_dirs_with_seed=False, save_args_yaml=True)
```

### Comparing `experiment-launcher-2.2/experiment_launcher/launcher.py` & `experiment-launcher-2.3/experiment_launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `experiment-launcher-2.2/experiment_launcher/utils.py` & `experiment-launcher-2.3/experiment_launcher/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,31 +42,31 @@
         print('------------------------------------------------------------------------------------')
         print('--------> Experiment arguments')
         print(json.dumps(args, indent=2))
         print('------------------------------------------------------------------------------------')
 
 
 def is_local():
-    return (which('slurm') is None) or (which('sbatch') is None)
+    return which('sbatch') is None
 
 
 def start_wandb(
         wandb_enabled=False,
         wandb_entity='experiment_launcher',
         wandb_project='test_experiment_launcher',
         wandb_group=None,
         wandb_run_name=None,
         **kwargs
 ):
     # https://github.com/wandb/wandb/issues/3911#issuecomment-1409769887
     # workaround to make sure that wandb does not crash
-    os.environ["WANDB__SERVICE_WAIT"] = "300"
+    os.environ["WANDB__SERVICE_WAIT"] = "600"
 
     if not wandb_enabled:
-        return wandb.init(mode="disabled")
+        return wandb.init(mode="disabled", reinit=True)
 
     init = {
         "entity": wandb_entity,
         "project": wandb_project,
         "group": wandb_group,
         "name": wandb_run_name,
         "reinit": True,
```

### Comparing `experiment-launcher-2.2/experiment_launcher.egg-info/PKG-INFO` & `experiment-launcher-2.3/experiment_launcher.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: experiment-launcher
-Version: 2.2
+Version: 2.3
 Summary: A Python toolkit for launching experiments.
 Home-page: https://git.ias.informatik.tu-darmstadt.de/common/experiment_launcher
 Author: Davide Tateo, Joao Carvalho
 Author-email: davide@robot-learning.de, joao@robot-learning.de
 License: MIT
+Description: experiment_launcher is a Python library used to run experiments. Supports Joblib and slurm jobs.
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
-
-experiment_launcher is a Python library used to run experiments. Supports Joblib and slurm jobs.
```

### Comparing `experiment-launcher-2.2/setup.py` & `experiment-launcher-2.3/setup.py`

 * *Files identical despite different names*

