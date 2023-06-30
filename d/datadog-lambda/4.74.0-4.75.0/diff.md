# Comparing `tmp/datadog_lambda-4.74.0.tar.gz` & `tmp/datadog_lambda-4.75.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.74.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.75.0.tar", max compression
```

## Comparing `datadog_lambda-4.74.0.tar` & `datadog_lambda-4.75.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11379 2023-06-22 16:35:13.671910 datadog_lambda-4.74.0/LICENSE
--rw-r--r--   0        0        0      394 2023-06-22 16:35:13.671995 datadog_lambda-4.74.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3422 2023-06-22 16:35:13.672177 datadog_lambda-4.74.0/README.md
--rw-r--r--   0        0        0      538 2023-06-22 16:35:13.672315 datadog_lambda-4.74.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2023-06-22 16:35:13.672408 datadog_lambda-4.74.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7232 2023-06-22 16:35:13.672514 datadog_lambda-4.74.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-06-22 16:35:13.672595 datadog_lambda-4.74.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2023-06-22 16:35:13.672683 datadog_lambda-4.74.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2023-06-22 16:35:13.672773 datadog_lambda-4.74.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2023-06-22 16:35:13.672859 datadog_lambda-4.74.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2023-06-22 16:35:13.672978 datadog_lambda-4.74.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2023-06-22 16:35:13.673071 datadog_lambda-4.74.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2023-06-22 16:35:13.673170 datadog_lambda-4.74.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2023-06-22 16:35:13.673254 datadog_lambda-4.74.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2023-06-22 16:35:13.673338 datadog_lambda-4.74.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2023-06-22 16:35:13.673428 datadog_lambda-4.74.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2023-06-22 16:35:13.673544 datadog_lambda-4.74.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2023-06-22 16:35:13.673636 datadog_lambda-4.74.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    47208 2023-06-22 16:35:13.673836 datadog_lambda-4.74.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-06-22 16:35:13.673975 datadog_lambda-4.74.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    14242 2023-06-22 16:35:13.674085 datadog_lambda-4.74.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-06-22 16:35:13.674183 datadog_lambda-4.74.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1271 2023-06-22 16:41:53.033918 datadog_lambda-4.74.0/pyproject.toml
--rw-r--r--   0        0        0     5002 1970-01-01 00:00:00.000000 datadog_lambda-4.74.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-09-22 18:30:00.504292 datadog_lambda-4.75.0/LICENSE
+-rw-r--r--   0        0        0      394 2022-09-22 18:30:00.504380 datadog_lambda-4.75.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3422 2023-04-18 14:29:41.172896 datadog_lambda-4.75.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-13 20:46:09.160997 datadog_lambda-4.75.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2022-09-22 18:30:00.504778 datadog_lambda-4.75.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     8013 2023-06-30 13:40:04.094622 datadog_lambda-4.75.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-01-25 19:31:51.675529 datadog_lambda-4.75.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2022-09-22 18:30:00.505031 datadog_lambda-4.75.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2022-09-22 18:30:00.505121 datadog_lambda-4.75.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-09-22 18:30:00.505207 datadog_lambda-4.75.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2022-09-22 18:30:00.505343 datadog_lambda-4.75.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2022-09-22 18:30:00.505417 datadog_lambda-4.75.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2022-09-22 18:30:00.505516 datadog_lambda-4.75.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2022-09-22 18:30:00.505686 datadog_lambda-4.75.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2022-09-22 18:30:00.505792 datadog_lambda-4.75.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2022-09-22 18:30:00.505884 datadog_lambda-4.75.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2022-09-22 18:30:00.505984 datadog_lambda-4.75.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2022-09-22 18:30:00.506089 datadog_lambda-4.75.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    47331 2023-06-30 13:40:04.095181 datadog_lambda-4.75.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 17:19:32.172228 datadog_lambda-4.75.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    14393 2023-06-30 13:40:04.095559 datadog_lambda-4.75.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-03-22 12:07:02.672991 datadog_lambda-4.75.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1271 2023-06-30 13:41:37.444527 datadog_lambda-4.75.0/pyproject.toml
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 datadog_lambda-4.75.0/PKG-INFO
```

### Comparing `datadog_lambda-4.74.0/LICENSE` & `datadog_lambda-4.75.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/README.md` & `datadog_lambda-4.75.0/README.md`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/__init__.py` & `datadog_lambda-4.75.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/api.py` & `datadog_lambda-4.75.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.75.0/datadog_lambda/cold_start.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,63 @@
 import os
 from typing import List, Hashable
 import logging
 
 logger = logging.getLogger(__name__)
 
 _cold_start = True
+_proactive_initialization = False
 _lambda_container_initialized = False
 
 
-def set_cold_start():
+def set_cold_start(init_timestamp_ns):
     """Set the value of the cold start global
 
     This should be executed once per Lambda execution before the execution
     """
     global _cold_start
     global _lambda_container_initialized
-    _cold_start = not _lambda_container_initialized
+    global _proactive_initialization
+    if not _lambda_container_initialized:
+        now = time.time_ns()
+        if (now - init_timestamp_ns) // 1_000_000_000 > 10:
+            _cold_start = False
+            _proactive_initialization = True
+        else:
+            _cold_start = not _lambda_container_initialized
+    else:
+        _cold_start = False
+        _proactive_initialization = False
     _lambda_container_initialized = True
 
 
 def is_cold_start():
     """Returns the value of the global cold_start"""
     return _cold_start
 
 
+def is_proactive_init():
+    """Returns the value of the global proactive_initialization"""
+    return _proactive_initialization
+
+
+def is_new_sandbox():
+    return is_cold_start() or is_proactive_init()
+
+
 def get_cold_start_tag():
     """Returns the cold start tag to be used in metrics"""
     return "cold_start:{}".format(str(is_cold_start()).lower())
 
 
+def get_proactive_init_tag():
+    """Returns the proactive init tag to be used in metrics"""
+    return "proactive_initialization:{}".format(str(is_proactive_init()).lower())
+
+
 class ImportNode(object):
     def __init__(self, module_name, full_file_path, start_time_ns, end_time_ns=None):
         self.module_name = module_name
         self.full_file_path = full_file_path
         self.start_time_ns = start_time_ns
         self.end_time_ns = end_time_ns
         self.children = []
@@ -111,15 +136,15 @@
         return spec
 
     return wrapped_find_spec
 
 
 def initialize_cold_start_tracing():
     if (
-        is_cold_start()
+        is_new_sandbox()
         and os.environ.get("DD_TRACE_ENABLED", "true").lower() == "true"
         and os.environ.get("DD_COLD_START_TRACING", "true").lower() == "true"
     ):
         from sys import version_info, meta_path
 
         if version_info >= (3, 7):  # current implementation only support version > 3.7
             for importer in meta_path:
```

### Comparing `datadog_lambda-4.74.0/datadog_lambda/constants.py` & `datadog_lambda-4.75.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.75.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/extension.py` & `datadog_lambda-4.75.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/handler.py` & `datadog_lambda-4.75.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/metric.py` & `datadog_lambda-4.75.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/patch.py` & `datadog_lambda-4.75.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.75.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/tags.py` & `datadog_lambda-4.75.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.75.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/tracing.py` & `datadog_lambda-4.75.0/datadog_lambda/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1207,14 +1207,15 @@
     return span
 
 
 def create_function_execution_span(
     context,
     function_name,
     is_cold_start,
+    is_proactive_init,
     trace_context_source,
     merge_xray_traces,
     trigger_tags,
     parent_span=None,
 ):
     tags = {}
     if context:
@@ -1231,14 +1232,16 @@
             "functionname": context.function_name.lower()
             if context.function_name
             else None,
             "datadog_lambda": datadog_lambda_version,
             "dd_trace": ddtrace_version,
             "span.name": "aws.lambda",
         }
+    if is_proactive_init:
+        tags["proactive_initialization"] = str(is_proactive_init).lower()
     if trace_context_source == TraceContextSource.XRAY and merge_xray_traces:
         tags["_dd.parent_source"] = trace_context_source
     tags.update(trigger_tags)
     args = {
         "service": "aws.lambda",
         "resource": function_name,
         "span_type": "serverless",
```

### Comparing `datadog_lambda-4.74.0/datadog_lambda/trigger.py` & `datadog_lambda-4.75.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.75.0/datadog_lambda/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 import logging
 import traceback
 from importlib import import_module
 import json
 from time import time_ns
 
 from datadog_lambda.extension import should_use_extension, flush_extension
-from datadog_lambda.cold_start import set_cold_start, is_cold_start, ColdStartTracer
+from datadog_lambda.cold_start import (
+    set_cold_start,
+    is_cold_start,
+    is_proactive_init,
+    is_new_sandbox,
+    ColdStartTracer,
+)
 from datadog_lambda.constants import (
     TraceContextSource,
     XraySubsegment,
     Headers,
     TraceHeader,
 )
 from datadog_lambda.metric import (
@@ -68,14 +74,16 @@
 DD_COLD_START_TRACE_SKIP_LIB = "DD_COLD_START_TRACE_SKIP_LIB"
 DD_REQUESTS_SERVICE_NAME = "DD_REQUESTS_SERVICE_NAME"
 DD_SERVICE = "DD_SERVICE"
 DD_ENV = "DD_ENV"
 
 env_env_var = os.environ.get(DD_ENV, None)
 
+init_timestamp_ns = time_ns()
+
 """
 Usage:
 
 import requests
 from datadog_lambda.wrapper import datadog_lambda_wrapper
 from datadog_lambda.metric import lambda_metric
 
@@ -241,15 +249,15 @@
         datadog_data = base64.b64encode(json.dumps(injected_headers).encode()).decode()
         self.response.setdefault("context", {})
         self.response["context"]["_datadog"] = datadog_data
 
     def _before(self, event, context):
         try:
             self.response = None
-            set_cold_start()
+            set_cold_start(init_timestamp_ns)
             submit_invocations_metric(context)
             self.trigger_tags = extract_trigger_tags(event, context)
             # Extract Datadog trace context and source from incoming requests
             dd_context, trace_context_source, event_source = extract_dd_trace_context(
                 event,
                 context,
                 extractor=self.trace_extractor,
@@ -268,22 +276,23 @@
                     self.inferred_span = create_inferred_span(
                         event, context, event_source, self.decode_authorizer_context
                     )
                 self.span = create_function_execution_span(
                     context,
                     self.function_name,
                     is_cold_start(),
+                    is_proactive_init(),
                     trace_context_source,
                     self.merge_xray_traces,
                     self.trigger_tags,
                     parent_span=self.inferred_span,
                 )
             else:
                 set_correlation_ids()
-            if profiling_env_var and is_cold_start():
+            if profiling_env_var and is_new_sandbox():
                 self.prof.start(stop_on_exit=False, profile_children=True)
             logger.debug("datadog_lambda_wrapper _before() done")
         except Exception:
             traceback.print_exc()
 
     def _after(self, event, context):
         try:
@@ -295,15 +304,15 @@
             # Create a new dummy Datadog subsegment for function trigger tags so we
             # can attach them to X-Ray spans when hybrid tracing is used
             if self.trigger_tags:
                 create_dd_dummy_metadata_subsegment(
                     self.trigger_tags, XraySubsegment.LAMBDA_FUNCTION_TAGS_KEY
                 )
             should_trace_cold_start = (
-                dd_tracing_enabled and self.cold_start_tracing and is_cold_start()
+                dd_tracing_enabled and self.cold_start_tracing and is_new_sandbox()
             )
             if should_trace_cold_start:
                 trace_ctx = tracer.current_trace_context()
 
             if self.span:
                 if dd_capture_lambda_payload_enabled:
                     tag_object(self.span, "function.request", event)
```

### Comparing `datadog_lambda-4.74.0/datadog_lambda/xray.py` & `datadog_lambda-4.75.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.74.0/pyproject.toml` & `datadog_lambda-4.75.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.74.0"
+version = "4.75.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
```

### Comparing `datadog_lambda-4.74.0/PKG-INFO` & `datadog_lambda-4.75.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.74.0
+Version: 4.75.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Requires-Dist: boto3 (>=1.10.33,<2.0.0) ; extra == "dev"
 Requires-Dist: datadog (>=0.41.0,<1.0.0)
 Requires-Dist: ddtrace (>=1.15.0,<2.0.0)
 Requires-Dist: flake8 (>=3.7.9,<4.0.0) ; extra == "dev"
 Requires-Dist: httpretty (>=0.9.7,<0.10.0) ; extra == "dev"
 Requires-Dist: importlib_metadata (>=1.0,<2.0) ; python_version < "3.8"
```

