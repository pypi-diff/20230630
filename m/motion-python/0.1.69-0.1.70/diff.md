# Comparing `tmp/motion_python-0.1.69.tar.gz` & `tmp/motion_python-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.69.tar", max compression
+gzip compressed data, was "motion_python-0.1.70.tar", max compression
```

## Comparing `motion_python-0.1.69.tar` & `motion_python-0.1.70.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3344 2023-06-28 00:45:17.141307 motion_python-0.1.69/README.md
--rw-r--r--   0        0        0      338 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/cli.py
--rw-r--r--   0        0        0    23926 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/component.py
--rw-r--r--   0        0        0    17609 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/execute.py
--rw-r--r--   0        0        0    13071 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/instance.py
--rw-r--r--   0        0        0     4889 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/route.py
--rw-r--r--   0        0        0     5944 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/server/fit_task.py
--rw-r--r--   0        0        0     9481 2023-06-28 00:45:17.141307 motion_python-0.1.69/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-28 00:45:38.445933 motion_python-0.1.69/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.69/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-30 02:57:24.512919 motion_python-0.1.70/README.md
+-rw-r--r--   0        0        0      338 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/cli.py
+-rw-r--r--   0        0        0    24213 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/component.py
+-rw-r--r--   0        0        0    17749 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/execute.py
+-rw-r--r--   0        0        0    13924 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/instance.py
+-rw-r--r--   0        0        0     4889 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/route.py
+-rw-r--r--   0        0        0     5944 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/server/fit_task.py
+-rw-r--r--   0        0        0     9481 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-30 02:57:49.945693 motion_python-0.1.70/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.70/PKG-INFO
```

### Comparing `motion_python-0.1.69/README.md` & `motion_python-0.1.70/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/cli.py` & `motion_python-0.1.70/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/component.py` & `motion_python-0.1.70/motion/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,14 +479,15 @@
         return decorator
 
     def __call__(
         self,
         name: str = "",
         init_state_params: Dict[str, Any] = {},
         logging_level: str = "WARNING",
+        disabled: bool = False,
     ) -> ComponentInstance:
         """Creates and returns a new instance of a Motion component.
         See `ComponentInstance` docs for more info.
 
         Usage:
         ```python
         from motion import Component
@@ -513,14 +514,18 @@
             name (str, optional):
                 Name of the component instance. Defaults to "".
             init_state_params (Dict[str, Any], optional):
                 Parameters to pass into the init_state function. Defaults to {}.
             logging_level (str, optional):
                 Logging level for the Motion logger. Uses the logging library.
                 Defaults to "WARNING".
+            disabled (bool, optional):
+                Whether or not to disable the component instance. Useful for
+                printing out state values without running dataflows.
+                Defaults to False.
         Returns:
             ComponentInstance: Component instance to run dataflows with.
         """
         if not name:
             name = random_passphrase()
 
         if "__" in name:
@@ -538,14 +543,15 @@
                 init_state_func=self._init_state_func,
                 init_state_params=init_state_params,
                 save_state_func=self._save_state_func,
                 load_state_func=self._load_state_func,
                 infer_routes=self._infer_routes,
                 fit_routes=self._fit_routes,
                 logging_level=logging_level,
+                disabled=disabled,
             )
         except RuntimeError:
             raise RuntimeError(
                 "Error creating component instance. Make sure the entry point "
                 + "of your program is protected, using `if __name__ == '__main__':`"
             )
```

### Comparing `motion_python-0.1.69/motion/execute.py` & `motion_python-0.1.70/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         instance_name: str,
         init_state_func: Optional[Callable],
         init_state_params: Dict[str, Any],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
         infer_routes: Dict[str, Route],
         fit_routes: Dict[str, List[Route]],
+        disabled: bool = False,
     ):
         self._instance_name = instance_name
 
         self._init_state_func = init_state_func
         self._init_state_params = init_state_params
         self._load_state_func = load_state_func
         self._save_state_func = save_state_func
@@ -87,15 +88,17 @@
             for rkey, routes in fit_routes.items()
         }
 
         # Set up shutdown event
         # self._shutdown_event = threading.Event()
 
         # Set up fit queues, batch sizes, and threads
-        self._build_fit_jobs()
+        self.disabled = disabled
+        if not disabled:
+            self._build_fit_jobs()
 
     def _connectToRedis(self) -> redis.Redis:
         rp = RedisParams()
         r = redis.Redis(
             host=rp.host,
             port=rp.port,
             password=rp.password,
@@ -194,14 +197,17 @@
         return f"MOTION_QUEUE:{self._instance_name}/{route_key}/{udf_name}"
 
     def _get_channel_identifier(self, route_key: str, udf_name: str) -> str:
         """Gets the channel identifier for a given route key and UDF name."""
         return f"MOTION_CHANNEL:{self._instance_name}/{route_key}/{udf_name}"
 
     def shutdown(self, is_open: bool) -> None:
+        if self.disabled:
+            return
+
         if not self.running.value:
             return
 
         if is_open:
             logger.info("Running fit operations on remaining data...")
 
         # Set shutdown event
```

### Comparing `motion_python-0.1.69/motion/instance.py` & `motion_python-0.1.70/motion/instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         init_state_func: Optional[Callable],
         init_state_params: Optional[Dict[str, Any]],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
         infer_routes: Dict[str, Route],
         fit_routes: Dict[str, List[Route]],
         logging_level: str = "WARNING",
+        disabled: bool = False,
     ):
         """Creates a new instance of a Motion component.
 
         Args:
             name (str):
                 Name of the component we are creating an instance of.
             instance_name (str):
@@ -49,22 +50,24 @@
         logger.info(f"Creating local instance of {self._component_name}...")
         atexit.register(self.shutdown)
 
         # Create instance name
         self._instance_name = instance_name
 
         self.running = False
+        self.disabled = disabled
         self._executor = Executor(
             self._instance_name,
             init_state_func=init_state_func,
             init_state_params=init_state_params if init_state_params else {},
             save_state_func=save_state_func,
             load_state_func=load_state_func,
             infer_routes=infer_routes,
             fit_routes=fit_routes,
+            disabled=self.disabled,
         )
         self.running = True
 
     @property
     def instance_name(self) -> str:
         """Component name with a random phrase or user-defined ID to represent
         the name of this instance."""
@@ -94,14 +97,17 @@
 
         c_instance = C()
         c_instance.run(...)
         c_instance.run(...)
         c_instance.shutdown()
         ```
         """
+        if self.disabled:
+            return
+
         if not self.running:
             return
 
         is_open = is_logger_open(logger)
 
         if is_open:
             logger.info(f"Shutting down {self._instance_name}...")
@@ -235,15 +241,22 @@
         c.run(add=2) # This will use the updated state
 
         # 1. Runs the fit op even though only one element is in the batch
         ```
 
         Args:
             dataflow_key (str): Key of the dataflow.
+
+        Raises:
+            RuntimeError: If the component instance was initialized to
+            be disabled.
         """
+        if self.disabled:
+            raise RuntimeError("Cannot run a disabled component instance.")
+
         self._executor.flush_fit(dataflow_key)
 
     def run(
         self,
         *,
         cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
@@ -312,20 +325,25 @@
                 state after the fit op completes. Defaults to False.
             **kwargs:
                 Keyword arguments for the infer and fit ops. You can only
                 pass in one pair.
 
         Raises:
             ValueError: If more than one dataflow key-value pair is passed.
+            RuntimeError: If the component instance was initialized to
+            be disabled.
 
         Returns:
             Any: Result of the inference call. Might take a long time
             to run if `flush_fit = True` and the fit operation is
             computationally expensive.
         """
+        if self.disabled:
+            raise RuntimeError("Cannot run a disabled component instance.")
+
         if len(kwargs) != 1:
             raise ValueError("Only one key-value pair is allowed in kwargs.")
 
         key, value = next(iter(kwargs.items()))
 
         infer_result = self._executor.run(
             key=key,
@@ -386,17 +404,24 @@
                 returning. If the fit queue hasn't reached batch_size
                 yet, the fit op runs anyways. Force refreshes the
                 state after the fit op completes. Defaults to False.
             **kwargs:
                 Keyword arguments for the infer and fit ops. You can only
                 pass in one pair.
 
+        Raises:
+            ValueError: If more than one dataflow key-value pair is passed.
+            RuntimeError: If the component instance was initialized to
+            be disabled.
+
         Returns:
             Awaitable[Any]: Awaitable Result of the inference call.
         """
+        if self.disabled:
+            raise RuntimeError("Cannot run a disabled component instance.")
 
         if len(kwargs) != 1:
             raise ValueError("Only one key-value pair is allowed in kwargs.")
 
         key, value = next(iter(kwargs.items()))
 
         infer_result = await self._executor.arun(
```

### Comparing `motion_python-0.1.69/motion/migrate.py` & `motion_python-0.1.70/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.70/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/route.py` & `motion_python-0.1.70/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/server/fit_task.py` & `motion_python-0.1.70/motion/server/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/motion/utils.py` & `motion_python-0.1.70/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.69/pyproject.toml` & `motion_python-0.1.70/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.69"
+version = "0.1.70"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.69/PKG-INFO` & `motion_python-0.1.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.69
+Version: 0.1.70
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

