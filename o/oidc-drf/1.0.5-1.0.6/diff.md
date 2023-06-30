# Comparing `tmp/oidc_drf-1.0.5.tar.gz` & `tmp/oidc_drf-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.0.5.tar", last modified: Fri Jun 30 19:05:07 2023, max compression
+gzip compressed data, was "oidc_drf-1.0.6.tar", last modified: Fri Jun 30 19:15:50 2023, max compression
```

## Comparing `oidc_drf-1.0.5.tar` & `oidc_drf-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:05:07.474419 oidc_drf-1.0.5/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 19:05:07.474289 oidc_drf-1.0.5/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     4286 2023-06-22 20:44:43.000000 oidc_drf-1.0.5/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:05:07.473018 oidc_drf-1.0.5/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.5/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-06-21 20:00:07.000000 oidc_drf-1.0.5/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15595 2023-06-30 18:46:33.000000 oidc_drf-1.0.5/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4589 2023-06-21 20:00:07.000000 oidc_drf-1.0.5/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:05:07.474133 oidc_drf-1.0.5/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.5/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      332 2023-06-30 19:04:55.000000 oidc_drf-1.0.5/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.5/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.5/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     7751 2023-06-30 18:48:30.000000 oidc_drf-1.0.5/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:05:07.473984 oidc_drf-1.0.5/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 19:05:07.000000 oidc_drf-1.0.5/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-06-30 19:05:07.000000 oidc_drf-1.0.5/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-06-30 19:05:07.000000 oidc_drf-1.0.5/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-06-30 19:05:07.000000 oidc_drf-1.0.5/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-06-30 19:05:07.000000 oidc_drf-1.0.5/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-06-30 19:05:07.474453 oidc_drf-1.0.5/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-06-30 19:05:04.000000 oidc_drf-1.0.5/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:15:50.097388 oidc_drf-1.0.6/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 19:15:50.097239 oidc_drf-1.0.6/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4286 2023-06-22 20:44:43.000000 oidc_drf-1.0.6/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:15:50.095865 oidc_drf-1.0.6/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.6/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-06-21 20:00:07.000000 oidc_drf-1.0.6/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15614 2023-06-30 19:15:36.000000 oidc_drf-1.0.6/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4589 2023-06-21 20:00:07.000000 oidc_drf-1.0.6/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:15:50.097078 oidc_drf-1.0.6/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.6/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      332 2023-06-30 19:04:55.000000 oidc_drf-1.0.6/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.6/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.6/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7751 2023-06-30 18:48:30.000000 oidc_drf-1.0.6/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 19:15:50.096937 oidc_drf-1.0.6/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 19:15:50.000000 oidc_drf-1.0.6/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-06-30 19:15:50.000000 oidc_drf-1.0.6/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-06-30 19:15:50.000000 oidc_drf-1.0.6/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-06-30 19:15:50.000000 oidc_drf-1.0.6/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-06-30 19:15:50.000000 oidc_drf-1.0.6/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-06-30 19:15:50.097424 oidc_drf-1.0.6/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-06-30 19:15:44.000000 oidc_drf-1.0.6/setup.py
```

### Comparing `oidc_drf-1.0.5/PKG-INFO` & `oidc_drf-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.0.5
+Version: 1.0.6
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.5/README.md` & `oidc_drf-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.5/oidc_drf/admin.py` & `oidc_drf-1.0.6/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.5/oidc_drf/backends.py` & `oidc_drf-1.0.6/oidc_drf/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         try:
             oidc_extra_data = user.oidcextradata
             oidc_extra_data.id_token = id_token
             oidc_extra_data.data = user_data
             oidc_extra_data.save()
         except OIDCExtraData.DoesNotExist:
             # Create a new OIDCExtraData object for the user
-            oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data)
+            oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data, id_token=id_token)
 
 
     
     def get_or_create_user(self, access_token, id_token, payload):
         """Returns a User instance if 1 user is found. Creates a user if not found
         and configured to do so. Returns nothing if multiple users are matched."""
```

### Comparing `oidc_drf-1.0.5/oidc_drf/drf.py` & `oidc_drf-1.0.6/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.5/oidc_drf/utils.py` & `oidc_drf-1.0.6/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.5/oidc_drf/views.py` & `oidc_drf-1.0.6/oidc_drf/views.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.5/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.0.6/oidc_drf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.0.5
+Version: 1.0.6
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.5/setup.py` & `oidc_drf-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.0.5',
+    version='1.0.6',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library',
     long_description="Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.",
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

