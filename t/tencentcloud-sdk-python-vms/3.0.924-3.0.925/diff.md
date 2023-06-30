# Comparing `tmp/tencentcloud-sdk-python-vms-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-vms-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vms-3.0.924.tar", last modified: Thu Jun 29 00:49:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vms-3.0.925.tar", last modified: Fri Jun 30 02:26:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vms-3.0.924.tar` & `tencentcloud-sdk-python-vms-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6878 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/models.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/vms_client.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:49:40.000000 tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6878 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/models.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/vms_client.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:26:06.000000 tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vms-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vms-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/models.py` & `tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/vms_client.py` & `tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/vms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.924/tencentcloud/vms/v20200902/errorcodes.py` & `tencentcloud-sdk-python-vms-3.0.925/tencentcloud/vms/v20200902/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 
 # 访问上下游模块超时。
 FAILEDOPERATION_ACCESSUPSTREAMTIMEOUT = 'FailedOperation.AccessUpstreamTimeout'
 
 # 语音内容中含有敏感词，请[联系我们](https://cloud.tencent.com/document/product/1128/37720)沟通解决。
 FAILEDOPERATION_CONTAINSENSITIVEWORD = 'FailedOperation.ContainSensitiveWord'
 
-# 后端请求包解析失败，通常由于没有遵守 API 接口说明规范导致的，请参见[1004错误详解](https://cloud.tencent.com/document/product/1128/38004#Q7)。
+# 后端请求包解析失败，通常由于没有遵守 API 接口说明规范导致的，请参见[1004错误详解](https://cloud.tencent.com/document/product/1128/38004#Q5)。
 FAILEDOPERATION_FAILRESOLVEPACKET = 'FailedOperation.FailResolvePacket'
 
-# 套餐包余量不足，请及时[购买语音套餐包](https://cloud.tencent.com/document/product/1128#buyPackage)。
+# 套餐包余量不足，请及时[购买语音套餐包](https://cloud.tencent.com/document/product/1128/90745)。
 FAILEDOPERATION_INSUFFICIENTBALANCEINVOICEPACKAGE = 'FailedOperation.InsufficientBalanceInVoicePackage'
 
 # 无效 JSON，请核查发送的请求是否为标准的 JSON 格式。
 FAILEDOPERATION_INVALIDJSONPARAMETERS = 'FailedOperation.InvalidJsonParameters'
 
 # 无效参数，请核查发送的请求参数是否为对应 API 所需参数。
 FAILEDOPERATION_INVALIDPARAMETERS = 'FailedOperation.InvalidParameters'
 
 # 解析请求包体时候失败。
 FAILEDOPERATION_JSONPARSEFAIL = 'FailedOperation.JsonParseFail'
 
 # 语音未知错误，请[联系我们](https://cloud.tencent.com/document/product/1128/37720)沟通解决。
 FAILEDOPERATION_PARAMETERSOTHERERROR = 'FailedOperation.ParametersOtherError'
 
-# 未申请号码或申请的号码资源已过期，请及时支付月功能费用和信息服务费用，具体操作请参见[购买指南](https://cloud.tencent.com/document/product/1128)。
+# 未申请号码或申请的号码资源已过期，请及时支付月功能费用和信息服务费用，具体操作请参见[购买指南](https://cloud.tencent.com/document/product/1128/90745)。
 FAILEDOPERATION_PHONENUMBERUNAPPLIEDOREXPIRED = 'FailedOperation.PhonenumberUnappliedOrExpired'
 
-# 模板未审核或请求的内容与审核通过的模板内容不匹配，请参见[1014错误详解](https://cloud.tencent.com/document/product/1128/38004
+# 模板未审核或请求的内容与审核通过的模板内容不匹配，请参见[1014错误详解](https://cloud.tencent.com/document/product/1128/38004#Q7)
 FAILEDOPERATION_TEMPLATEINCORRECTORUNAPPROVED = 'FailedOperation.TemplateIncorrectOrUnapproved'
 
 # 访问上游超时网络，请稍后重试。
 INTERNALERROR_ACCESSUPSTREAMTIMEOUT = 'InternalError.AccessUpstreamTimeout'
 
 # 请求发起时间不正常，通常由您的服务器与腾讯云服务器之间的时间差超过10分钟引起。
 INTERNALERROR_REQUESTTIMEEXCEPTION = 'InternalError.RequestTimeException'
```

### Comparing `tencentcloud-sdk-python-vms-3.0.924/README.rst` & `tencentcloud-sdk-python-vms-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-vms-3.0.925/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vms
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Vms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vms-3.0.924/setup.py` & `tencentcloud-sdk-python-vms-3.0.925/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vms-3.0.924/tencentcloud_sdk_python_vms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vms-3.0.925/tencentcloud_sdk_python_vms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vms
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Vms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

