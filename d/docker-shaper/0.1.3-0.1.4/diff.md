# Comparing `tmp/docker_shaper-0.1.3.tar.gz` & `tmp/docker_shaper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.3.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.4.tar", max compression
```

## Comparing `docker_shaper-0.1.3.tar` & `docker_shaper-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     2299 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/Readme.md
--rw-r--r--   0        0        0        0 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/common.py
--rw-r--r--   0        0        0        1 2023-06-26 12:05:10.251336 docker_shaper-0.1.3/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0    13194 2023-06-26 15:22:16.795198 docker_shaper-0.1.3/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     6488 2023-06-26 14:51:02.321955 docker_shaper-0.1.3/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-06-26 15:27:42.516049 docker_shaper-0.1.3/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-06-23 06:50:12.242199 docker_shaper-0.1.3/docker_shaper/static/base.css
--rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.3/docker_shaper/static/normalize.css
--rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.3/docker_shaper/static/pills.css
--rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.3/docker_shaper/static/style.css
--rw-r--r--   0        0        0        0 2023-06-26 15:27:53.160076 docker_shaper-0.1.3/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0      528 2023-06-26 15:29:05.292266 docker_shaper-0.1.3/docker_shaper/templates/base.html
--rw-r--r--   0        0        0     1749 2023-06-26 15:18:56.202659 docker_shaper-0.1.3/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0     4641 2023-06-26 14:51:01.673953 docker_shaper-0.1.3/docker_shaper/utils.py
--rw-r--r--   0        0        0     2209 2023-06-26 15:29:39.828358 docker_shaper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 docker_shaper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2298 2023-06-30 06:59:52.910235 docker_shaper-0.1.4/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/common.py
+-rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0    18188 2023-06-30 09:17:28.289771 docker_shaper-0.1.4/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     6675 2023-06-30 07:36:14.166779 docker_shaper-0.1.4/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/static/bootstrap.css
+-rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.4/docker_shaper/static/normalize.css
+-rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.4/docker_shaper/static/pills.css
+-rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.4/docker_shaper/static/style.css
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0      737 2023-06-30 09:18:56.813988 docker_shaper-0.1.4/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.4/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0      388 2023-06-30 07:37:58.639311 docker_shaper-0.1.4/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.4/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0     4641 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2232 2023-06-30 09:23:23.086961 docker_shaper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 docker_shaper-0.1.4/PKG-INFO
```

### Comparing `docker_shaper-0.1.3/Readme.md` & `docker_shaper-0.1.4/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 ## Development & Contribution
 
 ### Todo
 
 - [x] pip package
 - [x] Quart interface
-- [ ] bring in dockermon
-- [ ] auto update
+- [x] bring in dockermon
+- [x] auto update
+- [x] outsource config
 - [ ] bring in dgcd
 - [ ] bring in list_volumes
-- [ ] outsource config
-- [ ] 	increase/decrease logging
+- [ ] increase/decrease logging
 - [ ] new: untag certain tags
 - [ ] new: container cleanup
 
 
 ### Setup
 
 ### Prerequisites
```

### Comparing `docker_shaper-0.1.3/docker_shaper/cli.py` & `docker_shaper-0.1.4/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/docker_shaper/dynamic.py` & `docker_shaper-0.1.4/docker_shaper/dynamic.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import time
 from contextlib import suppress
 from datetime import datetime, timedelta
 from subprocess import CalledProcessError
 from typing import MutableMapping, Optional
 
 from aiodocker import DockerError
-from quart import render_template
+from flask_table import Col, Table
+from quart import render_template, request, url_for
 
 from docker_shaper.utils import process_output, watchdog
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.dynamic")
@@ -30,24 +31,34 @@
     """
     if not docker_id:
         return docker_id
     assert docker_id.startswith("sha256:")
     return docker_id[7:17]
 
 
-def age_str(seconds: Optional[int]) -> str:
+def age_str(age: Optional[int]) -> str:
     """Turn a number of seconds into something human readable"""
-    if seconds is None:
+    if age is None:
         return "Unknown"
-    return str(timedelta(seconds=seconds))
+    return str(timedelta(seconds=int(age.total_seconds() if isinstance(age, timedelta) else age)))
 
 
-def timestamp_from(string):
+def date_str(date: datetime) -> str:
+    return (datetime.fromtimestamp(date) if isinstance(date, int) else date).strftime(
+        "%Y.%m.%d-%H:%M:%S"
+    )
+
+
+def date_from(timestamp: str) -> datetime:
     with suppress(ValueError):
-        return datetime.strptime(string[:26], "%Y-%m-%dT%H:%M:%S.%f")
+        return (
+            datetime.fromtimestamp(timestamp)
+            if isinstance(timestamp, int)
+            else datetime.strptime(timestamp[:26], "%Y-%m-%dT%H:%M:%S.%f")
+        )
     return None
 
 
 def event_from(line: str):
     """Reads a line from event log and turns it into a tuple containing the data"""
     match = re.match(r"^(.*) \((.*)\)$", line)
     assert match, f"line did not match the expected format: {line!r}"
@@ -209,59 +220,194 @@
     print(global_state.intervals)
     print(f"counter: {global_state.counter}")
     print(f"images: {len(global_state.images)}")
     print(f"containers: {len(global_state.containers)}")
     print(f"tag_rules: {len(global_state.tag_rules)}")
 
 
+class BaseTable(Table):
+    allow_sort = True
+    classes = ["table", "table-striped"]
+
+    def __init__(self, endpoint, items):
+        super().__init__(items)
+        self.endpoint = endpoint
+
+    def get_tr_attrs(self, item):
+        return {'class': item.get("class")}
+
+
+class ImageTable(BaseTable):
+    short_id = Col("short_id")
+    tags = Col("tags")
+    created_at = Col("created_at")
+    last_referenced = Col("last_referenced")
+
+    def sort_url(self, col_key, reverse=False):
+        return url_for(
+            self.endpoint,
+            sort_key_images=col_key,
+            sort_direction_images="desc" if reverse else "asc",
+        )
+
+    @staticmethod
+    def html_from(endpoint, global_state, sort, reverse):
+        # - max(
+        # referenced.get(image_id, 0),
+        # GLOBALS["EVENT_HORIZON"],
+        # datetime.strptime(
+        # docker_images.get(image_id).attrs["Created"][:19], "%Y-%m-%dT%H:%M:%S"
+        # ).timestamp(),
+        # ),
+        def last_referenced_str(image_id):
+            if ref := global_state.last_referenced.get(image_id):
+                return age_str(time.time() - ref)
+            return "??"
+
+        return ImageTable(
+            endpoint,
+            items=sorted(
+                (
+                    {
+                        "short_id": image["short_id"],
+                        "tags": image["tags"],
+                        "created_at": date_str(image["created_at"]),
+                        "age": age_str(datetime.now() - date_from(image["created_at"])),
+                        "last_referenced": last_referenced_str(image["short_id"]),
+                        "class": "text-danger",
+                    }
+                    for image in global_state.images.values()
+                ),
+                key=lambda e: e[sort],
+                reverse=reverse,
+            ),
+        ).__html__()
+
+
+class ContainerTable(BaseTable):
+    short_id = Col("short_id")
+    name = Col("name")
+    mem_usage = Col("mem_usage")
+    cpu = Col("cpu")
+    cmd = Col("cmd")
+    job = Col("job")
+    created_at = Col("created_at")
+    started_at = Col("started_at")
+    uptime = Col("uptime")
+    status = Col("status")
+    hints = Col("hints")
+    pid = Col("pid")
+    # link = LinkCol('Link', 'route_containers', url_kwargs=dict(id='id'), allow_sort=False)
+
+    def sort_url(self, col_key, reverse=False):
+        return url_for(
+            self.endpoint,
+            sort_key_containers=col_key,
+            sort_direction_containers="desc" if reverse else "asc",
+        )
+
+    @staticmethod
+    def html_from(endpoint, global_state, sort, reverse):
+        return ContainerTable(
+            endpoint,
+            items=sorted(
+                (
+                    {
+                        "short_id": cnt["short_id"],
+                        "name": cnt["name"],
+                        "mem_usage": mem_stats.get("usage", 0),
+                        "cpu": cpu_perc(cpu_stats, last_cpu_stats),
+                        "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
+                        "job": jobname_from(
+                            cnt["show"]["HostConfig"]["Binds"]
+                            or list(cnt["show"]["Config"]["Volumes"] or [])
+                        ),
+                        "created_at": date_str(date_from(cnt["show"]["Created"])),
+                        "started_at": date_str(date_from(cnt["show"]["State"]["StartedAt"])),
+                        "uptime": age_str(
+                            datetime.now() - date_from(cnt["show"]["State"]["StartedAt"])
+                        ),
+                        "status": cnt["show"]["State"]["Status"],
+                        "hints": label_filter(cnt["show"]["Config"]["Labels"]),
+                        "pid": int(cnt["show"]["State"]["Pid"]),
+                    }
+                    for cnt, mem_stats, cpu_stats, last_cpu_stats in (
+                        (
+                            c,
+                            c["stats"].get("memory_stats", {}),
+                            c["stats"]["cpu_stats"],
+                            c["last_stats"].get("cpu_stats"),
+                        )
+                        for c in global_state.containers.values()
+                        if c.keys() > {"short_id", "name", "stats"}
+                    )
+                ),
+                key=lambda e: e[sort],
+                reverse=reverse,
+            ),
+        ).__html__()
+
+
+async def container_table_html(global_state):
+    # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
+    return await render_template(
+        "containers.html",
+        meta={
+            "refresh_interval": 3,
+            "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
+            "container_count": len(global_state.containers),
+        },
+        containers_html=ContainerTable.html_from(
+            "route_containers",
+            global_state,
+            sort=request.args.get("sort_key_containers", "cpu"),
+            reverse=request.args.get("sort_direction_containers", "asc") == "desc",
+        ),
+    )
+
+
+async def image_table_html(global_state):
+    # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
+    return await render_template(
+        "containers.html",
+        meta={
+            "refresh_interval": 3,
+            "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
+            "image_count": len(global_state.images),
+        },
+        images_html=ImageTable.html_from(
+            "route_images",
+            global_state,
+            sort=request.args.get("sort_key_images", "last_referenced"),
+            reverse=request.args.get("sort_direction_images", "asc") == "desc",
+        ),
+    )
+
+
 async def dashboard(global_state):
     return await render_template(
         "dashboard.html",
-        data={
+        meta={
             "refresh_interval": 3,
             "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
-            "containers": [
-                {
-                    "short_id": cnt["short_id"],
-                    "name": cnt["name"],
-                    "usage": mem_stats.get("usage", 0),
-                    "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
-                    "job": jobname_from(
-                        cnt["show"]["HostConfig"]["Binds"]
-                        or list(cnt["show"]["Config"]["Volumes"] or [])
-                    ),
-                    "cpu": cpu_perc(cpu_stats, last_cpu_stats),
-                    "created_at": timestamp_from(cnt["show"]["Created"]),
-                    "started_at": timestamp_from(cnt["show"]["State"]["StartedAt"]),
-                    "status": cnt["show"]["State"]["Status"],
-                    "hints": label_filter(cnt["show"]["Config"]["Labels"]),
-                    "pid": int(cnt["show"]["State"]["Pid"]),
-                    # "container": cnt["container"],
-                }
-                for cnt, mem_stats, cpu_stats, last_cpu_stats in (
-                    (
-                        c,
-                        c["stats"].get("memory_stats", {}),
-                        c["stats"]["cpu_stats"],
-                        c["last_stats"].get("cpu_stats"),
-                    )
-                    for c in global_state.containers.values()
-                    if c.keys() > {"short_id", "name", "stats"}
-                )
-            ],
-            "images": [
-                {
-                    "short_id": image["short_id"],
-                    "tags": image["tags"],
-                    "created_at": image["created_at"],
-                    "last_referenced": "abc",  # timestamp_from(cnt["show"]["Created"]),
-                }
-                for image in global_state.images.values()
-            ],
+            "container_count": len(global_state.containers),
+            "image_count": len(global_state.images),
         },
+        containers_html=ContainerTable.html_from(
+            "route_dashboard",
+            global_state,
+            sort=request.args.get("sort_key_containers", "cpu"),
+            reverse=request.args.get("sort_direction_containers", "asc") == "desc",
+        ),
+        images_html=ImageTable.html_from(
+            "route_dashboard",
+            global_state,
+            sort=request.args.get("sort_key_images", "last_referenced"),
+            reverse=request.args.get("sort_direction_images", "asc") == "desc",
+        ),
     )
 
 
 async def print_container_stats(global_state):
     hostname = open("/etc/hostname").read().strip()
     stats = [
         {
@@ -269,16 +415,16 @@
             "name": cnt["name"],
             "usage": mem_stats.get("usage", 0),
             "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
             "job": jobname_from(
                 cnt["show"]["HostConfig"]["Binds"] or list(cnt["show"]["Config"]["Volumes"] or [])
             ),
             "cpu": cpu_perc(cpu_stats, last_cpu_stats),
-            "created_at": timestamp_from(cnt["show"]["Created"]),
-            "started_at": timestamp_from(cnt["show"]["State"]["StartedAt"]),
+            "created_at": date_from(cnt["show"]["Created"]),
+            "started_at": date_from(cnt["show"]["State"]["StartedAt"]),
             "status": cnt["show"]["State"]["Status"],
             "hints": label_filter(cnt["show"]["Config"]["Labels"]),
             "pid": int(cnt["show"]["State"]["Pid"]),
             "container": cnt["container"],
         }
         for cnt, mem_stats, cpu_stats, last_cpu_stats in (
             (
```

### Comparing `docker_shaper-0.1.3/docker_shaper/server.py` & `docker_shaper-0.1.4/docker_shaper/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #!/usr/bin/env python3
 
 import asyncio
 import importlib
 import logging
-import os
 import time
 from contextlib import suppress
 from dataclasses import dataclass
-from datetime import datetime
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from typing import MutableMapping
 
 from aiodocker import Docker
 from quart import Quart
@@ -174,29 +172,37 @@
     """"""
     app = Quart(__name__)
     app.config["TEMPLATES_AUTO_RELOAD"] = True
 
     global_state = GlobalState()
     load_config(CONFIG_FILE, global_state)
 
-    @app.route("/shutdown")  # , methods=['POST'])
-    def shutdown():
-        app.terminator.set()
-        return "Server shutting down..."
-
     @watchdog
     async def self_destroy():
         await app.terminator.wait()
         print("BOOM")
         app.shutdown()
         asyncio.get_event_loop().stop()
         print("!!!!")
 
-    @app.route("/", methods=["GET", "POST"])
-    async def dashboard():
+    @app.route("/shutdown")
+    def route_shutdown():
+        app.terminator.set()
+        return "Server shutting down..."
+
+    @app.route("/containers")
+    async def route_containers():
+        return await dynamic.container_table_html(global_state)
+
+    @app.route("/images")
+    async def route_images():
+        return await dynamic.image_table_html(global_state)
+
+    @app.route("/", methods=["GET"])
+    async def route_dashboard():
         return await dynamic.dashboard(global_state)
 
     @app.before_serving
     async def create_db_pool():
         asyncio.ensure_future(self_destroy())
         asyncio.ensure_future(watch_fs_changes(global_state))
         # asyncio.ensure_future(print_container_stats(global_state))
```

### Comparing `docker_shaper-0.1.3/docker_shaper/static/base.css` & `docker_shaper-0.1.4/docker_shaper/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/docker_shaper/static/normalize.css` & `docker_shaper-0.1.4/docker_shaper/static/normalize.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/docker_shaper/static/pills.css` & `docker_shaper-0.1.4/docker_shaper/static/pills.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/docker_shaper/static/style.css` & `docker_shaper-0.1.4/docker_shaper/static/style.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/docker_shaper/utils.py` & `docker_shaper-0.1.4/docker_shaper/utils.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.3/pyproject.toml` & `docker_shaper-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.3"
+version = "0.1.4"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
@@ -15,14 +15,15 @@
 docker-shaper = 'docker_shaper.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 aiodocker = "^0.21.0"
 asyncinotify = "^4.0.1"
 quart = "^0.18.4"
+flask-table = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `docker_shaper-0.1.3/PKG-INFO` & `docker_shaper-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
+Requires-Dist: flask-table (>=0.5.0,<0.6.0)
 Requires-Dist: quart (>=0.18.4,<0.19.0)
 Project-URL: Repository, https://github.com/Checkmk/checkmk-dev-tools
 Description-Content-Type: text/markdown
 
 # Docker Shaper
 
 This repository includes scripts/tools for Checkmk developers.
@@ -36,20 +37,20 @@
 
 ## Development & Contribution
 
 ### Todo
 
 - [x] pip package
 - [x] Quart interface
-- [ ] bring in dockermon
-- [ ] auto update
+- [x] bring in dockermon
+- [x] auto update
+- [x] outsource config
 - [ ] bring in dgcd
 - [ ] bring in list_volumes
-- [ ] outsource config
-- [ ] 	increase/decrease logging
+- [ ] increase/decrease logging
 - [ ] new: untag certain tags
 - [ ] new: container cleanup
 
 
 ### Setup
 
 ### Prerequisites
```

