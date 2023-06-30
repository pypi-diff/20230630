# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.924.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.924.tar", last modified: Thu Jun 29 00:39:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.925.tar", last modified: Fri Jun 30 02:19:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.924.tar` & `tencentcloud-sdk-python-organization-3.0.925.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73820 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)    10169 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23487 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/organization_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30659 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19620 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/organization_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/README.rst
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-29 00:39:31.000000 tencentcloud-sdk-python-organization-3.0.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76362 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)    10778 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24418 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/organization_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30659 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19620 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/organization_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      764 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-30 02:19:11.000000 tencentcloud-sdk-python-organization-3.0.925/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-30 02:19:10.000000 tencentcloud-sdk-python-organization-3.0.925/setup.py
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2126,14 +2126,80 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UpdateOrganizationMemberRequest(AbstractModel):
+    """UpdateOrganizationMember请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MemberUin: 成员Uin。
+        :type MemberUin: int
+        :param Name: 成员名称。最大长度为25个字符，支持英文字母、数字、汉字、符号+@、&._[]-:,
+        :type Name: str
+        :param Remark: 备注。最大长度为40个字符
+        :type Remark: str
+        :param PolicyType: 关系策略类型。PolicyType不为空，PermissionIds不能为空。取值：Financial
+        :type PolicyType: str
+        :param PermissionIds: 成员财务权限ID列表。PermissionIds不为空，PolicyType不能为空。
+取值：1-查看账单、2-查看余额、3-资金划拨、4-合并出账、5-开票、6-优惠继承、7-代付费、8-成本分析，如果有值，1、2 默认必须
+        :type PermissionIds: list of int non-negative
+        :param IsAllowQuit: 是否允许成员退出组织。取值：Allow-允许、Denied-不允许
+        :type IsAllowQuit: str
+        :param PayUin: 代付者Uin。成员财务权限有代付费时需要，取值为成员对应主体的主体管理员Uin
+        :type PayUin: str
+        """
+        self.MemberUin = None
+        self.Name = None
+        self.Remark = None
+        self.PolicyType = None
+        self.PermissionIds = None
+        self.IsAllowQuit = None
+        self.PayUin = None
+
+
+    def _deserialize(self, params):
+        self.MemberUin = params.get("MemberUin")
+        self.Name = params.get("Name")
+        self.Remark = params.get("Remark")
+        self.PolicyType = params.get("PolicyType")
+        self.PermissionIds = params.get("PermissionIds")
+        self.IsAllowQuit = params.get("IsAllowQuit")
+        self.PayUin = params.get("PayUin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateOrganizationMemberResponse(AbstractModel):
+    """UpdateOrganizationMember返回参数结构体
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
 class UpdateOrganizationNodeRequest(AbstractModel):
     """UpdateOrganizationNode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 
 # 该帐号已被注册。
 FAILEDOPERATION_ACCOUNTALREADYREGISTER = 'FailedOperation.AccountAlreadyRegister'
 
 # 用户未实名。
 FAILEDOPERATION_AUTHINFOEMPTY = 'FailedOperation.AuthInfoEmpty'
 
+# 企业实名不一样。
+FAILEDOPERATION_AUTHINFONOTSAME = 'FailedOperation.AuthInfoNotSame'
+
 # 用户非企业实名。
 FAILEDOPERATION_AUTHNOTENTERPRISE = 'FailedOperation.AuthNotEnterprise'
 
 # 绑定邮箱链接过期。
 FAILEDOPERATION_BINDEMAILLINKEXPIRED = 'FailedOperation.BindEmailLinkExpired'
 
 # 绑定邮箱链接无效。
 FAILEDOPERATION_BINDEMAILLINKINVALID = 'FailedOperation.BindEmailLinkInvalid'
 
+# 成员权限变更记录存在。
+FAILEDOPERATION_CHANGEPERMISSIONRECORDEXIST = 'FailedOperation.ChangePermissionRecordExist'
+
 # 检查手机绑定上限失败。
 FAILEDOPERATION_CHECKACCOUNTPHONEBINDLIMIT = 'FailedOperation.CheckAccountPhoneBindLimit'
 
 # 检查邮箱绑定状态失败。
 FAILEDOPERATION_CHECKMAILACCOUNT = 'FailedOperation.CheckMailAccount'
 
 # 创建成员异常。
@@ -145,14 +151,17 @@
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
+# 成员代付费模式，不允许主动退出组织。
+INVALIDPARAMETER_ALLOWQUITILLEGAL = 'InvalidParameter.AllowQuitIllegal'
+
 # 手机验证码错误。
 INVALIDPARAMETER_CODEERROR = 'InvalidParameter.CodeError'
 
 # 手机验证码已过期。
 INVALIDPARAMETER_CODEEXPIRED = 'InvalidParameter.CodeExpired'
 
 # 无效的邮箱。
@@ -217,14 +226,17 @@
 
 # 不允许添加优惠继承关系。
 UNSUPPORTEDOPERATION_ADDDISCOUNTINHERITNOTALLOW = 'UnsupportedOperation.AddDiscountInheritNotAllow'
 
 # 创建的成员不允许删除。
 UNSUPPORTEDOPERATION_CREATEMEMBERNOTALLOWDELETE = 'UnsupportedOperation.CreateMemberNotAllowDelete'
 
+# 不允许删除代付关系。
+UNSUPPORTEDOPERATION_DELETEDELEGATEPAYERNOTALLOW = 'UnsupportedOperation.DeleteDelegatePayerNotAllow'
+
 # 成员或者代付者存在经销商。
 UNSUPPORTEDOPERATION_EXISTEDAGENT = 'UnsupportedOperation.ExistedAgent'
 
 # 成员或者代付者存在经销商子客。
 UNSUPPORTEDOPERATION_EXISTEDCLIENT = 'UnsupportedOperation.ExistedClient'
 
 # 用户类型不一致。
@@ -250,14 +262,17 @@
 
 # 成员是代理商或代客。
 UNSUPPORTEDOPERATION_MEMBERISAGENT = 'UnsupportedOperation.MemberIsAgent'
 
 # 成员没有绑卡。
 UNSUPPORTEDOPERATION_MEMBERNOPAYMENT = 'UnsupportedOperation.MemberNoPayment'
 
+# 成员不支持主动退出。
+UNSUPPORTEDOPERATION_MEMBERNOTALLOWQUIT = 'UnsupportedOperation.MemberNotAllowQuit'
+
 # 存在在途订单。
 UNSUPPORTEDOPERATION_ORDERINPROGRESSEXISTED = 'UnsupportedOperation.OrderInProgressExisted'
 
 # 管理员存在优惠继承。
 UNSUPPORTEDOPERATION_OWNERDISCOUNTINHERITEXISTED = 'UnsupportedOperation.OwnerDiscountInheritExisted'
 
 # 代付者欠费且未开通信用账户。
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20210331/organization_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def UpdateOrganizationMember(self, request):
+        """更新组织成员信息
+
+        :param request: Request instance for UpdateOrganizationMember.
+        :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateOrganizationMember", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateOrganizationMemberResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def UpdateOrganizationMemberEmailBind(self, request):
         """修改绑定成员邮箱
 
         :param request: Request instance for UpdateOrganizationMemberEmailBind.
         :type request: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberEmailBindRequest`
         :rtype: :class:`tencentcloud.organization.v20210331.models.UpdateOrganizationMemberEmailBindResponse`
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.924/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.925/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/README.rst` & `tencentcloud-sdk-python-organization-3.0.925/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.924/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.925/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.924
+Version: 3.0.925
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.924/setup.py` & `tencentcloud-sdk-python-organization-3.0.925/setup.py`

 * *Files identical despite different names*

