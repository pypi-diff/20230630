# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.924.tar", last modified: Thu Jun 29 00:20:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.925.tar", last modified: Fri Jun 30 01:59:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.924.tar` & `tencentcloud-sdk-python-apigateway-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95979 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)   408275 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    20869 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-29 00:20:20.000000 tencentcloud-sdk-python-apigateway-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95979 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)   408275 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    21272 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 01:59:44.000000 tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-30 01:59:43.000000 tencentcloud-sdk-python-apigateway-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,23 +445,29 @@
 
 # 账号余额不足
 UNSUPPORTEDOPERATION_ACCOUNTARREARS = 'UnsupportedOperation.AccountArrears'
 
 # 密钥已绑定使用计划。
 UNSUPPORTEDOPERATION_ALREADYBINDUSAGEPLAN = 'UnsupportedOperation.AlreadyBindUsagePlan'
 
+# API列表不为空
+UNSUPPORTEDOPERATION_APILISTNOTEMPTY = 'UnsupportedOperation.ApiListNotEmpty'
+
 # 当前插件不支持绑定。
 UNSUPPORTEDOPERATION_ATTACHPLUGIN = 'UnsupportedOperation.AttachPlugin'
 
 # 基础版服务不能创建超过一个API。
 UNSUPPORTEDOPERATION_BASICSERVICENOMOREAPI = 'UnsupportedOperation.BasicServiceNoMoreApi'
 
 # 日志检索起始时间间隔。
 UNSUPPORTEDOPERATION_CLSSEARCHTIME = 'UnsupportedOperation.ClsSearchTime'
 
+# 存在现网环境
+UNSUPPORTEDOPERATION_EXISTINGONLINEENVIRONMENT = 'UnsupportedOperation.ExistingOnlineEnvironment'
+
 # 协议为HTTP时，不支持强制Https。
 UNSUPPORTEDOPERATION_FORCEHTTPS = 'UnsupportedOperation.ForceHttps'
 
 # 接口错误。
 UNSUPPORTEDOPERATION_INVALIDACTION = 'UnsupportedOperation.InvalidAction'
 
 # 不支持后端类型。
@@ -496,17 +502,23 @@
 
 # 密钥已绑定使用计划，请先解绑再试。
 UNSUPPORTEDOPERATION_RESOURCEISINUSE = 'UnsupportedOperation.ResourceIsInUse'
 
 # 资源未关联。
 UNSUPPORTEDOPERATION_RESOURCEUNASSOCIATED = 'UnsupportedOperation.ResourceUnassociated'
 
+# 标签不为空
+UNSUPPORTEDOPERATION_TAGSNOTEMPTY = 'UnsupportedOperation.TagsNotEmpty'
+
 # 当前Uin未在手工密钥白名单列表内。
 UNSUPPORTEDOPERATION_UINNOTINWHITELIST = 'UnsupportedOperation.UinNotInWhiteList'
 
+# Unpack函数错误
+UNSUPPORTEDOPERATION_UNPACKERROR = 'UnsupportedOperation.UnpackError'
+
 # 密钥已绑定使用计划。
 UNSUPPORTEDOPERATION_UNSUPPORTEDBINDAPIKEY = 'UnsupportedOperation.UnsupportedBindApiKey'
 
 # 不支持绑定环境。
 UNSUPPORTEDOPERATION_UNSUPPORTEDBINDENVIRONMENT = 'UnsupportedOperation.UnsupportedBindEnvironment'
 
 # 当前API已绑定业务API，请先解绑再试。
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.925/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.924/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.925/setup.py`

 * *Files identical despite different names*

