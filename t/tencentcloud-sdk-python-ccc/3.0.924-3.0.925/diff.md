# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.924.tar", last modified: Thu Jun 29 00:25:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.925.tar", last modified: Fri Jun 30 02:02:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.924.tar` & `tencentcloud-sdk-python-ccc-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142398 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)    36406 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:25:44.000000 tencentcloud-sdk-python-ccc-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143030 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:02:12.000000 tencentcloud-sdk-python-ccc-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,24 +756,32 @@
         r"""
         :param SdkAppId: TCCC 实例应用 ID
         :type SdkAppId: int
         :param ExtensionId: 分机号
         :type ExtensionId: str
         :param ExtensionName: 分机名称
         :type ExtensionName: str
+        :param SkillGroupIds: 绑定的技能组列表
+        :type SkillGroupIds: list of int non-negative
+        :param Relation: 绑定的坐席邮箱
+        :type Relation: str
         """
         self.SdkAppId = None
         self.ExtensionId = None
         self.ExtensionName = None
+        self.SkillGroupIds = None
+        self.Relation = None
 
 
     def _deserialize(self, params):
         self.SdkAppId = params.get("SdkAppId")
         self.ExtensionId = params.get("ExtensionId")
         self.ExtensionName = params.get("ExtensionName")
+        self.SkillGroupIds = params.get("SkillGroupIds")
+        self.Relation = params.get("Relation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4018,14 +4026,17 @@
         :type Remark: str
         :param QueuedSkillGroupName: 排队技能组名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type QueuedSkillGroupName: str
         :param VoicemailRecordURL: 通话中语音留言录音URL
 注意：此字段可能返回 null，表示取不到有效值。
         :type VoicemailRecordURL: list of str
+        :param VoicemailAsrURL: 通话中语音留言ASR文本信息地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoicemailAsrURL: list of str
         """
         self.Caller = None
         self.Callee = None
         self.Time = None
         self.Direction = None
         self.Duration = None
         self.RecordURL = None
@@ -4052,14 +4063,15 @@
         self.Uui = None
         self.IVRKeyPressedEx = None
         self.AsrUrl = None
         self.CustomRecordURL = None
         self.Remark = None
         self.QueuedSkillGroupName = None
         self.VoicemailRecordURL = None
+        self.VoicemailAsrURL = None
 
 
     def _deserialize(self, params):
         self.Caller = params.get("Caller")
         self.Callee = params.get("Callee")
         self.Time = params.get("Time")
         self.Direction = params.get("Direction")
@@ -4105,14 +4117,15 @@
                 obj._deserialize(item)
                 self.IVRKeyPressedEx.append(obj)
         self.AsrUrl = params.get("AsrUrl")
         self.CustomRecordURL = params.get("CustomRecordURL")
         self.Remark = params.get("Remark")
         self.QueuedSkillGroupName = params.get("QueuedSkillGroupName")
         self.VoicemailRecordURL = params.get("VoicemailRecordURL")
+        self.VoicemailAsrURL = params.get("VoicemailAsrURL")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.925/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.925/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/README.rst` & `tencentcloud-sdk-python-ccc-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.925/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.924/setup.py` & `tencentcloud-sdk-python-ccc-3.0.925/setup.py`

 * *Files identical despite different names*

