# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.924.tar", last modified: Thu Jun 29 00:45:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.925.tar", last modified: Fri Jun 30 02:23:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.924.tar` & `tencentcloud-sdk-python-tcss-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1047353 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/models.py
--rw-r--r--   0 root         (0) root         (0)   317082 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-29 00:45:22.000000 tencentcloud-sdk-python-tcss-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1047619 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/models.py
+-rw-r--r--   0 root         (0) root         (0)   317082 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-30 02:23:01.000000 tencentcloud-sdk-python-tcss-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-30 02:23:00.000000 tencentcloud-sdk-python-tcss-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3447,22 +3447,27 @@
         r"""
         :param DockerVersion: 主机上的Docker版本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DockerVersion: str
         :param K8SVersion: 主机上的K8S的版本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type K8SVersion: str
+        :param ContainerdVersion: 主机上Containerd版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ContainerdVersion: str
         """
         self.DockerVersion = None
         self.K8SVersion = None
+        self.ContainerdVersion = None
 
 
     def _deserialize(self, params):
         self.DockerVersion = params.get("DockerVersion")
         self.K8SVersion = params.get("K8SVersion")
+        self.ContainerdVersion = params.get("ContainerdVersion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.925/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/README.rst` & `tencentcloud-sdk-python-tcss-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.925/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.924/setup.py` & `tencentcloud-sdk-python-tcss-3.0.925/setup.py`

 * *Files identical despite different names*

