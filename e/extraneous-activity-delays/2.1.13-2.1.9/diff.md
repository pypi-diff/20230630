# Comparing `tmp/extraneous_activity_delays-2.1.13.tar.gz` & `tmp/extraneous_activity_delays-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extraneous_activity_delays-2.1.13.tar", max compression
+gzip compressed data, was "extraneous_activity_delays-2.1.9.tar", max compression
```

## Comparing `extraneous_activity_delays-2.1.13.tar` & `extraneous_activity_delays-2.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11349 2023-06-30 08:06:11.410017 extraneous_activity_delays-2.1.13/LICENSE
--rw-r--r--   0        0        0     9404 2023-06-30 08:06:11.410017 extraneous_activity_delays-2.1.13/README.md
--rw-r--r--   0        0        0      556 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/__init__.py
--rw-r--r--   0        0        0     6740 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/config.py
--rw-r--r--   0        0        0    13561 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/delay_discoverer.py
--rw-r--r--   0        0        0    16092 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/enhance_with_delays.py
--rw-r--r--   0        0        0       53 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/prosimos/__init__.py
--rw-r--r--   0        0        0     2358 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
--rw-r--r--   0        0        0     2118 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/prosimos/simulator.py
--rw-r--r--   0        0        0       53 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/qbp/__init__.py
--rw-r--r--   0        0        0     4372 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
--rw-r--r--   0        0        0     1593 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/qbp/simulator.py
--rw-r--r--   0        0        0       60 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/utils/__init__.py
--rw-r--r--   0        0        0     3194 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/utils/bpmn_enhancement.py
--rw-r--r--   0        0        0      810 2023-06-30 08:06:11.474018 extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/utils/file_manager.py
--rw-r--r--   0        0        0    10114 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.13/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:11:52.365418 extraneous_activity_delays-2.1.9/LICENSE
+-rw-r--r--   0        0        0     9404 2023-05-24 10:39:33.962708 extraneous_activity_delays-2.1.9/README.md
+-rw-r--r--   0        0        0      553 2023-05-24 10:27:55.491113 extraneous_activity_delays-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-24 10:09:51.247101 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/__init__.py
+-rw-r--r--   0        0        0     6580 2023-05-24 10:36:04.338823 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py
+-rw-r--r--   0        0        0    13561 2023-05-24 10:11:56.745400 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py
+-rw-r--r--   0        0        0    16020 2023-05-24 10:11:56.759114 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.253732 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-24 10:11:56.721128 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     2118 2023-05-24 10:11:56.715176 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py
+-rw-r--r--   0        0        0       53 2023-05-24 10:09:51.260582 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-24 10:11:56.729581 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py
+-rw-r--r--   0        0        0     1593 2023-05-24 10:11:56.717662 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py
+-rw-r--r--   0        0        0       60 2023-05-24 10:09:51.266529 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-24 10:11:56.736893 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py
+-rw-r--r--   0        0        0      810 2023-05-24 10:11:56.726632 extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py
+-rw-r--r--   0        0        0    10110 1970-01-01 00:00:00.000000 extraneous_activity_delays-2.1.9/PKG-INFO
```

### Comparing `extraneous_activity_delays-2.1.13/LICENSE` & `extraneous_activity_delays-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/README.md` & `extraneous_activity_delays-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/pyproject.toml` & `extraneous_activity_delays-2.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "extraneous-activity-delays"
-version = "2.1.13"
+version = "2.1.9"
 description = ""
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
-prosimos = "^1.2.6"
+prosimos = "^1.2.4"
 hyperopt = "^0.2.7"
 lxml = "^4.9.2"
 log-distance-measures = "^1.0.2"
-start-time-estimator = "^1.10.10"
-pix-framework = "^0.10.0"
+start-time-estimator = "^1.10.9"
+pix-framework = "^0.8.3"
 
 [tool.ruff]
 line-length = 120
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/config.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         concurrency_thresholds      Thresholds for the concurrency oracle (heuristics or overlapping).
         working_schedules           Dictionary with the resources as key and the working calendars (RCalendar) as value.
 
     General parameters:
         process_name                Name of the process to use in the output files (BPMN and simulated log files).
         log_ids                     Identifiers for each key element (e.g. executed activity or resource).
         debug                       Boolean denoting whether to print debug information or not.
-        clean_intermediate_files    Boolean denoting whether to remove the folders of the non-best solutions or not.
     """
 
     # Extraneous delays options
     discovery_method: DiscoveryMethod = DiscoveryMethod.NAIVE
     timer_placement: TimerPlacement = TimerPlacement.BEFORE
     simulation_engine: SimulationEngine = SimulationEngine.PROSIMOS
     optimization_metric: OptimizationMetric = OptimizationMetric.RELATIVE_EMD
@@ -123,15 +122,14 @@
         default_factory=lambda: ConcurrencyThresholds(df=0.5)
     )
     working_schedules: dict = field(default_factory=dict)
     # General parameters
     process_name: str = "process"
     log_ids: EventLogIDs = field(default_factory=lambda: DEFAULT_CSV_IDS)
     debug: bool = False
-    clean_intermediate_files: bool = False
     # Paths
     PATH_PROJECT = get_project_dir()
     PATH_INPUTS = PATH_PROJECT.joinpath("inputs")
     PATH_OUTPUTS = PATH_PROJECT.joinpath("outputs")
     PATH_EXTERNAL_TOOLS = PATH_PROJECT.joinpath("external_tools")
     PATH_QBP = (
         PATH_PROJECT.joinpath("external_tools")
```

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/delay_discoverer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/delay_discoverer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/enhance_with_delays.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/enhance_with_delays.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,18 +164,17 @@
                 space=self.opt_space,
                 algo=tpe.suggest,
                 max_evals=self.configuration.num_iterations,
                 trials=self.opt_trials,
                 show_progressbar=False,
             )
             # Remove all folders except best trial one
-            if self.configuration.clean_intermediate_files:
-                for result in self.opt_trials.results:
-                    if result["output_folder"] != self.opt_trials.best_trial["result"]["output_folder"]:
-                        delete_folder(result["output_folder"])
+            for result in self.opt_trials.results:
+                if result["output_folder"] != self.opt_trials.best_trial["result"]["output_folder"]:
+                    delete_folder(result["output_folder"])
             # Process the best parameters result
             best_alphas = {activity: round(best_result[activity], 2) for activity in best_result}
             # Transform timers based on [best_alphas]
             scaled_timers = self._get_scaled_timers(best_alphas)
             self.best_timers = scaled_timers
             # Enhance process model
             if self.configuration.simulation_engine == SimulationEngine.PROSIMOS:
```

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/prosimos/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/prosimos/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulation_model_enhancer.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/qbp/simulator.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/qbp/simulator.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/utils/bpmn_enhancement.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/bpmn_enhancement.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/src/extraneous_activity_delays/utils/file_manager.py` & `extraneous_activity_delays-2.1.9/src/extraneous_activity_delays/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `extraneous_activity_delays-2.1.13/PKG-INFO` & `extraneous_activity_delays-2.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: extraneous-activity-delays
-Version: 2.1.13
+Version: 2.1.9
 Summary: 
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: log-distance-measures (>=1.0.2,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pix-framework (>=0.10.0,<0.11.0)
-Requires-Dist: prosimos (>=1.2.6,<2.0.0)
-Requires-Dist: start-time-estimator (>=1.10.10,<2.0.0)
+Requires-Dist: pix-framework (>=0.8.3,<0.9.0)
+Requires-Dist: prosimos (>=1.2.4,<2.0.0)
+Requires-Dist: start-time-estimator (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Extraneous activity delays BPS model enhancer
 
 ![build](https://github.com/AutomatedProcessImprovement/extraneous-activity-delays/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/extraneous-activity-delays)
```

