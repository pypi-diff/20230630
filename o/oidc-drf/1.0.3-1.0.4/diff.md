# Comparing `tmp/oidc_drf-1.0.3.tar.gz` & `tmp/oidc_drf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.0.3.tar", last modified: Thu Jun 22 18:22:07 2023, max compression
+gzip compressed data, was "oidc_drf-1.0.4.tar", last modified: Fri Jun 30 18:51:00 2023, max compression
```

## Comparing `oidc_drf-1.0.3.tar` & `oidc_drf-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-22 18:22:07.783013 oidc_drf-1.0.3/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-22 18:22:07.782847 oidc_drf-1.0.3/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     1428 2023-06-22 18:20:26.000000 oidc_drf-1.0.3/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-22 18:22:07.781379 oidc_drf-1.0.3/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.3/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-06-21 20:00:07.000000 oidc_drf-1.0.3/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15520 2023-06-21 20:00:07.000000 oidc_drf-1.0.3/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4589 2023-06-21 20:00:07.000000 oidc_drf-1.0.3/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-22 18:22:07.782659 oidc_drf-1.0.3/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.3/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-06-21 19:29:58.000000 oidc_drf-1.0.3/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.3/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.3/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     7926 2023-06-22 18:20:07.000000 oidc_drf-1.0.3/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-22 18:22:07.782432 oidc_drf-1.0.3/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-22 18:22:07.000000 oidc_drf-1.0.3/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-06-22 18:22:07.000000 oidc_drf-1.0.3/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-06-22 18:22:07.000000 oidc_drf-1.0.3/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-06-22 18:22:07.000000 oidc_drf-1.0.3/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-06-22 18:22:07.000000 oidc_drf-1.0.3/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-06-22 18:22:07.783053 oidc_drf-1.0.3/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-06-22 18:20:14.000000 oidc_drf-1.0.3/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 18:51:00.293932 oidc_drf-1.0.4/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 18:51:00.293766 oidc_drf-1.0.4/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4286 2023-06-22 20:44:43.000000 oidc_drf-1.0.4/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 18:51:00.292764 oidc_drf-1.0.4/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.4/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-06-21 20:00:07.000000 oidc_drf-1.0.4/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15595 2023-06-30 18:46:33.000000 oidc_drf-1.0.4/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4589 2023-06-21 20:00:07.000000 oidc_drf-1.0.4/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 18:51:00.293577 oidc_drf-1.0.4/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.4/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      312 2023-06-30 18:45:59.000000 oidc_drf-1.0.4/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.4/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.4/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7751 2023-06-30 18:48:30.000000 oidc_drf-1.0.4/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-06-30 18:51:00.293461 oidc_drf-1.0.4/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-06-30 18:51:00.000000 oidc_drf-1.0.4/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-06-30 18:51:00.000000 oidc_drf-1.0.4/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-06-30 18:51:00.000000 oidc_drf-1.0.4/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-06-30 18:51:00.000000 oidc_drf-1.0.4/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-06-30 18:51:00.000000 oidc_drf-1.0.4/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-06-30 18:51:00.293970 oidc_drf-1.0.4/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-06-30 18:50:01.000000 oidc_drf-1.0.4/setup.py
```

### Comparing `oidc_drf-1.0.3/PKG-INFO` & `oidc_drf-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.3/oidc_drf/admin.py` & `oidc_drf-1.0.4/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.3/oidc_drf/backends.py` & `oidc_drf-1.0.4/oidc_drf/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,21 +222,22 @@
         user_json = {**user_info_json, **decoded_access_token, **decoded_id_token}
         
         # Remove excluded fields from decoded id_token
         user_json = {key: value for key, value in user_json.items() if key not in excluded_fields}
         
         return user_json
     
-    def save_user_data(self,user, user_json):
+    def save_user_data(self,user, user_json,id_token):
         # Serialize the remaining user_json
         user_data = json.dumps(user_json)
 
         # Check if the user's OIDCExtraData already exists
         try:
             oidc_extra_data = user.oidcextradata
+            oidc_extra_data.id_token = id_token
             oidc_extra_data.data = user_data
             oidc_extra_data.save()
         except OIDCExtraData.DoesNotExist:
             # Create a new OIDCExtraData object for the user
             oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data)
 
 
@@ -254,27 +255,27 @@
         users = self.filter_users_by_claims(user_info)
 
         if len(users) == 1:
             user = self.update_user(users[0], user_info)
             
             if user_info and access_token and id_token:
                 user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json)
+                self.save_user_data(user, user_json,id_token)
             return user
 
         elif len(users) > 1:
             # In the rare case that two user accounts have the same email address,
             # bail. Randomly selecting one seems really wrong.
             msg = "Multiple users returned"
             raise SuspiciousOperation(msg)
         elif import_from_settings("OIDC_CREATE_USER", True):
             user = self.create_user(user_info)
             if user_info and access_token and id_token:
                 user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json)
+                self.save_user_data(user, user_json,id_token)
 
 
             return user
         else:
             LOGGER.debug(
                 "Login failed: No user with %s found, and " "OIDC_CREATE_USER is False",
                 self.describe_user_by_claims(user_info),
```

### Comparing `oidc_drf-1.0.3/oidc_drf/drf.py` & `oidc_drf-1.0.4/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.3/oidc_drf/utils.py` & `oidc_drf-1.0.4/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.3/oidc_drf/views.py` & `oidc_drf-1.0.4/oidc_drf/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,17 @@
         
         data = {
             'access': str(oidc_access_token),
             'refresh': str(oidc_refresh_token),
             'oidc_id_token': str(oidc_id_token),
         } 
         
-        
-        if not import_from_settings("OIDC_STORE_ACCESS_TOKEN", False):
-            del self.request.session["oidc_access_token"]
-
-        if not import_from_settings("OIDC_STORE_ID_TOKEN", False):
-            del self.request.session["oidc_id_token"]
-
-        if not import_from_settings("OIDC_STORE_REFRESH_TOKEN", False):
-            del self.request.session["oidc_refresh_token"]
-        
+        del self.request.session["oidc_access_token"]
+        del self.request.session["oidc_id_token"]
+        del self.request.session["oidc_refresh_token"]
         self.request.session.save()
 
            
         return JsonResponse(data)
     
 
 
@@ -127,18 +120,20 @@
             if self.user and self.user.is_active:
                 return self.login_success()
         
         return self.login_failure()
 
 class OIDCLogoutView(APIView):
     permission_classes = [AllowAny]    
+    
+    
 
     def post(self, request):     
-        oidc_id_token = request.data.get('oidcIdToken', '')
-    
+        # oidc_id_token = request.data.get('oidcIdToken', '')
+        oidc_id_token = request.user.oidcextradata.id_token
         if oidc_id_token:
             
             logout_endpoint = import_from_settings("OIDC_OP_LOGOUT_ENDPOINT", "")
             post_logout_redirect_uri = import_from_settings("OIDC_LOGOUT_REDIRECT_URL", "http://localhost:3000")
             
             headers = {
                 'Content-Type': 'application/x-www-form-urlencoded',
```

### Comparing `oidc_drf-1.0.3/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.0.4/oidc_drf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.3/setup.py` & `oidc_drf-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.0.3',
+    version='1.0.4',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library',
     long_description="Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.",
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

