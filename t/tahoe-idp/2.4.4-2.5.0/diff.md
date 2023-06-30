# Comparing `tmp/tahoe-idp-2.4.4.tar.gz` & `tmp/tahoe-idp-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoe-idp-2.4.4.tar", last modified: Thu Jun 29 16:42:01 2023, max compression
+gzip compressed data, was "tahoe-idp-2.5.0.tar", last modified: Fri Jun 30 18:25:38 2023, max compression
```

## Comparing `tahoe-idp-2.4.4.tar` & `tahoe-idp-2.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:01.825171 tahoe-idp-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-29 16:42:01.825171 tahoe-idp-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-29 16:42:01.825171 tahoe-idp-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:01.821171 tahoe-idp-2.4.4/tahoe_idp/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/magiclink_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/magiclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/magiclink_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/magiclink_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:01.825171 tahoe-idp-2.4.4/tahoe_idp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/migrations/0002_allow_null_redirect_url.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:01.825171 tahoe-idp-2.4.4/tahoe_idp/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/settings/cms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/settings/common_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/settings/lms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 16:41:50.000000 tahoe-idp-2.4.4/tahoe_idp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:01.821171 tahoe-idp-2.4.4/tahoe_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-29 16:42:01.000000 tahoe-idp-2.4.4/tahoe_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-29 16:42:01.000000 tahoe-idp-2.4.4/tahoe_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:42:01.000000 tahoe-idp-2.4.4/tahoe_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 16:42:01.000000 tahoe-idp-2.4.4/tahoe_idp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 16:42:01.000000 tahoe-idp-2.4.4/tahoe_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:38.259781 tahoe-idp-2.5.0/tahoe_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/magiclink_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/magiclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/magiclink_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/magiclink_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/tahoe_idp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/migrations/0002_allow_null_redirect_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/tahoe_idp/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/settings/cms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/settings/common_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/settings/lms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 18:25:27.000000 tahoe-idp-2.5.0/tahoe_idp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:38.263780 tahoe-idp-2.5.0/tahoe_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-30 18:25:38.000000 tahoe-idp-2.5.0/tahoe_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-30 18:25:38.000000 tahoe-idp-2.5.0/tahoe_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:25:38.000000 tahoe-idp-2.5.0/tahoe_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-30 18:25:38.000000 tahoe-idp-2.5.0/tahoe_idp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 18:25:38.000000 tahoe-idp-2.5.0/tahoe_idp.egg-info/top_level.txt
```

### Comparing `tahoe-idp-2.4.4/LICENSE` & `tahoe-idp-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/PKG-INFO` & `tahoe-idp-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.4.4
+Version: 2.5.0
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.4.4/README.md` & `tahoe-idp-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/setup.cfg` & `tahoe-idp-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/setup.py` & `tahoe-idp-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/api.py` & `tahoe-idp-2.5.0/tahoe_idp/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,27 @@
  * The parameters of existing functions should change in a backward compatible way:
    - No parameters should be removed from the function
    - New parameters should have safe defaults
  * For breaking changes, new functions should be created
 """
 
 from datetime import datetime
+import logging
 import pytz
 from social_django.models import UserSocialAuth
 
 from urllib.parse import urlencode
 
 from .constants import BACKEND_NAME
 from . import helpers
 
 
+log = logging.getLogger(__name__)
+
+
 def request_password_reset(email):
     """
     Start password reset email for Username|Password Database Connection users.
     """
     api_client = helpers.get_api_client()
     client_response = api_client.forgot_password({'loginId': email})
     http_response = helpers.get_successful_fusion_auth_http_response(client_response)
@@ -60,28 +64,38 @@
     """
     if not user:
         raise ValueError('User should be provided')
 
     if user.is_anonymous:
         raise ValueError('Non-anonymous User should be provided')
 
-    social_auth_entry = UserSocialAuth.objects.get(
-        user_id=user.id, provider=BACKEND_NAME,
-    )
-    return social_auth_entry.uid
+    try:
+        social_auth_entry = UserSocialAuth.objects.get(
+            user_id=user.id, provider=BACKEND_NAME,
+        )
+        return social_auth_entry.uid
+    except UserSocialAuth.DoesNotExist:
+        # should only be an internal Appsembler admin user that was not migrated to IdP
+        log.warning(
+            'Could not find tahoe IdP id: No UserSocialAuth record connecting {} to Tahoe IdP.'.format(user.username)
+            )
+        return None
 
 
 def update_user(user, properties):
     """
     Update user properties via PATCH /api/user/{userId}.
 
     See: https://fusionauth.io/docs/v1/tech/apis/users#update-a-user
     """
     api_client = helpers.get_api_client()
     idp_user_id = get_tahoe_idp_id_by_user(user)
+    if idp_user_id is None:
+        return
+
     client_response = api_client.patch_user(
         user_id=idp_user_id,
         request=properties,
     )
     http_response = helpers.get_successful_fusion_auth_http_response(client_response)
     return http_response
```

### Comparing `tahoe-idp-2.4.4/tahoe_idp/apps.py` & `tahoe-idp-2.5.0/tahoe_idp/apps.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/backend.py` & `tahoe-idp-2.5.0/tahoe_idp/backend.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/helpers.py` & `tahoe-idp-2.5.0/tahoe_idp/helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/magiclink_backends.py` & `tahoe-idp-2.5.0/tahoe_idp/magiclink_backends.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/magiclink_helpers.py` & `tahoe-idp-2.5.0/tahoe_idp/magiclink_helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/magiclink_views.py` & `tahoe-idp-2.5.0/tahoe_idp/magiclink_views.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/migrations/0001_initial.py` & `tahoe-idp-2.5.0/tahoe_idp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/models.py` & `tahoe-idp-2.5.0/tahoe_idp/models.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/permissions.py` & `tahoe-idp-2.5.0/tahoe_idp/permissions.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/receivers.py` & `tahoe-idp-2.5.0/tahoe_idp/receivers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp/settings/common_production.py` & `tahoe-idp-2.5.0/tahoe_idp/settings/common_production.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.4.4/tahoe_idp.egg-info/PKG-INFO` & `tahoe-idp-2.5.0/tahoe_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.4.4
+Version: 2.5.0
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.4.4/tahoe_idp.egg-info/SOURCES.txt` & `tahoe-idp-2.5.0/tahoe_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

