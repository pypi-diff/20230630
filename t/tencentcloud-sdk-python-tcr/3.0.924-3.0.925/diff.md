# Comparing `tmp/tencentcloud-sdk-python-tcr-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-tcr-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.924.tar", last modified: Thu Jun 29 00:45:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.925.tar", last modified: Fri Jun 30 02:22:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcr-3.0.924.tar` & `tencentcloud-sdk-python-tcr-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)   272068 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)   102647 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/tcr_client.py
--rw-r--r--   0 root         (0) root         (0)     8520 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:45:17.000000 tencentcloud-sdk-python-tcr-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   269587 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)   100588 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/tcr_client.py
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:22:55.000000 tencentcloud-sdk-python-tcr-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.925/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,63 +567,14 @@
 
 
     def _deserialize(self, params):
         self.RegistryId = params.get("RegistryId")
         self.RequestId = params.get("RequestId")
 
 
-class CreateImageLifecyclePersonalRequest(AbstractModel):
-    """CreateImageLifecyclePersonal请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RepoName: 仓库名称
-        :type RepoName: str
-        :param Type: keep_last_days:保留最近几天的数据;keep_last_nums:保留最近多少个
-        :type Type: str
-        :param Val: 策略值
-        :type Val: int
-        """
-        self.RepoName = None
-        self.Type = None
-        self.Val = None
-
-
-    def _deserialize(self, params):
-        self.RepoName = params.get("RepoName")
-        self.Type = params.get("Type")
-        self.Val = params.get("Val")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CreateImageLifecyclePersonalResponse(AbstractModel):
-    """CreateImageLifecyclePersonal返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
-
-
 class CreateImmutableTagRulesRequest(AbstractModel):
     """CreateImmutableTagRules请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1868,55 +1819,14 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
-        """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
-
-
-class DeleteImageLifecyclePersonalRequest(AbstractModel):
-    """DeleteImageLifecyclePersonal请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RepoName: 仓库名称
-        :type RepoName: str
-        """
-        self.RepoName = None
-
-
-    def _deserialize(self, params):
-        self.RepoName = params.get("RepoName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DeleteImageLifecyclePersonalResponse(AbstractModel):
-    """DeleteImageLifecyclePersonal返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,39 +183,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def CreateImageLifecyclePersonal(self, request):
-        """前端与现有逻辑均不再使用，可下线
-
-        用于在个人版中创建清理策略
-
-        :param request: Request instance for CreateImageLifecyclePersonal.
-        :type request: :class:`tencentcloud.tcr.v20190924.models.CreateImageLifecyclePersonalRequest`
-        :rtype: :class:`tencentcloud.tcr.v20190924.models.CreateImageLifecyclePersonalResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("CreateImageLifecyclePersonal", params, headers=headers)
-            response = json.loads(body)
-            model = models.CreateImageLifecyclePersonalResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def CreateImmutableTagRules(self, request):
         """创建镜像不可变规则
 
         :param request: Request instance for CreateImmutableTagRules.
         :type request: :class:`tencentcloud.tcr.v20190924.models.CreateImmutableTagRulesRequest`
         :rtype: :class:`tencentcloud.tcr.v20190924.models.CreateImmutableTagRulesResponse`
 
@@ -735,39 +710,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DeleteImageLifecyclePersonal(self, request):
-        """前端与后端目前现有逻辑均不再使用，可下线
-
-        用于在个人版镜像仓库中删除仓库Tag自动清理策略
-
-        :param request: Request instance for DeleteImageLifecyclePersonal.
-        :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImageLifecyclePersonalRequest`
-        :rtype: :class:`tencentcloud.tcr.v20190924.models.DeleteImageLifecyclePersonalResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DeleteImageLifecyclePersonal", params, headers=headers)
-            response = json.loads(body)
-            model = models.DeleteImageLifecyclePersonalResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteImagePersonal(self, request):
         """用于在个人版中删除tag
 
         :param request: Request instance for DeleteImagePersonal.
         :type request: :class:`tencentcloud.tcr.v20190924.models.DeleteImagePersonalRequest`
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-tcr-3.0.925/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/README.rst` & `tencentcloud-sdk-python-tcr-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.925/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.924/setup.py` & `tencentcloud-sdk-python-tcr-3.0.925/setup.py`

 * *Files identical despite different names*

