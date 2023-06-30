# Comparing `tmp/xj_role-1.0.8.tar.gz` & `tmp/xj_role-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_role-1.0.8.tar", last modified: Tue Sep 13 07:57:45 2022, max compression
+gzip compressed data, was "dist\xj_role-1.0.9.tar", last modified: Thu Sep 15 05:32:40 2022, max compression
```

## Comparing `xj_role-1.0.8.tar` & `xj_role-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/
--rw-rw-rw-   0        0        0      581 2022-09-13 07:57:45.000000 xj_role-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_role-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2022-09-13 07:57:45.000000 xj_role-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2119 2022-09-13 07:57:34.000000 xj_role-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/__init__.py
--rw-rw-rw-   0        0        0     1916 2022-09-07 02:09:37.000000 xj_role-1.0.8/xj_role/admin.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/apis/__init__.py
--rw-rw-rw-   0        0        0     3133 2022-09-09 01:10:05.000000 xj_role-1.0.8/xj_role/apis/group_api.py
--rw-rw-rw-   0        0        0     2506 2022-09-07 02:01:28.000000 xj_role-1.0.8/xj_role/apis/permission_api.py
--rw-rw-rw-   0        0        0      756 2022-09-08 09:00:53.000000 xj_role-1.0.8/xj_role/apis/role_api.py
--rw-rw-rw-   0        0        0      202 2022-09-06 06:05:16.000000 xj_role-1.0.8/xj_role/apps.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role/migrations/
--rw-rw-rw-   0        0        0      546 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1684 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0002_baseinfo.py
--rw-rw-rw-   0        0        0     1373 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0003_auto_20210511_1250.py
--rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0004_auto_20220101_1450.py
--rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0004_auto_20220101_1707.py
--rw-rw-rw-   0        0        0     1469 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0005_auth.py
--rw-rw-rw-   0        0        0      287 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0005_merge_0004_auto_20220101_1450_0004_auto_20220101_1707.py
--rw-rw-rw-   0        0        0      658 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0006_auto_20220205_1300.py
--rw-rw-rw-   0        0        0      322 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0007_merge_20220205_1325.py
--rw-rw-rw-   0        0        0     1071 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/0008_auto_20220206_2238.py
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/migrations/__init__.py
--rw-rw-rw-   0        0        0     6808 2022-09-07 02:09:37.000000 xj_role-1.0.8/xj_role/models.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/services/__init__.py
--rw-rw-rw-   0        0        0     7475 2022-09-13 07:53:08.000000 xj_role-1.0.8/xj_role/services/group_service.py
--rw-rw-rw-   0        0        0     6082 2022-09-08 06:49:36.000000 xj_role-1.0.8/xj_role/services/permission_service.py
--rw-rw-rw-   0        0        0     3619 2022-09-13 01:51:54.000000 xj_role-1.0.8/xj_role/services/role_service.py
--rw-rw-rw-   0        0        0     1340 2022-09-09 05:49:03.000000 xj_role-1.0.8/xj_role/urls.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/custom_response.py
--rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/j_dict.py
--rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/join_list.py
--rw-rw-rw-   0        0        0     7024 2022-09-02 08:00:24.000000 xj_role-1.0.8/xj_role/utils/model_handle.py
--rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_role-1.0.8/xj_role/utils/validator.py
-drwxrwxrwx   0        0        0        0 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role.egg-info/
--rw-rw-rw-   0        0        0      581 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1168 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-09-13 07:57:45.000000 xj_role-1.0.8/xj_role.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/
+-rw-rw-rw-   0        0        0      581 2022-09-15 05:32:40.000000 xj_role-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_role-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-15 05:32:40.000000 xj_role-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2119 2022-09-15 05:32:08.000000 xj_role-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/__init__.py
+-rw-rw-rw-   0        0        0     1916 2022-09-07 02:09:37.000000 xj_role-1.0.9/xj_role/admin.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/apis/__init__.py
+-rw-rw-rw-   0        0        0     3133 2022-09-09 01:10:05.000000 xj_role-1.0.9/xj_role/apis/group_api.py
+-rw-rw-rw-   0        0        0     2506 2022-09-07 02:01:28.000000 xj_role-1.0.9/xj_role/apis/permission_api.py
+-rw-rw-rw-   0        0        0      756 2022-09-08 09:00:53.000000 xj_role-1.0.9/xj_role/apis/role_api.py
+-rw-rw-rw-   0        0        0      202 2022-09-06 06:05:16.000000 xj_role-1.0.9/xj_role/apps.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/migrations/
+-rw-rw-rw-   0        0        0      546 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1684 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0002_baseinfo.py
+-rw-rw-rw-   0        0        0     1373 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0003_auto_20210511_1250.py
+-rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1450.py
+-rw-rw-rw-   0        0        0      527 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1707.py
+-rw-rw-rw-   0        0        0     1469 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0005_auth.py
+-rw-rw-rw-   0        0        0      287 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0005_merge_0004_auto_20220101_1450_0004_auto_20220101_1707.py
+-rw-rw-rw-   0        0        0      658 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0006_auto_20220205_1300.py
+-rw-rw-rw-   0        0        0      322 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0007_merge_20220205_1325.py
+-rw-rw-rw-   0        0        0     1071 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/0008_auto_20220206_2238.py
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6808 2022-09-07 02:09:37.000000 xj_role-1.0.9/xj_role/models.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/services/__init__.py
+-rw-rw-rw-   0        0        0     7475 2022-09-13 07:53:08.000000 xj_role-1.0.9/xj_role/services/group_service.py
+-rw-rw-rw-   0        0        0     6099 2022-09-15 05:24:28.000000 xj_role-1.0.9/xj_role/services/permission_service.py
+-rw-rw-rw-   0        0        0     3619 2022-09-13 01:51:54.000000 xj_role-1.0.9/xj_role/services/role_service.py
+-rw-rw-rw-   0        0        0     1340 2022-09-09 05:49:03.000000 xj_role-1.0.9/xj_role/urls.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/custom_response.py
+-rw-rw-rw-   0        0        0      429 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/j_dict.py
+-rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/join_list.py
+-rw-rw-rw-   0        0        0     7024 2022-09-02 08:00:24.000000 xj_role-1.0.9/xj_role/utils/model_handle.py
+-rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_role-1.0.9/xj_role/utils/validator.py
+drwxrwxrwx   0        0        0        0 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/
+-rw-rw-rw-   0        0        0      581 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1168 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-09-15 05:32:40.000000 xj_role-1.0.9/xj_role.egg-info/top_level.txt
```

### Comparing `xj_role-1.0.8/PKG-INFO` & `xj_role-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_role
-Version: 1.0.8
+Version: 1.0.9
 Summary: 权限模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # Xj-User Module
         
         > 用户模块
```

### Comparing `xj_role-1.0.8/setup.py` & `xj_role-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_role',  # 模块名称
-    version='1.0.8',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='权限模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     # author='sieyoo',
     # author_email='sieyoo@163.com',
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
```

### Comparing `xj_role-1.0.8/xj_role/admin.py` & `xj_role-1.0.9/xj_role/admin.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/apis/group_api.py` & `xj_role-1.0.9/xj_role/apis/group_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/apis/permission_api.py` & `xj_role-1.0.9/xj_role/apis/permission_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/apis/role_api.py` & `xj_role-1.0.9/xj_role/apis/role_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0001_initial.py` & `xj_role-1.0.9/xj_role/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0002_baseinfo.py` & `xj_role-1.0.9/xj_role/migrations/0002_baseinfo.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0003_auto_20210511_1250.py` & `xj_role-1.0.9/xj_role/migrations/0003_auto_20210511_1250.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0004_auto_20220101_1450.py` & `xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1450.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0004_auto_20220101_1707.py` & `xj_role-1.0.9/xj_role/migrations/0004_auto_20220101_1707.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0005_auth.py` & `xj_role-1.0.9/xj_role/migrations/0005_auth.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0006_auto_20220205_1300.py` & `xj_role-1.0.9/xj_role/migrations/0006_auto_20220205_1300.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/migrations/0008_auto_20220206_2238.py` & `xj_role-1.0.9/xj_role/migrations/0008_auto_20220206_2238.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/models.py` & `xj_role-1.0.9/xj_role/models.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/services/group_service.py` & `xj_role-1.0.9/xj_role/services/group_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/services/permission_service.py` & `xj_role-1.0.9/xj_role/services/permission_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             return None, "编辑权限错误：" + str(e)
         return None, None
 
     @staticmethod
     def list(params):
         page = params.pop("page", 1)
         size = params.pop("size", 20)
-        params = format_params_handle(param_dict=params, filter_filed_list=["id", "page", "size", "module", "feature"])
+        params = format_params_handle(param_dict=params, filter_filed_list=["id", "page", "size", "module", "feature", "permission_id"])
         query_set = RolePermissionValue.objects.filter(**params).annotate(permission_name=F("permission__permission_name")).annotate(permission_description=F("permission__description"))
         count = query_set.count()
         query_list = query_set.values() if query_set else []
         finish_set = list(Paginator(query_list, size).page(page).object_list)
         return {"count": count, "page": int(page), "size": int(size), "list": finish_set}, None
```

### Comparing `xj_role-1.0.8/xj_role/services/role_service.py` & `xj_role-1.0.9/xj_role/services/role_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/urls.py` & `xj_role-1.0.9/xj_role/urls.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/utils/custom_authorization.py` & `xj_role-1.0.9/xj_role/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/utils/custom_response.py` & `xj_role-1.0.9/xj_role/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/utils/model_handle.py` & `xj_role-1.0.9/xj_role/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role/utils/validator.py` & `xj_role-1.0.9/xj_role/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.8/xj_role.egg-info/PKG-INFO` & `xj_role-1.0.9/xj_role.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-role
-Version: 1.0.8
+Version: 1.0.9
 Summary: 权限模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # Xj-User Module
         
         > 用户模块
```

### Comparing `xj_role-1.0.8/xj_role.egg-info/SOURCES.txt` & `xj_role-1.0.9/xj_role.egg-info/SOURCES.txt`

 * *Files identical despite different names*

