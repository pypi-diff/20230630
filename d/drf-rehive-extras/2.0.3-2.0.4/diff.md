# Comparing `tmp/drf-rehive-extras-2.0.3.tar.gz` & `tmp/drf-rehive-extras-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.0.3.tar", last modified: Fri Jun 30 11:47:50 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.0.4.tar", last modified: Fri Jun 30 12:07:13 2023, max compression
```

## Comparing `drf-rehive-extras-2.0.3.tar` & `drf-rehive-extras-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.3/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7159 2023-06-30 11:46:49.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6117 2023-06-30 11:46:55.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2685 2023-06-30 09:48:56.000000 drf-rehive-extras-2.0.3/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-30 11:47:01.000000 drf-rehive-extras-2.0.3/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.3/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 11:47:50.000000 drf-rehive-extras-2.0.3/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.4/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7035 2023-06-30 12:04:34.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6578 2023-06-30 12:05:21.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2685 2023-06-30 09:48:56.000000 drf-rehive-extras-2.0.4/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-30 12:06:37.000000 drf-rehive-extras-2.0.4/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.4/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-30 12:07:13.000000 drf-rehive-extras-2.0.4/PKG-INFO
```

### Comparing `drf-rehive-extras-2.0.3/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.0.4/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.3
+Version: 2.0.4
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.3.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.4.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.0.3/README.md` & `drf-rehive-extras-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.3/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.0.4/drf_rehive_extras/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.settings import api_settings
 from django_filters.rest_framework import DjangoFilterBackend
 
 from .pagination import PageNumberPagination, CursorPagination
 
 
@@ -38,17 +37,14 @@
 
 
 class CreateModelMixin:
     """
     Create a model instance.
     """
 
-    # Modify the default status code.
-    response_status_code = status.HTTP_201_CREATED
-
     def create(self, request, *args, **kwargs):
         """
         Handle object creation on the view.
         """
 
         # Handle the request serialization and creation.
         serializer = self.get_serializer(data=request.data)
```

### Comparing `drf-rehive-extras-2.0.3/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.0.4/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.3/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.0.4/drf_rehive_extras/generics.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,37 @@
 
 class BaseAPIView(GenericAPIView):
     """
     Generic view with extended features for Rehive usage. All viewsets should
     extend this class.
     """
 
-    # Modify serializer classes used by the view based on the request method.
+    # Modify the serializer classes used by the view based on the request
+    # method.
     # This attribute can take two formats:
     #  - {"GET": ObjectSerializer}
     #  - {"GET": (RequestObjectSerializer, ResponseObjectSerializer,)}
     serializer_classes = {}
 
-    # Modify statuses used by the view based on the request method.
+    # Modify the statuses used by the view based on the request method.
     # This attributes can take the following format:
     #  - `{"GET": status.HTTP_200_OK}`
-    response_status_codes = {}
+    response_status_codes ={}
 
-    # Modify the default status code.
-    response_status_code = status.HTTP_200_OK
+    # The default statuses used by the view based on the request method.
+    default_response_status_codes = {
+        "GET": status.HTTP_200_OK,
+        "POST": status.HTTP_201_CREATED,
+        "PUT": status.HTTP_200_OK,
+        "PATCH": status.HTTP_200_OK,
+        # NOTE : We use 200 for deletes instead of 204 because the Rehive
+        # response format supports a `status` in the body and by default
+        # 204 expects there to be no response body.
+        "DELETE": status.HTTP_200_OK,
+    }
 
     def get_serializer_class(self):
         """
         Retrieve the request serializer class for the view.
 
         If the item returned from the serializer_classes is a tuple or list then
         get the first class.
@@ -79,15 +89,15 @@
         """
         Get the response status code.
         """
 
         try:
             return self.response_status_codes[self.request.method]
         except KeyError:
-            return self.response_status_code
+            return self.default_response_status_codes[self.request.method]
 
 
 class CreateAPIView(mixins.CreateModelMixin,
                     BaseAPIView):
     """
     Concrete view for creating a model instance.
     """
```

### Comparing `drf-rehive-extras-2.0.3/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.0.4/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.3/setup.py` & `drf-rehive-extras-2.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.0.3'
+VERSION = '2.0.4'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.0.3/LICENSE` & `drf-rehive-extras-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.3/PKG-INFO` & `drf-rehive-extras-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.3
+Version: 2.0.4
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.3.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.4.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

