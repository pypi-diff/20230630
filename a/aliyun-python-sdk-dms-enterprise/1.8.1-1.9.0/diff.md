# Comparing `tmp/aliyun-python-sdk-dms-enterprise-1.8.1.tar.gz` & `tmp/aliyun-python-sdk-dms-enterprise-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dms-enterprise-1.8.1.tar", last modified: Thu Apr 23 14:34:55 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dms-enterprise-1.9.0.tar", last modified: Fri Sep 11 03:24:09 2020, max compression
```

## Comparing `aliyun-python-sdk-dms-enterprise-1.8.1.tar` & `aliyun-python-sdk-dms-enterprise-1.9.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/
--rw-rw-r--   0 admin      (531) admin      (531)       38 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/setup.cfg
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/
--rw-rw-r--   0 admin      (531) admin      (531)        1 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/dependency_links.txt
--rw-rw-r--   0 admin      (531) admin      (531)       31 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/requires.txt
--rw-rw-r--   0 admin      (531) admin      (531)     3758 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/SOURCES.txt
--rw-rw-r--   0 admin      (531) admin      (531)       24 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/top_level.txt
--rw-rw-r--   0 admin      (531) admin      (531)     1592 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/PKG-INFO
--rw-rw-r--   0 admin      (531) admin      (531)     2507 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/setup.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/
--rw-rw-r--   0 admin      (531) admin      (531)       21 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     1087 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/endpoint.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/__init__.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/
--rw-rw-r--   0 admin      (531) admin      (531)     1525 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DisableUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1665 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     1889 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SetOwnersRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2563 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SearchDatabaseRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1969 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDatabaseRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2189 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetOpLogRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2684 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RevokeUserPermissionRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1592 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SubmitOrderApprovalRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1935 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsDetailRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     4781 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/UpdateInstanceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1761 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectBackupFilesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1579 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowNodesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2739 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListInstancesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2409 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SearchTableRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2445 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2191 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListUsersRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1747 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataCorrectRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1575 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataExportOrderDetailRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2001 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RegisterUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2079 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListLogicTablesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1523 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/EnableUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1830 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DeleteInstanceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2679 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListUserPermissionsRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1577 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectOrderDetailRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1903 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListDatabasesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1797 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetInstanceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1575 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataExportDownloadURLRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1627 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetApprovalDetailRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2069 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListTablesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1772 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataExportRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1741 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListLogicDatabasesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2670 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GrantUserPermissionRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1541 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetLogicDatabaseRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1587 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowTemplatesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1828 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ApproveOrderRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2983 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListOrdersRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1691 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListColumnsRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1755 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SyncInstanceMetaRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1691 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListIndexesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2101 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CreateOrderRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2355 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListDatabaseUserPermssionsRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1559 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetOrderBaseInfoRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1523 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DeleteUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2238 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CreatePublishGroupTaskRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1752 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CloseOrderRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     4785 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RegisterInstanceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2395 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/UpdateUserRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1683 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SyncDatabaseMetaRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/MANIFEST.in
--rw-rw-r--   0 admin      (531) admin      (531)      549 2020-04-23 14:34:54.000000 aliyun-python-sdk-dms-enterprise-1.8.1/README.rst
--rw-rw-r--   0 admin      (531) admin      (531)     1592 2020-04-23 14:34:55.000000 aliyun-python-sdk-dms-enterprise-1.8.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1592 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1592 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3895 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/
+-rw-r--r--   0 root         (0) root         (0)       21 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/
+-rw-r--r--   0 root         (0) root         (0)     1828 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ApproveOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CheckFinishMissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CloseOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CreateOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CreatePublishGroupTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DeleteUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DisableUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/EnableUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataCorrectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataExportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteScriptRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetApprovalDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectBackupFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectOrderDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataExportDownloadURLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataExportOrderDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetLogicDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetOpLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetOrderBaseInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GrantUserPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListColumnsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListDatabaseUserPermssionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListIndexesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListLogicDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListLogicTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListTablesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListUserPermissionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RegisterInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RegisterUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RevokeUserPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SearchDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SearchTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SetOwnersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SubmitOrderApprovalRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SyncDatabaseMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SyncInstanceMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/UpdateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/UpdateUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-11 03:24:09.000000 aliyun-python-sdk-dms-enterprise-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2020-09-11 03:24:08.000000 aliyun-python-sdk-dms-enterprise-1.9.0/setup.py
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/SOURCES.txt` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 aliyun_python_sdk_dms_enterprise.egg-info/dependency_links.txt
 aliyun_python_sdk_dms_enterprise.egg-info/requires.txt
 aliyun_python_sdk_dms_enterprise.egg-info/top_level.txt
 aliyunsdkdms_enterprise/__init__.py
 aliyunsdkdms_enterprise/endpoint.py
 aliyunsdkdms_enterprise/request/__init__.py
 aliyunsdkdms_enterprise/request/v20181101/ApproveOrderRequest.py
+aliyunsdkdms_enterprise/request/v20181101/CheckFinishMissionRequest.py
 aliyunsdkdms_enterprise/request/v20181101/CloseOrderRequest.py
 aliyunsdkdms_enterprise/request/v20181101/CreateOrderRequest.py
 aliyunsdkdms_enterprise/request/v20181101/CreatePublishGroupTaskRequest.py
 aliyunsdkdms_enterprise/request/v20181101/DeleteInstanceRequest.py
 aliyunsdkdms_enterprise/request/v20181101/DeleteUserRequest.py
 aliyunsdkdms_enterprise/request/v20181101/DisableUserRequest.py
 aliyunsdkdms_enterprise/request/v20181101/EnableUserRequest.py
 aliyunsdkdms_enterprise/request/v20181101/ExecuteDataCorrectRequest.py
 aliyunsdkdms_enterprise/request/v20181101/ExecuteDataExportRequest.py
+aliyunsdkdms_enterprise/request/v20181101/ExecuteScriptRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetApprovalDetailRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectBackupFilesRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectOrderDetailRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetDataExportDownloadURLRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetDataExportOrderDetailRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetDatabaseRequest.py
 aliyunsdkdms_enterprise/request/v20181101/GetInstanceRequest.py
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyun_python_sdk_dms_enterprise.egg-info/PKG-INFO` & `aliyun-python-sdk-dms-enterprise-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dms-enterprise
-Version: 1.8.1
+Version: 1.9.0
 Summary: The dms-enterprise module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dms-enterprise
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/setup.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/endpoint.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DisableUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DisableUserRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class DisableUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'DisableUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'DisableUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Uid(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetUserRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Uid(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SetOwnersRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SetOwnersRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class SetOwnersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SetOwners','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SetOwners','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SearchDatabaseRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SearchDatabaseRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class SearchDatabaseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SearchDatabase','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SearchDatabase','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchKey(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDatabaseRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDatabaseRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetDatabaseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDatabase','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDatabase','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SchemaName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetOpLogRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetOpLogRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetOpLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetOpLog','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetOpLog','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Module(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RevokeUserPermissionRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RevokeUserPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SubmitOrderApprovalRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SubmitOrderApprovalRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsDetailRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsDetailRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListSensitiveColumnsDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListSensitiveColumnsDetail','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListSensitiveColumnsDetail','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SchemaName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/UpdateInstanceRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/UpdateInstanceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class UpdateInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'UpdateInstance','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'UpdateInstance','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SafeRuleId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectBackupFilesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectBackupFilesRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetDataCorrectBackupFilesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataCorrectBackupFiles','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataCorrectBackupFiles','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ActionDetail(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowNodesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowNodesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListWorkFlowNodesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListWorkFlowNodes','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListWorkFlowNodes','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListInstancesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListInstancesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListInstances','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListInstances','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchKey(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SearchTableRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SearchTableRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class SearchTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SearchTable','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SearchTable','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchTarget(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListSensitiveColumnsRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListSensitiveColumnsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListSensitiveColumns','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListSensitiveColumns','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SchemaName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListUsersRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListUsersRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListUsers','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListUsers','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_UserState(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataCorrectRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataCorrectRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ExecuteDataCorrectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ExecuteDataCorrect','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ExecuteDataCorrect','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ActionDetail(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataExportOrderDetailRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetOrderBaseInfoRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class GetDataExportOrderDetailRequest(RpcRequest):
+class GetOrderBaseInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataExportOrderDetail','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetOrderBaseInfo','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderId(self):
-		return self.get_body_params().get('OrderId')
+		return self.get_query_params().get('OrderId')
 
 	def set_OrderId(self,OrderId):
-		self.add_body_params('OrderId', OrderId)
+		self.add_query_param('OrderId',OrderId)
 
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
 		self.add_query_param('Tid',Tid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RegisterUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RegisterUserRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class RegisterUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'RegisterUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'RegisterUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_RoleNames(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListLogicTablesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListLogicTablesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListLogicTablesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListLogicTables','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListLogicTables','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/EnableUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/EnableUserRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class EnableUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'EnableUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'EnableUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Uid(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DeleteInstanceRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListUserPermissionsRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListUserPermissionsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListUserPermissionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListUserPermissions','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListUserPermissions','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_UserId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectOrderDetailRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataCorrectOrderDetailRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetDataCorrectOrderDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataCorrectOrderDetail','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataCorrectOrderDetail','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListDatabasesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListDatabasesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListDatabasesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListDatabases','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListDatabases','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_InstanceId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetInstanceRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/UpdateUserRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,40 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class GetInstanceRequest(RpcRequest):
+class UpdateUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetInstance','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'UpdateUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_Port(self):
-		return self.get_query_params().get('Port')
+	def get_RoleNames(self):
+		return self.get_query_params().get('RoleNames')
 
-	def set_Port(self,Port):
-		self.add_query_param('Port',Port)
+	def set_RoleNames(self,RoleNames):
+		self.add_query_param('RoleNames',RoleNames)
 
-	def get_Host(self):
-		return self.get_query_params().get('Host')
+	def get_Uid(self):
+		return self.get_query_params().get('Uid')
 
-	def set_Host(self,Host):
-		self.add_query_param('Host',Host)
+	def set_Uid(self,Uid):
+		self.add_query_param('Uid',Uid)
+
+	def get_MaxResultCount(self):
+		return self.get_query_params().get('MaxResultCount')
+
+	def set_MaxResultCount(self,MaxResultCount):
+		self.add_query_param('MaxResultCount',MaxResultCount)
+
+	def get_MaxExecuteCount(self):
+		return self.get_query_params().get('MaxExecuteCount')
+
+	def set_MaxExecuteCount(self,MaxExecuteCount):
+		self.add_query_param('MaxExecuteCount',MaxExecuteCount)
+
+	def get_UserNick(self):
+		return self.get_query_params().get('UserNick')
+
+	def set_UserNick(self,UserNick):
+		self.add_query_param('UserNick',UserNick)
+
+	def get_Mobile(self):
+		return self.get_query_params().get('Mobile')
+
+	def set_Mobile(self,Mobile):
+		self.add_query_param('Mobile',Mobile)
 
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
-		self.add_query_param('Tid',Tid)
-
-	def get_Sid(self):
-		return self.get_query_params().get('Sid')
-
-	def set_Sid(self,Sid):
-		self.add_query_param('Sid',Sid)
+		self.add_query_param('Tid',Tid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetDataExportDownloadURLRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetDataExportDownloadURLRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetDataExportDownloadURLRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataExportDownloadURL','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetDataExportDownloadURL','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetApprovalDetailRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetApprovalDetailRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetApprovalDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetApprovalDetail','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetApprovalDetail','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Tid(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListTablesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListTablesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListTablesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListTables','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListTables','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataExportRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteDataExportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListLogicDatabasesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListLogicDatabasesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListLogicDatabasesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListLogicDatabases','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListLogicDatabases','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_PageSize(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GrantUserPermissionRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GrantUserPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetLogicDatabaseRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetLogicDatabaseRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class GetLogicDatabaseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetLogicDatabase','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetLogicDatabase','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_DbId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowTemplatesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListWorkFlowTemplatesRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListWorkFlowTemplatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListWorkFlowTemplates','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListWorkFlowTemplates','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_SearchName(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ApproveOrderRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ApproveOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListOrdersRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListOrdersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListOrdersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListOrders','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListOrders','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderStatus(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListColumnsRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListColumnsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListColumnsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListColumns','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListColumns','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_TableId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SyncInstanceMetaRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SyncInstanceMetaRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class SyncInstanceMetaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SyncInstanceMeta','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SyncInstanceMeta','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_InstanceId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListIndexesRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListIndexesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListIndexesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListIndexes','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListIndexes','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_TableId(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CreateOrderRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CreateOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class CreateOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'CreateOrder','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'CreateOrder','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_PluginType(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/ListDatabaseUserPermssionsRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ListDatabaseUserPermssionsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class ListDatabaseUserPermssionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListDatabaseUserPermssions','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ListDatabaseUserPermssions','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_PermType(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/GetOrderBaseInfoRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/DeleteUserRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class GetOrderBaseInfoRequest(RpcRequest):
+class DeleteUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetOrderBaseInfo','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'DeleteUser','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_OrderId(self):
-		return self.get_query_params().get('OrderId')
+	def get_Uid(self):
+		return self.get_query_params().get('Uid')
 
-	def set_OrderId(self,OrderId):
-		self.add_query_param('OrderId',OrderId)
+	def set_Uid(self,Uid):
+		self.add_query_param('Uid',Uid)
 
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
 		self.add_query_param('Tid',Tid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/DeleteUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/SyncDatabaseMetaRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,28 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class DeleteUserRequest(RpcRequest):
+class SyncDatabaseMetaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'DeleteUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SyncDatabaseMeta','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_Uid(self):
-		return self.get_query_params().get('Uid')
+	def get_DbId(self):
+		return self.get_query_params().get('DbId')
 
-	def set_Uid(self,Uid):
-		self.add_query_param('Uid',Uid)
+	def set_DbId(self,DbId):
+		self.add_query_param('DbId',DbId)
+
+	def get_Logic(self):
+		return self.get_query_params().get('Logic')
+
+	def set_Logic(self,Logic):
+		self.add_query_param('Logic',Logic)
 
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
 		self.add_query_param('Tid',Tid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CreatePublishGroupTaskRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CreatePublishGroupTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/CloseOrderRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/CloseOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/RegisterInstanceRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/RegisterInstanceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
 class RegisterInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'RegisterInstance','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'RegisterInstance','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_EcsRegion(self):
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/UpdateUserRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/GetInstanceRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,58 +16,41 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class UpdateUserRequest(RpcRequest):
+class GetInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'UpdateUser','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'GetInstance','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_RoleNames(self):
-		return self.get_query_params().get('RoleNames')
+	def get_Port(self):
+		return self.get_query_params().get('Port')
 
-	def set_RoleNames(self,RoleNames):
-		self.add_query_param('RoleNames',RoleNames)
+	def set_Port(self,Port):
+		self.add_query_param('Port',Port)
 
-	def get_Uid(self):
-		return self.get_query_params().get('Uid')
+	def get_Host(self):
+		return self.get_query_params().get('Host')
 
-	def set_Uid(self,Uid):
-		self.add_query_param('Uid',Uid)
-
-	def get_MaxResultCount(self):
-		return self.get_query_params().get('MaxResultCount')
-
-	def set_MaxResultCount(self,MaxResultCount):
-		self.add_query_param('MaxResultCount',MaxResultCount)
-
-	def get_MaxExecuteCount(self):
-		return self.get_query_params().get('MaxExecuteCount')
-
-	def set_MaxExecuteCount(self,MaxExecuteCount):
-		self.add_query_param('MaxExecuteCount',MaxExecuteCount)
-
-	def get_UserNick(self):
-		return self.get_query_params().get('UserNick')
-
-	def set_UserNick(self,UserNick):
-		self.add_query_param('UserNick',UserNick)
-
-	def get_Mobile(self):
-		return self.get_query_params().get('Mobile')
-
-	def set_Mobile(self,Mobile):
-		self.add_query_param('Mobile',Mobile)
+	def set_Host(self,Host):
+		self.add_query_param('Host',Host)
 
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
-		self.add_query_param('Tid',Tid)
+		self.add_query_param('Tid',Tid)
+
+	def get_Sid(self):
+		return self.get_query_params().get('Sid')
+
+	def set_Sid(self,Sid):
+		self.add_query_param('Sid',Sid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/aliyunsdkdms_enterprise/request/v20181101/SyncDatabaseMetaRequest.py` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyunsdkdms_enterprise/request/v20181101/ExecuteScriptRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdms_enterprise.endpoint import endpoint_data
 
-class SyncDatabaseMetaRequest(RpcRequest):
+class ExecuteScriptRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'SyncDatabaseMeta','dmsenterprise')
+		RpcRequest.__init__(self, 'dms-enterprise', '2018-11-01', 'ExecuteScript','dmsenterprise')
+		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_DbId(self):
@@ -38,12 +39,18 @@
 
 	def get_Logic(self):
 		return self.get_query_params().get('Logic')
 
 	def set_Logic(self,Logic):
 		self.add_query_param('Logic',Logic)
 
+	def get_Script(self):
+		return self.get_query_params().get('Script')
+
+	def set_Script(self,Script):
+		self.add_query_param('Script',Script)
+
 	def get_Tid(self):
 		return self.get_query_params().get('Tid')
 
 	def set_Tid(self,Tid):
 		self.add_query_param('Tid',Tid)
```

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/README.rst` & `aliyun-python-sdk-dms-enterprise-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dms-enterprise-1.8.1/PKG-INFO` & `aliyun-python-sdk-dms-enterprise-1.9.0/aliyun_python_sdk_dms_enterprise.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dms-enterprise
-Version: 1.8.1
+Version: 1.9.0
 Summary: The dms-enterprise module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dms-enterprise
```

