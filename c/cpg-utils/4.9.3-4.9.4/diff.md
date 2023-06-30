# Comparing `tmp/cpg-utils-4.9.3.tar.gz` & `tmp/cpg-utils-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-4.9.3.tar", last modified: Thu Oct 20 23:04:00 2022, max compression
+gzip compressed data, was "cpg-utils-4.9.4.tar", last modified: Wed Oct 26 05:43:42 2022, max compression
```

## Comparing `cpg-utils-4.9.3.tar` & `cpg-utils-4.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 23:04:00.946134 cpg-utils-4.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-20 23:04:00.946134 cpg-utils-4.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 23:04:00.942134 cpg-utils-4.9.3/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10352 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/config-template.toml
--rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8110 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (121)    20487 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/hail_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 23:04:00.946134 cpg-utils-4.9.3/cpg_utils/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24422 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/metamist.py
--rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/status.py
--rw-r--r--   0 runner    (1001) docker     (121)    19302 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/targets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    39375 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/cpg_utils/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 23:04:00.942134 cpg-utils-4.9.3/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-20 23:04:00.000000 cpg-utils-4.9.3/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-20 23:04:00.000000 cpg-utils-4.9.3/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 23:04:00.000000 cpg-utils-4.9.3/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-20 23:04:00.000000 cpg-utils-4.9.3/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-20 23:04:00.000000 cpg-utils-4.9.3/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 23:04:00.946134 cpg-utils-4.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 23:04:00.946134 cpg-utils-4.9.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     8393 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/test/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-10-20 23:03:56.000000 cpg-utils-4.9.3/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/config-template.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8110 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20487 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/hail_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8758 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24422 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/metamist.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10250 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/slack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19302 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/targets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39375 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/cpg_utils/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-26 05:43:42.000000 cpg-utils-4.9.4/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 05:43:42.506573 cpg-utils-4.9.4/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8393 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-10-26 05:43:41.000000 cpg-utils-4.9.4/test/test_workflow.py
```

### Comparing `cpg-utils-4.9.3/LICENSE` & `cpg-utils-4.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/PKG-INFO` & `cpg-utils-4.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 4.9.3
+Version: 4.9.4
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-4.9.3/README.md` & `cpg-utils-4.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/__init__.py` & `cpg-utils-4.9.4/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/cloud.py` & `cpg-utils-4.9.4/cpg_utils/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,20 +104,22 @@
             secret_manager.disable_secret_version(request={'name': version.name})
 
 
 def get_google_identity_token(
     target_audience: str | None, request: google.auth.transport.Request = None
 ) -> str:
     """Returns a Google identity token for the given audience."""
+    if request is None:
+        request = requests.Request()
     # Unfortunately this requires different handling for at least
     # three different cases and the standard libraries don't provide
     # a single helper function that captures all of them:
     # https://github.com/googleapis/google-auth-library-python/issues/590
     creds = _get_default_id_token_credentials(target_audience, request)
-    creds.refresh(request=requests.Request())
+    creds.refresh(request)
     return creds.token
 
 
 class IDTokenCredentialsAdapter(google_auth_credentials.Credentials):
     """Convert Credentials with ``openid`` scope to IDTokenCredentials."""
 
     def __init__(self, credentials: oauth2_credentials.Credentials):
@@ -160,15 +162,15 @@
 
     # The type key should indicate that the file is either a service account
     # credentials file or an authorized user credentials file.
     credential_type = info.get('type')
 
     if credential_type == _AUTHORIZED_USER_TYPE:
         current_credentials = oauth2_credentials.Credentials.from_authorized_user_info(
-            info, scopes=['openid', 'email']
+            info, scopes=['openid', 'https://www.googleapis.com/auth/userinfo.email']
         )
         current_credentials = IDTokenCredentialsAdapter(credentials=current_credentials)
 
         return current_credentials
 
     if credential_type == _SERVICE_ACCOUNT_TYPE:
         try:
```

### Comparing `cpg-utils-4.9.3/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-4.9.4/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/config-template.toml` & `cpg-utils-4.9.4/cpg_utils/config-template.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/config.py` & `cpg-utils-4.9.4/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/git.py` & `cpg-utils-4.9.4/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/hail_batch.py` & `cpg-utils-4.9.4/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/batch.py` & `cpg-utils-4.9.4/cpg_utils/workflows/batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/filetypes.py` & `cpg-utils-4.9.4/cpg_utils/workflows/filetypes.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/inputs.py` & `cpg-utils-4.9.4/cpg_utils/workflows/inputs.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/metamist.py` & `cpg-utils-4.9.4/cpg_utils/workflows/metamist.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/resources.py` & `cpg-utils-4.9.4/cpg_utils/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/slack.py` & `cpg-utils-4.9.4/cpg_utils/workflows/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/status.py` & `cpg-utils-4.9.4/cpg_utils/workflows/status.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/targets.py` & `cpg-utils-4.9.4/cpg_utils/workflows/targets.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/utils.py` & `cpg-utils-4.9.4/cpg_utils/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils/workflows/workflow.py` & `cpg-utils-4.9.4/cpg_utils/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-4.9.4/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 4.9.3
+Version: 4.9.4
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-4.9.3/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-4.9.4/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/setup.py` & `cpg-utils-4.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='4.9.3',
+    version='4.9.4',
     description='Library of convenience functions specific to the CPG',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `cpg-utils-4.9.3/test/test_batch.py` & `cpg-utils-4.9.4/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/test/test_cohort.py` & `cpg-utils-4.9.4/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/test/test_status.py` & `cpg-utils-4.9.4/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-4.9.3/test/test_workflow.py` & `cpg-utils-4.9.4/test/test_workflow.py`

 * *Files identical despite different names*

