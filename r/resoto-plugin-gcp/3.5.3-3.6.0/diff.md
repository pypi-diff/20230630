# Comparing `tmp/resoto-plugin-gcp-3.5.3.tar.gz` & `tmp/resoto-plugin-gcp-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.5.3.tar", last modified: Wed Jun 21 14:23:20 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.6.0.tar", last modified: Fri Jun 30 19:31:54 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.5.3.tar` & `resoto-plugin-gcp-3.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24264 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   284330 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.537868 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:19:27.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 14:23:20.000000 resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:20.541868 resoto-plugin-gcp-3.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 14:18:17.000000 resoto-plugin-gcp-3.5.3/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.372810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.376810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284432 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.372810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:13.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.5.3/PKG-INFO` & `resoto-plugin-gcp-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.5.3/pyproject.toml` & `resoto-plugin-gcp-3.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-gcp"
 description = "Resoto GCP Collector Plugin"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.3",
+    "resotolib==3.6.0",
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from concurrent.futures import ThreadPoolExecutor
 import logging
-from typing import Type, List
+from concurrent.futures import ThreadPoolExecutor
+from typing import Type, List, Any, Optional
 
 from resoto_plugin_gcp.config import GcpConfig
 from resoto_plugin_gcp.gcp_client import GcpApiSpec
-from resoto_plugin_gcp.utils import Credentials
 from resoto_plugin_gcp.resources import compute, container, billing, sqladmin, storage
 from resoto_plugin_gcp.resources.base import GcpResource, GcpProject, ExecutorQueue, GraphBuilder, GcpRegion, GcpZone
+from resoto_plugin_gcp.utils import Credentials
 from resotolib.baseresources import Cloud
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 
 log = logging.getLogger("resoto.plugins.gcp")
 all_resources: List[Type[GcpResource]] = (
     compute.resources + container.resources + billing.resources + sqladmin.resources + storage.resources
@@ -77,40 +77,58 @@
                     global_builder.submit_work(resource_class.collect_resources, global_builder)
 
             # fetch all region level resources
             for region in global_builder.resources_of(GcpRegion):
                 if region.name == "global":
                     continue
                 global_builder.submit_work(self.collect_region, region, global_builder.for_region(region))
-
             global_builder.executor.wait_for_submitted_work()
+
             # connect nodes
             for node, data in list(self.graph.nodes(data=True)):
                 if isinstance(node, GcpResource):
                     node.connect_in_graph(global_builder, data.get("source", {}))
 
-            log.info(f"[GCP:{self.project.id}] Collecting resources done.")
+            # remove unconnected nodes
             self.remove_unconnected_nodes()
 
+            # post process nodes
+            for node, data in list(self.graph.nodes(data=True)):
+                if isinstance(node, GcpResource):
+                    node.post_process_instance(global_builder, data.get("source", {}))
+
+            log.info(f"[GCP:{self.project.id}] Collecting resources done.")
+
     def remove_unconnected_nodes(self):
-        remove_nodes = set()
+        remove_nodes = []
 
-        def rmnodes(cls) -> None:
+        def rm_nodes(cls, ignore_kinds: Optional[Type[Any]] = None) -> None:
             for node in self.graph.nodes:
-                if isinstance(node, cls) and not any(True for _ in self.graph.successors(node)):
-                    remove_nodes.add(node)
+                if not isinstance(node, cls):
+                    continue
+                suc = list(self.graph.successors(node))
+                filtered = [s for s in suc if not isinstance(s, ignore_kinds)] if ignore_kinds else suc
+                if not filtered:
+                    remove_nodes.extend(suc)
+                    remove_nodes.append(node)
+            removed = set()
             for node in remove_nodes:
+                if node in removed:
+                    continue
+                removed.add(node)
                 self.graph.remove_node(node)
             log.debug(f"Removing {len(remove_nodes)} unreferenced nodes of type {cls}")
             remove_nodes.clear()
 
         # nodes need to be removed in the correct order
-        rmnodes((compute.GcpNodeType, compute.GcpMachineType, compute.GcpDiskType, compute.GcpAcceleratorType))
-        rmnodes(billing.GcpSku)
-        rmnodes(billing.GcpService)
+        rm_nodes((compute.GcpNodeType, compute.GcpDiskType))
+        rm_nodes(compute.GcpMachineType, compute.GcpAcceleratorType)  # ignore accelerator types
+        rm_nodes(compute.GcpAcceleratorType)
+        rm_nodes(billing.GcpSku)
+        rm_nodes(billing.GcpService)
 
     def collect_region(self, region: GcpRegion, regional_builder: GraphBuilder) -> None:
         # fetch all region level resources
         for resource_class in all_resources:
             if not self.config.should_collect(resource_class.kind):
                 continue
             if resource_class.api_spec and not resource_class.api_spec.is_project_level:
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/gcp_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Optional, List, Dict, Any, Set
+from typing import Optional, List, Dict, Any, Set, Tuple
 
 from attr import define, evolve
 from google.auth.credentials import Credentials
 from googleapiclient import discovery
 
 from resoto_plugin_gcp.utils import MemoryCache
 from resotolib.core.actions import CoreFeedback
@@ -156,19 +156,19 @@
         params = {k: v.format_map(params_map) for k, v in api_spec.request_parameter.items()}
         result: List[Json] = []
 
         def next_responses(request: Any) -> None:
             response = request.execute()
             page = value_in_path(response, api_spec.response_path)
             if (sub_path := api_spec.response_regional_sub_path) is not None and isinstance(page, dict):
-                for zone_marker, zone_response in page.items():
-                    zone = zone_marker.split("/")[-1]
-                    for item in value_in_path(zone_response, sub_path) or []:
+                for zonal_marker, zonal_response in page.items():
+                    zone_prop, zonal_name = self.__extract_zonal_prop(zonal_marker)
+                    for item in value_in_path(zonal_response, sub_path) or []:
                         # store the zone as part of the item
-                        item[InternalZoneProp] = zone
+                        item[zone_prop] = zonal_name
                         result.append(item)
             elif isinstance(page, list):
                 result.extend(page)
             elif page is None:
                 pass
             else:
                 raise ValueError(f"Unexpected response type: {type(page)}")
@@ -176,7 +176,21 @@
             if hasattr(executor, api_spec.next_action) and (
                 nxt_req := getattr(executor, api_spec.next_action)(previous_request=request, previous_response=response)
             ):
                 return next_responses(nxt_req)
 
         next_responses(getattr(executor, api_spec.action)(**params))
         return result
+
+    @staticmethod
+    def __extract_zonal_prop(name: str) -> Tuple[str, str]:
+        if name == "global":
+            return RegionProp, name
+        if "/" not in name:
+            raise ValueError(f"Unexpected zonal name: {name}")
+        zonal_kind, zonal_name = name.split("/", maxsplit=1)
+        if zonal_kind == "regions":
+            return RegionProp, zonal_name
+        elif zonal_kind == "zones":
+            return InternalZoneProp, zonal_name
+        else:
+            raise ValueError(f"Unexpected zonal kind: {zonal_kind}")
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from __future__ import annotations
 
-import json
 import concurrent
+import json
 import logging
 from concurrent.futures import Executor, Future
 from threading import Lock
-from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict, Set
 from types import TracebackType
+from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict, Set
 
 from attr import define, field
 from google.auth.credentials import Credentials as GoogleAuthCredentials
 from googleapiclient.errors import HttpError
 
 from resoto_plugin_gcp.gcp_client import GcpClient, GcpApiSpec, InternalZoneProp, RegionProp
 from resoto_plugin_gcp.utils import Credentials
 from resotolib.baseresources import (
     BaseResource,
     BaseAccount,
     Cloud,
     EdgeType,
     BaseRegion,
     BaseZone,
-    BaseQuota,
     ModelReference,
 )
+from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, EdgeKey
 from resotolib.json import from_json as from_js, value_in_path
-from resotolib.json_bender import bend, Bender, S, Bend
+from resotolib.json_bender import bend, Bender, S, Bend, MapDict, F
 from resotolib.types import Json
-from resotolib.config import Config
-
 
 log = logging.getLogger("resoto.plugins.gcp")
 
 
 T = TypeVar("T")
 
 
@@ -191,59 +189,62 @@
         return result
 
     def add_node(self, node: GcpResourceType, source: Optional[Json] = None) -> Optional[GcpResourceType]:
         log.debug(f"{self.name}: add node {node}")
         node._cloud = self.cloud
         node._account = self.project
 
-        self._standard_edges(node, source)
-
-        with self.graph_nodes_access:
-            self.graph.add_node(node, source=source or {})
-        return node
+        if self._standard_edges(node, source):
+            with self.graph_nodes_access:
+                self.graph.add_node(node, source=source or {})
+            return node
+        return None
 
-    def _standard_edges(self, node: GcpResourceType, source: Optional[Json] = None) -> None:
+    def _standard_edges(self, node: GcpResourceType, source: Optional[Json] = None) -> bool:
         if isinstance(node, GcpRegion):
             self.add_edge(node, node=self.project, reverse=True)
-            return
+            return True
         if node._zone:
             self.add_edge(node, node=node._zone, reverse=True)
-            return
+            return True
         if node._region:
             self.add_edge(node, node=node._region, reverse=True)
-            return
+            return True
 
         if source is not None:
             if InternalZoneProp in source:
                 if zone := self.zone_by_name.get(source[InternalZoneProp]):
                     node._zone = zone
                     node._region = self.region_by_zone_name[source[InternalZoneProp]]
                     self.add_edge(node, node=zone, reverse=True)
-                    return
+                    return True
                 else:
-                    log.debug(f"Zone {source[InternalZoneProp]} not found for node: {node}.")
+                    log.debug(f"Zone {source[InternalZoneProp]} not found for node: {node}. Ignore resource.")
+                    return False
 
             if RegionProp in source:
                 region_name = source[RegionProp].rsplit("/", 1)[-1]
                 if region := self.region_by_name.get(region_name):
                     node._region = region
                     self.add_edge(node, node=region, reverse=True)
-                    return
+                    return True
                 else:
-                    log.debug(f"Region {region_name} not found for node: {node}.")
+                    log.debug(f"Region {region_name} not found for node: {node}. Ignore resource.")
+                    return False
 
         # Fallback to GraphBuilder region, i.e. regional collection
         if self.region is not None:
             node._region = self.region
             self.add_edge(node, node=self.region, reverse=True)
-            return
+            return True
 
         # Fallback to global region
+        node._region = self.fallback_global_region
         self.add_edge(node, node=self.fallback_global_region, reverse=True)
-        return
+        return True
 
     def add_edge(
         self,
         from_node: BaseResource,
         edge_type: EdgeType = EdgeType.default,
         reverse: bool = False,
         filter: Optional[Callable[[Any], bool]] = None,
@@ -391,18 +392,25 @@
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         """
         Hook method which is called when all resources have been collected.
         Connect the resource to other resources in the graph.
         """
         pass
 
+    def post_process_instance(self, builder: GraphBuilder, source: Json) -> None:
+        """
+        Hook method to post process the resource after all connections are done.
+        Default: do nothing.
+        """
+        pass
+
     @classmethod
     def collect_resources(cls: Type[GcpResource], builder: GraphBuilder, **kwargs: Any) -> List[GcpResource]:
         # Default behavior: in case the class has an ApiSpec, call the api and call collect.
-        log.info(f"[Gcp:{builder.project.id}] Collecting {cls.__name__} with ({kwargs})")
+        log.debug(f"[Gcp:{builder.project.id}] Collecting {cls.__name__} with ({kwargs})")
         if spec := cls.api_spec:
             expected_errors = GcpExpectedErrorCodes | (spec.expected_errors or set())
             with GcpErrorHandler(builder.core_feedback, expected_errors, f" in {builder.project.id} kind {cls.kind}"):
                 items = builder.client.list(spec, **kwargs)
                 return cls.collect(items, builder)
         return []
 
@@ -477,25 +485,39 @@
     deprecated: Optional[str] = field(default=None)
     obsolete: Optional[str] = field(default=None)
     replacement: Optional[str] = field(default=None)
     state: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class GcpQuota(GcpResource, BaseQuota):
+class GcpLimit:
     kind: ClassVar[str] = "gcp_quota"
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("metric"),
         "limit": S("limit"),
-        "owner": S("owner"),
         "usage": S("usage"),
+        "percentage": F(lambda x: round(x.get("usage", 0) / max(x.get("limit", 1), 1) * 100, 2)),
     }
     limit: Optional[float] = field(default=None)
-    owner: Optional[str] = field(default=None)
     usage: Optional[float] = field(default=None)
+    percentage: Optional[float] = field(default=None)
+
+
+@define(eq=False, slots=False)
+class GcpRegionQuota(GcpResource):
+    kind: ClassVar[str] = "gcp_region_quota"
+    mapping: ClassVar[Dict[str, Bender]] = {
+        "id": S("name").or_else(S("id")).or_else(S("selfLink")),
+        "name": S("name"),
+        "ctime": S("creationTimestamp"),
+        "link": S("selfLink"),
+        "label_fingerprint": S("labelFingerprint"),
+        "description": S("description"),
+        "quotas": S("quotas", default=[]) >> MapDict(S("metric") >> F(lambda x: x.lower()), Bend(GcpLimit.mapping)),
+    }
+    quotas: Optional[Dict[str, GcpLimit]] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpRegion(GcpResource, BaseRegion):
     kind: ClassVar[str] = "gcp_region"
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
         service="compute",
@@ -525,18 +547,17 @@
     region_supports_pzs: Optional[bool] = field(default=None)
 
     @classmethod
     def fallback_global_region(cls: Type[GcpRegion], project: GcpProject) -> GcpRegion:
         return cls(id="global", tags={}, name="global", account=project)
 
     def post_process(self, graph_builder: GraphBuilder, source: Json) -> None:
-        for quota_js in source.get("quotas", []):
-            quota = GcpQuota.from_api(quota_js)
-            quota._region = self
-            graph_builder.add_node(quota, quota_js)
+        region_quota = GcpRegionQuota.from_api(source)
+        graph_builder.add_node(region_quota, source)
+        graph_builder.add_edge(self, node=region_quota)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         for zone_link in source.get("zones", []):
             builder.add_edge(self, clazz=GcpZone, link=zone_link)
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
     resource_group_map: ClassVar[Dict[str, str]] = {
         "local-ssd": "LocalSSD",
         "pd-balanced": "SSD",
         "pd-ssd": "SSD",
         "pd-standard": "PDStandard",
     }
 
-    def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
+    def post_process_instance(self, builder: GraphBuilder, source: Json) -> None:
         """Adds edges from disk_types type to SKUs and determines ondemand pricing"""
         if not self.name:
             return
 
         log.debug((f"Looking up pricing for {self.rtdname} in {self.region().rtdname}"))
         resource_group = self.resource_group_map.get(self.name)
 
@@ -3417,15 +3417,17 @@
                 return False
         return True
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         # Add edge from machine type to accelerator type
         for at in self.accelerators or []:
             # The accelerator type resource name, not a full URL, e.g. nvidia-tesla-t4.
-            builder.add_edge(self, clazz=GcpAcceleratorType, id=at.guest_accelerator_type)
+            builder.add_edge(self, clazz=GcpAcceleratorType, id=at.guest_accelerator_type, reverse=True)
+
+    def post_process_instance(self, builder: GraphBuilder, source: Json) -> None:
         # Adds edges from machine type to SKUs and determines ondemand pricing
         if not self.name:
             return
 
         def filter(sku: GcpSku) -> bool:
             if not self.name or not self._region:
                 return False
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.3
+Version: 3.6.0
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.5.3/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/conftest.py` & `resoto-plugin-gcp-3.6.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/random_client.py` & `resoto-plugin-gcp-3.6.0/test/random_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 # random client: will not return any regions or zones
 PredefinedResults = {
     "compute.regions.list": {"id": "regions", "items": []},
     "compute.zones.list": {"id": "regions", "items": []},
 }
 # dictionary keys under .items (used for aggregated list zone result) -> return zone ids
-PredefinedDictKeys = {".items": [a.id for a in random_zones]}
+PredefinedDictKeys = {".items": [f"zones/{a.id}" for a in random_zones]}
 
 # type_name -> property_name -> callable that returns fixed value
 FixtureReplies: Dict[str, Dict[str, Callable[[], JsonElement]]] = {}
 
 # type_name -> property_name -> parameter_name
 Overrides: Dict[str, Dict[str, str]] = {}
```

### Comparing `resoto-plugin-gcp-3.5.3/test/test_base.py` & `resoto-plugin-gcp-3.6.0/test/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,12 @@
     assert len(nodes) == 7
 
 
 def test_gcp_region_collects_quotas(random_builder: GraphBuilder) -> None:
     with open(os.path.dirname(__file__) + "/files/gcp_regions.json") as f:
         GcpRegion.collect(raw=json.load(f)["items"], builder=random_builder)
 
-    assert len(random_builder.nodes(clazz=GcpQuota)) > 0
+    region_quotas = random_builder.nodes(clazz=GcpRegionQuota)
+    assert len(region_quotas) == 2  # 2 regions in the file
 
-    predecessor = list(random_builder.graph.predecessors(random_builder.node(clazz=GcpQuota)))[0]  # type: ignore
-    assert isinstance(predecessor, GcpRegion)
+    for predecessor in random_builder.graph.predecessors(region_quotas[0]):
+        assert isinstance(predecessor, GcpRegion)
```

### Comparing `resoto-plugin-gcp-3.5.3/test/test_billing.py` & `resoto-plugin-gcp-3.6.0/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/test_collector.py` & `resoto-plugin-gcp-3.6.0/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/test_compute.py` & `resoto-plugin-gcp-3.6.0/test/test_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,20 @@
 
 
 def test_disk_type_ondemand_cost(random_builder: GraphBuilder) -> None:
     known_prices_per_gig = [
         ("pd-standard", "us-east1", 0.08),
     ]
     with open(os.path.dirname(__file__) + "/files/skus.json") as f:
-        GcpSku.collect(raw=json.load(f)["skus"], builder=random_builder)
+        for r in GcpSku.collect(raw=json.load(f)["skus"], builder=random_builder):
+            r.post_process_instance(random_builder, {})
 
     with open(os.path.dirname(__file__) + "/files/disk_type.json") as f:
-        GcpDiskType.collect(raw=json.load(f)["items"]["diskTypes"], builder=random_builder)
+        for r in GcpDiskType.collect(raw=json.load(f)["items"]["diskTypes"], builder=random_builder):
+            r.post_process_instance(random_builder, {})
 
     regions = random_builder.resources_of(GcpRegion)
     disk_types = random_builder.resources_of(GcpDiskType)
 
     for price in known_prices_per_gig:
         region = next((obj for obj in regions if obj.id == price[1]), None)
         disk_type = next((obj for obj in disk_types if obj.name == price[0]), None)
@@ -187,15 +189,15 @@
     machine_types = random_builder.resources_of(GcpMachineType)
 
     for price in known_prices_linux_ondemand_hourly:
         region = next((obj for obj in regions if obj.id == price[1]), None)
         machine_type = next((obj for obj in machine_types if obj.name == price[0]), None)
         assert machine_type
         machine_type._region = region
-        machine_type.connect_in_graph(random_builder, {"Dummy": "Source"})
+        machine_type.post_process_instance(random_builder, {"Dummy": "Source"})
         assert machine_type.ondemand_cost
         assert round(machine_type.ondemand_cost, 5) == price[2]
 
 
 def test_gcp_interconnect_attachment(random_builder: GraphBuilder) -> None:
     roundtrip(GcpInterconnectAttachment, random_builder)
```

### Comparing `resoto-plugin-gcp-3.5.3/test/test_config.py` & `resoto-plugin-gcp-3.6.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/test_container.py` & `resoto-plugin-gcp-3.6.0/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.3/test/test_sqladmin.py` & `resoto-plugin-gcp-3.6.0/test/test_sqladmin.py`

 * *Files identical despite different names*

