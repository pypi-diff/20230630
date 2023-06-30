# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.924.tar", last modified: Thu Jun 29 00:27:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.925.tar", last modified: Fri Jun 30 02:03:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.924.tar` & `tencentcloud-sdk-python-ckafka-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   486906 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-29 00:27:03.000000 tencentcloud-sdk-python-ckafka-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   486893 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         :param ResourceType: Acl资源类型，（0:UNKNOWN，1:ANY，2:TOPIC，3:GROUP，4:CLUSTER，5:TRANSACTIONAL_ID）当前只有TOPIC，
         :type ResourceType: int
         :param ResourceName: 资源名称，和resourceType相关如当resourceType为TOPIC时，则该字段表示topic名称，当resourceType为GROUP时，该字段表示group名称
         :type ResourceName: str
         :param Principal: 用户列表，默认为User:*，表示任何user都可以访问，当前用户只能是用户列表中包含的用户
 注意：此字段可能返回 null，表示取不到有效值。
         :type Principal: str
-        :param Host: 默认为：*，表示任何host都可以访问，当前ckafka不支持host为：*，但是后面开源kafka的产品化会直接支持
+        :param Host: 默认\*,表示任何host都可以访问，当前ckafka不支持host为\*，但是后面开源kafka的产品化会直接支持
 注意：此字段可能返回 null，表示取不到有效值。
         :type Host: str
         :param Operation: Acl操作方式(0:UNKNOWN，1:ANY，2:ALL，3:READ，4:WRITE，5:CREATE，6:DELETE，7:ALTER，8:DESCRIBE，9:CLUSTER_ACTION，10:DESCRIBE_CONFIGS，11:ALTER_CONFIGS，12:IDEMPOTEN_WRITE)
         :type Operation: int
         :param PermissionType: 权限类型(0:UNKNOWN，1:ANY，2:DENY，3:ALLOW)
         :type PermissionType: int
         """
@@ -190,15 +190,15 @@
 
     def __init__(self):
         r"""
         :param Operation: Acl操作方式，枚举值(所有操作: All, 读：Read，写：Write)
         :type Operation: str
         :param PermissionType: 权限类型，(Deny，Allow)
         :type PermissionType: str
-        :param Host: 默认为：*，表示任何host都可以访问，当前ckafka不支持host为：* 和 ip网段
+        :param Host: 默认为\*，表示任何host都可以访问，当前ckafka不支持host为\* 和 ip网段
         :type Host: str
         :param Principal: 用户列表，默认为User:*，表示任何user都可以访问，当前用户只能是用户列表中包含的用户。传入格式需要带【User:】前缀。例如用户A，传入为User:A。
         :type Principal: str
         """
         self.Operation = None
         self.PermissionType = None
         self.Host = None
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.924/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.925/setup.py`

 * *Files identical despite different names*

