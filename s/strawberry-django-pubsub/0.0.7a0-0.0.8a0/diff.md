# Comparing `tmp/strawberry_django_pubsub-0.0.7a0.tar.gz` & `tmp/strawberry_django_pubsub-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_pubsub-0.0.7a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "strawberry_django_pubsub-0.0.8a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `strawberry_django_pubsub-0.0.7a0.tar` & `strawberry_django_pubsub-0.0.8a0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.7a0/.flake8
--rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.7a0/.gitignore
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.7a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.7a0/LICENSE
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.7a0/Makefile
--rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.7a0/README.md
--rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.7a0/pyproject.toml
--rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.7a0/requirements/compile.py
--rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.7a0/requirements/py310-django41.txt
--rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.7a0/requirements/py310-django42.txt
--rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.7a0/requirements/py311-django41.txt
--rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.7a0/requirements/py311-django42.txt
--rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.7a0/requirements/py39-django41.txt
--rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.7a0/requirements/py39-django42.txt
--rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.7a0/requirements/requirements.in
--rw-r--r--   0        0        0       61 2023-06-29 11:59:58.254909 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/__init__.py
--rw-r--r--   0        0        0     6550 2023-06-29 09:18:36.409856 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/asgi.py
--rw-r--r--   0        0        0      521 2023-06-28 20:06:16.062832 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/context.py
--rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/debug.py
--rw-r--r--   0        0        0     6616 2023-05-30 19:26:00.787412 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/auth.py
--rw-r--r--   0        0        0      562 2023-05-30 19:26:00.787702 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/db.py
--rw-r--r--   0        0        0      756 2023-05-30 19:26:00.788092 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/middleware.py
--rw-r--r--   0        0        0     5177 2023-06-29 11:59:33.542786 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/router.py
--rw-r--r--   0        0        0    10093 2023-05-30 19:26:00.788614 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/sessions.py
--rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/event.py
--rw-r--r--   0        0        0      841 2023-05-30 10:26:07.846938 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/exceptions.py
--rw-r--r--   0        0        0     1990 2023-06-28 20:34:06.719562 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
--rw-r--r--   0        0        0     4119 2023-06-29 11:46:03.627036 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/queue.py
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/types.py
--rw-r--r--   0        0        0      798 2023-06-29 11:46:18.556383 strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/utils.py
--rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.7a0/tox.ini
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.7a0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.8a0/.flake8
+-rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.8a0/.gitignore
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.8a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.8a0/LICENSE
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.8a0/Makefile
+-rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.8a0/README.md
+-rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.8a0/pyproject.toml
+-rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.8a0/requirements/compile.py
+-rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.8a0/requirements/py310-django41.txt
+-rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.8a0/requirements/py310-django42.txt
+-rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.8a0/requirements/py311-django41.txt
+-rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.8a0/requirements/py311-django42.txt
+-rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.8a0/requirements/py39-django41.txt
+-rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.8a0/requirements/py39-django42.txt
+-rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.8a0/requirements/requirements.in
+-rw-r--r--   0        0        0       61 2023-06-29 16:18:26.350235 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/__init__.py
+-rw-r--r--   0        0        0     6550 2023-06-29 16:18:06.398578 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/asgi.py
+-rw-r--r--   0        0        0      521 2023-06-28 20:06:16.062832 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/context.py
+-rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/debug.py
+-rw-r--r--   0        0        0     6616 2023-05-30 19:26:00.787412 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/auth.py
+-rw-r--r--   0        0        0      562 2023-05-30 19:26:00.787702 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/db.py
+-rw-r--r--   0        0        0      756 2023-05-30 19:26:00.788092 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/middleware.py
+-rw-r--r--   0        0        0     5577 2023-06-29 16:18:06.398935 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/router.py
+-rw-r--r--   0        0        0    10093 2023-05-30 19:26:00.788614 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/sessions.py
+-rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/event.py
+-rw-r--r--   0        0        0      841 2023-05-30 10:26:07.846938 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/exceptions.py
+-rw-r--r--   0        0        0     1990 2023-06-28 20:34:06.719562 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
+-rw-r--r--   0        0        0     4119 2023-06-29 16:18:06.399306 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/queue.py
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/types.py
+-rw-r--r--   0        0        0      798 2023-06-29 16:18:06.399687 strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/utils.py
+-rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.8a0/tox.ini
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.8a0/PKG-INFO
```

### Comparing `strawberry_django_pubsub-0.0.7a0/.gitignore` & `strawberry_django_pubsub-0.0.8a0/.gitignore`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/LICENSE` & `strawberry_django_pubsub-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/pyproject.toml` & `strawberry_django_pubsub-0.0.8a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/compile.py` & `strawberry_django_pubsub-0.0.8a0/requirements/compile.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py310-django41.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py310-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py310-django42.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py311-django41.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py311-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py311-django42.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py39-django41.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py39-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/requirements/py39-django42.txt` & `strawberry_django_pubsub-0.0.8a0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/asgi.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/asgi.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/context.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/debug.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/debug.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/auth.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/auth.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/db.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/db.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/middleware.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/middleware.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/router.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 """
 All Routing instances inside this file are also valid ASGI applications - with
 new Channels routing, whatever you end up with as the top level object is just
 served up as the "ASGI application".
 """
 
 
+async def queue_lifespan_emulate() -> None:
+    """
+    Lifespan is not supported by all servers; here we emulate a lifespan session
+    For example Daphne does NOT support lifespan protocol (yet).
+    """
+    if not getattr(queue._queue, '_published', False):
+        await queue.connect()
+
+    return None
+
+
 def get_default_application():
     """
     Gets the default application, set in the ASGI_APPLICATION setting.
     """
     try:
         path, name = settings.ASGI_APPLICATION.rsplit(".", 1)
     except (ValueError, AttributeError):
@@ -31,46 +42,49 @@
     except AttributeError:
         raise ImproperlyConfigured(
             "Cannot find %r in ASGI_APPLICATION module %s" % (name, path)
         )
     return value
 
 
-class QueueProtocolTypeRouter:
+class ProtocolTypeRouter:
     """
     Takes a mapping of protocol type names to other Application instances,
     and dispatches to the right one based on protocol name (or raises an error)
     """
 
-    def __init__(
-        self,
-        application_mapping,
-    ):
+    def __init__(self, application_mapping, no_lifespan=False):
         self.application_mapping = application_mapping
+        self.no_lifespan = no_lifespan
 
     async def __call__(self, scope, receive, send):
-        # Need to move this into QueueLifeSpanRouter
+        if self.no_lifespan:
+            await queue_lifespan_emulate()
+
+        if scope["type"] in self.application_mapping:
+            application = self.application_mapping[scope["type"]]
+            return await application(scope, receive, send)
+        else:
+            raise ValueError(
+                "No application configured for scope type %r" % scope["type"]
+            )
+
+
+class QueueLifeSpanManager:
+    async def __call__(self, scope, receive, send):
         if scope['type'] == 'lifespan':
             while True:
                 message = await receive()
                 if message['type'] == 'lifespan.startup':
                     await queue.connect()
                     await send({'type': 'lifespan.startup.complete'})
                 elif message['type'] == 'lifespan.shutdown':
                     await queue.disconnect()
                     await send({'type': 'lifespan.shutdown.complete'})
                     return
-        else:
-            if scope["type"] in self.application_mapping:
-                application = self.application_mapping[scope["type"]]
-                return await application(scope, receive, send)
-            else:
-                raise ValueError(
-                    "No application configured for scope type %r" % scope["type"]
-                )
 
 
 class URLRouter:
     """
     Routes to different applications/consumers based on the URL path.
 
     Works with anything that has a ``path`` key, but intended for WebSocket
```

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/django/sessions.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/django/sessions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/exceptions.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/queue.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/queue.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/strawberry_django_pubsub/utils.py` & `strawberry_django_pubsub-0.0.8a0/strawberry_django_pubsub/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.7a0/PKG-INFO` & `strawberry_django_pubsub-0.0.8a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-pubsub
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: Strawberry Django PubSub 
 Author-email: DK <dk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

