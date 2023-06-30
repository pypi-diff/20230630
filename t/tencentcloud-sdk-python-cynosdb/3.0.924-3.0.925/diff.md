# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.924.tar", last modified: Thu Jun 29 00:28:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.925.tar", last modified: Fri Jun 30 02:05:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.924.tar` & `tencentcloud-sdk-python-cynosdb-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   415815 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)   118494 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    11292 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-29 00:28:36.000000 tencentcloud-sdk-python-cynosdb-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-29 00:28:35.000000 tencentcloud-sdk-python-cynosdb-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   416155 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)   118494 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-30 02:05:09.000000 tencentcloud-sdk-python-cynosdb-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2022,25 +2022,29 @@
 
     def __init__(self):
         r"""
         :param FlowId: 异步流程ID
         :type FlowId: int
         :param TaskId: 异步任务ID
         :type TaskId: int
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.FlowId = None
         self.TaskId = None
+        self.ProxyGroupId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.TaskId = params.get("TaskId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
         self.RequestId = params.get("RequestId")
 
 
 class CreateProxyRequest(AbstractModel):
     """CreateProxy请求参数结构体
 
     """
@@ -2120,25 +2124,29 @@
 
     def __init__(self):
         r"""
         :param FlowId: 异步流程ID
         :type FlowId: int
         :param TaskId: 异步任务ID
         :type TaskId: int
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.FlowId = None
         self.TaskId = None
+        self.ProxyGroupId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.TaskId = params.get("TaskId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
         self.RequestId = params.get("RequestId")
 
 
 class CreateResourcePackageRequest(AbstractModel):
     """CreateResourcePackage请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.925/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.924/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.925/setup.py`

 * *Files identical despite different names*

