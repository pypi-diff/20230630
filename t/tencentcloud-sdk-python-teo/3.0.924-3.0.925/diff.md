# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.924.tar", last modified: Thu Jun 29 00:45:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.925.tar", last modified: Fri Jun 30 02:23:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.924.tar` & `tencentcloud-sdk-python-teo-3.0.925.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   513081 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    84601 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    22107 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:45:57.000000 tencentcloud-sdk-python-teo-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   513081 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    84601 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    22107 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:23:38.000000 tencentcloud-sdk-python-teo-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/README.rst` & `tencentcloud-sdk-python-teo-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.925/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.924/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.925/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.924/setup.py` & `tencentcloud-sdk-python-teo-3.0.925/setup.py`

 * *Files identical despite different names*

