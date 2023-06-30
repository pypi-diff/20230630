# Comparing `tmp/antchain_mytc-1.6.0.tar.gz` & `tmp/antchain_mytc-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_mytc-1.6.0.tar", last modified: Thu Jun 29 06:54:49 2023, max compression
+gzip compressed data, was "dist/antchain_mytc-1.6.2.tar", last modified: Fri Jun 30 09:39:13 2023, max compression
```

## Comparing `antchain_mytc-1.6.0.tar` & `antchain_mytc-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_mytc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_sdk_mytc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_sdk_mytc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86735 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_sdk_mytc/client.py
--rw-r--r--   0 root         (0) root         (0)   157796 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/antchain_sdk_mytc/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-29 06:54:49.000000 antchain_mytc-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_mytc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86735 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/client.py
+-rw-r--r--   0 root         (0) root         (0)   158210 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/antchain_sdk_mytc/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 09:39:13.000000 antchain_mytc-1.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-30 09:39:12.000000 antchain_mytc-1.6.2/setup.py
```

### Comparing `antchain_mytc-1.6.0/LICENSE` & `antchain_mytc-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.0/PKG-INFO` & `antchain_mytc-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_mytc
-Version: 1.6.0
+Version: 1.6.2
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.6.0/README-CN.md` & `antchain_mytc-1.6.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.0/README.md` & `antchain_mytc-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.6.0/antchain_mytc.egg-info/PKG-INFO` & `antchain_mytc-1.6.2/antchain_mytc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-mytc
-Version: 1.6.0
+Version: 1.6.2
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.6.0/antchain_sdk_mytc/client.py` & `antchain_mytc-1.6.2/antchain_sdk_mytc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.0',
+                    'sdk_version': '1.6.2',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.6.0',
+                    'sdk_version': '1.6.2',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_mytc-1.6.0/antchain_sdk_mytc/models.py` & `antchain_mytc-1.6.2/antchain_sdk_mytc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,24 +1327,29 @@
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         device_type: str = None,
         unflashed_file_id: str = None,
         flashed_file_id: str = None,
+        file_type: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 设备型号
         self.device_type = device_type
         # 未闪光图片的fileId
         self.unflashed_file_id = unflashed_file_id
         # 闪光后图片fileId
         self.flashed_file_id = flashed_file_id
+        # 上传文件类型，默认为id。
+        # id标识通过网关上传，参数为网关的fileId。
+        # url标识上传的为图片可访问链接。
+        self.file_type = file_type
 
     def validate(self):
         self.validate_required(self.unflashed_file_id, 'unflashed_file_id')
         self.validate_required(self.flashed_file_id, 'flashed_file_id')
 
     def to_map(self):
         _map = super().to_map()
@@ -1358,28 +1363,32 @@
             result['product_instance_id'] = self.product_instance_id
         if self.device_type is not None:
             result['device_type'] = self.device_type
         if self.unflashed_file_id is not None:
             result['unflashed_file_id'] = self.unflashed_file_id
         if self.flashed_file_id is not None:
             result['flashed_file_id'] = self.flashed_file_id
+        if self.file_type is not None:
+            result['file_type'] = self.file_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('device_type') is not None:
             self.device_type = m.get('device_type')
         if m.get('unflashed_file_id') is not None:
             self.unflashed_file_id = m.get('unflashed_file_id')
         if m.get('flashed_file_id') is not None:
             self.flashed_file_id = m.get('flashed_file_id')
+        if m.get('file_type') is not None:
+            self.file_type = m.get('file_type')
         return self
 
 
 class JudgeCodeFakescreenResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_mytc-1.6.0/setup.py` & `antchain_mytc-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_mytc.
 
-Created on 29/06/2023
+Created on 30/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_mytc"
 NAME = "antchain_mytc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain MYTC SDK Library for Python"
```

