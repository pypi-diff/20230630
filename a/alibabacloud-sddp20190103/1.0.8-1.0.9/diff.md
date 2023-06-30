# Comparing `tmp/alibabacloud_sddp20190103-1.0.8.tar.gz` & `tmp/alibabacloud_sddp20190103-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sddp20190103-1.0.8.tar", last modified: Wed May 25 11:04:45 2022, max compression
+gzip compressed data, was "dist/alibabacloud_sddp20190103-1.0.9.tar", last modified: Thu Jun 29 09:37:43 2023, max compression
```

## Comparing `alibabacloud_sddp20190103-1.0.8.tar` & `alibabacloud_sddp20190103-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 11:04:45.000000 alibabacloud_sddp20190103-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2369 2022-05-25 11:04:45.000000 alibabacloud_sddp20190103-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 11:04:45.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146714 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103/client.py
--rw-r--r--   0 root         (0) root         (0)   290167 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 11:04:45.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2369 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-25 11:04:45.000000 alibabacloud_sddp20190103-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2022-05-25 11:04:44.000000 alibabacloud_sddp20190103-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   218342 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103/client.py
+-rw-r--r--   0 root         (0) root         (0)   426743 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-29 09:37:43.000000 alibabacloud_sddp20190103-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-06-29 09:37:42.000000 alibabacloud_sddp20190103-1.0.9/setup.py
```

### Comparing `alibabacloud_sddp20190103-1.0.8/LICENSE` & `alibabacloud_sddp20190103-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.0.8/PKG-INFO` & `alibabacloud_sddp20190103-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sddp20190103
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sddp20190103-1.0.8/README-CN.md` & `alibabacloud_sddp20190103-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.0.8/README.md` & `alibabacloud_sddp20190103-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.0.8/alibabacloud_sddp20190103.egg-info/PKG-INFO` & `alibabacloud_sddp20190103-1.0.9/alibabacloud_sddp20190103.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sddp20190103
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sddp20190103-1.0.8/setup.py` & `alibabacloud_sddp20190103-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sddp20190103.
 
-Created on 25/05/2022
+Created on 29/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sddp20190103"
 NAME = "alibabacloud_sddp20190103" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

