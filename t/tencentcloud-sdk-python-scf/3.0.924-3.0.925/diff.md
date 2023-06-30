# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.924.tar", last modified: Thu Jun 29 00:40:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.925.tar", last modified: Fri Jun 30 02:20:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.924.tar` & `tencentcloud-sdk-python-scf-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191703 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    42711 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:40:45.000000 tencentcloud-sdk-python-scf-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   192210 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:20:18.000000 tencentcloud-sdk-python-scf-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-scf-3.0.924/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.925/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,14 +566,18 @@
         :type InitTimeout: int
         :param Tags: 函数 Tag 参数，以键值对数组形式传入
         :type Tags: list of Tag
         :param AsyncRunEnable: 是否开启异步属性，TRUE 为开启，FALSE为关闭
         :type AsyncRunEnable: str
         :param TraceEnable: 是否开启事件追踪，TRUE 为开启，FALSE为关闭
         :type TraceEnable: str
+        :param AutoDeployClsTopicIndex: 是否自动创建cls索引，TRUE 为开启，FALSE为关闭
+        :type AutoDeployClsTopicIndex: str
+        :param AutoCreateClsTopic: 是否自动创建cls主题，TRUE 为开启，FALSE为关闭
+        :type AutoCreateClsTopic: str
         :param ProtocolType: HTTP函数支持的访问协议。当前支持WebSockets协议，值为WS
         :type ProtocolType: str
         :param ProtocolParams: HTTP函数配置ProtocolType访问协议，当前协议可配置的参数
         :type ProtocolParams: :class:`tencentcloud.scf.v20180416.models.ProtocolParams`
         :param InstanceConcurrencyConfig: 单实例多并发配置。只支持Web函数。
         :type InstanceConcurrencyConfig: :class:`tencentcloud.scf.v20180416.models.InstanceConcurrencyConfig`
         """
@@ -597,14 +601,16 @@
         self.DeadLetterConfig = None
         self.PublicNetConfig = None
         self.CfsConfig = None
         self.InitTimeout = None
         self.Tags = None
         self.AsyncRunEnable = None
         self.TraceEnable = None
+        self.AutoDeployClsTopicIndex = None
+        self.AutoCreateClsTopic = None
         self.ProtocolType = None
         self.ProtocolParams = None
         self.InstanceConcurrencyConfig = None
 
 
     def _deserialize(self, params):
         self.FunctionName = params.get("FunctionName")
@@ -649,14 +655,16 @@
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.AsyncRunEnable = params.get("AsyncRunEnable")
         self.TraceEnable = params.get("TraceEnable")
+        self.AutoDeployClsTopicIndex = params.get("AutoDeployClsTopicIndex")
+        self.AutoCreateClsTopic = params.get("AutoCreateClsTopic")
         self.ProtocolType = params.get("ProtocolType")
         if params.get("ProtocolParams") is not None:
             self.ProtocolParams = ProtocolParams()
             self.ProtocolParams._deserialize(params.get("ProtocolParams"))
         if params.get("InstanceConcurrencyConfig") is not None:
             self.InstanceConcurrencyConfig = InstanceConcurrencyConfig()
             self.InstanceConcurrencyConfig._deserialize(params.get("InstanceConcurrencyConfig"))
```

### Comparing `tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.924/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.925/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.924/README.rst` & `tencentcloud-sdk-python-scf-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.925/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.924/setup.py` & `tencentcloud-sdk-python-scf-3.0.925/setup.py`

 * *Files identical despite different names*

