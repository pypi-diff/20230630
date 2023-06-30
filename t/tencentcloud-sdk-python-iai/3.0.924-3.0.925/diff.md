# Comparing `tmp/tencentcloud-sdk-python-iai-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-iai-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.924.tar", last modified: Thu Jun 29 00:32:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.925.tar", last modified: Fri Jun 30 02:15:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iai-3.0.924.tar` & `tencentcloud-sdk-python-iai-3.0.925.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175621 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/models.py
--rw-r--r--   0 root         (0) root         (0)    49376 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/iai_client.py
--rw-r--r--   0 root         (0) root         (0)    12105 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164095 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)    46159 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/iai_client.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:32:32.000000 tencentcloud-sdk-python-iai-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175629 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/models.py
+-rw-r--r--   0 root         (0) root         (0)    49375 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)    12105 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164095 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)    46159 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:15:16.000000 tencentcloud-sdk-python-iai-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud_sdk_python_iai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud_sdk_python_iai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/models.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1304,17 +1304,17 @@
     """
 
     def __init__(self):
         r"""
         :param MaxFaceNum: 最多处理的人脸数目。默认值为1（仅检测图片中面积最大的那张人脸），最大值为120。 
 此参数用于控制处理待检测图片中的人脸个数，值越小，处理速度越快。
         :type MaxFaceNum: int
-        :param MinFaceSize: 人脸长和宽的最小尺寸，单位为像素。
-默认为34。建议不低于34。
-低于MinFaceSize值的人脸不会被检测。
+        :param MinFaceSize: 人脸长和宽的最小尺寸，单位为像素，低于MinFaceSize值的人脸不会被检测。
+只支持设置34和20，建议使用34。
+
         :type MinFaceSize: int
         :param Image: 图片 base64 数据，base64 编码后大小不可超过5M。
 jpg格式长边像素不可超过4000，其他格式图片长边像素不可超2000。
 支持PNG、JPG、JPEG、BMP，不支持 GIF 图片。
         :type Image: str
         :param Url: 图片的 Url 。对应图片 base64 编码后大小不可超过5M。
 jpg格式长边像素不可超过4000，其他格式图片长边像素不可超2000。
```

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/iai_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,14 @@
         3） [人脸验证](https://cloud.tencent.com/document/product/867/44983)：保证人脸信息的质量，避免明明是本人却认证不通过的情况。
 
         4） 人脸融合：保证上传的人脸质量，人脸融合的效果更好。
 
         >
         - 公共参数中的签名方式请使用V3版本，即配置SignatureMethod参数为TC3-HMAC-SHA256。
 
-
         :param request: Request instance for DetectFace.
         :type request: :class:`tencentcloud.iai.v20200303.models.DetectFaceRequest`
         :rtype: :class:`tencentcloud.iai.v20200303.models.DetectFaceResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20200303/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20200303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/models.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/tencentcloud/iai/v20180301/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.925/tencentcloud/iai/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/README.rst` & `tencentcloud-sdk-python-iai-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.925/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.924/setup.py` & `tencentcloud-sdk-python-iai-3.0.925/setup.py`

 * *Files identical despite different names*

