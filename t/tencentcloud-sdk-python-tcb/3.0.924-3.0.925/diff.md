# Comparing `tmp/tencentcloud-sdk-python-tcb-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-tcb-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.924.tar", last modified: Thu Jun 29 00:42:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.925.tar", last modified: Fri Jun 30 02:22:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcb-3.0.924.tar` & `tencentcloud-sdk-python-tcb-3.0.925.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)   296250 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)    76655 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/tcb_client.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 00:42:50.000000 tencentcloud-sdk-python-tcb-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   339910 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)    83901 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/tcb_client.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:22:27.000000 tencentcloud-sdk-python-tcb-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/models.py` & `tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -252,14 +252,50 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BanConfig(AbstractModel):
+    """封禁配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param IpWhiteList: ip白名单，支持ipv4、ipv6，支持CIDR
+        :type IpWhiteList: list of str
+        :param IpBlackList: ip黑名单，支持ipv4、ipv6，支持CIDR
+        :type IpBlackList: list of str
+        :param CountryWhiteList: 地域白名单（国家英文名）
+        :type CountryWhiteList: list of str
+        :param CountryBlackList: 地域黑名单（国家英文名）
+        :type CountryBlackList: list of str
+        """
+        self.IpWhiteList = None
+        self.IpBlackList = None
+        self.CountryWhiteList = None
+        self.CountryBlackList = None
+
+
+    def _deserialize(self, params):
+        self.IpWhiteList = params.get("IpWhiteList")
+        self.IpBlackList = params.get("IpBlackList")
+        self.CountryWhiteList = params.get("CountryWhiteList")
+        self.CountryBlackList = params.get("CountryBlackList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BindEnvGatewayRequest(AbstractModel):
     """BindEnvGateway请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -293,14 +329,84 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CbrPackageInfo(AbstractModel):
+    """代码包信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PackageName: 代码包名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageName: str
+        :param PackageVersion: 代码包版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageVersion: str
+        """
+        self.PackageName = None
+        self.PackageVersion = None
+
+
+    def _deserialize(self, params):
+        self.PackageName = params.get("PackageName")
+        self.PackageVersion = params.get("PackageVersion")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CbrRepoInfo(AbstractModel):
+    """仓库信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Repo: 仓库名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Repo: str
+        :param RepoType: 仓库平台
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RepoType: str
+        :param RepoLanguage: 仓库语言
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RepoLanguage: str
+        :param Branch: 分支名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Branch: str
+        """
+        self.Repo = None
+        self.RepoType = None
+        self.RepoLanguage = None
+        self.Branch = None
+
+
+    def _deserialize(self, params):
+        self.Repo = params.get("Repo")
+        self.RepoType = params.get("RepoType")
+        self.RepoLanguage = params.get("RepoLanguage")
+        self.Branch = params.get("Branch")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CheckTcbServiceRequest(AbstractModel):
     """CheckTcbService请求参数结构体
 
     """
 
 
 class CheckTcbServiceResponse(AbstractModel):
@@ -2217,15 +2323,15 @@
         :type EnvId: str
         :param WxAppId: 微信 AppId，微信必传
         :type WxAppId: str
         :param Source: 付费来源
 <li>miniapp</li>
 <li>qcloud</li>
         :type Source: str
-        :param FreeQuota: 用户享有的免费额度级别，目前只能为“basic”，不传该字段或该字段为空，标识不享受免费额度。
+        :param FreeQuota: 用户享有的免费额度级别，目前只能为“basic”，不传该字段或该字段为空，表示不享受免费额度。
         :type FreeQuota: str
         :param EnvSource: 环境创建来源，取值：
 <li>miniapp</li>
 <li>qcloud</li>
 用法同CreateEnv接口的Source参数
 和 Channel 参数同时传，或者同时不传；EnvId 为空时必传。
         :type EnvSource: str
@@ -2559,14 +2665,58 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CustomLogConfig(AbstractModel):
+    """安全网关自定义日志配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NeedReqBodyLog: 是否需要请求体
+        :type NeedReqBodyLog: bool
+        :param NeedReqHeaderLog: 是否需要请求头
+        :type NeedReqHeaderLog: bool
+        :param NeedRspBodyLog: 是否需要回包体
+        :type NeedRspBodyLog: bool
+        :param NeedRspHeaderLog: 是否需要回包头部信息
+        :type NeedRspHeaderLog: bool
+        :param LogSetId: cls set信息
+        :type LogSetId: str
+        :param LogTopicId: cls topicId
+        :type LogTopicId: str
+        """
+        self.NeedReqBodyLog = None
+        self.NeedReqHeaderLog = None
+        self.NeedRspBodyLog = None
+        self.NeedRspHeaderLog = None
+        self.LogSetId = None
+        self.LogTopicId = None
+
+
+    def _deserialize(self, params):
+        self.NeedReqBodyLog = params.get("NeedReqBodyLog")
+        self.NeedReqHeaderLog = params.get("NeedReqHeaderLog")
+        self.NeedRspBodyLog = params.get("NeedRspBodyLog")
+        self.NeedRspHeaderLog = params.get("NeedRspHeaderLog")
+        self.LogSetId = params.get("LogSetId")
+        self.LogTopicId = params.get("LogTopicId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DatabasesInfo(AbstractModel):
     """数据库资源信息
 
     """
 
     def __init__(self):
         r"""
@@ -2761,14 +2911,83 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteGatewayVersionRequest(AbstractModel):
+    """DeleteGatewayVersion请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境id
+        :type EnvId: str
+        :param GatewayId: 网关id
+        :type GatewayId: str
+        :param VersionName: 版本名
+        :type VersionName: str
+        :param IsDeleteServer: 是否删除服务
+        :type IsDeleteServer: bool
+        :param IsDeleteImage: 是否删除镜像
+        :type IsDeleteImage: bool
+        :param IsForce: 是否强制删除
+        :type IsForce: bool
+        :param OperatorRemark: 操作记录
+        :type OperatorRemark: str
+        """
+        self.EnvId = None
+        self.GatewayId = None
+        self.VersionName = None
+        self.IsDeleteServer = None
+        self.IsDeleteImage = None
+        self.IsForce = None
+        self.OperatorRemark = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.GatewayId = params.get("GatewayId")
+        self.VersionName = params.get("VersionName")
+        self.IsDeleteServer = params.get("IsDeleteServer")
+        self.IsDeleteImage = params.get("IsDeleteImage")
+        self.IsForce = params.get("IsForce")
+        self.OperatorRemark = params.get("OperatorRemark")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteGatewayVersionResponse(AbstractModel):
+    """DeleteGatewayVersion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 删除结果
+        :type Result: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Result = params.get("Result")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteWxGatewayRouteRequest(AbstractModel):
     """DeleteWxGatewayRoute请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2957,15 +3176,15 @@
 class DescribeAuthDomainsResponse(AbstractModel):
     """DescribeAuthDomains返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Domains: 安全域名列表列表
+        :param Domains: 安全域名列表
         :type Domains: list of AuthDomain
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Domains = None
         self.RequestId = None
 
@@ -3060,14 +3279,272 @@
             for item in params.get("PackageList"):
                 obj = BaasPackageInfo()
                 obj._deserialize(item)
                 self.PackageList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBillingInfoRequest(AbstractModel):
+    """DescribeBillingInfo请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境ID
+        :type EnvId: str
+        """
+        self.EnvId = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBillingInfoResponse(AbstractModel):
+    """DescribeBillingInfo返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvBillingInfoList: 环境计费信息列表
+        :type EnvBillingInfoList: list of EnvBillingInfoItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.EnvBillingInfoList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("EnvBillingInfoList") is not None:
+            self.EnvBillingInfoList = []
+            for item in params.get("EnvBillingInfoList"):
+                obj = EnvBillingInfoItem()
+                obj._deserialize(item)
+                self.EnvBillingInfoList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeCbrServerVersionRequest(AbstractModel):
+    """DescribeCbrServerVersion请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境ID
+        :type EnvId: str
+        :param ServerName: 服务名称
+        :type ServerName: str
+        :param VersionName: 版本名称
+        :type VersionName: str
+        """
+        self.EnvId = None
+        self.ServerName = None
+        self.VersionName = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.ServerName = params.get("ServerName")
+        self.VersionName = params.get("VersionName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeCbrServerVersionResponse(AbstractModel):
+    """DescribeCbrServerVersion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VersionName: 版本名称
+        :type VersionName: str
+        :param Remark: 备注
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Remark: str
+        :param DockerfilePath: Dockefile的路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DockerfilePath: str
+        :param BuildDir: DockerBuild的目录
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BuildDir: str
+        :param Cpu: Cpu大小
+        :type Cpu: float
+        :param Mem: Mem大小
+        :type Mem: float
+        :param MinNum: 副本最小值
+        :type MinNum: int
+        :param MaxNum: 副本最大值
+        :type MaxNum: int
+        :param EnvParams: 环境变量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnvParams: str
+        :param CreatedTime: 创建时间
+        :type CreatedTime: str
+        :param UpdatedTime: 更新时间
+        :type UpdatedTime: str
+        :param VersionIP: 版本的IP
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VersionIP: str
+        :param VersionPort: 版本的端口号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VersionPort: int
+        :param Status: 版本状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param UploadType: 枚举（package/repository/image)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UploadType: str
+        :param ServerName: 服务名字
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServerName: str
+        :param IsPublic: 是否对于外网开放
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsPublic: bool
+        :param VpcId: vpc id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param SubnetIds: 子网实例id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetIds: list of str
+        :param CustomLogs: 日志采集路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CustomLogs: str
+        :param ContainerPort: 监听端口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ContainerPort: int
+        :param InitialDelaySeconds: 延迟多长时间开始健康检查（单位s）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InitialDelaySeconds: int
+        :param ImageUrl: 镜像地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageUrl: str
+        :param HasDockerfile: 是否有Dockerfile：0-default has, 1-has, 2-has not
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasDockerfile: int
+        :param BaseImage: 基础镜像
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BaseImage: str
+        :param EntryPoint: 容器启动入口命令
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EntryPoint: str
+        :param PolicyDetail: 自动扩缩容策略组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PolicyDetail: list of HpaPolicy
+        :param TkeClusterInfo: Tke集群信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TkeClusterInfo: :class:`tencentcloud.tcb.v20180608.models.TkeClusterInfo`
+        :param TkeWorkloadType: 版本工作负载类型；deployment/deamonset
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TkeWorkloadType: str
+        :param PackageInfo: 代码包信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageInfo: :class:`tencentcloud.tcb.v20180608.models.CbrPackageInfo`
+        :param RepoInfo: 仓库信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RepoInfo: :class:`tencentcloud.tcb.v20180608.models.CbrRepoInfo`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.VersionName = None
+        self.Remark = None
+        self.DockerfilePath = None
+        self.BuildDir = None
+        self.Cpu = None
+        self.Mem = None
+        self.MinNum = None
+        self.MaxNum = None
+        self.EnvParams = None
+        self.CreatedTime = None
+        self.UpdatedTime = None
+        self.VersionIP = None
+        self.VersionPort = None
+        self.Status = None
+        self.UploadType = None
+        self.ServerName = None
+        self.IsPublic = None
+        self.VpcId = None
+        self.SubnetIds = None
+        self.CustomLogs = None
+        self.ContainerPort = None
+        self.InitialDelaySeconds = None
+        self.ImageUrl = None
+        self.HasDockerfile = None
+        self.BaseImage = None
+        self.EntryPoint = None
+        self.PolicyDetail = None
+        self.TkeClusterInfo = None
+        self.TkeWorkloadType = None
+        self.PackageInfo = None
+        self.RepoInfo = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.VersionName = params.get("VersionName")
+        self.Remark = params.get("Remark")
+        self.DockerfilePath = params.get("DockerfilePath")
+        self.BuildDir = params.get("BuildDir")
+        self.Cpu = params.get("Cpu")
+        self.Mem = params.get("Mem")
+        self.MinNum = params.get("MinNum")
+        self.MaxNum = params.get("MaxNum")
+        self.EnvParams = params.get("EnvParams")
+        self.CreatedTime = params.get("CreatedTime")
+        self.UpdatedTime = params.get("UpdatedTime")
+        self.VersionIP = params.get("VersionIP")
+        self.VersionPort = params.get("VersionPort")
+        self.Status = params.get("Status")
+        self.UploadType = params.get("UploadType")
+        self.ServerName = params.get("ServerName")
+        self.IsPublic = params.get("IsPublic")
+        self.VpcId = params.get("VpcId")
+        self.SubnetIds = params.get("SubnetIds")
+        self.CustomLogs = params.get("CustomLogs")
+        self.ContainerPort = params.get("ContainerPort")
+        self.InitialDelaySeconds = params.get("InitialDelaySeconds")
+        self.ImageUrl = params.get("ImageUrl")
+        self.HasDockerfile = params.get("HasDockerfile")
+        self.BaseImage = params.get("BaseImage")
+        self.EntryPoint = params.get("EntryPoint")
+        if params.get("PolicyDetail") is not None:
+            self.PolicyDetail = []
+            for item in params.get("PolicyDetail"):
+                obj = HpaPolicy()
+                obj._deserialize(item)
+                self.PolicyDetail.append(obj)
+        if params.get("TkeClusterInfo") is not None:
+            self.TkeClusterInfo = TkeClusterInfo()
+            self.TkeClusterInfo._deserialize(params.get("TkeClusterInfo"))
+        self.TkeWorkloadType = params.get("TkeWorkloadType")
+        if params.get("PackageInfo") is not None:
+            self.PackageInfo = CbrPackageInfo()
+            self.PackageInfo._deserialize(params.get("PackageInfo"))
+        if params.get("RepoInfo") is not None:
+            self.RepoInfo = CbrRepoInfo()
+            self.RepoInfo._deserialize(params.get("RepoInfo"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeCloudBaseBuildServiceRequest(AbstractModel):
     """DescribeCloudBaseBuildService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5429,14 +5906,185 @@
         self.EndTime = params.get("EndTime")
         self.Period = params.get("Period")
         self.Values = params.get("Values")
         self.Time = params.get("Time")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeGatewayVersionsRequest(AbstractModel):
+    """DescribeGatewayVersions请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境id
+        :type EnvId: str
+        :param GatewayId: 网关id
+        :type GatewayId: str
+        :param VersionName: 版本名
+        :type VersionName: str
+        """
+        self.EnvId = None
+        self.GatewayId = None
+        self.VersionName = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.GatewayId = params.get("GatewayId")
+        self.VersionName = params.get("VersionName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeGatewayVersionsResponse(AbstractModel):
+    """DescribeGatewayVersions返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GatewayId: 网关id
+        :type GatewayId: str
+        :param TotalCount: 版本总数
+        :type TotalCount: int
+        :param GatewayVersionItems: 版本信息详情
+        :type GatewayVersionItems: list of GatewayVersionItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.GatewayId = None
+        self.TotalCount = None
+        self.GatewayVersionItems = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.GatewayId = params.get("GatewayId")
+        self.TotalCount = params.get("TotalCount")
+        if params.get("GatewayVersionItems") is not None:
+            self.GatewayVersionItems = []
+            for item in params.get("GatewayVersionItems"):
+                obj = GatewayVersionItem()
+                obj._deserialize(item)
+                self.GatewayVersionItems.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeGraphDataRequest(AbstractModel):
+    """DescribeGraphData请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境ID
+        :type EnvId: str
+        :param MetricName: 指标名: 
+StorageRead: 存储读请求次数 
+StorageWrite: 存储写请求次数 
+StorageCdnOriginFlux: CDN回源流量, 单位字节 
+CDNFlux: CDN回源流量, 单位字节 
+FunctionInvocation: 云函数调用次数 
+FunctionGBs: 云函数资源使用量, 单位Mb*Ms 
+FunctionFlux: 云函数流量, 单位千字节(KB) 
+FunctionError: 云函数调用错误次数 
+FunctionDuration: 云函数运行时间, 单位毫秒 
+DbRead: 数据库读请求数 
+DbWrite: 数据库写请求数 
+DbCostTime10ms: 数据库耗时在10ms~50ms请求数 
+DbCostTime50ms: 数据库耗时在50ms~100ms请求数 
+DbCostTime100ms: 数据库耗时在100ms以上请求数 
+TkeCpuRatio: 容器CPU占用率 
+TkeMemRatio: 容器内存占用率 
+TkeCpuUsed: 容器CPU使用量 
+TkeMemUsed: 容器内存使用量 
+TkeInvokeNum: 调用量 
+FunctionConcurrentExecutions: 云函数并发执行个数
+FunctionIdleProvisioned: 云函数预置并发闲置量 
+FunctionConcurrencyMemoryMB: 云函数并发执行内存量 
+FunctionThrottle: 云函数受限次数 
+FunctionProvisionedConcurrency: 云函数预置并发 
+        :type MetricName: str
+        :param StartTime: 开始时间，如2018-08-24 10:50:00, 开始时间需要早于结束时间至少五分钟(原因是因为目前统计粒度最小是5分钟).
+        :type StartTime: str
+        :param EndTime: 结束时间，如2018-08-24 10:50:00, 结束时间需要晚于开始时间至少五分钟(原因是因为目前统计粒度最小是5分钟)..
+        :type EndTime: str
+        :param ResourceID: 资源ID, 目前仅对云函数、容器托管相关的指标有意义。云函数(FunctionInvocation, FunctionGBs, FunctionFlux, FunctionError, FunctionDuration)、容器托管（服务名称）, 如果想查询某个云函数的指标则在ResourceId中传入函数名; 如果只想查询整个namespace的指标, 则留空或不传.如果想查询数据库某个集合相关信息，传入集合名称
+        :type ResourceID: str
+        """
+        self.EnvId = None
+        self.MetricName = None
+        self.StartTime = None
+        self.EndTime = None
+        self.ResourceID = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.MetricName = params.get("MetricName")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.ResourceID = params.get("ResourceID")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeGraphDataResponse(AbstractModel):
+    """DescribeGraphData返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartTime: 开始时间, 会根据数据的统计周期进行取整.
+        :type StartTime: str
+        :param EndTime: 结束时间, 会根据数据的统计周期进行取整.
+        :type EndTime: str
+        :param MetricName: 指标名
+        :type MetricName: str
+        :param Period: 统计周期(单位秒), 当时间区间为1天内, 统计周期为5分钟; 当时间区间选择为1天以上, 15天以下, 统计周期为1小时; 当时间区间选择为15天以上, 180天以下, 统计周期为1天.
+        :type Period: int
+        :param Values: 有效的监控数据, 每个有效监控数据的上报时间可以从时间数组中的对应位置上获取到.
+        :type Values: list of float
+        :param Time: 时间数据, 标识监控数据Values中的点是哪个时间段上报的.
+        :type Time: list of int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.StartTime = None
+        self.EndTime = None
+        self.MetricName = None
+        self.Period = None
+        self.Values = None
+        self.Time = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.MetricName = params.get("MetricName")
+        self.Period = params.get("Period")
+        self.Values = params.get("Values")
+        self.Time = params.get("Time")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeHostingDomainTaskRequest(AbstractModel):
     """DescribeHostingDomainTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6076,14 +6724,150 @@
 
 
     def _deserialize(self, params):
         self.SubNetIds = params.get("SubNetIds")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeWxGatewayRoutesRequest(AbstractModel):
+    """DescribeWxGatewayRoutes请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境ID
+        :type EnvId: str
+        :param GatewayId: 网关名称
+        :type GatewayId: str
+        :param GatewayRouteName: 网关路由名称
+        :type GatewayRouteName: str
+        :param GatewayVersion: 网关版本名
+        :type GatewayVersion: str
+        """
+        self.EnvId = None
+        self.GatewayId = None
+        self.GatewayRouteName = None
+        self.GatewayVersion = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.GatewayId = params.get("GatewayId")
+        self.GatewayRouteName = params.get("GatewayRouteName")
+        self.GatewayVersion = params.get("GatewayVersion")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeWxGatewayRoutesResponse(AbstractModel):
+    """DescribeWxGatewayRoutes返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 返回的服务个数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param WxGatewayRouteSet: 返回的服务列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WxGatewayRouteSet: list of WxGatewayRountItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.WxGatewayRouteSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("WxGatewayRouteSet") is not None:
+            self.WxGatewayRouteSet = []
+            for item in params.get("WxGatewayRouteSet"):
+                obj = WxGatewayRountItem()
+                obj._deserialize(item)
+                self.WxGatewayRouteSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeWxGatewaysRequest(AbstractModel):
+    """DescribeWxGateways请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境ID
+        :type EnvId: str
+        :param GatewayName: 服务名称，精确匹配
+        :type GatewayName: str
+        :param Limit: 分页参数
+        :type Limit: int
+        :param Offset: 分页参数
+        :type Offset: int
+        """
+        self.EnvId = None
+        self.GatewayName = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.GatewayName = params.get("GatewayName")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeWxGatewaysResponse(AbstractModel):
+    """DescribeWxGateways返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Gateways: 返回的服务列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Gateways: list of GatewayItem
+        :param TotalCount: 网关总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Gateways = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Gateways") is not None:
+            self.Gateways = []
+            for item in params.get("Gateways"):
+                obj = GatewayItem()
+                obj._deserialize(item)
+                self.Gateways.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DestroyEnvRequest(AbstractModel):
     """DestroyEnv请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6470,14 +7254,20 @@
         :type EnvType: str
         :param IsDauPackage: 是否是dau新套餐
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsDauPackage: bool
         :param PackageType: 套餐类型:空\baas\tcbr
 注意：此字段可能返回 null，表示取不到有效值。
         :type PackageType: str
+        :param ArchitectureType: 架构类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ArchitectureType: str
+        :param Recycle: 回收标志，默认为空
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Recycle: str
         """
         self.EnvId = None
         self.Source = None
         self.Alias = None
         self.CreateTime = None
         self.UpdateTime = None
         self.Status = None
@@ -6494,14 +7284,16 @@
         self.IsDefault = None
         self.Region = None
         self.Tags = None
         self.CustomLogServices = None
         self.EnvType = None
         self.IsDauPackage = None
         self.PackageType = None
+        self.ArchitectureType = None
+        self.Recycle = None
 
 
     def _deserialize(self, params):
         self.EnvId = params.get("EnvId")
         self.Source = params.get("Source")
         self.Alias = params.get("Alias")
         self.CreateTime = params.get("CreateTime")
@@ -6555,14 +7347,16 @@
             for item in params.get("CustomLogServices"):
                 obj = ClsInfo()
                 obj._deserialize(item)
                 self.CustomLogServices.append(obj)
         self.EnvType = params.get("EnvType")
         self.IsDauPackage = params.get("IsDauPackage")
         self.PackageType = params.get("PackageType")
+        self.ArchitectureType = params.get("ArchitectureType")
+        self.Recycle = params.get("Recycle")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6879,15 +7673,15 @@
 class FreezeCloudBaseRunServersResponse(AbstractModel):
     """FreezeCloudBaseRunServers返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Result: 批量状态状态
+        :param Result: 批量状态
 成功：succ
 失败：fail
 部分：partial（部分成功、部分失败）
 注意：此字段可能返回 null，表示取不到有效值。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Result: str
         :param FailServerList: 冻结失败服务列表
@@ -6904,14 +7698,42 @@
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.FailServerList = params.get("FailServerList")
         self.RequestId = params.get("RequestId")
 
 
+class FrequencyLimitConfig(AbstractModel):
+    """安全网关版本路由信息限额配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LimitObject: 限额对象 "ConnectionsLimit" 或 "QPSLimit"
+        :type LimitObject: str
+        :param LimitConfig: 限额配置
+        :type LimitConfig: str
+        """
+        self.LimitObject = None
+        self.LimitConfig = None
+
+
+    def _deserialize(self, params):
+        self.LimitObject = params.get("LimitObject")
+        self.LimitConfig = params.get("LimitConfig")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FunctionInfo(AbstractModel):
     """函数的信息
 
     """
 
     def __init__(self):
         r"""
@@ -6933,14 +7755,195 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class GatewayItem(AbstractModel):
+    """网关信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Uin: 用户uin
+        :type Uin: str
+        :param AppId: 用户appid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param EnvId: 环境id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnvId: str
+        :param GatewayId: Gateway唯一id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayId: str
+        :param GatewayName: Gateway名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayName: str
+        :param GatewayType: Gateway类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayType: str
+        :param GatewayDesc: Gateway描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayDesc: str
+        :param PackageVersion: 套餐版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageVersion: str
+        :param PackageId: 套餐唯一id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PackageId: int
+        :param VpcId: vpc唯一id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param SubnetIds: 子网id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetIds: list of str
+        :param Status: 网关状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param L5Addr: l5地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type L5Addr: str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param IsolateTime: 隔离时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsolateTime: str
+        :param ExpireTime: 到期时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpireTime: str
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 变更时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param AllowUncertified: 允许未登录访问
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AllowUncertified: int
+        :param VersionNumLimit: 网关版本限额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VersionNumLimit: int
+        """
+        self.Uin = None
+        self.AppId = None
+        self.EnvId = None
+        self.GatewayId = None
+        self.GatewayName = None
+        self.GatewayType = None
+        self.GatewayDesc = None
+        self.PackageVersion = None
+        self.PackageId = None
+        self.VpcId = None
+        self.SubnetIds = None
+        self.Status = None
+        self.L5Addr = None
+        self.Region = None
+        self.IsolateTime = None
+        self.ExpireTime = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.AllowUncertified = None
+        self.VersionNumLimit = None
+
+
+    def _deserialize(self, params):
+        self.Uin = params.get("Uin")
+        self.AppId = params.get("AppId")
+        self.EnvId = params.get("EnvId")
+        self.GatewayId = params.get("GatewayId")
+        self.GatewayName = params.get("GatewayName")
+        self.GatewayType = params.get("GatewayType")
+        self.GatewayDesc = params.get("GatewayDesc")
+        self.PackageVersion = params.get("PackageVersion")
+        self.PackageId = params.get("PackageId")
+        self.VpcId = params.get("VpcId")
+        self.SubnetIds = params.get("SubnetIds")
+        self.Status = params.get("Status")
+        self.L5Addr = params.get("L5Addr")
+        self.Region = params.get("Region")
+        self.IsolateTime = params.get("IsolateTime")
+        self.ExpireTime = params.get("ExpireTime")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.AllowUncertified = params.get("AllowUncertified")
+        self.VersionNumLimit = params.get("VersionNumLimit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GatewayVersionItem(AbstractModel):
+    """网关版本详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VersionName: 版本名
+        :type VersionName: str
+        :param Weight: 版本流量权重
+        :type Weight: int
+        :param Status: 创建状态
+        :type Status: str
+        :param CreatedTime: 创建时间
+        :type CreatedTime: str
+        :param UpdatedTime: 更新时间
+        :type UpdatedTime: str
+        :param BuildId: 构建ID
+        :type BuildId: int
+        :param Remark: 备注
+        :type Remark: str
+        :param Priority: 优先级
+        :type Priority: int
+        :param IsDefault: 是否默认版本
+        :type IsDefault: bool
+        :param CustomConfig: 网关版本自定义配置
+        :type CustomConfig: :class:`tencentcloud.tcb.v20180608.models.WxGatewayCustomConfig`
+        """
+        self.VersionName = None
+        self.Weight = None
+        self.Status = None
+        self.CreatedTime = None
+        self.UpdatedTime = None
+        self.BuildId = None
+        self.Remark = None
+        self.Priority = None
+        self.IsDefault = None
+        self.CustomConfig = None
+
+
+    def _deserialize(self, params):
+        self.VersionName = params.get("VersionName")
+        self.Weight = params.get("Weight")
+        self.Status = params.get("Status")
+        self.CreatedTime = params.get("CreatedTime")
+        self.UpdatedTime = params.get("UpdatedTime")
+        self.BuildId = params.get("BuildId")
+        self.Remark = params.get("Remark")
+        self.Priority = params.get("Priority")
+        self.IsDefault = params.get("IsDefault")
+        if params.get("CustomConfig") is not None:
+            self.CustomConfig = WxGatewayCustomConfig()
+            self.CustomConfig._deserialize(params.get("CustomConfig"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class HpaPolicy(AbstractModel):
     """扩缩容策略
 
     """
 
     def __init__(self):
         r"""
@@ -7423,15 +8426,15 @@
 
     def __init__(self):
         r"""
         :param EnvId: 环境ID
         :type EnvId: str
         :param UUId: C端用户端的唯一ID
         :type UUId: str
-        :param Status: 帐号的状态
+        :param Status: 账号的状态
 <li>ENABLE</li>
 <li>DISABLE</li>
         :type Status: str
         """
         self.EnvId = None
         self.UUId = None
         self.Status = None
@@ -7508,14 +8511,68 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyGatewayVersionTrafficRequest(AbstractModel):
+    """ModifyGatewayVersionTraffic请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EnvId: 环境id
+        :type EnvId: str
+        :param GatewayId: 网关id
+        :type GatewayId: str
+        :param VersionsWeight: 网关版本流量比例信息
+        :type VersionsWeight: list of GatewayVersionItem
+        """
+        self.EnvId = None
+        self.GatewayId = None
+        self.VersionsWeight = None
+
+
+    def _deserialize(self, params):
+        self.EnvId = params.get("EnvId")
+        self.GatewayId = params.get("GatewayId")
+        if params.get("VersionsWeight") is not None:
+            self.VersionsWeight = []
+            for item in params.get("VersionsWeight"):
+                obj = GatewayVersionItem()
+                obj._deserialize(item)
+                self.VersionsWeight.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyGatewayVersionTrafficResponse(AbstractModel):
+    """ModifyGatewayVersionTraffic返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ObjectKV(AbstractModel):
     """Key-Value类型，模拟的 object 类型
 
     """
 
     def __init__(self):
         r"""
@@ -8719,8 +9776,141 @@
         self.FailServerList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Result = params.get("Result")
         self.FailServerList = params.get("FailServerList")
-        self.RequestId = params.get("RequestId")
+        self.RequestId = params.get("RequestId")
+
+
+class WxGatewayCustomConfig(AbstractModel):
+    """安全网关自定义配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param IsOpenXRealIp: 是否开启x-real-ip
+        :type IsOpenXRealIp: bool
+        :param BanConfig: 封禁配置
+        :type BanConfig: :class:`tencentcloud.tcb.v20180608.models.BanConfig`
+        :param SourceIpType: 获取源ip方式，PPV1(Proxy Protocol V1)、PPV2(Proxy Protocol V2)、TOA(tcp option address)
+        :type SourceIpType: str
+        :param LogConfig: 日志信息
+        :type LogConfig: :class:`tencentcloud.tcb.v20180608.models.CustomLogConfig`
+        :param IsAcceptHttpOne: 是否开启http1.0
+        :type IsAcceptHttpOne: bool
+        """
+        self.IsOpenXRealIp = None
+        self.BanConfig = None
+        self.SourceIpType = None
+        self.LogConfig = None
+        self.IsAcceptHttpOne = None
+
+
+    def _deserialize(self, params):
+        self.IsOpenXRealIp = params.get("IsOpenXRealIp")
+        if params.get("BanConfig") is not None:
+            self.BanConfig = BanConfig()
+            self.BanConfig._deserialize(params.get("BanConfig"))
+        self.SourceIpType = params.get("SourceIpType")
+        if params.get("LogConfig") is not None:
+            self.LogConfig = CustomLogConfig()
+            self.LogConfig._deserialize(params.get("LogConfig"))
+        self.IsAcceptHttpOne = params.get("IsAcceptHttpOne")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class WxGatewayRountItem(AbstractModel):
+    """安全网关路由
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GatewayRouteName: 安全网关路由名称
+        :type GatewayRouteName: str
+        :param GatewayRouteProtocol: 安全网关路由协议
+        :type GatewayRouteProtocol: str
+        :param GatewayRouteAddr: 安全网关路由地址
+        :type GatewayRouteAddr: str
+        :param GatewayRouteDesc: 安全网关路由描述
+        :type GatewayRouteDesc: str
+        :param GatewayRouteClusterId: 安全网关后端集群id，如果是外网服务，该id与GatewayRountName相同
+        :type GatewayRouteClusterId: str
+        :param GatewayRouteCreateTime: 安全网关创建时间
+        :type GatewayRouteCreateTime: str
+        :param FrequencyLimitConfig: 安全网关路由限制
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FrequencyLimitConfig: list of FrequencyLimitConfig
+        :param GatewayRouteServerType: ip代表绑定后端ip。cbr代表云托管服务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRouteServerType: str
+        :param GatewayRouteServerName: 服务名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRouteServerName: str
+        :param GatewayRewriteHost: ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRewriteHost: str
+        :param GatewayVersion: 网关版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayVersion: str
+        :param GatewayRoutePath: 请求路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRoutePath: str
+        :param GatewayRouteMethod: 请求模式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRouteMethod: str
+        :param GatewayRoutePort: 4层端口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayRoutePort: int
+        """
+        self.GatewayRouteName = None
+        self.GatewayRouteProtocol = None
+        self.GatewayRouteAddr = None
+        self.GatewayRouteDesc = None
+        self.GatewayRouteClusterId = None
+        self.GatewayRouteCreateTime = None
+        self.FrequencyLimitConfig = None
+        self.GatewayRouteServerType = None
+        self.GatewayRouteServerName = None
+        self.GatewayRewriteHost = None
+        self.GatewayVersion = None
+        self.GatewayRoutePath = None
+        self.GatewayRouteMethod = None
+        self.GatewayRoutePort = None
+
+
+    def _deserialize(self, params):
+        self.GatewayRouteName = params.get("GatewayRouteName")
+        self.GatewayRouteProtocol = params.get("GatewayRouteProtocol")
+        self.GatewayRouteAddr = params.get("GatewayRouteAddr")
+        self.GatewayRouteDesc = params.get("GatewayRouteDesc")
+        self.GatewayRouteClusterId = params.get("GatewayRouteClusterId")
+        self.GatewayRouteCreateTime = params.get("GatewayRouteCreateTime")
+        if params.get("FrequencyLimitConfig") is not None:
+            self.FrequencyLimitConfig = []
+            for item in params.get("FrequencyLimitConfig"):
+                obj = FrequencyLimitConfig()
+                obj._deserialize(item)
+                self.FrequencyLimitConfig.append(obj)
+        self.GatewayRouteServerType = params.get("GatewayRouteServerType")
+        self.GatewayRouteServerName = params.get("GatewayRouteServerName")
+        self.GatewayRewriteHost = params.get("GatewayRewriteHost")
+        self.GatewayVersion = params.get("GatewayVersion")
+        self.GatewayRoutePath = params.get("GatewayRoutePath")
+        self.GatewayRouteMethod = params.get("GatewayRouteMethod")
+        self.GatewayRoutePort = params.get("GatewayRoutePort")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/tcb_client.py` & `tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/tcb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,14 +390,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteGatewayVersion(self, request):
+        """删除网关某版本
+
+        :param request: Request instance for DeleteGatewayVersion.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteGatewayVersionRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DeleteGatewayVersionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteGatewayVersion", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteGatewayVersionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteWxGatewayRoute(self, request):
         """删除安全网关路由
 
         :param request: Request instance for DeleteWxGatewayRoute.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DeleteWxGatewayRouteRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.DeleteWxGatewayRouteResponse`
 
@@ -505,14 +528,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeBillingInfo(self, request):
+        """获取计费相关信息
+
+        :param request: Request instance for DescribeBillingInfo.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeBillingInfoRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeBillingInfoResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBillingInfo", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBillingInfoResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeCbrServerVersion(self, request):
+        """查询服务版本的详情
+
+        :param request: Request instance for DescribeCbrServerVersion.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCbrServerVersionRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeCbrServerVersionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCbrServerVersion", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCbrServerVersionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeCloudBaseBuildService(self, request):
         """获取云托管代码上传url
 
         :param request: Request instance for DescribeCloudBaseBuildService.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseBuildServiceRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeCloudBaseBuildServiceResponse`
 
@@ -1195,14 +1264,61 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeGatewayVersions(self, request):
+        """查询网关版本信息
+        暂不鉴权
+
+        :param request: Request instance for DescribeGatewayVersions.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeGatewayVersionsRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeGatewayVersionsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeGatewayVersions", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeGatewayVersionsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeGraphData(self, request):
+        """根据用户传入的指标, 拉取一段时间内的监控数据。
+
+        :param request: Request instance for DescribeGraphData.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeGraphDataRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeGraphDataResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeGraphData", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeGraphDataResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeHostingDomainTask(self, request):
         """查询静态托管域名任务状态
 
         :param request: Request instance for DescribeHostingDomainTask.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeHostingDomainTaskRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeHostingDomainTaskResponse`
 
@@ -1451,14 +1567,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeWxGatewayRoutes(self, request):
+        """查看安全网关路由
+
+        :param request: Request instance for DescribeWxGatewayRoutes.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewayRoutesRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewayRoutesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeWxGatewayRoutes", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeWxGatewayRoutesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeWxGateways(self, request):
+        """查看安全网关
+
+        :param request: Request instance for DescribeWxGateways.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewaysRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.DescribeWxGatewaysResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeWxGateways", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeWxGatewaysResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DestroyEnv(self, request):
         """销毁环境
 
         :param request: Request instance for DestroyEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.DestroyEnvRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.DestroyEnvResponse`
 
@@ -1727,14 +1889,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyGatewayVersionTraffic(self, request):
+        """设置网关版本的流量比例
+
+        :param request: Request instance for ModifyGatewayVersionTraffic.
+        :type request: :class:`tencentcloud.tcb.v20180608.models.ModifyGatewayVersionTrafficRequest`
+        :rtype: :class:`tencentcloud.tcb.v20180608.models.ModifyGatewayVersionTrafficResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyGatewayVersionTraffic", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyGatewayVersionTrafficResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ReinstateEnv(self, request):
         """针对已隔离的免费环境，可以通过本接口将其恢复访问。
 
         :param request: Request instance for ReinstateEnv.
         :type request: :class:`tencentcloud.tcb.v20180608.models.ReinstateEnvRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.ReinstateEnvResponse`
 
@@ -1797,15 +1982,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SearchClsLog(self, request):
-        """搜索CLS日志，TCB角色秘钥访问
+        """搜索CLS日志，TCB角色密钥访问
 
         :param request: Request instance for SearchClsLog.
         :type request: :class:`tencentcloud.tcb.v20180608.models.SearchClsLogRequest`
         :rtype: :class:`tencentcloud.tcb.v20180608.models.SearchClsLogResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/tencentcloud/tcb/v20180608/errorcodes.py` & `tencentcloud-sdk-python-tcb-3.0.925/tencentcloud/tcb/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/README.rst` & `tencentcloud-sdk-python-tcb-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.925/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.924/setup.py` & `tencentcloud-sdk-python-tcb-3.0.925/setup.py`

 * *Files identical despite different names*

