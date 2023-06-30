# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.924.tar", last modified: Thu Jun 29 00:31:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.925.tar", last modified: Fri Jun 30 02:13:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.924.tar` & `tencentcloud-sdk-python-ess-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259472 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    59451 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:31:04.000000 tencentcloud-sdk-python-ess-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260887 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    59451 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:13:51.000000 tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:13:50.000000 tencentcloud-sdk-python-ess-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -915,24 +915,31 @@
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param FlowIds: 需要执行撤回的签署流程id数组，最多100个
         :type FlowIds: list of str
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowIds = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowIds = params.get("FlowIds")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1419,24 +1426,31 @@
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param FlowId: 签署流程编号
         :type FlowId: str
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowId = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowId = params.get("FlowId")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1482,24 +1496,30 @@
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param FlowIds: 需要执行催办的签署流程id数组，最多100个
         :type FlowIds: list of str
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowIds = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.FlowIds = params.get("FlowIds")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3385,24 +3405,31 @@
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param ReportId: 出证报告编号
         :type ReportId: str
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.ReportId = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.ReportId = params.get("ReportId")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.924/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.925/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.924/README.rst` & `tencentcloud-sdk-python-ess-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.924/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.925/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.924/setup.py` & `tencentcloud-sdk-python-ess-3.0.925/setup.py`

 * *Files identical despite different names*

