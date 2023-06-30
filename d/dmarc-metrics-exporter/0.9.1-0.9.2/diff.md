# Comparing `tmp/dmarc_metrics_exporter-0.9.1.tar.gz` & `tmp/dmarc_metrics_exporter-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmarc_metrics_exporter-0.9.1.tar", max compression
+gzip compressed data, was "dmarc_metrics_exporter-0.9.2.tar", max compression
```

## Comparing `dmarc_metrics_exporter-0.9.1.tar` & `dmarc_metrics_exporter-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1073 2023-02-09 20:22:35.622541 dmarc_metrics_exporter-0.9.1/LICENSE
--rw-r--r--   0        0        0    10258 2023-02-09 20:22:35.622541 dmarc_metrics_exporter-0.9.1/README.rst
--rw-r--r--   0        0        0       22 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/__init__.py
--rw-r--r--   0        0        0      109 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/__main__.py
--rw-r--r--   0        0        0     5096 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/app.py
--rw-r--r--   0        0        0     4447 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/deserialization.py
--rw-r--r--   0        0        0      703 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/dmarc_event.py
--rw-r--r--   0        0        0     1716 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/dmarc_metrics.py
--rw-r--r--   0        0        0     2104 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/expiring_set.py
--rw-r--r--   0        0        0    13839 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_client.py
--rw-r--r--   0        0        0     5784 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_parser.py
--rwxr-xr-x   0        0        0     5172 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_queue.py
--rw-r--r--   0        0        0     1793 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/metrics_persister.py
--rw-r--r--   0        0        0      461 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/__init__.py
--rw-r--r--   0        0        0     9773 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
--rw-r--r--   0        0        0        0 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/tests/__init__.py
--rw-r--r--   0        0        0     2972 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/tests/sample_data.py
--rw-r--r--   0        0        0      403 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/tests/test_deserialization.py
--rw-r--r--   0        0        0     5093 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/prometheus_exporter.py
--rw-r--r--   0        0        0        0 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/__init__.py
--rw-r--r--   0        0        0     2976 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/conftest.py
--rw-r--r--   0        0        0     1769 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/sample_emails.py
--rw-r--r--   0        0        0     2983 2023-02-09 20:22:35.626541 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_app.py
--rw-r--r--   0        0        0     1357 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_deserialization.py
--rw-r--r--   0        0        0     1428 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
--rw-r--r--   0        0        0     3499 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_e2e.py
--rw-r--r--   0        0        0      932 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_expiring_set.py
--rw-r--r--   0        0        0    16524 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_client.py
--rw-r--r--   0        0        0    10834 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_parser.py
--rw-r--r--   0        0        0     4757 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_queue.py
--rw-r--r--   0        0        0     1192 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_metrics_persister.py
--rw-r--r--   0        0        0     3960 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
--rwxr-xr-x   0        0        0     2133 2023-02-09 20:22:35.630540 dmarc_metrics_exporter-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    11705 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.1/setup.py
--rw-r--r--   0        0        0    11752 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 17:31:40.186472 dmarc_metrics_exporter-0.9.2/LICENSE
+-rw-r--r--   0        0        0    10258 2023-06-30 17:31:40.186472 dmarc_metrics_exporter-0.9.2/README.rst
+-rw-r--r--   0        0        0       22 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/__main__.py
+-rw-r--r--   0        0        0     5096 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/app.py
+-rw-r--r--   0        0        0     4447 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/deserialization.py
+-rw-r--r--   0        0        0      703 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_event.py
+-rw-r--r--   0        0        0     1716 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_metrics.py
+-rw-r--r--   0        0        0     2104 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/expiring_set.py
+-rw-r--r--   0        0        0    13739 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_client.py
+-rw-r--r--   0        0        0     5784 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_parser.py
+-rwxr-xr-x   0        0        0     5172 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_queue.py
+-rw-r--r--   0        0        0     1793 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/metrics_persister.py
+-rw-r--r--   0        0        0      461 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/__init__.py
+-rw-r--r--   0        0        0     9773 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/__init__.py
+-rw-r--r--   0        0        0     2972 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/sample_data.py
+-rw-r--r--   0        0        0      403 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/test_deserialization.py
+-rw-r--r--   0        0        0     5093 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/prometheus_exporter.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/__init__.py
+-rw-r--r--   0        0        0     2976 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/conftest.py
+-rw-r--r--   0        0        0     1769 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/sample_emails.py
+-rw-r--r--   0        0        0     2983 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_app.py
+-rw-r--r--   0        0        0     1357 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_deserialization.py
+-rw-r--r--   0        0        0     1428 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
+-rw-r--r--   0        0        0     3499 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_e2e.py
+-rw-r--r--   0        0        0      932 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_expiring_set.py
+-rw-r--r--   0        0        0    16524 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_client.py
+-rw-r--r--   0        0        0    10834 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_parser.py
+-rw-r--r--   0        0        0     4757 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_queue.py
+-rw-r--r--   0        0        0     1192 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_metrics_persister.py
+-rw-r--r--   0        0        0     3960 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
+-rwxr-xr-x   0        0        0     2133 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    11550 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.2/PKG-INFO
```

### Comparing `dmarc_metrics_exporter-0.9.1/LICENSE` & `dmarc_metrics_exporter-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/README.rst` & `dmarc_metrics_exporter-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/app.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/deserialization.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/dmarc_event.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_event.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/expiring_set.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_client.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,18 @@
     async def write_int(self, num: int):
         self.writer.write(str(num).encode("ascii"))
         await self._drain()
 
     async def write_string_literal(self, string: str):
         encoded = string.encode("utf-8")
         self._server_ready.clear()
-        self.writer.write(b"{")
-        self.writer.write(str(len(encoded)).encode("ascii"))
-        self.writer.write(b"}\r\n")
-        await self._drain()
+        await self.write_raw(b"{" + str(len(encoded)).encode("ascii") + b"}\r\n")
         await self._server_ready.wait()
 
-        self.writer.write(encoded)
-        await self._drain()
+        await self.write_raw(encoded)
 
 
 class _CommandsInUse:
     def __init__(self):
         self._in_use = set()
         self._change_condition = asyncio.Condition()
```

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_parser.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/imap_queue.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/metrics_persister.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/dmarc_aggregate_report.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/dmarc_aggregate_report.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/model/tests/sample_data.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/sample_data.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/conftest.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/sample_emails.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/sample_emails.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_app.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_deserialization.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_e2e.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_expiring_set.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_client.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_client.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_parser.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_imap_queue.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_metrics_persister.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/dmarc_metrics_exporter/tests/test_prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.1/pyproject.toml` & `dmarc_metrics_exporter-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 description = "Export Prometheus metrics from DMARC reports."
 keywords = ["DMARC", "DKIM", "SPF", "Prometheus"]
 license = "MIT"
 name = "dmarc-metrics-exporter"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/dmarc-metrics-exporter/"
-version = "0.9.1" # Update also in __init__.py!
+version = "0.9.2" # Update also in __init__.py!
 
 [tool.poetry.scripts]
 dmarc-metrics-exporter = "dmarc_metrics_exporter.__main__:run"
 
 [tool.poetry.dependencies]
 bite-parser = "^0.2.2"
 dataclasses-serialization = "^1.3.1"
```

### Comparing `dmarc_metrics_exporter-0.9.1/setup.py` & `dmarc_metrics_exporter-0.9.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,316 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dmarc-metrics-exporter
+Version: 0.9.2
+Summary: Export Prometheus metrics from DMARC reports.
+Home-page: https://github.com/jgosmann/dmarc-metrics-exporter/
+License: MIT
+Keywords: DMARC,DKIM,SPF,Prometheus
+Author: Jan Gosmann
+Author-email: jan@hyper-world.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Communications :: Email
+Classifier: Topic :: System :: Monitoring
+Requires-Dist: bite-parser (>=0.2.2,<0.3.0)
+Requires-Dist: dataclasses-serialization (>=1.3.1,<2.0.0)
+Requires-Dist: prometheus_client (>=0.15.0,<0.16.0)
+Requires-Dist: typing-extensions (>=4.0.1,<5.0.0)
+Requires-Dist: uvicorn[standard] (>=0.19.0,<0.20.0)
+Requires-Dist: xsdata (>=21.9)
+Project-URL: Repository, https://github.com/jgosmann/dmarc-metrics-exporter/
+Description-Content-Type: text/x-rst
 
-packages = \
-['dmarc_metrics_exporter',
- 'dmarc_metrics_exporter.model',
- 'dmarc_metrics_exporter.model.tests',
- 'dmarc_metrics_exporter.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bite-parser>=0.2.2,<0.3.0',
- 'dataclasses-serialization>=1.3.1,<2.0.0',
- 'prometheus_client>=0.15.0,<0.16.0',
- 'typing-extensions>=4.0.1,<5.0.0',
- 'uvicorn[standard]>=0.19.0,<0.20.0',
- 'xsdata>=21.9']
-
-entry_points = \
-{'console_scripts': ['dmarc-metrics-exporter = '
-                     'dmarc_metrics_exporter.__main__:run']}
-
-setup_kwargs = {
-    'name': 'dmarc-metrics-exporter',
-    'version': '0.9.1',
-    'description': 'Export Prometheus metrics from DMARC reports.',
-    'long_description': '.. image:: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml/badge.svg\n  :target: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml\n  :alt: CI and release pipeline\n.. image:: https://codecov.io/gh/jgosmann/dmarc-metrics-exporter/branch/main/graph/badge.svg?token=O4M05YWNQK\n  :target: https://codecov.io/gh/jgosmann/dmarc-metrics-exporter\n  :alt: Codecov coverage\n.. image:: https://img.shields.io/pypi/v/dmarc-metrics-exporter\n  :target: https://pypi.org/project/dmarc-metrics-exporter/\n  :alt: PyPI\n.. image:: https://img.shields.io/pypi/pyversions/dmarc-metrics-exporter\n  :target: https://pypi.org/project/dmarc-metrics-exporter/\n  :alt: PyPI - Python Version\n.. image:: https://img.shields.io/pypi/l/dmarc-metrics-exporter\n  :target: https://pypi.org/project/dmarc-metrics-exporter/\n  :alt: PyPI - License\n\ndmarcs-metrics-exporter\n=======================\n\nExport metrics derived from DMARC aggregate reports to Prometheus.\nThis exporter regularly polls\nfor new aggregate report emails\nvia IMAP.\nThe following metrics will be collected\nand exposed at an HTTP endpoint\nfor Prometheus:\n\n* ``dmarc_total``: Total number of reported messages.\n* ``dmarc_compliant_total``: Total number of DMARC compliant messages.\n* ``dmarc_quarantine_total``: Total number of quarantined messages.\n* ``dmarc_reject_total``: Total number of rejected messages.\n* ``dmarc_spf_aligned_total``: Total number of SPF algined messages.\n* ``dmarc_spf_pass_total``: Total number of messages with raw SPF pass.\n* ``dmarc_dkim_aligned_total``: Total number of DKIM algined messages.\n* ``dmarc_dkim_pass_total``: Total number of messages with raw DKIM pass.\n\nEach of these metrics is subdivided by the following labels:\n\n* ``reporter``: Domain from which a DMARC aggregate report originated.\n* ``from_domain``: Domain from which the evaluated email originated.\n* ``dkim_domain``: Domain the DKIM signature is for.\n* ``spf_domain``: Domain used for the SPF check.\n\n\nInstallation\n------------\n\nThis describes the manual setup fo dmarc-metrics-exporter.\nAn Ansible role for automated deployment is provided in ``roles``.\nFurther instructions for Ansible are given in the readme file\nprovided in that directory.\n\nIt is best to run dmarc-metrics-exporter under a separate system user account.\nCreate one for example with\n\n.. code-block:: bash\n\n    adduser --system --group dmarc-metrics\n\nThen you can install dmarc-metrics-exporter with ``pip`` from PyPI for that\nuser:\n\n.. code-block:: bash\n\n    sudo -u dmarc-metrics pip3 install dmarc-metrics-exporter\n\nYou will need a location to store the ``metrics.db`` that is writable by that\nuser, for example:\n\n.. code-block:: bash\n\n    mkdir /var/lib/dmarc-metrics-exporter\n    chown dmarc-metrics:dmarc-metrics /var/lib/dmarc-metrics-exporter\n\n\nConfiguration\n-------------\n\nTo run dmarc-metrics-exporter a configuration file in JSON format is required.\nThe default location is ``/etc/dmarc-metrics-exporter.json``.\n\nBecause the configuration file will contain the IMAP password,\nmake sure to ensure proper permissions on it,\nfor example:\n\n.. code-block:: bash\n\n    chown root:dmarc-metrics /etc/dmarc-metrics-exporter.json\n    chmod 640 /etc/dmarc-metrics-exporter.json\n\nAn example configuration file is provided in this repository in\n``config/dmarc-metrics-exporter.sample.json``.\n\nThe following configuration options are available:\n\n* ``listen_addr`` (string, default ``"127.0.0.1"``): Listen address for the HTTP endpoint. Use ``"0.0.0.0"`` if running in a dockerized environment.\n* ``port`` (number, default ``9797``): Port to listen on for the HTTP endpoint.\n* ``imap`` (object, required): IMAP configuration to check for aggregate reports.\n\n  * ``host`` (string, default ``"localhost"``): Hostname of IMAP server to connect to.\n  * ``port`` (number, default ``993``): Port of the IMAP server to connect to.\n  * ``username`` (string, required): Login username for the IMAP connection.\n  * ``password``: (string, required): Login password for the IMAP connection.\n  * ``use_ssl``: (boolean, default ``true``): Whether to use SSL encryption for the connection. Disabling this will transmit the password in clear text! Currently, there is no support for STARTTLS.\n  * ``verify_certificate``: (boolean, default ``true``): Whether to verify the server\'s SSL certificate. You might have to set this to ``false`` if you are using a self-signed certificate. If this is disabled, someone else could impersonate the server and obtain the login data.\n\n* ``folders`` (object):\n\n  * ``inbox`` (string, default ``"INBOX"``): IMAP mailbox that is checked for incoming DMARC aggregate reports.\n  * ``done`` (string, default ``"Archive"``): IMAP mailbox that successfully processed reports are moved to.\n  * ``error``: (string, default ``"Invalid"``): IMAP mailbox that emails are moved to that could not be processed.\n\n* ``storage_path`` (string, default ``"/var/lib/dmarc-metrics-exporter"``):\n  Directory to persist data in that has to persisted between restarts.\n* ``poll_interval_seconds`` (number, default ``60``): How often to poll the IMAP server in seconds.\n* ``deduplication_max_seconds`` (number, default ``604800`` which is 7 days): How long individual report IDs will be remembered to avoid counting double delivered reports twice.\n* ``logging`` (object, default ``{ "version": 1, "disable_existing_loggers": false }``): Logging configuration. `See logging.config documentation. <https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema>`_\n\nUsage\n-----\n\nTo run dmarc-metrics-exporter with the default configuration in\n``/etc/dmarc-metrics-exporter.json``:\n\n.. code-block:: bash\n\n    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter\n\nTo use a different configuration file:\n\n.. code-block:: bash\n\n    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter --configuration <path>\n\nYou can enable debug logging with the `--debug`\nif you do not want to provide your own logging configuration:\n\n.. code-block:: bash\n\n    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter --debug\n\n\nsystemd\n^^^^^^^\n\nInstead of manually starting the dmarc-metrics-exporter,\nyou likely want to have it run as a system service.\nAn example systemd service file is provided in this repository in\n``config/dmarc-metrics-exporter.service``.\nMake sure that the paths and user/group names match your configuration\nand copy it to ``/etc/systemd/system`` to use it.\nTo have systemd pick it up a ``systemctl daemon-reload`` might be necessary.\n\nYou can than start/stop dmarc-metrics-exorter with:\n\n.. code-block:: bash\n\n    systemctl start dmarc-metrics-exporter\n    systemctl stop dmarc-metrics-exporter\n\nTo have dmarc-metrics-exporter start on system boot:\n\n.. code-block:: bash\n\n    systemctl enable dmarc-metrics-exporter\n\nDocker\n^^^^^^\n\nA new docker image is build for each release\nwith GitHub Actions as described in this yaml-file:\n``.github/workflows/docker-publish.yml``.\n\nNote that you should configure the `listen_addr` to `0.0.0.0` to be able to\naccess the metrics exporter from outside the container.\n\nExample docker-compose file:\n\n.. code-block:: yml\n\n    version: "3"\n\n    services:\n\n      dmarc-metrics-exporter:\n        # source: https://github.com/jamborjan/dmarc-metrics-exporter/pkgs/container/dmarc-metrics-exporter\n        container_name: dmarc-metrics-exporter\n        hostname: dmarc-metrics-exporter\n        image: jgosmann/dmarc-metrics-exporter:0.3.0\n        restart: unless-stopped\n        user: 1000:1000 #PUID=1000:PGID=1000\n        expose:\n          - 9797\n        volumes:\n          - \'/host/folder/dmarc-metrics-exporter.json:/etc/dmarc-metrics-exporter.json\'\n          - \'/host/folder/dmarc-metrics-exporter/metrics:/var/lib/dmarc-metrics-exporter:rw\'\n        logging:\n          driver: "json-file"\n          options:\n            tag: "{{.ImageName}}|{{.Name}}|{{.ImageFullID}}|{{.FullID}}"\n        networks:\n          - YourDockerLan\n\n    # $ docker network create -d bridge --attachable YourDockerLan\n    networks:\n      YourDockerLan:\n        external:\n          name: YourDockerLan\n\nPrometheus\n^^^^^^^^^^\n\nExample prometheus config file:\n\n.. code-block:: yml\n\n    global:\n      scrape_interval: 15s\n      evaluation_interval: 15s\n\n    rule_files:\n\n    scrape_configs:\n\n      - job_name: \'dmarc-metrics-exporter\'\n        static_configs:\n          - targets: [\'dmarc-metrics-exporter:9797\']\n\nGrafana\n^^^^^^^\n\nAn example configuration file is provided in this repository in\n``config/dmarc-metrics-exporter.grafana.sample.json``. This example dashboard displays the collected metrics as shown in the screenshot below.\n\n.. figure:: config/dmarc-metrics-exporter.grafana.sample.png\n\n   Example grafana dashboard\n\nHints\n^^^^^\n\nYou should not use your normal email and password credentials for the dmarc-metrics-exporter.\nIf you are not able to create a dedicated service account email account, you should use an app password.\n\nMicrosoft Exchange Online\n"""""""""""""""""""""""""\n\n* App passwords are available when you are using Multi Factor Authentication (MFA).\n  `Manage app passwords for two-step verification <https://account.activedirectory.windowsazure.com/AppPasswords.aspx>`_\n* If you don\'t see the app passwords option or get an error,\n  `check if MFA is enabled <https://account.activedirectory.windowsazure.com/UserManagement/MultifactorVerification.aspx>`_\n  for the user.\n* If you still don\'t see the app passwords option,\n  `check if app passwords are allowed in your organization <https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-mfa-app-passwords#allow-users-to-create-app-passwords>`_\n* Finally, `ensure that IMAP is enabled for the user <https://docs.microsoft.com/en-us/exchange/clients-and-mobile-in-exchange-online/pop3-and-imap4/enable-or-disable-pop3-or-imap4-access>`_.\n\n\nDevelopment\n-----------\n\nPrerequisites\n^^^^^^^^^^^^^\n\n* `Python <https://www.python.org/>`_\n* `pre-commit <https://pre-commit.com/>`_\n* `Poetry <https://python-poetry.org/>`_\n* `Docker <https://www.docker.com/>`_\n\nSetup development environment\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n.. code-block:: bash\n\n    pre-commit install\n    poetry install\n\n\nRun tests\n^^^^^^^^^\n\n.. code-block:: bash\n\n    docker-compose up -d\n    poetry run pytest\n',
-    'author': 'Jan Gosmann',
-    'author_email': 'jan@hyper-world.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jgosmann/dmarc-metrics-exporter/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+.. image:: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml/badge.svg
+  :target: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml
+  :alt: CI and release pipeline
+.. image:: https://codecov.io/gh/jgosmann/dmarc-metrics-exporter/branch/main/graph/badge.svg?token=O4M05YWNQK
+  :target: https://codecov.io/gh/jgosmann/dmarc-metrics-exporter
+  :alt: Codecov coverage
+.. image:: https://img.shields.io/pypi/v/dmarc-metrics-exporter
+  :target: https://pypi.org/project/dmarc-metrics-exporter/
+  :alt: PyPI
+.. image:: https://img.shields.io/pypi/pyversions/dmarc-metrics-exporter
+  :target: https://pypi.org/project/dmarc-metrics-exporter/
+  :alt: PyPI - Python Version
+.. image:: https://img.shields.io/pypi/l/dmarc-metrics-exporter
+  :target: https://pypi.org/project/dmarc-metrics-exporter/
+  :alt: PyPI - License
 
+dmarcs-metrics-exporter
+=======================
+
+Export metrics derived from DMARC aggregate reports to Prometheus.
+This exporter regularly polls
+for new aggregate report emails
+via IMAP.
+The following metrics will be collected
+and exposed at an HTTP endpoint
+for Prometheus:
+
+* ``dmarc_total``: Total number of reported messages.
+* ``dmarc_compliant_total``: Total number of DMARC compliant messages.
+* ``dmarc_quarantine_total``: Total number of quarantined messages.
+* ``dmarc_reject_total``: Total number of rejected messages.
+* ``dmarc_spf_aligned_total``: Total number of SPF algined messages.
+* ``dmarc_spf_pass_total``: Total number of messages with raw SPF pass.
+* ``dmarc_dkim_aligned_total``: Total number of DKIM algined messages.
+* ``dmarc_dkim_pass_total``: Total number of messages with raw DKIM pass.
+
+Each of these metrics is subdivided by the following labels:
+
+* ``reporter``: Domain from which a DMARC aggregate report originated.
+* ``from_domain``: Domain from which the evaluated email originated.
+* ``dkim_domain``: Domain the DKIM signature is for.
+* ``spf_domain``: Domain used for the SPF check.
+
+
+Installation
+------------
+
+This describes the manual setup fo dmarc-metrics-exporter.
+An Ansible role for automated deployment is provided in ``roles``.
+Further instructions for Ansible are given in the readme file
+provided in that directory.
+
+It is best to run dmarc-metrics-exporter under a separate system user account.
+Create one for example with
+
+.. code-block:: bash
+
+    adduser --system --group dmarc-metrics
+
+Then you can install dmarc-metrics-exporter with ``pip`` from PyPI for that
+user:
+
+.. code-block:: bash
+
+    sudo -u dmarc-metrics pip3 install dmarc-metrics-exporter
+
+You will need a location to store the ``metrics.db`` that is writable by that
+user, for example:
+
+.. code-block:: bash
+
+    mkdir /var/lib/dmarc-metrics-exporter
+    chown dmarc-metrics:dmarc-metrics /var/lib/dmarc-metrics-exporter
+
+
+Configuration
+-------------
+
+To run dmarc-metrics-exporter a configuration file in JSON format is required.
+The default location is ``/etc/dmarc-metrics-exporter.json``.
+
+Because the configuration file will contain the IMAP password,
+make sure to ensure proper permissions on it,
+for example:
+
+.. code-block:: bash
+
+    chown root:dmarc-metrics /etc/dmarc-metrics-exporter.json
+    chmod 640 /etc/dmarc-metrics-exporter.json
+
+An example configuration file is provided in this repository in
+``config/dmarc-metrics-exporter.sample.json``.
+
+The following configuration options are available:
+
+* ``listen_addr`` (string, default ``"127.0.0.1"``): Listen address for the HTTP endpoint. Use ``"0.0.0.0"`` if running in a dockerized environment.
+* ``port`` (number, default ``9797``): Port to listen on for the HTTP endpoint.
+* ``imap`` (object, required): IMAP configuration to check for aggregate reports.
+
+  * ``host`` (string, default ``"localhost"``): Hostname of IMAP server to connect to.
+  * ``port`` (number, default ``993``): Port of the IMAP server to connect to.
+  * ``username`` (string, required): Login username for the IMAP connection.
+  * ``password``: (string, required): Login password for the IMAP connection.
+  * ``use_ssl``: (boolean, default ``true``): Whether to use SSL encryption for the connection. Disabling this will transmit the password in clear text! Currently, there is no support for STARTTLS.
+  * ``verify_certificate``: (boolean, default ``true``): Whether to verify the server's SSL certificate. You might have to set this to ``false`` if you are using a self-signed certificate. If this is disabled, someone else could impersonate the server and obtain the login data.
+
+* ``folders`` (object):
+
+  * ``inbox`` (string, default ``"INBOX"``): IMAP mailbox that is checked for incoming DMARC aggregate reports.
+  * ``done`` (string, default ``"Archive"``): IMAP mailbox that successfully processed reports are moved to.
+  * ``error``: (string, default ``"Invalid"``): IMAP mailbox that emails are moved to that could not be processed.
+
+* ``storage_path`` (string, default ``"/var/lib/dmarc-metrics-exporter"``):
+  Directory to persist data in that has to persisted between restarts.
+* ``poll_interval_seconds`` (number, default ``60``): How often to poll the IMAP server in seconds.
+* ``deduplication_max_seconds`` (number, default ``604800`` which is 7 days): How long individual report IDs will be remembered to avoid counting double delivered reports twice.
+* ``logging`` (object, default ``{ "version": 1, "disable_existing_loggers": false }``): Logging configuration. `See logging.config documentation. <https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema>`_
+
+Usage
+-----
+
+To run dmarc-metrics-exporter with the default configuration in
+``/etc/dmarc-metrics-exporter.json``:
+
+.. code-block:: bash
+
+    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter
+
+To use a different configuration file:
+
+.. code-block:: bash
+
+    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter --configuration <path>
+
+You can enable debug logging with the `--debug`
+if you do not want to provide your own logging configuration:
+
+.. code-block:: bash
+
+    sudo -u dmarc-metrics python3 -m dmarc_metrics_exporter --debug
+
+
+systemd
+^^^^^^^
+
+Instead of manually starting the dmarc-metrics-exporter,
+you likely want to have it run as a system service.
+An example systemd service file is provided in this repository in
+``config/dmarc-metrics-exporter.service``.
+Make sure that the paths and user/group names match your configuration
+and copy it to ``/etc/systemd/system`` to use it.
+To have systemd pick it up a ``systemctl daemon-reload`` might be necessary.
+
+You can than start/stop dmarc-metrics-exorter with:
+
+.. code-block:: bash
+
+    systemctl start dmarc-metrics-exporter
+    systemctl stop dmarc-metrics-exporter
+
+To have dmarc-metrics-exporter start on system boot:
+
+.. code-block:: bash
+
+    systemctl enable dmarc-metrics-exporter
+
+Docker
+^^^^^^
+
+A new docker image is build for each release
+with GitHub Actions as described in this yaml-file:
+``.github/workflows/docker-publish.yml``.
+
+Note that you should configure the `listen_addr` to `0.0.0.0` to be able to
+access the metrics exporter from outside the container.
+
+Example docker-compose file:
+
+.. code-block:: yml
+
+    version: "3"
+
+    services:
+
+      dmarc-metrics-exporter:
+        # source: https://github.com/jamborjan/dmarc-metrics-exporter/pkgs/container/dmarc-metrics-exporter
+        container_name: dmarc-metrics-exporter
+        hostname: dmarc-metrics-exporter
+        image: jgosmann/dmarc-metrics-exporter:0.3.0
+        restart: unless-stopped
+        user: 1000:1000 #PUID=1000:PGID=1000
+        expose:
+          - 9797
+        volumes:
+          - '/host/folder/dmarc-metrics-exporter.json:/etc/dmarc-metrics-exporter.json'
+          - '/host/folder/dmarc-metrics-exporter/metrics:/var/lib/dmarc-metrics-exporter:rw'
+        logging:
+          driver: "json-file"
+          options:
+            tag: "{{.ImageName}}|{{.Name}}|{{.ImageFullID}}|{{.FullID}}"
+        networks:
+          - YourDockerLan
+
+    # $ docker network create -d bridge --attachable YourDockerLan
+    networks:
+      YourDockerLan:
+        external:
+          name: YourDockerLan
+
+Prometheus
+^^^^^^^^^^
+
+Example prometheus config file:
+
+.. code-block:: yml
+
+    global:
+      scrape_interval: 15s
+      evaluation_interval: 15s
+
+    rule_files:
+
+    scrape_configs:
+
+      - job_name: 'dmarc-metrics-exporter'
+        static_configs:
+          - targets: ['dmarc-metrics-exporter:9797']
+
+Grafana
+^^^^^^^
+
+An example configuration file is provided in this repository in
+``config/dmarc-metrics-exporter.grafana.sample.json``. This example dashboard displays the collected metrics as shown in the screenshot below.
+
+.. figure:: config/dmarc-metrics-exporter.grafana.sample.png
+
+   Example grafana dashboard
+
+Hints
+^^^^^
+
+You should not use your normal email and password credentials for the dmarc-metrics-exporter.
+If you are not able to create a dedicated service account email account, you should use an app password.
+
+Microsoft Exchange Online
+"""""""""""""""""""""""""
+
+* App passwords are available when you are using Multi Factor Authentication (MFA).
+  `Manage app passwords for two-step verification <https://account.activedirectory.windowsazure.com/AppPasswords.aspx>`_
+* If you don't see the app passwords option or get an error,
+  `check if MFA is enabled <https://account.activedirectory.windowsazure.com/UserManagement/MultifactorVerification.aspx>`_
+  for the user.
+* If you still don't see the app passwords option,
+  `check if app passwords are allowed in your organization <https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-mfa-app-passwords#allow-users-to-create-app-passwords>`_
+* Finally, `ensure that IMAP is enabled for the user <https://docs.microsoft.com/en-us/exchange/clients-and-mobile-in-exchange-online/pop3-and-imap4/enable-or-disable-pop3-or-imap4-access>`_.
+
+
+Development
+-----------
+
+Prerequisites
+^^^^^^^^^^^^^
+
+* `Python <https://www.python.org/>`_
+* `pre-commit <https://pre-commit.com/>`_
+* `Poetry <https://python-poetry.org/>`_
+* `Docker <https://www.docker.com/>`_
+
+Setup development environment
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: bash
+
+    pre-commit install
+    poetry install
+
+
+Run tests
+^^^^^^^^^
+
+.. code-block:: bash
+
+    docker-compose up -d
+    poetry run pytest
 
-setup(**setup_kwargs)
```

