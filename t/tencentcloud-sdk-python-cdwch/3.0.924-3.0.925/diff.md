# Comparing `tmp/tencentcloud-sdk-python-cdwch-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-cdwch-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.924.tar", last modified: Thu Jun 29 00:26:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.925.tar", last modified: Fri Jun 30 02:02:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdwch-3.0.924.tar` & `tencentcloud-sdk-python-cdwch-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82547 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/models.py
--rw-r--r--   0 root         (0) root         (0)    20026 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/cdwch_client.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-29 00:26:15.000000 tencentcloud-sdk-python-cdwch-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83862 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/models.py
+-rw-r--r--   0 root         (0) root         (0)    20026 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/cdwch_client.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-30 02:02:45.000000 tencentcloud-sdk-python-cdwch-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/models.py` & `tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,37 +111,52 @@
     """备份表信息
 
     """
 
     def __init__(self):
         r"""
         :param Database: 数据库
+注意：此字段可能返回 null，表示取不到有效值。
         :type Database: str
         :param Table: 表
+注意：此字段可能返回 null，表示取不到有效值。
         :type Table: str
         :param TotalBytes: 表总字节数
+注意：此字段可能返回 null，表示取不到有效值。
         :type TotalBytes: int
         :param VCluster: 虚拟cluster
+注意：此字段可能返回 null，表示取不到有效值。
         :type VCluster: str
         :param Ips: 表ip
+注意：此字段可能返回 null，表示取不到有效值。
         :type Ips: str
+        :param ZooPath: zk路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ZooPath: str
+        :param Rip: cvm的ip地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Rip: str
         """
         self.Database = None
         self.Table = None
         self.TotalBytes = None
         self.VCluster = None
         self.Ips = None
+        self.ZooPath = None
+        self.Rip = None
 
 
     def _deserialize(self, params):
         self.Database = params.get("Database")
         self.Table = params.get("Table")
         self.TotalBytes = params.get("TotalBytes")
         self.VCluster = params.get("VCluster")
         self.Ips = params.get("Ips")
+        self.ZooPath = params.get("ZooPath")
+        self.Rip = params.get("Rip")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -540,22 +555,26 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type DataStrategy: :class:`tencentcloud.cdwch.v20200915.models.ScheduleStrategy`
         :param BackUpContents: 备份表列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackUpContents: list of BackupTableContent
         :param BackUpStatus: 备份的状态
         :type BackUpStatus: int
+        :param ErrorMsg: 错误信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorMsg: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.BackUpOpened = None
         self.MetaStrategy = None
         self.DataStrategy = None
         self.BackUpContents = None
         self.BackUpStatus = None
+        self.ErrorMsg = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.BackUpOpened = params.get("BackUpOpened")
         if params.get("MetaStrategy") is not None:
             self.MetaStrategy = ScheduleStrategy()
@@ -566,14 +585,15 @@
         if params.get("BackUpContents") is not None:
             self.BackUpContents = []
             for item in params.get("BackUpContents"):
                 obj = BackupTableContent()
                 obj._deserialize(item)
                 self.BackUpContents.append(obj)
         self.BackUpStatus = params.get("BackUpStatus")
+        self.ErrorMsg = params.get("ErrorMsg")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeCkSqlApisRequest(AbstractModel):
     """DescribeCkSqlApis请求参数结构体
 
     """
@@ -1001,33 +1021,37 @@
         :type SearchInstanceName: str
         :param Offset: 分页参数，第一页为0，第二页为10
         :type Offset: int
         :param Limit: 分页参数，分页步长，默认为10
         :type Limit: int
         :param SearchTags: 搜索标签列表
         :type SearchTags: list of SearchTags
+        :param IsSimple: 信息详细与否
+        :type IsSimple: bool
         """
         self.SearchInstanceId = None
         self.SearchInstanceName = None
         self.Offset = None
         self.Limit = None
         self.SearchTags = None
+        self.IsSimple = None
 
 
     def _deserialize(self, params):
         self.SearchInstanceId = params.get("SearchInstanceId")
         self.SearchInstanceName = params.get("SearchInstanceName")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         if params.get("SearchTags") is not None:
             self.SearchTags = []
             for item in params.get("SearchTags"):
                 obj = SearchTags()
                 obj._deserialize(item)
                 self.SearchTags.append(obj)
+        self.IsSimple = params.get("IsSimple")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2305,28 +2329,33 @@
         :type RetainDays: int
         :param WeekDays: 备份的天
         :type WeekDays: str
         :param ExecuteHour: 备份小时
         :type ExecuteHour: int
         :param ScheduleId: 策略id
         :type ScheduleId: int
+        :param NextBackupTime: 下次备份时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NextBackupTime: str
         """
         self.CosBucketName = None
         self.RetainDays = None
         self.WeekDays = None
         self.ExecuteHour = None
         self.ScheduleId = None
+        self.NextBackupTime = None
 
 
     def _deserialize(self, params):
         self.CosBucketName = params.get("CosBucketName")
         self.RetainDays = params.get("RetainDays")
         self.WeekDays = params.get("WeekDays")
         self.ExecuteHour = params.get("ExecuteHour")
         self.ScheduleId = params.get("ScheduleId")
+        self.NextBackupTime = params.get("NextBackupTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/cdwch_client.py` & `tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/cdwch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/tencentcloud/cdwch/v20200915/errorcodes.py` & `tencentcloud-sdk-python-cdwch-3.0.925/tencentcloud/cdwch/v20200915/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/README.rst` & `tencentcloud-sdk-python-cdwch-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.924/setup.py` & `tencentcloud-sdk-python-cdwch-3.0.925/setup.py`

 * *Files identical despite different names*

