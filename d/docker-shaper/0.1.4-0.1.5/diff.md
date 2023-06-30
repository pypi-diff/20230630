# Comparing `tmp/docker_shaper-0.1.4.tar.gz` & `tmp/docker_shaper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.4.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.5.tar", max compression
```

## Comparing `docker_shaper-0.1.4.tar` & `docker_shaper-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2298 2023-06-30 06:59:52.910235 docker_shaper-0.1.4/Readme.md
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/common.py
--rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0    18188 2023-06-30 09:17:28.289771 docker_shaper-0.1.4/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     6675 2023-06-30 07:36:14.166779 docker_shaper-0.1.4/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/static/bootstrap.css
--rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.4/docker_shaper/static/normalize.css
--rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.4/docker_shaper/static/pills.css
--rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.4/docker_shaper/static/style.css
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0      737 2023-06-30 09:18:56.813988 docker_shaper-0.1.4/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.4/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0      388 2023-06-30 07:37:58.639311 docker_shaper-0.1.4/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.4/docker_shaper/templates/images.html
--rw-r--r--   0        0        0     4641 2023-06-27 07:03:43.646288 docker_shaper-0.1.4/docker_shaper/utils.py
--rw-r--r--   0        0        0     2232 2023-06-30 09:23:23.086961 docker_shaper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 docker_shaper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2298 2023-06-30 06:59:52.910235 docker_shaper-0.1.5/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/common.py
+-rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0    19167 2023-06-30 14:42:40.587435 docker_shaper-0.1.5/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     7215 2023-06-30 13:27:56.721242 docker_shaper-0.1.5/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/static/bootstrap.css
+-rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.5/docker_shaper/static/normalize.css
+-rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.5/docker_shaper/static/pills.css
+-rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.5/docker_shaper/static/style.css
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-30 13:59:39.534821 docker_shaper-0.1.5/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.5/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0      378 2023-06-30 13:55:32.154530 docker_shaper-0.1.5/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.5/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0     4641 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2259 2023-06-30 14:43:03.363469 docker_shaper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 docker_shaper-0.1.5/PKG-INFO
```

### Comparing `docker_shaper-0.1.4/Readme.md` & `docker_shaper-0.1.5/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/cli.py` & `docker_shaper-0.1.5/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/dynamic.py` & `docker_shaper-0.1.5/docker_shaper/dynamic.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,27 +39,36 @@
     """Turn a number of seconds into something human readable"""
     if age is None:
         return "Unknown"
     return str(timedelta(seconds=int(age.total_seconds() if isinstance(age, timedelta) else age)))
 
 
 def date_str(date: datetime) -> str:
+    if not date:
+        return "--"
     return (datetime.fromtimestamp(date) if isinstance(date, int) else date).strftime(
         "%Y.%m.%d-%H:%M:%S"
     )
 
 
+from dateutil import tz
+
+
 def date_from(timestamp: str) -> datetime:
-    with suppress(ValueError):
+    if isinstance(timestamp, int):
+        datetime.fromtimestamp(timestamp)
+
+    if timestamp[-1] == "Z":
         return (
-            datetime.fromtimestamp(timestamp)
-            if isinstance(timestamp, int)
-            else datetime.strptime(timestamp[:26], "%Y-%m-%dT%H:%M:%S.%f")
+            datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
+            .replace(tzinfo=tz.tzutc())
+            .astimezone(tz.tzlocal())
         )
-    return None
+
+    return f"BAD: {timestamp}"
 
 
 def event_from(line: str):
     """Reads a line from event log and turns it into a tuple containing the data"""
     match = re.match(r"^(.*) \((.*)\)$", line)
     assert match, f"line did not match the expected format: {line!r}"
     cmd, params = match.groups()
@@ -229,15 +238,15 @@
     classes = ["table", "table-striped"]
 
     def __init__(self, endpoint, items):
         super().__init__(items)
         self.endpoint = endpoint
 
     def get_tr_attrs(self, item):
-        return {'class': item.get("class")}
+        return {"class": item.get("class")}
 
 
 class ImageTable(BaseTable):
     short_id = Col("short_id")
     tags = Col("tags")
     created_at = Col("created_at")
     last_referenced = Col("last_referenced")
@@ -269,15 +278,15 @@
                 (
                     {
                         "short_id": image["short_id"],
                         "tags": image["tags"],
                         "created_at": date_str(image["created_at"]),
                         "age": age_str(datetime.now() - date_from(image["created_at"])),
                         "last_referenced": last_referenced_str(image["short_id"]),
-                        "class": "text-danger",
+                        "class": "text-danger" if image.get("cleanup") else "text-success",
                     }
                     for image in global_state.images.values()
                 ),
                 key=lambda e: e[sort],
                 reverse=reverse,
             ),
         ).__html__()
@@ -286,15 +295,15 @@
 class ContainerTable(BaseTable):
     short_id = Col("short_id")
     name = Col("name")
     mem_usage = Col("mem_usage")
     cpu = Col("cpu")
     cmd = Col("cmd")
     job = Col("job")
-    created_at = Col("created_at")
+    # created_at = Col("created_at")
     started_at = Col("started_at")
     uptime = Col("uptime")
     status = Col("status")
     hints = Col("hints")
     pid = Col("pid")
     # link = LinkCol('Link', 'route_containers', url_kwargs=dict(id='id'), allow_sort=False)
 
@@ -303,36 +312,40 @@
             self.endpoint,
             sort_key_containers=col_key,
             sort_direction_containers="desc" if reverse else "asc",
         )
 
     @staticmethod
     def html_from(endpoint, global_state, sort, reverse):
+        now = datetime.now(tz=tz.tzutc())
         return ContainerTable(
             endpoint,
             items=sorted(
                 (
                     {
                         "short_id": cnt["short_id"],
                         "name": cnt["name"],
                         "mem_usage": mem_stats.get("usage", 0),
                         "cpu": cpu_perc(cpu_stats, last_cpu_stats),
                         "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
                         "job": jobname_from(
                             cnt["show"]["HostConfig"]["Binds"]
                             or list(cnt["show"]["Config"]["Volumes"] or [])
                         ),
-                        "created_at": date_str(date_from(cnt["show"]["Created"])),
-                        "started_at": date_str(date_from(cnt["show"]["State"]["StartedAt"])),
-                        "uptime": age_str(
-                            datetime.now() - date_from(cnt["show"]["State"]["StartedAt"])
+                        # "created_at": date_str(date_from(cnt["show"]["Created"])),
+                        # "created_at": cnt["show"]["Created"],
+                        "started_at": date_str(
+                            started_at := date_from(cnt["show"]["State"]["StartedAt"])
                         ),
+                        "uptime": age_str(now - started_at) if started_at else "--",
                         "status": cnt["show"]["State"]["Status"],
                         "hints": label_filter(cnt["show"]["Config"]["Labels"]),
                         "pid": int(cnt["show"]["State"]["Pid"]),
+                        # https://getbootstrap.com/docs/4.0/utilities/colors/
+                        "class": "text-danger" if cnt.get("cleanup") else "text-success",
                     }
                     for cnt, mem_stats, cpu_stats, last_cpu_stats in (
                         (
                             c,
                             c["stats"].get("memory_stats", {}),
                             c["stats"]["cpu_stats"],
                             c["last_stats"].get("cpu_stats"),
@@ -343,59 +356,57 @@
                 ),
                 key=lambda e: e[sort],
                 reverse=reverse,
             ),
         ).__html__()
 
 
+def meta_info(global_state):
+    return {
+        "refresh_interval": global_state.intervals.get("site_refresh", 10),
+        "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
+        "container_count": len(global_state.containers),
+        "image_count": len(global_state.images),
+        "extra_links": global_state.extra_links,
+        "intervals": global_state.intervals,
+    }
+
+
 async def container_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
-        meta={
-            "refresh_interval": 3,
-            "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
-            "container_count": len(global_state.containers),
-        },
+        meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_containers",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
             reverse=request.args.get("sort_direction_containers", "asc") == "desc",
         ),
     )
 
 
 async def image_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
-        meta={
-            "refresh_interval": 3,
-            "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
-            "image_count": len(global_state.images),
-        },
+        meta=meta_info(global_state),
         images_html=ImageTable.html_from(
             "route_images",
             global_state,
             sort=request.args.get("sort_key_images", "last_referenced"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
     )
 
 
 async def dashboard(global_state):
     return await render_template(
         "dashboard.html",
-        meta={
-            "refresh_interval": 3,
-            "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
-            "container_count": len(global_state.containers),
-            "image_count": len(global_state.images),
-        },
+        meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_dashboard",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
             reverse=request.args.get("sort_direction_containers", "asc") == "desc",
         ),
         images_html=ImageTable.html_from(
@@ -513,23 +524,50 @@
 
 async def watch_images(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl images..")
     for image in await docker_client.images.list(all=True):
         log().debug(image)
         if True or image["Id"] not in global_state.images:
-            global_state.images[image["Id"]] = {
-                "short_id": short_id(image["Id"]),
-                "created_at": image["Created"],
-                "tags": image["RepoTags"],
-                "size": image["Size"],
-                "parent": short_id(image["ParentId"]),
-            }
+            global_state.images.get(image["Id"], {}).update(
+                {
+                    "short_id": short_id(image["Id"]),
+                    "created_at": image["Created"],
+                    "tags": image["RepoTags"],
+                    "size": image["Size"],
+                    "parent": short_id(image["ParentId"]),
+                }
+            )
 
 
 async def watch_containers(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl containers..")
     for container in await docker_client.containers.list(all=True):
         if container.id not in global_state.containers:
             global_state.containers[container.id] = {}
             asyncio.ensure_future(watch_container(container, global_state.containers))
+
+
+def would_cleanup_container(container, global_state):
+    status = container["show"]["State"]["Status"]
+    if status in {"exited"}:
+        return True
+
+    return False
+
+
+def would_cleanup_image(image, global_state):
+    print(image)
+    return False
+
+
+async def cleanup(global_state):
+    log().info("Cleanup!..")
+
+    for container in global_state.containers.values():
+        container["cleanup"] = would_cleanup_container(container, global_state)
+
+    for image in global_state.images.values():
+        image["cleanup"] = would_cleanup_image(image, global_state)
+
+    log().info("Cleanup done!")
```

### Comparing `docker_shaper-0.1.4/docker_shaper/server.py` & `docker_shaper-0.1.5/docker_shaper/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,33 @@
     containers: MutableMapping[str, object]
 
     event_horizon: int
     last_referenced: MutableMapping[str, int]
 
     tag_rules: MutableMapping[str, int]
 
+    extra_links: MutableMapping[str, int]
+
     def __init__(self):
         self.intervals = {
             "state": 2,
             "image_stats": 2,
             "image_update": 2,
             "container_update": 2,
             "container_stats": 2,
+            "cleanup": 3600,
         }
         self.image_ids = {}
         self.images = {}
         self.containers = {}
         self.event_horizon = int(time.time())
         self.last_referenced = {}
         self.tag_rules = {}
         self.counter = 0
+        self.extra_links = {}
 
 
 @watchdog
 async def print_container_stats(global_state):
     while True:
         try:
             await dynamic.print_container_stats(global_state)
@@ -151,24 +155,36 @@
         try:
             await dynamic.handle_docker_event_line(global_state, line)
         except Exception:
             log().exception("Unhandled exception caught!")
             await asyncio.sleep(5)
 
 
+@watchdog
+async def cleanup(global_state):
+    while True:
+        try:
+            await dynamic.cleanup(global_state)
+            await asyncio.sleep(global_state.intervals.get("cleanup", 3600))
+        except Exception:
+            log().exception("Unhandled exception caught in cleanup()!")
+            await asyncio.sleep(5)
+
+
 def no_serve():
     global_state = GlobalState()
     load_config(CONFIG_FILE, global_state)
     with suppress(KeyboardInterrupt, BrokenPipeError):
         asyncio.ensure_future(watch_fs_changes(global_state))
         asyncio.ensure_future(print_container_stats(global_state))
         asyncio.ensure_future(print_state(global_state))
         asyncio.ensure_future(watch_containers(global_state))
         asyncio.ensure_future(watch_images(global_state))
         asyncio.ensure_future(handle_docker_events(global_state))
+        asyncio.ensure_future(cleanup(global_state))
         asyncio.get_event_loop().run_forever()
 
 
 def serve():
     """"""
     app = Quart(__name__)
     app.config["TEMPLATES_AUTO_RELOAD"] = True
@@ -206,14 +222,15 @@
         asyncio.ensure_future(self_destroy())
         asyncio.ensure_future(watch_fs_changes(global_state))
         # asyncio.ensure_future(print_container_stats(global_state))
         asyncio.ensure_future(print_state(global_state))
         asyncio.ensure_future(watch_containers(global_state))
         asyncio.ensure_future(watch_images(global_state))
         asyncio.ensure_future(handle_docker_events(global_state))
+        asyncio.ensure_future(cleanup(global_state))
 
     app.terminator = asyncio.Event()
     app.run(
         host="0.0.0.0",
         port=5432,
         debug=False,
         use_reloader=False,
```

### Comparing `docker_shaper-0.1.4/docker_shaper/static/bootstrap.css` & `docker_shaper-0.1.5/docker_shaper/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/static/normalize.css` & `docker_shaper-0.1.5/docker_shaper/static/normalize.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/static/pills.css` & `docker_shaper-0.1.5/docker_shaper/static/pills.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/static/style.css` & `docker_shaper-0.1.5/docker_shaper/static/style.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/docker_shaper/templates/base.html` & `docker_shaper-0.1.5/docker_shaper/templates/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,43 @@
   <head>
     <title>{{ title }}</title>
     <!--
     <link rel="stylesheet" href="{{ url_for('static', filename='normalize.css') }}">
     <link rel="stylesheet" href="{{ url_for('static', filename='style.css') }}">
     -->
     <link rel="stylesheet" href="{{ url_for('static', filename='bootstrap.css') }}">
-    <meta http-equiv="refresh" content="3" />
+    <meta http-equiv="refresh" content="{{ meta.refresh_interval }}" />
   </head>
 
   <body>
-    <table><tr>
+     <table class="table table-striped"><tr>
+      <td>Host: --</td>
+      <td></td>
+      {% for link in meta.extra_links %}
+          <td><a href="{{ meta.extra_links[link] }}">{{link}}</a></td>
+          <td></td>
+      {% endfor %}
+
+    </tr><tr>
+
+      {% for interval in meta.intervals %}
+          <td>{{interval}} = {{meta.intervals[interval]}}s  </td><td></td>
+      {% endfor %}
+
+    </tr><tr>
+
       <td><a href="/">Dashboard</a></td>
       <td></td>
       <td><a href="/containers">Containers</a></td>
       <td></td>
       <td><a href="/images">Images</a></td>
-      </tr></table>
+
+    </tr></table>
+
     <div class="dashboard">
       {% block content %}{% endblock %}
     </div>
+
     {% block scripts %}{% endblock %}
+
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
 
 
-Dashboard  Containers  Images
+Host: --                                      {{link}}
+{{interval}} = {{meta.intervals[interval]}}s
+Dashboard                                     Containers  Images
 {% block content %}{% endblock %}
 {% block scripts %}{% endblock %}
```

### Comparing `docker_shaper-0.1.4/docker_shaper/utils.py` & `docker_shaper-0.1.5/docker_shaper/utils.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.4/pyproject.toml` & `docker_shaper-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.4"
+version = "0.1.5"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
@@ -16,14 +16,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 aiodocker = "^0.21.0"
 asyncinotify = "^4.0.1"
 quart = "^0.18.4"
 flask-table = "^0.5.0"
+python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `docker_shaper-0.1.4/PKG-INFO` & `docker_shaper-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.4
+Version: 0.1.5
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
 Requires-Dist: flask-table (>=0.5.0,<0.6.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: quart (>=0.18.4,<0.19.0)
 Project-URL: Repository, https://github.com/Checkmk/checkmk-dev-tools
 Description-Content-Type: text/markdown
 
 # Docker Shaper
 
 This repository includes scripts/tools for Checkmk developers.
```

