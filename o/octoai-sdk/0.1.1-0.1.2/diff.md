# Comparing `tmp/octoai_sdk-0.1.1.tar.gz` & `tmp/octoai_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai_sdk-0.1.1.tar", max compression
+gzip compressed data, was "octoai_sdk-0.1.2.tar", max compression
```

## Comparing `octoai_sdk-0.1.1.tar` & `octoai_sdk-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.1.1/octoai/__init__.py
--rw-r--r--   0        0        0     7264 2023-06-22 15:51:11.411771 octoai_sdk-0.1.1/octoai/client.py
--rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.1.1/octoai/errors.py
--rw-r--r--   0        0        0       56 2023-06-09 21:08:23.294496 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/requirements.txt
--rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/service.py
--rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/test_request.py
--rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/requirements.txt
--rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/service.py
--rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/test_request.py
--rw-r--r--   0        0        0       34 2023-06-13 16:21:58.470830 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/requirements.txt
--rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/service.py
--rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/test_request.py
--rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/requirements.txt
--rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/service.py
--rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/test_request.py
--rw-r--r--   0        0        0     6199 2023-06-12 17:09:46.796808 octoai_sdk-0.1.1/octoai/server.py
--rw-r--r--   0        0        0     2698 2023-06-12 17:09:46.799814 octoai_sdk-0.1.1/octoai/service.py
--rw-r--r--   0        0        0    13192 2023-06-21 00:01:12.467552 octoai_sdk-0.1.1/octoai/types.py
--rw-r--r--   0        0        0     4000 2023-06-22 15:51:11.413837 octoai_sdk-0.1.1/octoai/utils.py
--rw-r--r--   0        0        0     1050 2023-06-22 18:25:34.256859 octoai_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.1.2/octoai/__init__.py
+-rw-r--r--   0        0        0     9967 2023-06-30 15:47:18.275698 octoai_sdk-0.1.2/octoai/client.py
+-rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.1.2/octoai/errors.py
+-rw-r--r--   0        0        0       56 2023-06-09 21:08:23.294496 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/requirements.txt
+-rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/service.py
+-rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/test_request.py
+-rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/requirements.txt
+-rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/service.py
+-rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/test_request.py
+-rw-r--r--   0        0        0       34 2023-06-13 16:21:58.470830 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/requirements.txt
+-rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/service.py
+-rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/test_request.py
+-rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/requirements.txt
+-rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/service.py
+-rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/test_request.py
+-rw-r--r--   0        0        0     6788 2023-06-28 18:01:35.201394 octoai_sdk-0.1.2/octoai/server.py
+-rw-r--r--   0        0        0     2698 2023-06-12 17:09:46.799814 octoai_sdk-0.1.2/octoai/service.py
+-rw-r--r--   0        0        0    13192 2023-06-29 17:19:44.000199 octoai_sdk-0.1.2/octoai/types.py
+-rw-r--r--   0        0        0     4000 2023-06-29 01:18:48.788389 octoai_sdk-0.1.2/octoai/utils.py
+-rw-r--r--   0        0        0     1050 2023-06-30 15:49:19.565770 octoai_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.1.2/PKG-INFO
```

### Comparing `octoai_sdk-0.1.1/octoai/errors.py` & `octoai_sdk-0.1.2/octoai/errors.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/service.py` & `octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/test_request.py` & `octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/hello-world/test_request.py` & `octoai_sdk-0.1.2/octoai/scaffolds/hello-world/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/service.py` & `octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/test_request.py` & `octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/yolov8/service.py` & `octoai_sdk-0.1.2/octoai/scaffolds/yolov8/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/scaffolds/yolov8/test_request.py` & `octoai_sdk-0.1.2/octoai/scaffolds/yolov8/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/server.py` & `octoai_sdk-0.1.2/octoai/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 command-line interface, which directs them to implement the
 ``octoai.service.Service`` class and use the ``octoai`` CLI to help
 build and deploy their endpoint.
 """
 import importlib
 import inspect
 import json
+import os
 import time
 from enum import Enum
 from typing import Any, Dict, Optional
 
 import click
 import uvicorn
 from fastapi import FastAPI
@@ -50,14 +51,18 @@
     """
 
     def __init__(self, service: Service):
         self.app = FastAPI()
         self.service = service
         self.status = HealthStatus.STARTING
 
+        self.response_headers = {
+            "OCTOAI_REPLICA_NAME": os.environ.get("OCTOAI_REPLICA_NAME", ""),
+        }
+
         Input = inspect_input_types(service)
         Output = inspect_output_types(service)
 
         @self.app.get("/healthcheck")
         def health() -> JSONResponse:
             return JSONResponse(
                 status_code=self.status.value, content={"status": self.status.name}
@@ -84,20 +89,24 @@
             start_process = time.process_time_ns()
             # track time elapsed in nanoseconds including any sleep time
             start_perf = time.perf_counter_ns()
             prediction = service.infer(**infer_args)
             inference_time_ms = (time.process_time_ns() - start_process) / 1e6
             performance_time_ms = (time.perf_counter_ns() - start_perf) / 1e6
 
-            return Output(
-                output=prediction,
-                analytics=ResponseAnalytics(
-                    inference_time_ms=inference_time_ms,
-                    performance_time_ms=performance_time_ms,
-                ),
+            return JSONResponse(
+                status_code=200,
+                headers=self.response_headers,
+                content=Output(
+                    output=prediction,
+                    analytics=ResponseAnalytics(
+                        inference_time_ms=inference_time_ms,
+                        performance_time_ms=performance_time_ms,
+                    ),
+                ).dict(),
             )
 
     def get_api_schema(self) -> Dict[str, Any]:
         """Return the Open API schema for the underlying service."""
         return self.app.openapi()
 
     def init(self):
@@ -105,17 +114,22 @@
         try:
             self.service.setup()
             self.status = HealthStatus.READY
         except Exception as e:
             self.status = HealthStatus.UNKNOWN
             raise e
 
-    def run(self, port: int):
+    def run(self, port: int, timeout_keep_alive: int):
         """Run the server exposing the underlying service."""
-        uvicorn.run(self.app, host="0.0.0.0", port=port)
+        uvicorn.run(
+            self.app,
+            host="0.0.0.0",
+            port=port,
+            timeout_keep_alive=timeout_keep_alive,
+        )
 
 
 def load_service(module_name: str, class_name: Optional[str]) -> Service:
     """Load the service implementation."""
     try:
         module = importlib.import_module(module_name)
 
@@ -186,17 +200,23 @@
     server = ctx.obj["server"]
     server.init()
 
 
 @server.command()
 @click.pass_context
 @click.option("--port", type=int, default=8080)
-def run(ctx, port):
+@click.option(
+    "--timeout-keep-alive",
+    type=int,
+    default=900,
+    help="Connection keep alive timeout in seconds",
+)
+def run(ctx, port, timeout_keep_alive):
     """Run the server for the given service."""
     click.echo("run")
     server = ctx.obj["server"]
     server.init()
-    server.run(port)
+    server.run(port, timeout_keep_alive)
 
 
 if __name__ == "__main__":
     server(obj={})
```

### Comparing `octoai_sdk-0.1.1/octoai/service.py` & `octoai_sdk-0.1.2/octoai/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/types.py` & `octoai_sdk-0.1.2/octoai/types.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/octoai/utils.py` & `octoai_sdk-0.1.2/octoai/utils.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.1/pyproject.toml` & `octoai_sdk-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai-sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = "A runtime library for OctoAI."
 authors = ["OctoML"]
 packages = [
     { include = "octoai" }
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `octoai_sdk-0.1.1/PKG-INFO` & `octoai_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A runtime library for OctoAI.
 Author: OctoML
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

