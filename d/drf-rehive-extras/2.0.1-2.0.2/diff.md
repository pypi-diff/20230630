# Comparing `tmp/drf-rehive-extras-2.0.1.tar.gz` & `tmp/drf-rehive-extras-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.0.1.tar", last modified: Fri Jun 30 09:51:00 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.0.2.tar", last modified: Fri Jun 30 11:11:40 2023, max compression
```

## Comparing `drf-rehive-extras-2.0.1.tar` & `drf-rehive-extras-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.1/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7164 2023-06-29 20:18:25.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2685 2023-06-30 09:48:56.000000 drf-rehive-extras-2.0.1/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-30 09:49:30.000000 drf-rehive-extras-2.0.1/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.1/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 09:50:59.000000 drf-rehive-extras-2.0.1/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.2/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7069 2023-06-30 11:07:36.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6207 2023-06-30 11:07:34.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2685 2023-06-30 09:48:56.000000 drf-rehive-extras-2.0.2/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-30 11:07:41.000000 drf-rehive-extras-2.0.2/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.2/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 11:11:40.000000 drf-rehive-extras-2.0.2/PKG-INFO
```

### Comparing `drf-rehive-extras-2.0.1/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.0.2/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.1
+Version: 2.0.2
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.1.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.2.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.0.1/README.md` & `drf-rehive-extras-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.1/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.0.2/drf_rehive_extras/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         # Handle the response serialization. Sometimes the serialization of
         # responses should be different from the request serialization.
         data = self.get_response_serializer(serializer.instance).data
 
         return Response(
             data={'status': 'success', 'data': data},
-            status=self.get_response_status_code(status.HTTP_201_CREATED),
+            status=self.get_response_status_code(),
             headers=headers
         )
 
     def perform_create(self, serializer):
         """
         Perform creation using the serializer.
         """
@@ -139,15 +139,15 @@
             return self.get_paginated_response(serializer.data)
 
         # Handle serialization.
         serializer = self.get_serializer(queryset, many=True)
 
         return Response(
             data={'status': 'success', 'data': serializer.data},
-            status=self.get_response_status_code(status.HTTP_200_OK)
+            status=self.get_response_status_code()
         )
 
 
 class RetrieveModelMixin:
     """
     Retrieve a model instance.
     """
@@ -164,15 +164,15 @@
         add_resource_data(request, instance)
 
         # Handle serialization.
         serializer = self.get_serializer(instance)
 
         return Response(
             data={'status': 'success', 'data': serializer.data},
-            status=self.get_response_status_code(status.HTTP_200_OK)
+            status=self.get_response_status_code()
         )
 
 
 class UpdateModelMixin:
     """
     Update a model instance.
     """
@@ -200,15 +200,15 @@
 
         # Handle the response serialization. Sometimes the serialization of
         # responses should be different from the request serialization.
         data = self.get_response_serializer(serializer.instance).data
 
         return Response(
             data={'status': 'success', 'data': data},
-            status=self.get_response_status_code(status.HTTP_200_OK),
+            status=self.get_response_status_code(),
         )
 
     def perform_update(self, serializer):
         """
         Perform update using the serializer.
         """
 
@@ -241,15 +241,15 @@
 
         # Handle serialization and destroy.
         serializer = self.get_serializer(instance, data=request.data)
         self.perform_destroy(serializer)
 
         return Response(
             data={'status': 'success'},
-            status=self.get_response_status_code(status.HTTP_200_OK)
+            status=self.get_response_status_code()
         )
 
     def perform_destroy(self, serializer):
         """
         Perform destroy using the serializer.
         """
```

### Comparing `drf-rehive-extras-2.0.1/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.0.2/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.1/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.0.2/drf_rehive_extras/generics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.translation import gettext_lazy as _
+from rest_framework import status
 from rest_framework.generics import GenericAPIView
 
 from . import mixins
 
 
 class BaseAPIView(GenericAPIView):
     """
@@ -17,14 +18,17 @@
     serializer_classes = {}
 
     # Modify statuses used by the view based on the request method.
     # This attributes can take the following format:
     #  - `{"GET": status.HTTP_200_OK}`
     response_status_codes = {}
 
+    # Modify the default status code.
+    response_status_code = status.HTTP_200_OK
+
     def get_serializer_class(self):
         """
         Retrieve the request serializer class for the view.
 
         If the item returned from the serializer_classes is a tuple or list then
         get the first class.
         """
@@ -67,32 +71,34 @@
         `get_serializer_class`.
         """
 
         serializer_class = self.get_response_serializer_class()
         kwargs.setdefault('context', self.get_serializer_context())
         return serializer_class(*args, **kwargs)
 
-    def get_response_status_code(self, default):
+    def get_response_status_code(self):
         """
-        Get the response status code. Will use a custom one if one exists for
-        the method.
+        Get the response status code.
         """
 
         try:
             return self.response_status_codes[self.request.method]
         except KeyError:
-            return default
+            return self.response_status_code
 
 
 class CreateAPIView(mixins.CreateModelMixin,
                     BaseAPIView):
     """
     Concrete view for creating a model instance.
     """
 
+    # Modify the default status code.
+    response_status_code = status.HTTP_201_CREATED
+
     def post(self, request, *args, **kwargs):
         return self.create(request, *args, **kwargs)
 
 
 class ListAPIView(mixins.ListModelMixin,
                   BaseAPIView):
     """
```

### Comparing `drf-rehive-extras-2.0.1/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.0.2/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.1/setup.py` & `drf-rehive-extras-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.0.1'
+VERSION = '2.0.2'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.0.1/LICENSE` & `drf-rehive-extras-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.1/PKG-INFO` & `drf-rehive-extras-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.1
+Version: 2.0.2
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.1.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.2.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

