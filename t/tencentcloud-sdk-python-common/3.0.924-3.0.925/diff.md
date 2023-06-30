# Comparing `tmp/tencentcloud-sdk-python-common-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-common-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.924.tar", last modified: Thu Jun 29 00:27:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-common-3.0.925.tar", last modified: Fri Jun 30 02:04:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-common-3.0.924.tar` & `tencentcloud-sdk-python-common-3.0.925.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15666 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/http/request.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/abstract_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/common_client.py
--rw-r--r--   0 root         (0) root         (0)    18549 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/sign.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:27:52.000000 tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15666 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/common_client.py
+-rw-r--r--   0 root         (0) root         (0)    18594 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/sign.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      837 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:04:24.000000 tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.924'
+__version__ = '3.0.925'
```

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/credential.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/http/request.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/abstract_model.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/exception/__init__.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/http_profile.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/profile/client_profile.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/common_client.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/abstract_client.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/abstract_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from tencentcloud.common.exception.tencent_cloud_sdk_exception import TencentCloudSDKException
 from tencentcloud.common.exception import TencentCloudSDKException as SDKError
 from tencentcloud.common.http.request import ApiRequest
 from tencentcloud.common.http.request import RequestInternal
 from tencentcloud.common.profile.client_profile import ClientProfile
 from tencentcloud.common.sign import Sign
 
-warnings.filterwarnings("ignore")
+warnings.filterwarnings("ignore", module="tencentcloud", category=UserWarning)
 
 _json_content = 'application/json'
 _multipart_content = 'multipart/form-data'
 _form_urlencoded_content = 'application/x-www-form-urlencoded'
 _octet_stream = "application/octet-stream"
```

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud/common/sign.py` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/README.rst` & `tencentcloud-sdk-python-common-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.925/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-common-3.0.924/setup.py` & `tencentcloud-sdk-python-common-3.0.925/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-common-3.0.924/tencentcloud_sdk_python_common.egg-info/PKG-INFO` & `tencentcloud-sdk-python-common-3.0.925/tencentcloud_sdk_python_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-common
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Common SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

