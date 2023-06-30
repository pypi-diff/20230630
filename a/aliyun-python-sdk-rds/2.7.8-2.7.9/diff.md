# Comparing `tmp/aliyun-python-sdk-rds-2.7.8.tar.gz` & `tmp/aliyun-python-sdk-rds-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-rds-2.7.8.tar", last modified: Mon Jun 26 06:03:37 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-rds-2.7.9.tar", last modified: Thu Jun 29 05:59:41 2023, max compression
```

## Comparing `aliyun-python-sdk-rds-2.7.8.tar` & `aliyun-python-sdk-rds-2.7.9.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16817 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3092 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/
--rw-r--r--   0 root         (0) root         (0)     2339 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ActivateMigrationTargetInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4674 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AddTagsToResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AllocateInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AllocateReadWriteSplittingConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CalculateDBInstanceWeightRequest.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CancelImportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckAccountNameAvailableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckCloudResourceAuthorizedRequest.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckCreateDdrDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckDBNameAvailableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckInstanceExistRequest.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     6956 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CloneDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CloneParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ConfirmNotifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CopyDatabaseBetweenInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CopyDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     3165 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateCloudMigrationPrecheckTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateCloudMigrationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3651 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     5352 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceForRebuildRequest.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3383 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBProxyEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     7313 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDdrInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDiagnosticReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     6219 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateGADInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     5448 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateGadInstanceMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     3483 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateMigrateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateOnlineDatabaseTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     8074 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateReadOnlyDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateSecretRequest.py
--rw-r--r--   0 root         (0) root         (0)     2158 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateTempDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteADSettingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2651 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteBackupFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2158 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBProxyEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteGadInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteSecretRequest.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteUserBackupFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescibeImportsFromDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeADInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeActionEventPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeActiveOperationTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAnalyticdbByPrimaryDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableClassesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableCrossRegionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableRecoveryTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBinlogFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCharacterSetNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCloudMigrationPrecheckResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCloudMigrationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCollationTimeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossBackupMetaListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3113 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionLogBackupFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceByTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceEncryptionKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceHAConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceIPArrayListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceIpHostnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1945 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoForChannelRequest.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancePromoteActivityRequest.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceProxyConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesAsCsvRequest.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesByExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     5663 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesByPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     6259 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesForCloneRequest.py
--rw-r--r--   0 root         (0) root         (0)     7620 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBMiniEngineVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDTCSecurityIpHostsForSQLServerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDedicatedHostGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3328 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDedicatedHostsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDetachedBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDiagnosticReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeErrorLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeGadInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHADiagnoseConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHASwitchConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     4430 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHistoryTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHostWebShellRequest.py
--rw-r--r--   0 root         (0) root         (0)     3101 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceCrossBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceKeywordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeLocalAvailableRecoveryTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3061 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeLogBackupFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMetaListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2558 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMigrateTaskByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMigrateTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3117 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeModifyPGHbaConfigLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeModifyParameterLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeOssDownloadsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribePGHbaConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribePriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRdsResourceSettingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeReadDBInstanceDelayRequest.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRegionInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRenewalPriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeResourceUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2755 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLCollectorRetentionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSecretsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlowLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSupportOnlineResizeDiskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3145 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionPrecheckTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3131 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeVSwitchesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DestroyDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DetachGadInstanceMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GetDBInstanceTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1720 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GetDbProxyInstanceSslRequest.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GrantAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GrantOperatorPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2751 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ImportDatabaseBetweenInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3248 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ImportUserBackupFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListClassesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2988 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListUserBackupFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/LockAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateConnectionToOtherZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     3837 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateSecurityIPModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4472 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateToOtherZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyADInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyActionEventPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyActiveOperationTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     7490 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyCollationTimeZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceAutoUpgradeMinorVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3472 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     2421 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDelayedReplicationTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDeletionProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceHAConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4289 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstancePayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2676 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceProxyConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     4580 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     3805 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDTCSecurityIpHostsForSQLServerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDasInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDbProxyInstanceSslRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyHADiagnoseConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyHASwitchConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2914 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3414 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyInstanceCrossBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4061 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyPGHbaConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyReadWriteSplittingConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyReadonlyInstanceDelayReplicationTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySQLCollectorRetentionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/PurgeDBInstanceLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/QueryNotifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RebuildDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReceiveDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4536 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RecoveryDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseInstanceConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2616 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseReadWriteSplittingConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RemoveTagsFromResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RenewInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2743 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ResetAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3742 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestoreDdrTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestoreTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RevokeAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RevokeOperatorPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     4930 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/StartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/StopDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceHARequest.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceNetTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceVpcRequest.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchGuardToMasterInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2795 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TerminateMigrateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3443 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TransformDBInstancePayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UnlockAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpdateUserBackupFileRequest.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceEngineVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceKernelVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionPrecheckRequest.py
--rw-r--r--   0 root         (0) root         (0)     5400 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBProxyInstanceKernelVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-06-26 06:03:37.000000 aliyun-python-sdk-rds-2.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16817 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3092 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ActivateMigrationTargetInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4674 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AddTagsToResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AllocateInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AllocateReadWriteSplittingConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CalculateDBInstanceWeightRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CancelImportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckAccountNameAvailableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckCloudResourceAuthorizedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckCreateDdrDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckDBNameAvailableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckInstanceExistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6956 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CloneDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CloneParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ConfirmNotifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CopyDatabaseBetweenInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CopyDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateCloudMigrationPrecheckTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateCloudMigrationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5352 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceForRebuildRequest.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBProxyEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7313 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDdrInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDiagnosticReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateGADInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5448 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateGadInstanceMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3483 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateMigrateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateOnlineDatabaseTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateReadOnlyDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateSecretRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateTempDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteADSettingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteBackupFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBProxyEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteGadInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteSecretRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteUserBackupFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescibeImportsFromDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeADInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeActionEventPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeActiveOperationTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAnalyticdbByPrimaryDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableClassesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableCrossRegionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableRecoveryTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBinlogFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCharacterSetNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCloudMigrationPrecheckResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCloudMigrationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCollationTimeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossBackupMetaListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionLogBackupFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceByTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceEncryptionKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceHAConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceIPArrayListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceIpHostnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoForChannelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancePromoteActivityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceProxyConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceTDERequest.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesAsCsvRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesByExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesByPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesForCloneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7620 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBMiniEngineVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDTCSecurityIpHostsForSQLServerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDedicatedHostGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDedicatedHostsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDetachedBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDiagnosticReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeErrorLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeGadInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHADiagnoseConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHASwitchConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHistoryTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHostWebShellRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceCrossBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceKeywordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeLocalAvailableRecoveryTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeLogBackupFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMetaListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMigrateTaskByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMigrateTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeModifyPGHbaConfigLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeModifyParameterLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeOssDownloadsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribePGHbaConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribePriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRdsResourceSettingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeReadDBInstanceDelayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRegionInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRenewalPriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeResourceUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLCollectorRetentionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSecretsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlowLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSupportOnlineResizeDiskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionPrecheckTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeVSwitchesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DestroyDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DetachGadInstanceMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GetDBInstanceTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GetDbProxyInstanceSslRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GrantAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GrantOperatorPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ImportDatabaseBetweenInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ImportUserBackupFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListClassesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListUserBackupFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/LockAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateConnectionToOtherZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateSecurityIPModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateToOtherZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyADInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyActionEventPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyActiveOperationTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7490 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyCollationTimeZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceAutoUpgradeMinorVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDelayedReplicationTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDeletionProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceHAConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4289 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstancePayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceProxyConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceTDERequest.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDTCSecurityIpHostsForSQLServerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDasInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDbProxyInstanceSslRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyHADiagnoseConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyHASwitchConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyInstanceCrossBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyPGHbaConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyReadWriteSplittingConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyReadonlyInstanceDelayReplicationTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySQLCollectorRetentionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/PurgeDBInstanceLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/QueryNotifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RebuildDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReceiveDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4536 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RecoveryDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseInstanceConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseReadWriteSplittingConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RemoveTagsFromResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RenewInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ResetAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestoreDdrTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestoreTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RevokeAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RevokeOperatorPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/StartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/StopDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2858 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceHARequest.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceNetTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceVpcRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchGuardToMasterInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TerminateMigrateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TransformDBInstancePayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UnlockAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpdateUserBackupFileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceEngineVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceKernelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionPrecheckRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5400 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBProxyInstanceKernelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-29 05:59:41.000000 aliyun-python-sdk-rds-2.7.9/setup.py
```

### Comparing `aliyun-python-sdk-rds-2.7.8/LICENSE` & `aliyun-python-sdk-rds-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/PKG-INFO` & `aliyun-python-sdk-rds-2.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-rds
-Version: 2.7.8
+Version: 2.7.9
 Summary: The rds module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-rds
```

### Comparing `aliyun-python-sdk-rds-2.7.8/README.rst` & `aliyun-python-sdk-rds-2.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/PKG-INFO` & `aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-rds
-Version: 2.7.8
+Version: 2.7.9
 Summary: The rds module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-rds
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyun_python_sdk_rds.egg-info/SOURCES.txt` & `aliyun-python-sdk-rds-2.7.9/aliyun_python_sdk_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/endpoint.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ActivateMigrationTargetInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ActivateMigrationTargetInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AddTagsToResourceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AddTagsToResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AllocateInstancePublicConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyInstanceAutoRenewalAttributeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,40 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class AllocateInstancePublicConnectionRequest(RpcRequest):
+class ModifyInstanceAutoRenewalAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'AllocateInstancePublicConnection','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyInstanceAutoRenewalAttribute','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ConnectionStringPrefix(self): # String
-		return self.get_query_params().get('ConnectionStringPrefix')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
-		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
-	def get_GeneralGroupName(self): # String
-		return self.get_query_params().get('GeneralGroupName')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_Duration(self): # String
+		return self.get_query_params().get('Duration')
 
-	def set_GeneralGroupName(self, GeneralGroupName):  # String
-		self.add_query_param('GeneralGroupName', GeneralGroupName)
+	def set_Duration(self, Duration):  # String
+		self.add_query_param('Duration', Duration)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -62,17 +62,12 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_BabelfishPort(self): # String
-		return self.get_query_params().get('BabelfishPort')
+	def get_AutoRenew(self): # String
+		return self.get_query_params().get('AutoRenew')
 
-	def set_BabelfishPort(self, BabelfishPort):  # String
-		self.add_query_param('BabelfishPort', BabelfishPort)
-	def get_Port(self): # String
-		return self.get_query_params().get('Port')
-
-	def set_Port(self, Port):  # String
-		self.add_query_param('Port', Port)
+	def set_AutoRenew(self, AutoRenew):  # String
+		self.add_query_param('AutoRenew', AutoRenew)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/AllocateReadWriteSplittingConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AllocateReadWriteSplittingConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CalculateDBInstanceWeightRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CalculateDBInstanceWeightRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CancelImportRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CancelImportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckAccountNameAvailableRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckAccountNameAvailableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckCloudResourceAuthorizedRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckCloudResourceAuthorizedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckCreateDdrDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckCreateDdrDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckDBNameAvailableRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckDBNameAvailableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckInstanceExistRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckInstanceExistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CheckServiceLinkedRoleRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CheckServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CloneDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CloneDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CloneParameterGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CloneParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ConfirmNotifyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ConfirmNotifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CopyDatabaseBetweenInstancesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CopyDatabaseBetweenInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CopyDatabaseRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CopyDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateAccountRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateBackupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateCloudMigrationPrecheckTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateCloudMigrationPrecheckTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateCloudMigrationTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateCloudMigrationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointAddressRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_IpType(self): # String
 		return self.get_query_params().get('IpType')
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceEndpointRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointAddressRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class CreateDBInstanceEndpointRequest(RpcRequest):
+class ModifyDBInstanceEndpointAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'CreateDBInstanceEndpoint','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceEndpointAddress','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -42,44 +42,39 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_ConnectionString(self): # String
+		return self.get_query_params().get('ConnectionString')
+
+	def set_ConnectionString(self, ConnectionString):  # String
+		self.add_query_param('ConnectionString', ConnectionString)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_DBInstanceEndpointDescription(self): # String
-		return self.get_query_params().get('DBInstanceEndpointDescription')
-
-	def set_DBInstanceEndpointDescription(self, DBInstanceEndpointDescription):  # String
-		self.add_query_param('DBInstanceEndpointDescription', DBInstanceEndpointDescription)
-	def get_DBInstanceEndpointType(self): # String
-		return self.get_query_params().get('DBInstanceEndpointType')
-
-	def set_DBInstanceEndpointType(self, DBInstanceEndpointType):  # String
-		self.add_query_param('DBInstanceEndpointType', DBInstanceEndpointType)
-	def get_NodeItems(self): # String
-		return self.get_query_params().get('NodeItems')
-
-	def set_NodeItems(self, NodeItems):  # String
-		self.add_query_param('NodeItems', NodeItems)
 	def get_VSwitchId(self): # String
 		return self.get_query_params().get('VSwitchId')
 
 	def set_VSwitchId(self, VSwitchId):  # String
 		self.add_query_param('VSwitchId', VSwitchId)
 	def get_PrivateIpAddress(self): # String
 		return self.get_query_params().get('PrivateIpAddress')
 
 	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
 		self.add_query_param('PrivateIpAddress', PrivateIpAddress)
+	def get_DBInstanceEndpointId(self): # String
+		return self.get_query_params().get('DBInstanceEndpointId')
+
+	def set_DBInstanceEndpointId(self, DBInstanceEndpointId):  # String
+		self.add_query_param('DBInstanceEndpointId', DBInstanceEndpointId)
 	def get_Port(self): # String
 		return self.get_query_params().get('Port')
 
 	def set_Port(self, Port):  # String
 		self.add_query_param('Port', Port)
 	def get_VpcId(self): # String
 		return self.get_query_params().get('VpcId')
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceForRebuildRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceForRebuildRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBNodesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBNodesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class CreateDBNodesRequest(RpcRequest):
+class DeleteDBNodesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'CreateDBNodes','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'DeleteDBNodes','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DBNodeId(self): # String
+		return self.get_query_params().get('DBNodeId')
+
+	def set_DBNodeId(self, DBNodeId):  # String
+		self.add_query_param('DBNodeId', DBNodeId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
@@ -57,12 +62,7 @@
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_DBNode(self): # String
-		return self.get_query_params().get('DBNode')
-
-	def set_DBNode(self, DBNode):  # String
-		self.add_query_param('DBNode', DBNode)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDBProxyEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBProxyEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDatabaseRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDdrInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDdrInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateDiagnosticReportRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDiagnosticReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateGADInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateGADInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateGadInstanceMemberRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateGadInstanceMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateMigrateTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateMigrateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateOnlineDatabaseTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateOnlineDatabaseTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateParameterGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateReadOnlyDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateReadOnlyDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateSecretRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateSecretRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateServiceLinkedRoleRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/CreateTempDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateTempDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteADSettingRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteADSettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteAccountRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteBackupFileRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteBackupFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteBackupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBNodesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceMonitorRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class DeleteDBNodesRequest(RpcRequest):
+class DescribeDBInstanceMonitorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'DeleteDBNodes','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'DescribeDBInstanceMonitor','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_DBNodeId(self): # String
-		return self.get_query_params().get('DBNodeId')
-
-	def set_DBNodeId(self, DBNodeId):  # String
-		self.add_query_param('DBNodeId', DBNodeId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDBProxyEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDBProxyEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteDatabaseRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteGadInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteGadInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteParameterGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteSecretRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteSecretRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteSlotRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DeleteUserBackupFileRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DeleteUserBackupFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescibeImportsFromDatabaseRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescibeImportsFromDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeADInfoRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeADInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAccountsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeActionEventPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeActionEventPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeActiveOperationTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeActiveOperationTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAnalyticdbByPrimaryDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAnalyticdbByPrimaryDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableClassesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableClassesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableCrossRegionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableCrossRegionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableMetricsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableRecoveryTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableRecoveryTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeAvailableZonesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeAvailableZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupDatabaseRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBackupsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeBinlogFilesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeBinlogFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCharacterSetNameRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCharacterSetNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCloudMigrationPrecheckResultRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCloudMigrationPrecheckResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCloudMigrationResultRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCloudMigrationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCollationTimeZonesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCollationTimeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossBackupMetaListRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossBackupMetaListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeCrossRegionLogBackupFilesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeCrossRegionLogBackupFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceAttributeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceByTagsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceByTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceDetailRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceEncryptionKeyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceEncryptionKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceEndpointsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceHAConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceHAConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceIPArrayListRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceIPArrayListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceIpHostnameRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceIpHostnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceMetricsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceMonitorRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestartDBInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class DescribeDBInstanceMonitorRequest(RpcRequest):
+class RestartDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'DescribeDBInstanceMonitor','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestartDBInstance','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ResourceOwnerAccount(self): # String
-		return self.get_query_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_DBInstanceId(self): # String
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self, DBInstanceId):  # String
+		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ResourceOwnerAccount(self): # String
+		return self.get_query_params().get('ResourceOwnerAccount')
+
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
-
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoForChannelRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoForChannelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceNetInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancePerformanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancePromoteActivityRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancePromoteActivityRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceProxyConfigurationRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceProxyConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceSSLRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstanceTDERequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstanceTDERequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesAsCsvRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesAsCsvRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesByExpireTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesByExpireTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesByPerformanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesByPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesForCloneRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesForCloneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBInstancesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBMiniEngineVersionsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBMiniEngineVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyEndpointRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyPerformanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDBProxyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDBProxyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDTCSecurityIpHostsForSQLServerRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDTCSecurityIpHostsForSQLServerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDatabasesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDedicatedHostGroupsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDedicatedHostGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDedicatedHostsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDedicatedHostsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDetachedBackupsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDetachedBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeDiagnosticReportListRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeDiagnosticReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeErrorLogsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeErrorLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeEventsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeGadInstancesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeGadInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHADiagnoseConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHADiagnoseConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHASwitchConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHASwitchConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHistoryTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHistoryTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeHostWebShellRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeHostWebShellRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceAutoRenewalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceCrossBackupPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceCrossBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeInstanceKeywordsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeInstanceKeywordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeLocalAvailableRecoveryTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeLocalAvailableRecoveryTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeLogBackupFilesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeLogBackupFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMetaListRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMetaListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMigrateTaskByIdRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMigrateTaskByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeMigrateTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeMigrateTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeModifyPGHbaConfigLogRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeModifyPGHbaConfigLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeModifyParameterLogRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeModifyParameterLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeOssDownloadsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeOssDownloadsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribePGHbaConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribePGHbaConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterGroupsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParameterTemplatesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParameterTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeParametersRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribePriceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRdsResourceSettingsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRdsResourceSettingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeReadDBInstanceDelayRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeReadDBInstanceDelayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRegionInfosRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRegionInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRegionsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeRenewalPriceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeRenewalPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeResourceUsageRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeResourceUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLCollectorPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLCollectorRetentionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLCollectorRetentionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogFilesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogRecordsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSQLLogReportListRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSQLLogReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSecretsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSecretsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlotsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSlowLogsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSlowLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeSupportOnlineResizeDiskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeSupportOnlineResizeDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeTagsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionPrecheckTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionPrecheckTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeUpgradeMajorVersionTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DescribeVSwitchesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DescribeVSwitchesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DestroyDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DestroyDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/DetachGadInstanceMemberRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/DetachGadInstanceMemberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GetDBInstanceTopologyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GetDBInstanceTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GetDbProxyInstanceSslRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GetDbProxyInstanceSslRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GrantAccountPrivilegeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GrantAccountPrivilegeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/GrantOperatorPermissionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/GrantOperatorPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ImportDatabaseBetweenInstancesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ImportDatabaseBetweenInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ImportUserBackupFileRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ImportUserBackupFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListClassesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListClassesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListTagResourcesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ListUserBackupFilesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ListUserBackupFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/LockAccountRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/LockAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateConnectionToOtherZoneRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateConnectionToOtherZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateSecurityIPModeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateSecurityIPModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/MigrateToOtherZoneRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/MigrateToOtherZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyADInfoRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyADInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyActionEventPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyActionEventPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyActiveOperationTasksRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyActiveOperationTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyCollationTimeZoneRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyCollationTimeZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBDescriptionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceAutoUpgradeMinorVersionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceAutoUpgradeMinorVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionModeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionStringRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceNetTypeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class ModifyDBInstanceConnectionStringRequest(RpcRequest):
+class SwitchDBInstanceNetTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceConnectionString','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'SwitchDBInstanceNetType','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,19 +37,19 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ConnectionStringPrefix(self): # String
 		return self.get_query_params().get('ConnectionStringPrefix')
 
 	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
 		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
-	def get_GeneralGroupName(self): # String
-		return self.get_query_params().get('GeneralGroupName')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_GeneralGroupName(self, GeneralGroupName):  # String
-		self.add_query_param('GeneralGroupName', GeneralGroupName)
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -62,22 +62,17 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_BabelfishPort(self): # String
-		return self.get_query_params().get('BabelfishPort')
+	def get_ConnectionStringType(self): # String
+		return self.get_query_params().get('ConnectionStringType')
 
-	def set_BabelfishPort(self, BabelfishPort):  # String
-		self.add_query_param('BabelfishPort', BabelfishPort)
-	def get_CurrentConnectionString(self): # String
-		return self.get_query_params().get('CurrentConnectionString')
-
-	def set_CurrentConnectionString(self, CurrentConnectionString):  # String
-		self.add_query_param('CurrentConnectionString', CurrentConnectionString)
+	def set_ConnectionStringType(self, ConnectionStringType):  # String
+		self.add_query_param('ConnectionStringType', ConnectionStringType)
 	def get_Port(self): # String
 		return self.get_query_params().get('Port')
 
 	def set_Port(self, Port):  # String
 		self.add_query_param('Port', Port)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDelayedReplicationTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDelayedReplicationTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDeletionProtectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDeletionProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceDescriptionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceTDERequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,68 +16,83 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class ModifyDBInstanceEndpointAddressRequest(RpcRequest):
+class ModifyDBInstanceTDERequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceEndpointAddress','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceTDE','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ConnectionStringPrefix(self): # String
-		return self.get_query_params().get('ConnectionStringPrefix')
-
-	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
-		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
+	def get_Certificate(self): # String
+		return self.get_query_params().get('Certificate')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_ConnectionString(self): # String
-		return self.get_query_params().get('ConnectionString')
+	def set_Certificate(self, Certificate):  # String
+		self.add_query_param('Certificate', Certificate)
+	def get_PrivateKey(self): # String
+		return self.get_query_params().get('PrivateKey')
+
+	def set_PrivateKey(self, PrivateKey):  # String
+		self.add_query_param('PrivateKey', PrivateKey)
+	def get_PassWord(self): # String
+		return self.get_query_params().get('PassWord')
 
-	def set_ConnectionString(self, ConnectionString):  # String
-		self.add_query_param('ConnectionString', ConnectionString)
+	def set_PassWord(self, PassWord):  # String
+		self.add_query_param('PassWord', PassWord)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_VSwitchId(self): # String
-		return self.get_query_params().get('VSwitchId')
+	def get_ResourceOwnerAccount(self): # String
+		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_VSwitchId(self, VSwitchId):  # String
-		self.add_query_param('VSwitchId', VSwitchId)
-	def get_PrivateIpAddress(self): # String
-		return self.get_query_params().get('PrivateIpAddress')
-
-	def set_PrivateIpAddress(self, PrivateIpAddress):  # String
-		self.add_query_param('PrivateIpAddress', PrivateIpAddress)
-	def get_DBInstanceEndpointId(self): # String
-		return self.get_query_params().get('DBInstanceEndpointId')
-
-	def set_DBInstanceEndpointId(self, DBInstanceEndpointId):  # String
-		self.add_query_param('DBInstanceEndpointId', DBInstanceEndpointId)
-	def get_Port(self): # String
-		return self.get_query_params().get('Port')
-
-	def set_Port(self, Port):  # String
-		self.add_query_param('Port', Port)
-	def get_VpcId(self): # String
-		return self.get_query_params().get('VpcId')
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_IsRotate(self): # Boolean
+		return self.get_query_params().get('IsRotate')
+
+	def set_IsRotate(self, IsRotate):  # Boolean
+		self.add_query_param('IsRotate', IsRotate)
+	def get_EncryptionKey(self): # String
+		return self.get_query_params().get('EncryptionKey')
+
+	def set_EncryptionKey(self, EncryptionKey):  # String
+		self.add_query_param('EncryptionKey', EncryptionKey)
+	def get_OwnerId(self): # Long
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_DBName(self): # String
+		return self.get_query_params().get('DBName')
+
+	def set_DBName(self, DBName):  # String
+		self.add_query_param('DBName', DBName)
+	def get_RoleArn(self): # String
+		return self.get_query_params().get('RoleArn')
+
+	def set_RoleArn(self, RoleArn):  # String
+		self.add_query_param('RoleArn', RoleArn)
+	def get_TDEStatus(self): # String
+		return self.get_query_params().get('TDEStatus')
 
-	def set_VpcId(self, VpcId):  # String
-		self.add_query_param('VpcId', VpcId)
+	def set_TDEStatus(self, TDEStatus):  # String
+		self.add_query_param('TDEStatus', TDEStatus)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceHAConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceHAConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMaintainTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMetricsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceMonitorRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkExpireTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkExpireTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkTypeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceNetworkTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstancePayTypeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstancePayTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceProxyConfigurationRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceProxyConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceSSLRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceSpecRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBInstanceTDERequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyParameterRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,83 +16,73 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class ModifyDBInstanceTDERequest(RpcRequest):
+class ModifyParameterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceTDE','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyParameter','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_Certificate(self): # String
-		return self.get_query_params().get('Certificate')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_Certificate(self, Certificate):  # String
-		self.add_query_param('Certificate', Certificate)
-	def get_PrivateKey(self): # String
-		return self.get_query_params().get('PrivateKey')
-
-	def set_PrivateKey(self, PrivateKey):  # String
-		self.add_query_param('PrivateKey', PrivateKey)
-	def get_PassWord(self): # String
-		return self.get_query_params().get('PassWord')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_SwitchTimeMode(self): # String
+		return self.get_query_params().get('SwitchTimeMode')
+
+	def set_SwitchTimeMode(self, SwitchTimeMode):  # String
+		self.add_query_param('SwitchTimeMode', SwitchTimeMode)
+	def get_ParameterGroupId(self): # String
+		return self.get_query_params().get('ParameterGroupId')
 
-	def set_PassWord(self, PassWord):  # String
-		self.add_query_param('PassWord', PassWord)
+	def set_ParameterGroupId(self, ParameterGroupId):  # String
+		self.add_query_param('ParameterGroupId', ParameterGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Forcerestart(self): # Boolean
+		return self.get_query_params().get('Forcerestart')
+
+	def set_Forcerestart(self, Forcerestart):  # Boolean
+		self.add_query_param('Forcerestart', Forcerestart)
+	def get_SwitchTime(self): # String
+		return self.get_query_params().get('SwitchTime')
+
+	def set_SwitchTime(self, SwitchTime):  # String
+		self.add_query_param('SwitchTime', SwitchTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
-	def get_IsRotate(self): # Boolean
-		return self.get_query_params().get('IsRotate')
-
-	def set_IsRotate(self, IsRotate):  # Boolean
-		self.add_query_param('IsRotate', IsRotate)
-	def get_EncryptionKey(self): # String
-		return self.get_query_params().get('EncryptionKey')
-
-	def set_EncryptionKey(self, EncryptionKey):  # String
-		self.add_query_param('EncryptionKey', EncryptionKey)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_DBName(self): # String
-		return self.get_query_params().get('DBName')
-
-	def set_DBName(self, DBName):  # String
-		self.add_query_param('DBName', DBName)
-	def get_RoleArn(self): # String
-		return self.get_query_params().get('RoleArn')
-
-	def set_RoleArn(self, RoleArn):  # String
-		self.add_query_param('RoleArn', RoleArn)
-	def get_TDEStatus(self): # String
-		return self.get_query_params().get('TDEStatus')
+	def get_Parameters(self): # String
+		return self.get_query_params().get('Parameters')
 
-	def set_TDEStatus(self, TDEStatus):  # String
-		self.add_query_param('TDEStatus', TDEStatus)
+	def set_Parameters(self, Parameters):  # String
+		self.add_query_param('Parameters', Parameters)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointAddressRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDBProxyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBProxyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDTCSecurityIpHostsForSQLServerRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDTCSecurityIpHostsForSQLServerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDasInstanceConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDasInstanceConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyDbProxyInstanceSslRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDbProxyInstanceSslRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyHADiagnoseConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyHADiagnoseConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyHASwitchConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyHASwitchConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RenewInstanceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class ModifyInstanceAutoRenewalAttributeRequest(RpcRequest):
+class RenewInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyInstanceAutoRenewalAttribute','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RenewInstance','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,34 +37,34 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_Duration(self): # String
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self, Duration):  # String
-		self.add_query_param('Duration', Duration)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_Period(self): # Integer
+		return self.get_query_params().get('Period')
+
+	def set_Period(self, Period):  # Integer
+		self.add_query_param('Period', Period)
+	def get_AutoPay(self): # String
+		return self.get_query_params().get('AutoPay')
+
+	def set_AutoPay(self, AutoPay):  # String
+		self.add_query_param('AutoPay', AutoPay)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
 	def get_AutoRenew(self): # String
 		return self.get_query_params().get('AutoRenew')
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyInstanceCrossBackupPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyInstanceCrossBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyPGHbaConfigRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyPGHbaConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyParameterGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyParameterRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestoreDdrTableRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,73 +16,78 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class ModifyParameterRequest(RpcRequest):
+class RestoreDdrTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyParameter','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestoreDdrTable','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_SourceDBInstanceName(self): # String
+		return self.get_query_params().get('SourceDBInstanceName')
+
+	def set_SourceDBInstanceName(self, SourceDBInstanceName):  # String
+		self.add_query_param('SourceDBInstanceName', SourceDBInstanceName)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_SwitchTimeMode(self): # String
-		return self.get_query_params().get('SwitchTimeMode')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_SwitchTimeMode(self, SwitchTimeMode):  # String
-		self.add_query_param('SwitchTimeMode', SwitchTimeMode)
-	def get_ParameterGroupId(self): # String
-		return self.get_query_params().get('ParameterGroupId')
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_TableMeta(self): # String
+		return self.get_query_params().get('TableMeta')
 
-	def set_ParameterGroupId(self, ParameterGroupId):  # String
-		self.add_query_param('ParameterGroupId', ParameterGroupId)
+	def set_TableMeta(self, TableMeta):  # String
+		self.add_query_param('TableMeta', TableMeta)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Forcerestart(self): # Boolean
-		return self.get_query_params().get('Forcerestart')
-
-	def set_Forcerestart(self, Forcerestart):  # Boolean
-		self.add_query_param('Forcerestart', Forcerestart)
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
+	def get_RestoreTime(self): # String
+		return self.get_query_params().get('RestoreTime')
 
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
+	def set_RestoreTime(self, RestoreTime):  # String
+		self.add_query_param('RestoreTime', RestoreTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_query_params().get('OwnerAccount')
+	def get_BackupId(self): # String
+		return self.get_query_params().get('BackupId')
 
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
+	def set_BackupId(self, BackupId):  # String
+		self.add_query_param('BackupId', BackupId)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_Parameters(self): # String
-		return self.get_query_params().get('Parameters')
+	def get_RestoreType(self): # String
+		return self.get_query_params().get('RestoreType')
+
+	def set_RestoreType(self, RestoreType):  # String
+		self.add_query_param('RestoreType', RestoreType)
+	def get_SourceRegion(self): # String
+		return self.get_query_params().get('SourceRegion')
 
-	def set_Parameters(self, Parameters):  # String
-		self.add_query_param('Parameters', Parameters)
+	def set_SourceRegion(self, SourceRegion):  # String
+		self.add_query_param('SourceRegion', SourceRegion)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyReadWriteSplittingConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyReadWriteSplittingConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyReadonlyInstanceDelayReplicationTimeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyReadonlyInstanceDelayReplicationTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifyResourceGroupRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySQLCollectorPolicyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySQLCollectorRetentionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySQLCollectorRetentionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/PurgeDBInstanceLogRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/PurgeDBInstanceLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/QueryNotifyRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/QueryNotifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RebuildDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RebuildDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReceiveDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReceiveDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RecoveryDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RecoveryDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseInstanceConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseInstanceConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseInstancePublicConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ReleaseReadWriteSplittingConnectionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ReleaseReadWriteSplittingConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RemoveTagsFromResourceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RemoveTagsFromResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RenewInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TransformDBInstancePayTypeRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class RenewInstanceRequest(RpcRequest):
+class TransformDBInstancePayTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RenewInstance','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'TransformDBInstancePayType','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -42,32 +42,47 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_Period(self): # Integer
+	def get_BusinessInfo(self): # String
+		return self.get_query_params().get('BusinessInfo')
+
+	def set_BusinessInfo(self, BusinessInfo):  # String
+		self.add_query_param('BusinessInfo', BusinessInfo)
+	def get_Period(self): # String
 		return self.get_query_params().get('Period')
 
-	def set_Period(self, Period):  # Integer
+	def set_Period(self, Period):  # String
 		self.add_query_param('Period', Period)
-	def get_AutoPay(self): # String
-		return self.get_query_params().get('AutoPay')
-
-	def set_AutoPay(self, AutoPay):  # String
-		self.add_query_param('AutoPay', AutoPay)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_UsedTime(self): # Integer
+		return self.get_query_params().get('UsedTime')
+
+	def set_UsedTime(self, UsedTime):  # Integer
+		self.add_query_param('UsedTime', UsedTime)
 	def get_AutoRenew(self): # String
 		return self.get_query_params().get('AutoRenew')
 
 	def set_AutoRenew(self, AutoRenew):  # String
 		self.add_query_param('AutoRenew', AutoRenew)
+	def get_PayType(self): # String
+		return self.get_query_params().get('PayType')
+
+	def set_PayType(self, PayType):  # String
+		self.add_query_param('PayType', PayType)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ResetAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/ResetAccountRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ResetAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestartDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RevokeOperatorPermissionRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,40 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class RestartDBInstanceRequest(RpcRequest):
+class RevokeOperatorPermissionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestartDBInstance','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RevokeOperatorPermission','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
-
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
@@ -57,7 +47,12 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_DBInstanceId(self): # String
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self, DBInstanceId):  # String
+		self.add_query_param('DBInstanceId', DBInstanceId)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestoreDdrTableRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RestoreTableRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,45 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class RestoreDdrTableRequest(RpcRequest):
+class RestoreTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestoreDdrTable','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestoreTable','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_SourceDBInstanceName(self): # String
-		return self.get_query_params().get('SourceDBInstanceName')
-
-	def set_SourceDBInstanceName(self, SourceDBInstanceName):  # String
-		self.add_query_param('SourceDBInstanceName', SourceDBInstanceName)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def get_InstantRecovery(self): # Boolean
+		return self.get_query_params().get('InstantRecovery')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def set_InstantRecovery(self, InstantRecovery):  # Boolean
+		self.add_query_param('InstantRecovery', InstantRecovery)
 	def get_TableMeta(self): # String
 		return self.get_query_params().get('TableMeta')
 
 	def set_TableMeta(self, TableMeta):  # String
 		self.add_query_param('TableMeta', TableMeta)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
@@ -72,22 +67,17 @@
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_BackupId(self): # String
 		return self.get_query_params().get('BackupId')
 
 	def set_BackupId(self, BackupId):  # String
 		self.add_query_param('BackupId', BackupId)
+	def get_OwnerAccount(self): # String
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_RestoreType(self): # String
-		return self.get_query_params().get('RestoreType')
-
-	def set_RestoreType(self, RestoreType):  # String
-		self.add_query_param('RestoreType', RestoreType)
-	def get_SourceRegion(self): # String
-		return self.get_query_params().get('SourceRegion')
-
-	def set_SourceRegion(self, SourceRegion):  # String
-		self.add_query_param('SourceRegion', SourceRegion)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RestoreTableRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceEngineVersionRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class RestoreTableRequest(RpcRequest):
+class UpgradeDBInstanceEngineVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RestoreTable','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBInstanceEngineVersion','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,44 +37,34 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_InstantRecovery(self): # Boolean
-		return self.get_query_params().get('InstantRecovery')
+	def get_EngineVersion(self): # String
+		return self.get_query_params().get('EngineVersion')
 
-	def set_InstantRecovery(self, InstantRecovery):  # Boolean
-		self.add_query_param('InstantRecovery', InstantRecovery)
-	def get_TableMeta(self): # String
-		return self.get_query_params().get('TableMeta')
+	def set_EngineVersion(self, EngineVersion):  # String
+		self.add_query_param('EngineVersion', EngineVersion)
+	def get_EffectiveTime(self): # String
+		return self.get_query_params().get('EffectiveTime')
 
-	def set_TableMeta(self, TableMeta):  # String
-		self.add_query_param('TableMeta', TableMeta)
+	def set_EffectiveTime(self, EffectiveTime):  # String
+		self.add_query_param('EffectiveTime', EffectiveTime)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_RestoreTime(self): # String
-		return self.get_query_params().get('RestoreTime')
-
-	def set_RestoreTime(self, RestoreTime):  # String
-		self.add_query_param('RestoreTime', RestoreTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_BackupId(self): # String
-		return self.get_query_params().get('BackupId')
-
-	def set_BackupId(self, BackupId):  # String
-		self.add_query_param('BackupId', BackupId)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RevokeAccountPrivilegeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/RevokeAccountPrivilegeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/RevokeOperatorPermissionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBProxyInstanceKernelVersionRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,43 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class RevokeOperatorPermissionRequest(RpcRequest):
+class UpgradeDBProxyInstanceKernelVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'RevokeOperatorPermission','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBProxyInstanceKernelVersion','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DBInstanceId(self): # String
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self, DBInstanceId):  # String
+		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_SwitchTime(self): # String
+		return self.get_query_params().get('SwitchTime')
+
+	def set_SwitchTime(self, SwitchTime):  # String
+		self.add_query_param('SwitchTime', SwitchTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_query_params().get('OwnerAccount')
+	def get_DBProxyEngineType(self): # String
+		return self.get_query_params().get('DBProxyEngineType')
 
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
+	def set_DBProxyEngineType(self, DBProxyEngineType):  # String
+		self.add_query_param('DBProxyEngineType', DBProxyEngineType)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
+	def get_UpgradeTime(self): # String
+		return self.get_query_params().get('UpgradeTime')
 
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
+	def set_UpgradeTime(self, UpgradeTime):  # String
+		self.add_query_param('UpgradeTime', UpgradeTime)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/StartDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/StartDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/StopDBInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/StopDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceHARequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceHARequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceNetTypeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/AllocateInstancePublicConnectionRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class SwitchDBInstanceNetTypeRequest(RpcRequest):
+class AllocateInstancePublicConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'SwitchDBInstanceNetType','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'AllocateInstancePublicConnection','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,19 +37,24 @@
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
 	def get_ConnectionStringPrefix(self): # String
 		return self.get_query_params().get('ConnectionStringPrefix')
 
 	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
 		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
+	def get_PGBouncerPort(self): # String
+		return self.get_query_params().get('PGBouncerPort')
 
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
+	def set_PGBouncerPort(self, PGBouncerPort):  # String
+		self.add_query_param('PGBouncerPort', PGBouncerPort)
+	def get_GeneralGroupName(self): # String
+		return self.get_query_params().get('GeneralGroupName')
+
+	def set_GeneralGroupName(self, GeneralGroupName):  # String
+		self.add_query_param('GeneralGroupName', GeneralGroupName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -62,17 +67,17 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_ConnectionStringType(self): # String
-		return self.get_query_params().get('ConnectionStringType')
+	def get_BabelfishPort(self): # String
+		return self.get_query_params().get('BabelfishPort')
 
-	def set_ConnectionStringType(self, ConnectionStringType):  # String
-		self.add_query_param('ConnectionStringType', ConnectionStringType)
+	def set_BabelfishPort(self, BabelfishPort):  # String
+		self.add_query_param('BabelfishPort', BabelfishPort)
 	def get_Port(self): # String
 		return self.get_query_params().get('Port')
 
 	def set_Port(self, Port):  # String
 		self.add_query_param('Port', Port)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchDBInstanceVpcRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchDBInstanceVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/SwitchGuardToMasterInstanceRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/SwitchGuardToMasterInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TagResourcesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TerminateMigrateTaskRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/TerminateMigrateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/TransformDBInstancePayTypeRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceKernelVersionRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,73 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class TransformDBInstancePayTypeRequest(RpcRequest):
+class UpgradeDBInstanceKernelVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'TransformDBInstancePayType','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBInstanceKernelVersion','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_BusinessInfo(self): # String
-		return self.get_query_params().get('BusinessInfo')
-
-	def set_BusinessInfo(self, BusinessInfo):  # String
-		self.add_query_param('BusinessInfo', BusinessInfo)
-	def get_Period(self): # String
-		return self.get_query_params().get('Period')
+	def get_SwitchTime(self): # String
+		return self.get_query_params().get('SwitchTime')
 
-	def set_Period(self, Period):  # String
-		self.add_query_param('Period', Period)
+	def set_SwitchTime(self, SwitchTime):  # String
+		self.add_query_param('SwitchTime', SwitchTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_UsedTime(self): # Integer
-		return self.get_query_params().get('UsedTime')
+	def get_TargetMinorVersion(self): # String
+		return self.get_query_params().get('TargetMinorVersion')
 
-	def set_UsedTime(self, UsedTime):  # Integer
-		self.add_query_param('UsedTime', UsedTime)
-	def get_AutoRenew(self): # String
-		return self.get_query_params().get('AutoRenew')
-
-	def set_AutoRenew(self, AutoRenew):  # String
-		self.add_query_param('AutoRenew', AutoRenew)
-	def get_PayType(self): # String
-		return self.get_query_params().get('PayType')
+	def set_TargetMinorVersion(self, TargetMinorVersion):  # String
+		self.add_query_param('TargetMinorVersion', TargetMinorVersion)
+	def get_UpgradeTime(self): # String
+		return self.get_query_params().get('UpgradeTime')
 
-	def set_PayType(self, PayType):  # String
-		self.add_query_param('PayType', PayType)
+	def set_UpgradeTime(self, UpgradeTime):  # String
+		self.add_query_param('UpgradeTime', UpgradeTime)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UnlockAccountRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UnlockAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UntagResourcesRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpdateUserBackupFileRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpdateUserBackupFileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceEngineVersionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionPrecheckRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,58 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class UpgradeDBInstanceEngineVersionRequest(RpcRequest):
+class UpgradeDBInstanceMajorVersionPrecheckRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBInstanceEngineVersion','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBInstanceMajorVersionPrecheck','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_EngineVersion(self): # String
-		return self.get_query_params().get('EngineVersion')
-
-	def set_EngineVersion(self, EngineVersion):  # String
-		self.add_query_param('EngineVersion', EngineVersion)
-	def get_EffectiveTime(self): # String
-		return self.get_query_params().get('EffectiveTime')
-
-	def set_EffectiveTime(self, EffectiveTime):  # String
-		self.add_query_param('EffectiveTime', EffectiveTime)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_ResourceOwnerAccount(self): # String
-		return self.get_query_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
-	def get_OwnerId(self): # Long
-		return self.get_query_params().get('OwnerId')
+	def get_TargetMajorVersion(self): # String
+		return self.get_query_params().get('TargetMajorVersion')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
+	def set_TargetMajorVersion(self, TargetMajorVersion):  # String
+		self.add_query_param('TargetMajorVersion', TargetMajorVersion)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceKernelVersionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/CreateDBNodesRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,53 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class UpgradeDBInstanceKernelVersionRequest(RpcRequest):
+class CreateDBNodesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBInstanceKernelVersion','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'CreateDBNodes','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
-
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_TargetMinorVersion(self): # String
-		return self.get_query_params().get('TargetMinorVersion')
-
-	def set_TargetMinorVersion(self, TargetMinorVersion):  # String
-		self.add_query_param('TargetMinorVersion', TargetMinorVersion)
-	def get_UpgradeTime(self): # String
-		return self.get_query_params().get('UpgradeTime')
+	def get_DBNode(self): # String
+		return self.get_query_params().get('DBNode')
 
-	def set_UpgradeTime(self, UpgradeTime):  # String
-		self.add_query_param('UpgradeTime', UpgradeTime)
+	def set_DBNode(self, DBNode):  # String
+		self.add_query_param('DBNode', DBNode)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/UpgradeDBInstanceMajorVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-rds-2.7.8/aliyunsdkrds/request/v20140815/UpgradeDBProxyInstanceKernelVersionRequest.py` & `aliyun-python-sdk-rds-2.7.9/aliyunsdkrds/request/v20140815/ModifyDBInstanceConnectionStringRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,53 +16,73 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkrds.endpoint import endpoint_data
 
-class UpgradeDBProxyInstanceKernelVersionRequest(RpcRequest):
+class ModifyDBInstanceConnectionStringRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'UpgradeDBProxyInstanceKernelVersion','rds')
+		RpcRequest.__init__(self, 'Rds', '2014-08-15', 'ModifyDBInstanceConnectionString','rds')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ConnectionStringPrefix(self): # String
+		return self.get_query_params().get('ConnectionStringPrefix')
+
+	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
+		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
+	def get_PGBouncerPort(self): # String
+		return self.get_query_params().get('PGBouncerPort')
+
+	def set_PGBouncerPort(self, PGBouncerPort):  # String
+		self.add_query_param('PGBouncerPort', PGBouncerPort)
+	def get_GeneralGroupName(self): # String
+		return self.get_query_params().get('GeneralGroupName')
+
+	def set_GeneralGroupName(self, GeneralGroupName):  # String
+		self.add_query_param('GeneralGroupName', GeneralGroupName)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
-
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_DBProxyEngineType(self): # String
-		return self.get_query_params().get('DBProxyEngineType')
+	def get_OwnerAccount(self): # String
+		return self.get_query_params().get('OwnerAccount')
 
-	def set_DBProxyEngineType(self, DBProxyEngineType):  # String
-		self.add_query_param('DBProxyEngineType', DBProxyEngineType)
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_UpgradeTime(self): # String
-		return self.get_query_params().get('UpgradeTime')
+	def get_BabelfishPort(self): # String
+		return self.get_query_params().get('BabelfishPort')
+
+	def set_BabelfishPort(self, BabelfishPort):  # String
+		self.add_query_param('BabelfishPort', BabelfishPort)
+	def get_CurrentConnectionString(self): # String
+		return self.get_query_params().get('CurrentConnectionString')
+
+	def set_CurrentConnectionString(self, CurrentConnectionString):  # String
+		self.add_query_param('CurrentConnectionString', CurrentConnectionString)
+	def get_Port(self): # String
+		return self.get_query_params().get('Port')
 
-	def set_UpgradeTime(self, UpgradeTime):  # String
-		self.add_query_param('UpgradeTime', UpgradeTime)
+	def set_Port(self, Port):  # String
+		self.add_query_param('Port', Port)
```

### Comparing `aliyun-python-sdk-rds-2.7.8/setup.py` & `aliyun-python-sdk-rds-2.7.9/setup.py`

 * *Files identical despite different names*

