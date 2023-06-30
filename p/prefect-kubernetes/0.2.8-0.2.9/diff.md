# Comparing `tmp/prefect-kubernetes-0.2.8.tar.gz` & `tmp/prefect-kubernetes-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-siz5suu5/prefect-kubernetes-0.2.8.tar", last modified: Thu May 25 19:29:13 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-nekx3usn/prefect-kubernetes-0.2.9.tar", last modified: Tue Jun 20 17:49:38 2023, max compression
```

## Comparing `prefect-kubernetes-0.2.8.tar` & `prefect-kubernetes-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33250 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:13.000000 prefect-kubernetes-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_events_replicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    82835 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-25 19:27:32.000000 prefect-kubernetes-0.2.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33572 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:49:38.000000 prefect-kubernetes-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82881 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-20 17:48:12.000000 prefect-kubernetes-0.2.9/versioneer.py
```

### Comparing `prefect-kubernetes-0.2.8/LICENSE` & `prefect-kubernetes-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/PKG-INFO` & `prefect-kubernetes-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.8/README.md` & `prefect-kubernetes-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/credentials.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/custom_objects.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/deployments.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/events.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/events.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/exceptions.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/flows.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/jobs.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/pods.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/services.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/utilities.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes/worker.py` & `prefect-kubernetes-0.2.9/prefect_kubernetes/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,15 +385,24 @@
                 "Unable to verify command due to invalid job manifest template."
             )
 
     def _populate_generate_name_if_not_present(self):
         """Ensures that the generateName is present in the job manifest."""
         manifest_generate_name = self.job_manifest["metadata"].get("generateName", "")
         has_placeholder = len(find_placeholders(manifest_generate_name)) > 0
-        if not manifest_generate_name or has_placeholder:
+        # if name wasn't present during template rendering, generateName will be
+        # just a hyphen
+        manifest_generate_name_templated_with_empty_string = (
+            manifest_generate_name == "-"
+        )
+        if (
+            not manifest_generate_name
+            or has_placeholder
+            or manifest_generate_name_templated_with_empty_string
+        ):
             generate_name = None
             if self.name:
                 generate_name = _slugify_name(self.name)
             # _slugify_name will return None if the slugified name in an exception
             if not generate_name:
                 generate_name = "prefect-job"
             self.job_manifest["metadata"]["generateName"] = f"{generate_name}-"
```

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/PKG-INFO` & `prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.8/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect-kubernetes-0.2.9/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/setup.cfg` & `prefect-kubernetes-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/setup.py` & `prefect-kubernetes-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_block_standards.py` & `prefect-kubernetes-0.2.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_credentials.py` & `prefect-kubernetes-0.2.9/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_custom_objects.py` & `prefect-kubernetes-0.2.9/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_deployments.py` & `prefect-kubernetes-0.2.9/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_events_replicator.py` & `prefect-kubernetes-0.2.9/tests/test_events_replicator.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_flows.py` & `prefect-kubernetes-0.2.9/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_jobs.py` & `prefect-kubernetes-0.2.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_pods.py` & `prefect-kubernetes-0.2.9/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_services.py` & `prefect-kubernetes-0.2.9/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_utilities.py` & `prefect-kubernetes-0.2.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.8/tests/test_worker.py` & `prefect-kubernetes-0.2.9/tests/test_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import uuid
 from contextlib import contextmanager
 from time import monotonic, sleep
 from unittest import mock
 from unittest.mock import MagicMock, Mock
 
 import anyio
 import anyio.abc
@@ -150,15 +151,15 @@
             name=None,
             namespace="default",
             job_manifest={
                 "apiVersion": "batch/v1",
                 "kind": "Job",
                 "metadata": {
                     "namespace": "default",
-                    "generateName": "{{ name }}-",
+                    "generateName": "-",
                     "labels": {},
                 },
                 "spec": {
                     "template": {
                         "spec": {
                             "parallelism": 1,
                             "completions": 1,
@@ -681,15 +682,15 @@
     ),
 ]
 
 
 class TestKubernetesWorkerJobConfiguration:
     @pytest.fixture
     def flow_run(self):
-        return FlowRun(name="my-flow-run-name")
+        return FlowRun(flow_id=uuid.uuid4(), name="my-flow-run-name")
 
     @pytest.fixture
     def deployment(self):
         return DeploymentResponse(name="my-deployment-name")
 
     @pytest.fixture
     def flow(self):
@@ -914,15 +915,15 @@
     async def default_configuration(self):
         return await KubernetesWorkerJobConfiguration.from_template_and_values(
             KubernetesWorker.get_default_base_job_template(), {}
         )
 
     @pytest.fixture
     def flow_run(self):
-        return FlowRun(name="my-flow-run-name")
+        return FlowRun(flow_id=uuid.uuid4(), name="my-flow-run-name")
 
     async def test_creates_job_by_building_a_manifest(
         self,
         default_configuration: KubernetesWorkerJobConfiguration,
         flow_run,
         mock_batch_client,
         mock_core_client,
```

### Comparing `prefect-kubernetes-0.2.8/versioneer.py` & `prefect-kubernetes-0.2.9/versioneer.py`

 * *Files identical despite different names*

