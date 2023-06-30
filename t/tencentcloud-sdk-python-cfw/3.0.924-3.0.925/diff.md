# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.924.tar", last modified: Thu Jun 29 00:26:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.925.tar", last modified: Fri Jun 30 02:03:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.924.tar` & `tencentcloud-sdk-python-cfw-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224528 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)    67446 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:26:29.000000 tencentcloud-sdk-python-cfw-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224910 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)    67446 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:03:00.000000 tencentcloud-sdk-python-cfw-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1996,34 +1996,38 @@
         :type Data: list of BlockIgnoreRule
         :param Total: 查询结果总数，用于分页
         :type Total: int
         :param ReturnCode: 状态值，0：查询成功，非0：查询失败
         :type ReturnCode: int
         :param ReturnMsg: 状态信息，success：查询成功，fail：查询失败
         :type ReturnMsg: str
+        :param SourceList: 安全事件来源下拉框
+        :type SourceList: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Data = None
         self.Total = None
         self.ReturnCode = None
         self.ReturnMsg = None
+        self.SourceList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self.Data = []
             for item in params.get("Data"):
                 obj = BlockIgnoreRule()
                 obj._deserialize(item)
                 self.Data.append(obj)
         self.Total = params.get("Total")
         self.ReturnCode = params.get("ReturnCode")
         self.ReturnMsg = params.get("ReturnMsg")
+        self.SourceList = params.get("SourceList")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeBlockStaticListRequest(AbstractModel):
     """DescribeBlockStaticList请求参数结构体
 
     """
@@ -3787,14 +3791,17 @@
         :type InsSource: str
         :param ResourcePath: [a,b]
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourcePath: list of str
         :param Server: 扫描结果
 注意：此字段可能返回 null，表示取不到有效值。
         :type Server: list of str
+        :param RegionKey: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RegionKey: str
         """
         self.AppId = None
         self.Region = None
         self.VpcId = None
         self.VPCName = None
         self.SubnetId = None
         self.InstanceId = None
@@ -3803,14 +3810,15 @@
         self.PublicIp = None
         self.PrivateIp = None
         self.PortNum = None
         self.LeakNum = None
         self.InsSource = None
         self.ResourcePath = None
         self.Server = None
+        self.RegionKey = None
 
 
     def _deserialize(self, params):
         self.AppId = params.get("AppId")
         self.Region = params.get("Region")
         self.VpcId = params.get("VpcId")
         self.VPCName = params.get("VPCName")
@@ -3821,14 +3829,15 @@
         self.PublicIp = params.get("PublicIp")
         self.PrivateIp = params.get("PrivateIp")
         self.PortNum = params.get("PortNum")
         self.LeakNum = params.get("LeakNum")
         self.InsSource = params.get("InsSource")
         self.ResourcePath = params.get("ResourcePath")
         self.Server = params.get("Server")
+        self.RegionKey = params.get("RegionKey")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.925/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/README.rst` & `tencentcloud-sdk-python-cfw-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.925/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.924/setup.py` & `tencentcloud-sdk-python-cfw-3.0.925/setup.py`

 * *Files identical despite different names*

