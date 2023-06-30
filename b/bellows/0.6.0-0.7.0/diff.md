# Comparing `tmp/bellows-0.6.0.tar.gz` & `tmp/bellows-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bellows-0.6.0.tar", last modified: Sun May  6 00:09:37 2018, max compression
+gzip compressed data, was "dist/bellows-0.7.0.tar", last modified: Tue Sep  4 01:44:33 2018, max compression
```

## Comparing `bellows-0.6.0.tar` & `bellows-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/
--rw-r--r--   0 russell   (1000) hass       (999)       65 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/requires.txt
--rw-r--r--   0 russell   (1000) hass       (999)      240 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/PKG-INFO
--rw-r--r--   0 russell   (1000) hass       (999)        8 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/top_level.txt
--rw-r--r--   0 russell   (1000) hass       (999)      115 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/dependency_links.txt
--rw-r--r--   0 russell   (1000) hass       (999)      617 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/SOURCES.txt
--rw-r--r--   0 russell   (1000) hass       (999)       51 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows.egg-info/entry_points.txt
--rw-rw-r--   0 russell   (1000) russell   (1000)      240 2018-05-06 00:09:37.000000 bellows-0.6.0/PKG-INFO
--rw-rw-r--   0 russell   (1000) russell   (1000)      793 2018-05-06 00:09:33.000000 bellows-0.6.0/setup.py
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows/
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows/cli/
--rw-rw-r--   0 russell   (1000) russell   (1000)     1470 2018-02-27 00:54:10.000000 bellows-0.6.0/bellows/cli/opts.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     5643 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/cli/util.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     1927 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/cli/dump.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     9483 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/cli/application.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     2460 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/cli/ncp.py
--rw-rw-r--   0 russell   (1000) russell   (1000)      100 2017-09-05 04:27:19.000000 bellows-0.6.0/bellows/cli/__init__.py
--rw-rw-r--   0 russell   (1000) russell   (1000)      344 2017-10-15 19:02:22.000000 bellows-0.6.0/bellows/cli/main.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     4735 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/cli/network.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     8904 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/uart.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     5876 2018-04-29 20:12:31.000000 bellows-0.6.0/bellows/ezsp.py
--rw-rw-r--   0 russell   (1000) russell   (1000)    19286 2017-07-26 00:51:52.000000 bellows-0.6.0/bellows/commands.py
--rw-rw-r--   0 russell   (1000) russell   (1000)        0 2017-01-10 02:34:40.000000 bellows-0.6.0/bellows/__init__.py
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows/zigbee/
--rw-rw-r--   0 russell   (1000) russell   (1000)     1134 2018-02-19 00:16:29.000000 bellows-0.6.0/bellows/zigbee/util.py
--rw-rw-r--   0 russell   (1000) russell   (1000)    10988 2018-05-05 23:57:16.000000 bellows-0.6.0/bellows/zigbee/application.py
--rw-rw-r--   0 russell   (1000) russell   (1000)        0 2017-02-05 17:48:19.000000 bellows-0.6.0/bellows/zigbee/__init__.py
-drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-05-06 00:09:37.000000 bellows-0.6.0/bellows/types/
--rw-rw-r--   0 russell   (1000) russell   (1000)    21637 2017-07-26 00:51:52.000000 bellows-0.6.0/bellows/types/struct.py
--rw-rw-r--   0 russell   (1000) russell   (1000)    76194 2018-02-19 00:16:29.000000 bellows-0.6.0/bellows/types/named.py
--rw-rw-r--   0 russell   (1000) russell   (1000)     2943 2018-02-19 00:16:29.000000 bellows-0.6.0/bellows/types/basic.py
--rw-rw-r--   0 russell   (1000) russell   (1000)      393 2017-02-05 17:48:19.000000 bellows-0.6.0/bellows/types/__init__.py
--rw-rw-r--   0 russell   (1000) russell   (1000)       59 2018-05-06 00:09:37.000000 bellows-0.6.0/setup.cfg
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows.egg-info/
+-rw-r--r--   0 russell   (1000) hass       (999)       65 2018-09-04 01:44:32.000000 bellows-0.7.0/bellows.egg-info/requires.txt
+-rw-r--r--   0 russell   (1000) hass       (999)      240 2018-09-04 01:44:32.000000 bellows-0.7.0/bellows.egg-info/PKG-INFO
+-rw-r--r--   0 russell   (1000) hass       (999)        8 2018-09-04 01:44:32.000000 bellows-0.7.0/bellows.egg-info/top_level.txt
+-rw-r--r--   0 russell   (1000) hass       (999)      115 2018-09-04 01:44:32.000000 bellows-0.7.0/bellows.egg-info/dependency_links.txt
+-rw-r--r--   0 russell   (1000) hass       (999)      617 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows.egg-info/SOURCES.txt
+-rw-r--r--   0 russell   (1000) hass       (999)       51 2018-09-04 01:44:32.000000 bellows-0.7.0/bellows.egg-info/entry_points.txt
+-rw-rw-r--   0 russell   (1000) russell   (1000)      240 2018-09-04 01:44:33.000000 bellows-0.7.0/PKG-INFO
+-rw-rw-r--   0 russell   (1000) russell   (1000)      793 2018-09-04 01:35:56.000000 bellows-0.7.0/setup.py
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows/
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows/cli/
+-rw-rw-r--   0 russell   (1000) russell   (1000)     1470 2018-02-27 00:54:10.000000 bellows-0.7.0/bellows/cli/opts.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     5648 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/cli/util.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     1927 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/cli/dump.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)    10384 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/cli/application.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     2470 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/cli/ncp.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)      100 2017-09-05 04:27:19.000000 bellows-0.7.0/bellows/cli/__init__.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)      344 2017-10-15 19:02:22.000000 bellows-0.7.0/bellows/cli/main.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     4750 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/cli/network.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     9762 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/uart.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     5876 2018-09-04 01:44:14.000000 bellows-0.7.0/bellows/ezsp.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)    19286 2017-07-26 00:51:52.000000 bellows-0.7.0/bellows/commands.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)        0 2017-01-10 02:34:40.000000 bellows-0.7.0/bellows/__init__.py
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows/zigbee/
+-rw-rw-r--   0 russell   (1000) russell   (1000)     1134 2018-02-19 00:16:29.000000 bellows-0.7.0/bellows/zigbee/util.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)    11184 2018-09-04 01:44:14.000000 bellows-0.7.0/bellows/zigbee/application.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)        0 2017-02-05 17:48:19.000000 bellows-0.7.0/bellows/zigbee/__init__.py
+drwxrwxr-x   0 russell   (1000) russell   (1000)        0 2018-09-04 01:44:33.000000 bellows-0.7.0/bellows/types/
+-rw-rw-r--   0 russell   (1000) russell   (1000)    21637 2017-07-26 00:51:52.000000 bellows-0.7.0/bellows/types/struct.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)    76275 2018-09-03 23:38:18.000000 bellows-0.7.0/bellows/types/named.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)     2943 2018-02-19 00:16:29.000000 bellows-0.7.0/bellows/types/basic.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)      393 2017-02-05 17:48:19.000000 bellows-0.7.0/bellows/types/__init__.py
+-rw-rw-r--   0 russell   (1000) russell   (1000)       59 2018-09-04 01:44:33.000000 bellows-0.7.0/setup.cfg
```

### Comparing `bellows-0.6.0/bellows.egg-info/SOURCES.txt` & `bellows-0.7.0/bellows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/setup.py` & `bellows-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for bellows"""
 
 from setuptools import find_packages, setup
 
 setup(
     name="bellows",
-    version="0.6.0",
+    version="0.7.0",
     description="Library implementing EZSP",
     url="http://github.com/zigpy/bellows",
     author="Russell Cloran",
     author_email="rcloran@gmail.com",
     license="GPL-3.0",
     packages=find_packages(exclude=['*.tests']),
     entry_points={
```

### Comparing `bellows-0.6.0/bellows/cli/opts.py` & `bellows-0.7.0/bellows/cli/opts.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/cli/util.py` & `bellows-0.7.0/bellows/cli/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def convert(self, value, param, ctx):
         if ":" not in value or len(value) != 23:
             self.fail("Node format should be a 8 byte hex string seprated by ':'")
         return t.EmberEUI64([t.uint8_t(p, base=16) for p in value.split(':')])
 
 
-def async(f):
+def background(f):
     @functools.wraps(f)
     def inner(*args, **kwargs):
         loop = asyncio.get_event_loop()
         loop.run_until_complete(f(*args, **kwargs))
 
     return inner
```

### Comparing `bellows-0.6.0/bellows/cli/dump.py` & `bellows-0.7.0/bellows/cli/dump.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/cli/application.py` & `bellows-0.7.0/bellows/cli/application.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @main.command()
 @opts.database_file
 @opts.channel
 @opts.extended_pan
 @opts.pan
 @click.pass_context
-async def form(ctx, database, channel, pan_id, extended_pan_id):
+def form(ctx, database, channel, pan_id, extended_pan_id):
     """Form a new ZigBee network"""
     ctx.obj['database_file'] = database
 
     async def inner(ctx):
         app = ctx.obj['app']
         await app.initialize()
         await app.form_network(channel, pan_id, extended_pan_id)
@@ -32,15 +32,15 @@
     return util.app(inner, app_startup=False)(ctx)
 
 
 @main.command()
 @opts.database_file
 @opts.duration_s
 @click.pass_context
-async def permit(ctx, database, duration_s):
+def permit(ctx, database, duration_s):
     """Allow devices to join this ZigBee network"""
     ctx.obj['database_file'] = database
 
     async def inner(ctx):
         app = ctx.obj['app']
         await app.permit(duration_s)
 
@@ -53,15 +53,15 @@
 
 @main.command()
 @click.argument('node', type=util.ZigbeeNodeParamType())
 @click.argument('code')
 @opts.database_file
 @opts.duration_s
 @click.pass_context
-async def permit_with_key(ctx, database, duration_s, node, code):
+def permit_with_key(ctx, database, duration_s, node, code):
     """Allow devices to join this ZigBee network using an install code"""
     ctx.obj['database_file'] = database
     code = binascii.unhexlify(code)
 
     async def inner(ctx):
         app = ctx.obj['app']
         try:
@@ -133,19 +133,22 @@
     app = ctx.obj['app']
     node = ctx.obj['node']
 
     dev = util.get_device(app, node)
     if dev is None:
         return
 
-    v = await dev.zdo.request(0x0005, dev.nwk)
-    if v[0] != t.EmberStatus.SUCCESS:
-        click.echo("Non-success response: %s" % (v, ))
-    else:
-        click.echo(v[2])
+    try:
+        v = await dev.zdo.request(0x0005, dev.nwk)
+        if v[0] != t.EmberStatus.SUCCESS:
+            click.echo("Non-success response: %s" % (v, ))
+        else:
+            click.echo(v[2])
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zdo.command()
 @click.pass_context
 @util.app
 @click.argument('endpoint', type=click.IntRange(1, 255))
 async def get_endpoint(ctx, endpoint):
@@ -153,19 +156,22 @@
     app = ctx.obj['app']
     node = ctx.obj['node']
 
     dev, endp = util.get_endpoint(app, node, endpoint)
     if endp is None:
         return
 
-    v = await dev.zdo.request(0x0004, dev.nwk, endpoint)
-    if v[0] != t.EmberStatus.SUCCESS:
-        click.echo("Non-success response: %s" % (v, ))
-    else:
-        click.echo(v[2])
+    try:
+        v = await dev.zdo.request(0x0004, dev.nwk, endpoint)
+        if v[0] != t.EmberStatus.SUCCESS:
+            click.echo("Non-success response: %s" % (v, ))
+        else:
+            click.echo(v[2])
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zdo.command()
 @click.pass_context
 @click.argument('endpoint', type=click.IntRange(1, 255))
 @click.argument('cluster', type=click.IntRange(0, 65535))
 @util.app
@@ -174,16 +180,19 @@
     app = ctx.obj['app']
     node = ctx.obj['node']
 
     dev, endp, clust = util.get_in_cluster(app, node, endpoint, cluster)
     if clust is None:
         return
 
-    v = await dev.zdo.bind(endpoint, cluster)
-    click.echo(v)
+    try:
+        v = await dev.zdo.bind(endpoint, cluster)
+        click.echo(v)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zdo.command()
 @click.pass_context
 @click.argument('endpoint', type=click.IntRange(1, 255))
 @click.argument('cluster', type=click.IntRange(0, 65535))
 @util.app
@@ -192,27 +201,33 @@
     app = ctx.obj['app']
     node = ctx.obj['node']
 
     dev, endp, clust = util.get_in_cluster(app, node, endpoint, cluster)
     if clust is None:
         return
 
-    v = await dev.zdo.unbind(endpoint, cluster)
-    click.echo(v)
+    try:
+        v = await dev.zdo.unbind(endpoint, cluster)
+        click.echo(v)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zdo.command()
 @click.pass_context
 @util.app
 async def leave(ctx):
     """Tell a node to leave the network"""
     app = ctx.obj['app']
 
-    v = await app.remove(ctx.obj['node'])
-    click.echo(v)
+    try:
+        v = await app.remove(ctx.obj['node'])
+        click.echo(v)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @main.group()
 @click.pass_context
 @opts.database_file
 @click.argument('node', type=util.ZigbeeNodeParamType())
 @click.argument('endpoint', type=click.IntRange(1, 255))
@@ -236,23 +251,26 @@
     endpoint_id = ctx.obj['endpoint']
     cluster_id = ctx.obj['cluster']
 
     dev, endpoint, cluster = util.get_in_cluster(app, node, endpoint_id, cluster_id)
     if cluster is None:
         return
 
-    v = await cluster.read_attributes([attribute], allow_cache=False, manufacturer=manufacturer)
-    if not v:
-        click.echo("Received empty response")
-    elif attribute not in v[0]:
-        click.echo("Attribute %s not successful. Status=%s" % (
-            attribute, v[1][attribute]
-        ))
-    else:
-        click.echo("%s=%s" % (attribute, v[0][attribute]))
+    try:
+        v = await cluster.read_attributes([attribute], allow_cache=False, manufacturer=manufacturer)
+        if not v:
+            click.echo("Received empty response")
+        elif attribute not in v[0]:
+            click.echo("Attribute %s not successful. Status=%s" % (
+                attribute, v[1][attribute]
+            ))
+        else:
+            click.echo("%s=%s" % (attribute, v[0][attribute]))
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zcl.command()
 @click.pass_context
 @click.argument('attribute', type=click.IntRange(0, 65535))
 @click.argument('value', type=click.IntRange(0, 65535))
 @opts.manufacturer
@@ -263,16 +281,19 @@
     endpoint_id = ctx.obj['endpoint']
     cluster_id = ctx.obj['cluster']
 
     dev, endpoint, cluster = util.get_in_cluster(app, node, endpoint_id, cluster_id)
     if cluster is None:
         return
 
-    v = await cluster.write_attributes({attribute: value}, manufacturer=manufacturer)
-    click.echo(v)
+    try:
+        v = await cluster.write_attributes({attribute: value}, manufacturer=manufacturer)
+        click.echo(v)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zcl.command()
 @click.pass_context
 def commands(ctx):
     database = ctx.obj['database_file']
     node = ctx.obj['node']
@@ -307,14 +328,16 @@
         return
 
     try:
         v = await getattr(cluster, command)(*parameters, manufacturer=manufacturer)
         click.echo(v)
     except ValueError as e:
         click.echo(e)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
 
 
 @zcl.command()
 @click.pass_context
 @click.argument('attribute', type=click.IntRange(0, 65535))
 @click.argument('min_interval', type=click.IntRange(0, 65535))
 @click.argument('max_interval', type=click.IntRange(0, 65535))
@@ -330,14 +353,17 @@
     endpoint_id = ctx.obj['endpoint']
     cluster_id = ctx.obj['cluster']
 
     dev, endpoint, cluster = util.get_in_cluster(app, node, endpoint_id, cluster_id)
     if cluster is None:
         return
 
-    v = await cluster.configure_reporting(
-        attribute,
-        min_interval,
-        max_interval,
-        reportable_change,
-    )
-    click.echo(v)
+    try:
+        v = await cluster.configure_reporting(
+            attribute,
+            min_interval,
+            max_interval,
+            reportable_change,
+        )
+        click.echo(v)
+    except bellows.zigbee.exceptions.DeliveryError as e:
+        click.echo(e)
```

### Comparing `bellows-0.6.0/bellows/cli/ncp.py` & `bellows-0.7.0/bellows/cli/ncp.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .main import main
 
 
 @main.command()
 @click.argument('config', required=False)
 @click.option('-a', '--all', 'all_', is_flag=True)
 @click.pass_context
-@util.async
+@util.background
 async def config(ctx, config, all_):
     """Get/set configuration on the NCP"""
     click.secho(
         "NOTE: Configuration changes do not persist across resets",
         fg='red'
     )
     if config and all_:
@@ -65,15 +65,15 @@
 
     v = await s.getConfigurationValue(config)
     click.echo(v)
 
 
 @main.command()
 @click.pass_context
-@util.async
+@util.background
 async def info(ctx):
     """Get NCP information"""
     s = await util.setup(ctx.obj['device'], ctx.obj['baudrate'])
     await util.network_init(s)
 
     commands = [
         'getEui64',
```

### Comparing `bellows-0.6.0/bellows/cli/network.py` & `bellows-0.7.0/bellows/cli/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @main.command()
 @opts.channels
 @opts.extended_pan
 @opts.pan
 @click.pass_context
-@util.async
+@util.background
 async def join(ctx, channels, pan_id, extended_pan_id):
     """Join an existing ZigBee network as an end device"""
     def cb(fut, frame_name, response):
         if frame_name == 'stackStatusHandler':
             fut.set_result(response)
 
     s = await util.setup(ctx.obj['device'], ctx.obj['baudrate'])
@@ -107,15 +107,15 @@
     s.remove_callback(cbid)
 
     s.close()
 
 
 @main.command()
 @click.pass_context
-@util.async
+@util.background
 async def leave(ctx):
     """Leave the ZigBee network"""
     s = await util.setup(ctx.obj['device'], ctx.obj['baudrate'])
     v = await util.network_init(s)
     if v[0] == t.EmberStatus.NOT_JOINED:
         click.echo("Not joined, not leaving")
     else:
@@ -126,15 +126,15 @@
 
 
 @main.command()
 @opts.channels
 @opts.duration_ms
 @click.option('-e', '--energy', 'energy_scan', is_flag=True)
 @click.pass_context
-@util.async
+@util.background
 async def scan(ctx, channels, duration_ms, energy_scan):
     """Scan for networks or radio interference"""
     s = await util.setup(ctx.obj['device'], ctx.obj['baudrate'])
 
     channel_mask = util.channel_mask(channels)
     click.echo("Scanning channels %s" % (' '.join(map(str, channels)), ))
```

### Comparing `bellows-0.6.0/bellows/uart.py` & `bellows-0.7.0/bellows/uart.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self._pending = (-1, None)
 
     def connection_made(self, transport):
         """Callback when the uart is connected"""
         self._transport = transport
         if self._connected_future is not None:
             self._connected_future.set_result(True)
-            asyncio.async(self._send_task())
+            asyncio.ensure_future(self._send_task())
 
     def data_received(self, data):
         """Callback when there is data received from the uart"""
         # TODO: Fix this handling for multiple instances of the characters
         # If a Cancel Byte or Substitute Byte is received, the bytes received
         # so far are discarded. In the case of a Substitute Byte, subsequent
         # bytes will also be discarded until the next Flag Byte.
@@ -63,15 +63,25 @@
                 break
             self.frame_received(frame)
 
     def _extract_frame(self, data):
         """Extract a frame from the data buffer"""
         if self.FLAG in data:
             place = data.find(self.FLAG)
-            return self._unstuff(data[:place + 1]), data[place + 1:]
+            frame = self._unstuff(data[:place + 1])
+            rest = data[place + 1:]
+            crc = binascii.crc_hqx(frame[:-3], 0xffff)
+            crc = bytes([crc >> 8, crc % 256])
+            if crc != frame[-3:-1]:
+                LOGGER.error("CRC error in frame %s (%s != %s)", binascii.hexlify(frame), binascii.hexlify(frame[-3:-1]), binascii.hexlify(crc))
+                self.write(self._nak_frame())
+                # Make sure that we also handle the next frame if it is already received
+                return self._extract_frame(rest)
+
+            return frame, rest
         return None, data
 
     def frame_received(self, data):
         """Frame receive handler"""
         if (data[0] & 0b10000000) == 0:
             self.data_frame_received(data)
         elif (data[0] & 0b11100000) == 0b10000000:
@@ -124,15 +134,17 @@
         if code is not t.NcpResetCode.RESET_SOFTWARE:
             return
 
         if self._reset_future is None:
             LOGGER.warn("Reset future is None")
             return
 
-        self._reset_future.set_result(True)
+        # Make sure that the reset_future is not done
+        if not self._reset_future.done():
+            self._reset_future.set_result(True)
 
     def error_frame_received(self, data):
         """Error frame receive handler"""
         LOGGER.debug("Error frame: %s", binascii.hexlify(data))
 
     def write(self, data):
         """Send data to the uart"""
@@ -196,14 +208,20 @@
 
     def _ack_frame(self):
         """Construct a acknowledgement frame"""
         assert 0 <= self._rec_seq < 8
         control = bytes([0b10000000 | (self._rec_seq & 0b00000111)])
         return self._frame(control, b'')
 
+    def _nak_frame(self):
+        """Construct a negative acknowledgement frame"""
+        assert 0 <= self._rec_seq < 8
+        control = bytes([0b10100000 | (self._rec_seq & 0b00000111)])
+        return self._frame(control, b'')
+
     def _rst_frame(self):
         """Construct a reset frame"""
         return self.CANCEL + self._frame(b'\xC0', b'')
 
     def _frame(self, control, data):
         """Construct a frame"""
         crc = binascii.crc_hqx(control + data, 0xffff)
```

### Comparing `bellows-0.6.0/bellows/ezsp.py` & `bellows-0.7.0/bellows/ezsp.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/commands.py` & `bellows-0.7.0/bellows/commands.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/zigbee/util.py` & `bellows-0.7.0/bellows/zigbee/util.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/zigbee/application.py` & `bellows-0.7.0/bellows/zigbee/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,20 @@
                 reply_fut.cancel()
             raise DeliveryError("Message send failure %s" % (v[0], ))
 
         # Wait for messageSentHandler message
         v = await send_fut
         if expect_reply:
             # Wait for reply
-            v = await asyncio.wait_for(reply_fut, timeout)
+            try:
+                v = await asyncio.wait_for(reply_fut, timeout)
+            except:  # noqa: E722
+                # If we timeout (or fail for any reason), clear the future
+                self._pending.pop(sequence)
+                raise
         return v
 
     def permit(self, time_s=60):
         assert 0 <= time_s <= 254
         return self._ezsp.permitJoining(time_s)
 
     async def permit_with_key(self, node, code, time_s=60):
```

### Comparing `bellows-0.6.0/bellows/types/struct.py` & `bellows-0.7.0/bellows/types/struct.py`

 * *Files identical despite different names*

### Comparing `bellows-0.6.0/bellows/types/named.py` & `bellows-0.7.0/bellows/types/named.py`

 * *Files 0% similar despite different names*

```diff
@@ -1088,14 +1088,16 @@
     SLEEPY_END_DEVICE = 0x04
     # A sleepy end device that can move through the network.
     MOBILE_END_DEVICE = 0x05
     # RF4CE target node.
     RF4CE_TARGET = 0x06
     # RF4CE controller node.
     RF4CE_CONTROLLER = 0x07
+    # Device is not joined or no network is formed.
+    UNKNOWN_NODE_TYPE = 0xFF
 
 
 class EmberNetworkStatus(basic.uint8_t, enum.Enum):
     # The possible join states for a node.
 
     # The node is not associated with a network in any way.
     NO_NETWORK = 0x00
```

### Comparing `bellows-0.6.0/bellows/types/basic.py` & `bellows-0.7.0/bellows/types/basic.py`

 * *Files identical despite different names*

