# Comparing `tmp/thoughtful-2.1.4.tar.gz` & `tmp/thoughtful-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.1.4.tar", max compression
+gzip compressed data, was "thoughtful-2.1.5.tar", max compression
```

## Comparing `thoughtful-2.1.4.tar` & `thoughtful-2.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-06-28 21:40:32.534625 thoughtful-2.1.4/LICENSE
--rw-r--r--   0        0        0     2992 2023-06-28 21:40:32.534625 thoughtful-2.1.4/README.md
--rw-r--r--   0        0        0     1935 2023-06-28 21:40:32.534625 thoughtful-2.1.4/pyproject.toml
--rw-r--r--   0        0        0      222 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/__init__.py
--rw-r--r--   0        0        0       54 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     6616 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0      922 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/event_bus.py
--rw-r--r--   0        0        0     8756 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10300 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7844 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     6441 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1347 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     3124 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     4372 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/streamer.py
--rw-r--r--   0        0        0     1352 2023-06-28 21:40:32.538626 thoughtful-2.1.4/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-29 20:57:31.848930 thoughtful-2.1.5/LICENSE
+-rw-r--r--   0        0        0     2992 2023-06-29 20:57:31.848930 thoughtful-2.1.5/README.md
+-rw-r--r--   0        0        0     1935 2023-06-29 20:57:31.848930 thoughtful-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     6616 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0      922 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/event_bus.py
+-rw-r--r--   0        0        0     8756 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2871 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    12297 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7831 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     6429 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     3124 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4372 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/streamer.py
+-rw-r--r--   0        0        0     1352 2023-06-29 20:57:31.852930 thoughtful-2.1.5/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.1.5/PKG-INFO
```

### Comparing `thoughtful-2.1.4/LICENSE` & `thoughtful-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/README.md` & `thoughtful-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/pyproject.toml` & `thoughtful-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.1.4"
+version = "2.1.5"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
```

### Comparing `thoughtful-2.1.4/thoughtful/environment_variables.py` & `thoughtful-2.1.5/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/default_instances.py` & `thoughtful-2.1.5/thoughtful/supervisor/default_instances.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/event_bus.py` & `thoughtful-2.1.5/thoughtful/supervisor/event_bus.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/main_context.py` & `thoughtful-2.1.5/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/manifest.py` & `thoughtful-2.1.5/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
     def __post_init__(self):
         """
         Validate the record message length
         """
         if len(self.message) > 120:
             raise ValueError("Record Message Field - 120 Character limit exceeded")
-
         validate_metadata_json_helper(self.metadata)
 
     def __json__(self):
         return {
             "id": self.record_id,
             "status": self.status.value,
             "message": self.message,
```

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/report_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 
 It returns this ``Report`` object as the final product of the run.
 """
 
 from __future__ import annotations
 
 import datetime
+import logging
 import time
 from collections import OrderedDict, defaultdict
 from dataclasses import dataclass, field
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 from thoughtful.supervisor.manifest import StepId
 from thoughtful.supervisor.reporting.record import Record
 from thoughtful.supervisor.reporting.record_report import RecordReport
 from thoughtful.supervisor.reporting.report import Report
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.reporting.timer import Timer
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class RecordAccumulator:
     """
     Manages a list of records that are being processed by a step.
     """
 
@@ -89,14 +92,35 @@
     """
 
     _record_accumulator: RecordAccumulator = field(default_factory=RecordAccumulator)
     """
     RecordAccumulator: Holds records that were processed by this step.
     """
 
+    def update_from(self, other: StepReportBuilder) -> None:
+        """
+        Update a new ``StepReportBuilder`` from an existing ``StepReportBuilder``.
+
+        Args:
+            other (StepReportBuilder): The step report builder to update from.
+        """
+        # this bypasses StepReports created by decorator method (ie. do not have
+        # records)
+        other_records_by_id = {r.record_id: r for r in other.records}
+        for record in self.records:
+            if record.record_id in other_records_by_id:
+                logger.warning(
+                    f"Duplicate record '{record.record_id}' found in step '{self.step_id}'"
+                )
+
+        self.end_time = other.end_time
+        self.status = other.status
+        for other_record in other.records:
+            self._record_accumulator.upsert(other_record)
+
     def to_reports(self) -> List[Union[StepReport, RecordReport]]:
         step_report = self._to_report()
         record_reports: List[
             Union[StepReport, RecordReport]
         ] = self._record_accumulator.to_reports(step_report)
         return record_reports + [step_report]
 
@@ -134,29 +158,30 @@
             status=self.status,
             start_time=self.start_time,
             end_time=self.end_time,
         )
 
 
 RecordId = str
+StepId = str
 
 
 @dataclass
 class ReportBuilder:
     """
     A work report builder that creates a new work report as a digital worker
     is executed.
     """
 
     timer: Timer = field(default_factory=Timer)
     """
     Timer: The timer used to time the execution of the workflow.
     """
 
-    step_report_builders: List[StepReportBuilder] = field(default_factory=list)
+    _step_report_builders: List[StepReportBuilder] = field(default_factory=list)
     """
     List[StepReportBuilder]: The list of step reports.
     """
 
     timer_start: float = time.perf_counter()
     """
     float: The start time of the workflow.
@@ -215,14 +240,40 @@
             step_id (str): The step id to override.
             status (Status | str): The status to override the step to.
         """
         # Convert the status to the correct type if necessary
         safe_status = Status(status)
         self._step_statuses_to_override[step_id] = safe_status
 
+    def find_index(self, step_report_builder: StepReportBuilder) -> Union[int, None]:
+        """
+        Find the index of the step_report_builder in the ReportBuilder's _step_report_builders
+        that matches the incoming steps and does not already have Records attached to it.
+        """
+        index = next(
+            (
+                index
+                for index, step in enumerate(self._step_report_builders)
+                if step.step_id == step_report_builder.step_id
+            ),
+            None,
+        )
+        return index
+
+    def add_step_report(self, step_report_builder: StepReportBuilder) -> None:
+        """
+        Add a StepReport if it doesn't exist already. If it does exist, update
+        the existing StepReport with the new StepReport's records.
+        """
+        index = self.find_index(step_report_builder)
+        if index is not None or index == 0:
+            self._step_report_builders[index].update_from(step_report_builder)
+        else:
+            self._step_report_builders.append(step_report_builder)
+
     def set_record_status(
         self,
         step_id: str,
         record_id: str,
         status: Union[Status, str],
         message: Optional[str] = None,
         metadata: Optional[dict] = None,
@@ -271,15 +322,15 @@
         and ``_records_to_override`` dictionaries.
 
         Returns:
             Report: The finalized work report.
         """
         timed = self.timer.end()
 
-        for step_builder in self.step_report_builders:
+        for step_builder in self._step_report_builders:
             # Override the step status if requested
             if step_builder.step_id in self._step_statuses_to_override:
                 new_status = self._step_statuses_to_override[step_builder.step_id]
                 step_builder.status = new_status
             # Override any of the step's record statuses if requested
             if step_builder.step_id in self._records_to_override:
                 records = self._records_to_override[step_builder.step_id]
@@ -288,15 +339,17 @@
                 for record_id, record in records.items():
                     step_builder.set_record_status(
                         record_id, record.status, record.message, record.metadata
                     )
 
         # Merge all the step reports together
         final_workflow = [
-            report for step in self.step_report_builders for report in step.to_reports()
+            report
+            for step in self._step_report_builders
+            for report in step.to_reports()
         ]
 
         # Set the run status
         self.status = Status.FAILED if self.run_had_exception else Status.SUCCEEDED
         if self._run_status_override is not None:
             self.status = self._run_status_override
```

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.1.5/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/step_context.py` & `thoughtful-2.1.5/thoughtful/supervisor/step_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,15 @@
         self.step_report_builder.end_time = timed_info.end
         self.step_report_builder.status = step_status
 
         for report in self.step_report_builder.to_reports():
             new_event = StepReportChangeEvent(step_report=report)
             self.event_bus.emit(new_event)
 
-        self.report_builder.step_report_builders.append(self.step_report_builder)
-
+        self.report_builder.add_step_report(self.step_report_builder)
         # Return False so that any exceptions inside this context
         # are still raised after this function ends
         return False
 
     def error(self) -> None:
         """
         Sets the status of this step to `Status.FAILED` in its `StepReport`.
@@ -222,15 +221,14 @@
         # Convert the status to the correct type if necessary
         if type(record_id) != str:
             raise TypeError("record_id must be a string")
         if message is not None and not type(message) == str:
             raise ValueError("Record message must be a string")
         if metadata is not None and not type(metadata) == dict:
             raise ValueError("Record metadata must be a dict")
-
         message = message or ""
         metadata = metadata or {}
         safe_status = Status(status)
         self.step_report_builder.set_record_status(
             record_id, safe_status, message, metadata
         )
 
@@ -242,8 +240,8 @@
 
     with substep(report_builder, 1) as s:
         print("hello world")
 
         with substep(report_builder, "1.1") as s2:
             print("inner step")
 
-    print(report_builder.step_report_builders)
+    print(report_builder._step_report_builders)
```

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.1.5/thoughtful/supervisor/step_decorator_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,16 @@
         caught_exception = ex
         final_status = Status.FAILED
     timer_result = func_timer.end()
 
     # Finish the report
     this_steps_report_builder.end_time = timer_result.end
     this_steps_report_builder.status = final_status
-    report_builder.step_report_builders.append(this_steps_report_builder)
 
+    report_builder.add_step_report(this_steps_report_builder)
     for report in this_steps_report_builder.to_reports():
         new_event = StepReportChangeEvent(step_report=report)
         event_bus.emit(new_event)
 
     """Passthrough the step's return value or raised exception"""
     # If the step failed and raised an exception, raise that instead
     # of returning None
```

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.1.5/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-2.1.5/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.1.5/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/streaming/streamer.py` & `thoughtful-2.1.5/thoughtful/supervisor/streaming/streamer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/thoughtful/supervisor/streaming/token.py` & `thoughtful-2.1.5/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.4/PKG-INFO` & `thoughtful-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.1.4
+Version: 2.1.5
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
```

