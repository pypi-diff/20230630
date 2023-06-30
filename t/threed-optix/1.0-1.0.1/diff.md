# Comparing `tmp/threed_optix-1.0.tar.gz` & `tmp/threed_optix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-1.0.tar", last modified: Thu Jun 29 16:55:22 2023, max compression
+gzip compressed data, was "threed_optix-1.0.1.tar", last modified: Fri Jun 30 18:06:53 2023, max compression
```

## Comparing `threed_optix-1.0.tar` & `threed_optix-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-29 16:55:22.121388 threed_optix-1.0/
--rw-rw-r--   0 elika     (1000) elika     (1000)      168 2023-06-29 16:55:22.121388 threed_optix-1.0/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0/README.rst
--rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-06-29 16:55:22.125388 threed_optix-1.0/setup.cfg
--rw-rw-r--   0 elika     (1000) elika     (1000)      366 2023-06-29 16:11:58.000000 threed_optix-1.0/setup.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-29 16:55:22.121388 threed_optix-1.0/src/
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-29 16:55:22.121388 threed_optix-1.0/src/threed_optix/
--rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0/src/threed_optix/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     5576 2023-06-28 18:11:26.000000 threed_optix-1.0/src/threed_optix/api.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-29 16:55:22.121388 threed_optix-1.0/src/threed_optix/examples/
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0/src/threed_optix/examples/__init__.py
--rwxrwxr-x   0 elika     (1000) elika     (1000)      409 2023-06-28 18:11:26.000000 threed_optix-1.0/src/threed_optix/examples/simple.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-29 16:55:22.121388 threed_optix-1.0/src/threed_optix.egg-info/
--rw-rw-r--   0 elika     (1000) elika     (1000)      168 2023-06-29 16:55:22.000000 threed_optix-1.0/src/threed_optix.egg-info/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)      355 2023-06-29 16:55:22.000000 threed_optix-1.0/src/threed_optix.egg-info/SOURCES.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-06-29 16:55:22.000000 threed_optix-1.0/src/threed_optix.egg-info/dependency_links.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)        9 2023-06-29 16:55:22.000000 threed_optix-1.0/src/threed_optix.egg-info/requires.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-06-29 16:55:22.000000 threed_optix-1.0/src/threed_optix.egg-info/top_level.txt
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-30 18:06:53.974342 threed_optix-1.0.1/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-06-30 18:06:53.978342 threed_optix-1.0.1/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0.1/README.rst
+-rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-06-30 18:06:53.978342 threed_optix-1.0.1/setup.cfg
+-rw-rw-r--   0 elika     (1000) elika     (1000)      368 2023-06-30 18:06:37.000000 threed_optix-1.0.1/setup.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-30 18:06:53.974342 threed_optix-1.0.1/src/
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-30 18:06:53.974342 threed_optix-1.0.1/src/threed_optix/
+-rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.1/src/threed_optix/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     5755 2023-06-30 12:46:37.000000 threed_optix-1.0.1/src/threed_optix/api.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-30 18:06:53.974342 threed_optix-1.0.1/src/threed_optix/examples/
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.1/src/threed_optix/examples/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     1146 2023-06-30 13:37:04.000000 threed_optix-1.0.1/src/threed_optix/examples/example_0.py
+-rwxrwxr-x   0 elika     (1000) elika     (1000)      550 2023-06-30 12:46:37.000000 threed_optix-1.0.1/src/threed_optix/examples/simple.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-06-30 18:06:53.974342 threed_optix-1.0.1/src/threed_optix.egg-info/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-06-30 18:06:53.000000 threed_optix-1.0.1/src/threed_optix.egg-info/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)      394 2023-06-30 18:06:53.000000 threed_optix-1.0.1/src/threed_optix.egg-info/SOURCES.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-06-30 18:06:53.000000 threed_optix-1.0.1/src/threed_optix.egg-info/dependency_links.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)        9 2023-06-30 18:06:53.000000 threed_optix-1.0.1/src/threed_optix.egg-info/requires.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-06-30 18:06:53.000000 threed_optix-1.0.1/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-1.0/src/threed_optix/api.py` & `threed_optix-1.0.1/src/threed_optix/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+import pandas as pd
 
 
 API_URL = "https://api-dev.3doptix.com/v1/"
 
 
 class ThreedOptixAPI(object):
     def __init__(self, api_key):
@@ -22,14 +23,16 @@
             raise Exception(message)
 
     def fetch(self, obj):
         if isinstance(obj, Setup):
             self.fetch_setup(obj)
         elif isinstance(obj, Part):
             self.fetch_part(obj)
+        elif isinstance(obj, AnalysisResult):
+            self.fetch_analysis_result(obj)
         else:
             raise TypeError(f"Cannot fetch instance of type '{obj.__class__.__name__}'")
 
     def update(self, obj):
         if isinstance(obj, Part):
             self.update_part(obj)
         else:
@@ -45,16 +48,19 @@
     def fetch_part(self, part):
         json, message = get_part(part.owner.id, part.id, self.api_key)
         if json is not None:
             part.set_from_json(json)
         else:
             raise Exception(message)
 
+    def fetch_analysis_result(self, result):
+        result.data = pd.read_csv(result.url)
+
     def update_part(self, part):
-        success, message = set_part(part.owner.id, part.id, part.as_json(), self.api_key)
+        success, message = set_part(part.owner.id, part.id, part.to_json(), self.api_key)
         if not success:
             raise Exception(message)
 
     def run(self, setup):
         data, message = run_simulation(setup.id, self.api_key)
         if data is not None:
             return AnalysisResult.new(data['simulation_result_link'])
@@ -105,50 +111,51 @@
 
     def set_from_json(self, json):
         json = json[self.id]
         self.pose = Pose().set_from_json(json['pose'])
 
         return self
 
-    def as_json(self):
+    def to_json(self):
         json = {}
         if self.pose is not None:
-            json['pose'] = self.pose.as_json()
-        return {self.id: json}
+            json['pose'] = self.pose.to_json()
+        return json
 
     def __str__(self):
         return self.label
 
 
 class AnalysisResult(object):
     def __init__(self):
         raise TypeError("Cannot create 'AnalysisResult' instances")
 
     @classmethod
     def new(cls, url):
         obj = object.__new__(cls)
         obj.url = url
+        obj.data = None
         return obj
 
 
 class Vector3(object):
     def __init__(self, x=0.0, y=0.0, z=0.0):
         self.x = x
         self.y = y
         self.z = z
 
     def set_from_json(self, json):
-        self.x = float(json[0])
-        self.y = float(json[1])
-        self.z = float(json[2])
+        self.x = json[0]
+        self.y = json[1]
+        self.z = json[2]
 
         return self
 
-    def as_json(self):
-        return [str(self.x), str(self.y), str(self.z)]
+    def to_json(self):
+        return [self.x, self.y, self.z]
 
     def __str__(self):
         return f'({self.x}, {self.y}, {self.z})'
 
 
 class Pose(object):
     def __init__(self, position=Vector3(), rotation=Vector3()):
@@ -157,16 +164,16 @@
 
     def set_from_json(self, json):
         self.position = Vector3().set_from_json(json['position'])
         self.rotation = Vector3().set_from_json(json['rotation'])
 
         return self
 
-    def as_json(self):
-        return {'position': self.position.as_json(), 'rotation': self.rotation.as_json()}
+    def to_json(self):
+        return {'position': self.position.to_json(), 'rotation': self.rotation.to_json()}
 
     def __str__(self):
         return f'position={self.position} rotation={self.rotation}'
 
 
 def healthcheck():
     url = API_URL + 'healthcheck'
```

