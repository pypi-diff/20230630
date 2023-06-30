# Comparing `tmp/dltool-0.1.tar.gz` & `tmp/dltool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltool-0.1.tar", last modified: Thu Jun 22 13:53:34 2023, max compression
+gzip compressed data, was "dltool-0.1.1.tar", last modified: Fri Jun 30 14:10:58 2023, max compression
```

## Comparing `dltool-0.1.tar` & `dltool-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:53:34.384877 dltool-0.1/
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-06-09 12:38:00.000000 dltool-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2392 2023-06-22 13:53:34.384877 dltool-0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      134 2023-06-22 13:04:02.000000 dltool-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:53:34.352877 dltool-0.1/dltool/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-19 01:34:38.000000 dltool-0.1/dltool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1884 2023-02-15 14:06:49.000000 dltool-0.1/dltool/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:53:34.372877 dltool-0.1/dltool/data/
--rw-rw-r--   0 root         (0) root         (0)      174 2023-04-29 04:26:16.000000 dltool-0.1/dltool/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6460 2023-06-09 12:38:12.000000 dltool-0.1/dltool/data/file.py
--rw-rw-r--   0 root         (0) root         (0)     5828 2023-04-29 04:22:08.000000 dltool-0.1/dltool/data/time.py
--rw-rw-r--   0 root         (0) root         (0)      439 2023-04-23 19:43:58.000000 dltool-0.1/dltool/data/union.py
--rw-rw-r--   0 root         (0) root         (0)     1268 2023-04-23 19:45:21.000000 dltool-0.1/dltool/data/utils.py
--rw-rw-r--   0 root         (0) root         (0)      689 2023-06-22 13:39:25.000000 dltool-0.1/dltool/hooks.py
--rw-rw-r--   0 root         (0) root         (0)     6910 2023-06-09 14:01:50.000000 dltool-0.1/dltool/log.py
--rw-rw-r--   0 root         (0) root         (0)     3889 2023-06-22 12:25:28.000000 dltool-0.1/dltool/train.py
--rw-rw-r--   0 root         (0) root         (0)     1625 2023-06-09 12:38:12.000000 dltool-0.1/dltool/types.py
--rw-rw-r--   0 root         (0) root         (0)     4099 2023-04-24 18:33:46.000000 dltool-0.1/dltool/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3823 2023-04-23 19:47:14.000000 dltool-0.1/dltool/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:53:34.352877 dltool-0.1/dltool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2392 2023-06-22 13:53:34.000000 dltool-0.1/dltool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-22 13:53:34.000000 dltool-0.1/dltool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 13:53:34.000000 dltool-0.1/dltool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:53:34.000000 dltool-0.1/dltool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 13:53:34.000000 dltool-0.1/dltool.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      727 2023-06-22 12:10:02.000000 dltool-0.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       37 2023-06-09 13:24:34.000000 dltool-0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:53:34.384877 dltool-0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.244140 dltool-0.1.1/
+-rw-rw-r--   0 root         (0) root         (0)     1497 2023-06-09 12:38:00.000000 dltool-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-30 14:10:58.244140 dltool-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-06-22 13:04:02.000000 dltool-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.240140 dltool-0.1.1/dltool/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-19 01:34:38.000000 dltool-0.1.1/dltool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1884 2023-02-15 14:06:49.000000 dltool-0.1.1/dltool/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.244140 dltool-0.1.1/dltool/data/
+-rw-rw-r--   0 root         (0) root         (0)      174 2023-04-29 04:26:16.000000 dltool-0.1.1/dltool/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6460 2023-06-09 12:38:12.000000 dltool-0.1.1/dltool/data/file.py
+-rw-rw-r--   0 root         (0) root         (0)     5828 2023-04-29 04:22:08.000000 dltool-0.1.1/dltool/data/time.py
+-rw-rw-r--   0 root         (0) root         (0)      439 2023-04-23 19:43:58.000000 dltool-0.1.1/dltool/data/union.py
+-rw-rw-r--   0 root         (0) root         (0)     1268 2023-04-23 19:45:21.000000 dltool-0.1.1/dltool/data/utils.py
+-rw-rw-r--   0 root         (0) root         (0)      762 2023-06-30 11:33:17.000000 dltool-0.1.1/dltool/hooks.py
+-rw-rw-r--   0 root         (0) root         (0)     9050 2023-06-30 11:46:48.000000 dltool-0.1.1/dltool/log.py
+-rw-rw-r--   0 root         (0) root         (0)     4026 2023-06-30 13:41:53.000000 dltool-0.1.1/dltool/train.py
+-rw-rw-r--   0 root         (0) root         (0)     1625 2023-06-09 12:38:12.000000 dltool-0.1.1/dltool/types.py
+-rw-rw-r--   0 root         (0) root         (0)     4099 2023-04-24 18:33:46.000000 dltool-0.1.1/dltool/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3823 2023-04-23 19:47:14.000000 dltool-0.1.1/dltool/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 14:10:58.240140 dltool-0.1.1/dltool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 14:10:58.000000 dltool-0.1.1/dltool.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      729 2023-06-30 10:27:23.000000 dltool-0.1.1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       49 2023-06-28 05:55:31.000000 dltool-0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 14:10:58.244140 dltool-0.1.1/setup.cfg
```

### Comparing `dltool-0.1/LICENSE` & `dltool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dltool-0.1/PKG-INFO` & `dltool-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltool
-Version: 0.1
+Version: 0.1.1
 Summary: A small library with handy methods for DL with Pytorch
 Author-email: Artem Mikhaylov <simplerick@yandex.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, simplerick
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `dltool-0.1/dltool/algorithm.py` & `dltool-0.1.1/dltool/algorithm.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/data/file.py` & `dltool-0.1.1/dltool/data/file.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/data/time.py` & `dltool-0.1.1/dltool/data/time.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/data/utils.py` & `dltool-0.1.1/dltool/data/utils.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/hooks.py` & `dltool-0.1.1/dltool/hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,14 @@
         metric_values = trainer.logger.history[metric]
         if len(metric_values) > 0 and select_fn(metric_values) == metric_values[-1]:
             trainer.best_model_state = cpu_state_dict(trainer.algorithm)
     return hook
 
 
 def save_state_hook(path: str | Path, best: bool = True):
+    path = Path(path)
+    path.parent.mkdir(parents=True, exist_ok=True)
     def hook(trainer):
         state = trainer.best_model_state if best else cpu_state_dict(trainer.algorithm)
         if state is not None:
             torch.save(state, path)
     return hook
```

### Comparing `dltool-0.1/dltool/log.py` & `dltool-0.1.1/dltool/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,60 @@
 from collections import defaultdict
 import numpy as np
 from collections.abc import Sequence, Mapping, Callable
 import torch
+import logging
+import re
+import yaml
+
+
+class ConsoleLogger(logging.Logger):
+    color_bold = "\033[1m"
+    color_darkcyan = "\033[36m"
+    color_darkblue = "\033[34m"
+    color_end = "\033[0m"
+
+    def __init__(self, name, formatting: str = None):
+        super().__init__(name)
+        formatting = formatting or \
+            f"{ConsoleLogger.color_bold}{ConsoleLogger.color_darkblue}%(name)s{ConsoleLogger.color_end}: %(message)s"
+        formatter = logging.Formatter(
+            formatting,
+            datefmt="%d-%b-%y %H:%M:%S")
+        handler = logging.StreamHandler()
+        handler.setFormatter(formatter)
+        self.addHandler(handler)
+
+def unflatten_dict(d: dict, sep: str = "."):
+    """
+    Unflatten a dictionary with keys like "a.b.c" to a nested dictionary. Supports regex separators.
+    """
+    unflatten_d = {}
+    for k, v in d.items():
+        k_lvls = re.split(sep, k)
+        cur_d = unflatten_d
+        for l in k_lvls[:-1]:
+            if l not in cur_d:
+                cur_d[l] = {}
+            cur_d = cur_d[l]
+        cur_d[k_lvls[-1]] = v
+    return unflatten_d
+
+def format_metrics_dict_to_str(d: dict, step: int = None) -> str:
+    """
+    Formats a dictionary to a beautiful string.
+    """
+    grouped_d = {k if "/" in k else "/"+k: v for k, v in d.items()}
+    grouped_d = {k: f"{v:.4g}" for k, v in grouped_d.items()}
+    grouped_d = unflatten_dict(grouped_d, "[/.]")
+    s = [f"step {step}\n" if step is not None else "\n"]
+    for group, metrics in grouped_d.items():
+        s.append(f"{ConsoleLogger.color_darkcyan}{group}{ConsoleLogger.color_end}")
+        s.append(yaml.dump({' ': metrics} if group else metrics).replace("\'", ""))
+    return "".join(s)
 
 
 def summarize(data: Sequence[dict], function: Callable, names: Sequence[str] = None, pop: bool = False) -> dict:
     """
     Summarizes values for each key in names.
 
     Args:
@@ -71,17 +120,19 @@
             if not hasattr(api, m):
                 raise ValueError(f"Api doesn't have {m} method. Currently only wandb is supported.")
         return super().__new__(cls)
 
     def __init__(self,
                  wandb_api,
                  logging_freq: int = 1,
+                 console_output: bool = True,
                  scalar_aggregation: Callable = np.mean,
                  tensor_aggregation: Callable = torch.cat):
         self.api = wandb_api
+        self.console_logger = ConsoleLogger(__name__) if console_output else None
         self.logging_freq = logging_freq
         self.scalar_aggregation = scalar_aggregation
         self.tensor_aggregation = tensor_aggregation
         self._step = 0  # last step
         self._max_step = 0  # maximum step
         self._last_writing_step = {}  # steps of last writing for each group
         self._data_storage: dict = defaultdict(list)  # {g: [{m: v, }, {m: v, }, ], }
@@ -115,43 +166,50 @@
         else:
             raise ValueError
 
     def clear(self):
         self._data_storage = defaultdict(list)
         self._data_types = defaultdict(dict)
 
+    @staticmethod
+    def path_cat(*parts: str):
+        return "/".join([x for x in parts if x])
+
     def write(self, step: int, groups: Sequence[str] = None, metric_names: Sequence[str] = None):
         scalar_metrics, tensor_metrics = {}, {}
         for g in self._data_storage.copy():
             if groups is not None and g not in groups:
                 continue
             self._last_writing_step[g] = step
             data = self._data_storage.pop(g)
-            g_str = f"{g}/" if g is not None else ""
+            g_str = str(g) if g is not None else ""
             metrics_to_write = metric_names or self._data_types[g].keys()
             # average scalar metrics
             scalar_metric_names = [m for m in metrics_to_write if self._data_types[g][m] in [float, int]]
-            scalar_metrics.update({g_str + n: m for n, m in
+            scalar_metrics.update({Logger.path_cat(g_str, n) : m for n, m in
                 summarize(data, self.scalar_aggregation, names=scalar_metric_names, pop=True).items()})
             # stack tensor metrics
             tensor_metric_names = [m for m in metrics_to_write if self._data_types[g][m] == torch.Tensor]
             if tensor_metric_names:
                 tensor_metrics[g_str] = {n: m for n, m in
                     summarize(data, self.tensor_aggregation, names=tensor_metric_names, pop=True).items()}
         # log scalar metrics
         if scalar_metrics:
             self.api.log(scalar_metrics, step)
+            if self.console_logger:
+                self.console_logger.info(format_metrics_dict_to_str(scalar_metrics, step))
             for n, v in scalar_metrics.items():
                 self.history[n].append(v)
         # save tensor metrics as artifact (dict with torch.tensors as wandb.Artifact)
         if tensor_metrics:
             artifact = self.api.Artifact(f"{self.api.run.id}_{step}", type='tensor')
             for g_str, metrics in tensor_metrics.items():
-                with artifact.new_file(g_str + "metrics.pt", mode='wb') as f:
+                with artifact.new_file(Logger.path_cat(g_str, "metrics.pt"), mode='wb') as f:
                     torch.save(metrics, f)
+                self.history[g_str].append(metrics)
             self.api.log_artifact(artifact)
 
     def plot(self, x_key, y_key, group=None, stroke=None, title=None):
         # needs to be refactored!!!
         y, x = conditional_expectation(self._data_storage[group], condition_on=x_key)[y_key]
         data = list(zip(x, y))
         y_key = f"{group}/{y_key}" if group is not None else y_key
```

### Comparing `dltool-0.1/dltool/train.py` & `dltool-0.1.1/dltool/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import warnings
 import torch
 import numpy as np
 
 from dltool.algorithm import Algorithm
 from dltool.data import DataIterator
 from dltool.log import Logger
-from dltool.utils import to, evaluating, cpu_state_dict
+from dltool.utils import to, evaluating
+
+
+class StopSignal(Exception):
+    pass
 
 
 class Trainer:
     def __init__(self, algorithm: Algorithm,
                  optimizer: torch.optim.Optimizer = None,
                  scheduler: object = None,
                  logger: Logger = None,
@@ -19,15 +23,15 @@
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.logger = logger if logger is not None else Logger(None)
         self.val_check_interval = val_check_interval
         self.device = next(self.algorithm.parameters(), torch.empty(0)).device
         self._step_count = 0
         self.best_model_state = None
-        self.val_hooks = []
+        self.hooks = []
 
     def opt_step(self, loss, optimizer, scheduler):
         loss.backward()
         optimizer.step()
         optimizer.zero_grad()
         if self.scheduler is not None:
             scheduler.step()
@@ -65,18 +69,18 @@
                 continue
             self.loop(len(chunk), train_iterator, self.algorithm.train_step)
             if val_dataloader is not None:
                 with evaluating(self.algorithm):
                     self.loop(len(val_dataloader), val_iterator, self.algorithm.val_step)
             # hooks
             try:
-                for fn in self.val_hooks:
+                for fn in self.hooks:
                     fn(self)
-            except Exception as e:
-                warnings.warn(str(e))
+            except StopSignal as e:  # allows to stop training from hook
+                self.logger.console_logger.info(f"{e.__class__.__name__}: {e}" if e.args else f"{e.__class__.__name__}")
                 break
         # load best model if any is saved
         if self.best_model_state is not None:
             self.algorithm.load_state_dict(self.best_model_state)
 
     def test(self, test_dataloader):
         # data iterator
```

### Comparing `dltool-0.1/dltool/types.py` & `dltool-0.1.1/dltool/types.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/utils.py` & `dltool-0.1.1/dltool/utils.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool/visualize.py` & `dltool-0.1.1/dltool/visualize.py`

 * *Files identical despite different names*

### Comparing `dltool-0.1/dltool.egg-info/PKG-INFO` & `dltool-0.1.1/dltool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltool
-Version: 0.1
+Version: 0.1.1
 Summary: A small library with handy methods for DL with Pytorch
 Author-email: Artem Mikhaylov <simplerick@yandex.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, simplerick
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `dltool-0.1/pyproject.toml` & `dltool-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dltool"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Artem Mikhaylov", email="simplerick@yandex.com" },
 ]
 description = "A small library with handy methods for DL with Pytorch"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

