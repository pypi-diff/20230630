# Comparing `tmp/vents-0.1.4.tar.gz` & `tmp/vents-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.1.4.tar", last modified: Tue Jun 13 13:29:09 2023, max compression
+gzip compressed data, was "vents-0.1.5.tar", last modified: Fri Jun 30 18:50:06 2023, max compression
```

## Comparing `vents-0.1.4.tar` & `vents-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.817380 vents-0.1.4/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-06-13 13:28:00.000000 vents-0.1.4/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-13 13:29:09.817480 vents-0.1.4/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-06-13 13:29:09.817940 vents-0.1.4/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-06-13 13:28:00.000000 vents-0.1.4/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.811830 vents-0.1.4/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-06-13 13:28:00.000000 vents-0.1.4/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.813426 vents-0.1.4/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      335 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     3842 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)      513 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-06-13 13:28:00.000000 vents-0.1.4/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.814746 vents-0.1.4/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-06-13 13:28:00.000000 vents-0.1.4/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.815129 vents-0.1.4/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.815684 vents-0.1.4/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.816249 vents-0.1.4/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.817215 vents-0.1.4/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-06-13 13:28:00.000000 vents-0.1.4/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.812702 vents-0.1.4/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.660574 vents-0.1.5/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-06-30 18:47:37.000000 vents-0.1.5/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-30 18:50:06.660687 vents-0.1.5/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-06-30 18:50:06.661143 vents-0.1.5/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-06-30 18:47:37.000000 vents-0.1.5/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.654784 vents-0.1.5/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-06-30 18:47:37.000000 vents-0.1.5/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.656684 vents-0.1.5/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3842 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      513 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-06-30 18:47:37.000000 vents-0.1.5/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.657980 vents-0.1.5/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-06-30 18:47:37.000000 vents-0.1.5/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.658638 vents-0.1.5/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.659324 vents-0.1.5/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1650 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.659907 vents-0.1.5/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.660442 vents-0.1.5/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-06-30 18:47:37.000000 vents-0.1.5/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.655891 vents-0.1.5/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       73 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/top_level.txt
```

### Comparing `vents-0.1.4/PKG-INFO` & `vents-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.4/setup.cfg` & `vents-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/setup.py` & `vents-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/config.py` & `vents-0.1.5/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/connections/catalog.py` & `vents-0.1.5/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/connections/connection.py` & `vents-0.1.5/vents/connections/connection.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/connections/connection_resource.py` & `vents-0.1.5/vents/connections/connection_resource.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/connections/connection_schema.py` & `vents-0.1.5/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/__init__.py` & `vents-0.1.5/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/base.py` & `vents-0.1.5/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/discord_webhook.py` & `vents-0.1.5/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/hipchat_webhook.py` & `vents-0.1.5/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/mattermost_webhook.py` & `vents-0.1.5/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/pagerduty_webhook.py` & `vents-0.1.5/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/slack_webhook.py` & `vents-0.1.5/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/notifiers/webhook.py` & `vents-0.1.5/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/aws/base.py` & `vents-0.1.5/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/aws/s3.py` & `vents-0.1.5/vents/providers/aws/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Optional
 
 from s3fs import S3FileSystem as BaseS3FileSystem
 
 from vents.providers.aws.service import AWSService
 
 
 class S3FileSystem(BaseS3FileSystem):
```

### Comparing `vents-0.1.4/vents/providers/aws/service.py` & `vents-0.1.5/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/azure/base.py` & `vents-0.1.5/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/azure/blob_storage.py` & `vents-0.1.5/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/azure/service.py` & `vents-0.1.5/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/base.py` & `vents-0.1.5/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/gcp/base.py` & `vents-0.1.5/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/gcp/gcs.py` & `vents-0.1.5/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/gcp/service.py` & `vents-0.1.5/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents/providers/kinds.py` & `vents-0.1.5/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.4/vents.egg-info/PKG-INFO` & `vents-0.1.5/vents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.4/vents.egg-info/SOURCES.txt` & `vents-0.1.5/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

