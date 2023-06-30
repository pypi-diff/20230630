# Comparing `tmp/aliyun-python-sdk-vpc-3.0.8.tar.gz` & `tmp/aliyun-python-sdk-vpc-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-vpc-3.0.8.tar", last modified: Wed Nov 27 07:24:09 2019, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-vpc-3.0.9.tar", last modified: Fri Feb 28 09:02:14 2020, max compression
```

## Comparing `aliyun-python-sdk-vpc-3.0.8.tar` & `aliyun-python-sdk-vpc-3.0.9.tar`

### file list

```diff
@@ -1,241 +1,246 @@
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/MANIFEST.in
--rw-rw-r--   0 admin     (1140) admin     (1140)     2452 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/setup.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1537 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       59 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/setup.cfg
--rw-rw-r--   0 admin     (1140) admin     (1140)      527 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/README.rst
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/
--rw-rw-r--   0 admin     (1140) admin     (1140)       30 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/requires.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)     1537 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       13 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)        1 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)    14912 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/SOURCES.txt
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/
--rw-rw-r--   0 admin     (1140) admin     (1140)     2679 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipMonitorDataRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2361 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpGroupRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3179 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCommonBandwidthPackagesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3261 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateFlowLogRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4635 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3855 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2193 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteNetworkAclRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3687 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2591 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2057 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ConnectRouterInterfaceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2535 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2369 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorAclListRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2639 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociatePhysicalConnectionFromVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3203 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionSetupOrderRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2903 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSnatEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2557 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddIPv6TranslatorAclListEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     5352 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipAddressesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3465 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSslVpnServerRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2537 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpNetworkRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2401 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3207 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnRouteEntryWeightRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3913 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeFlowLogsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3265 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2447 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TerminatePhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2917 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3007 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnSslServerLogsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2561 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySslVpnClientCertRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2831 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TagResourcesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3911 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeGlobalAccelerationInstancesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2477 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6InternetBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2417 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouterInterfaceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2059 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ActivateRouterInterfaceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2551 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnPbrRouteEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2353 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2525 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateNetworkAclRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2423 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CopyNetworkAclEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3069 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIpv6EgressOnlyRuleRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2391 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionLOARequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4069 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3637 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackagePayTypeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2243 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ConvertBandwidthPackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2675 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNatGatewaySpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2766 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveBandwidthPackageIpsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2531 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNatGatewayAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3225 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNetworkAclsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2707 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySnatEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3755 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2217 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNetworkAclAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2509 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddGlobalAccelerationInstanceIpRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2175 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ActiveFlowLogRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2539 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6AddressAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2985 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AllocateIpv6InternetBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2401 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteCommonBandwidthPackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2593 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/MoveResourceGroupRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2545 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnRouteEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2423 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelCommonBandwidthPackageIpBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3307 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateForwardEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2715 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBgpPeerRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4073 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6AddressesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2421 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageSpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3431 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSnatTableEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2357 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorAclListRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2673 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddBgpNetworkRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3283 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6EgressOnlyRulesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3029 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2561 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceSpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3189 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVSwitchRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2671 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2537 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSslVpnClientCertRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2747 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4105 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2365 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2557 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteExpressConnectRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2529 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeletionProtectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2587 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNetworkAclAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2739 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVSwitchAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2389 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBandwidthPackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2513 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVRoutersRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2589 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageIpBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4308 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ApplyPhysicalConnectionLOARequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2515 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveGlobalAccelerationInstanceIpRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2411 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteForwardEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3520 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpcsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2009 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeZonesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3297 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBgpGroupRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2181 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelExpressCloudConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2959 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2447 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveCommonBandwidthPackageIpRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     5825 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouterInterfaceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2337 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteHaVipRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2899 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBgpPeerAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2433 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageSpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2717 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CompletePhysicalConnectionLOARequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2479 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpcAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2787 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIpv6GatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2441 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6EgressOnlyRuleRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2741 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2669 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateNetworkAclRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2669 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyHaVipAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2193 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2143 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpcRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3391 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnPbrRouteEntryWeightRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2987 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateGlobalAccelerationInstanceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2769 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBandwidthPackagesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3477 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySslVpnServerRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2347 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVSwitchAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2377 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2549 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateRouteTableRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     5092 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateNatGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2821 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6InternetBandwidthRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2353 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpPeerRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2411 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeServerRelatedGlobalAccelerationInstancesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2441 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddCommonBandwidthPackageIpRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2847 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpGroupsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2175 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteFlowLogRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2179 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeactiveFlowLogRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3861 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteEntryListRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2063 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeactivateRouterInterfaceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2501 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceSpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2823 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewaysRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2709 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnGatewayAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3947 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AllocateEipAddressRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2515 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateHaVipRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3175 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionOccupancyOrderRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2355 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RecoverVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2239 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DownloadVpnConnectionConfigRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2829 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateHaVipRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2409 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3023 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnGatewaysRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3557 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociatePhysicalConnectionToVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2915 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateEipAddressRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2697 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyEipAddressAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2553 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateRouteTableRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2709 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouteTableRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2035 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouterInterfaceAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2683 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateCustomerGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2661 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2765 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeGrantRulesToCenRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2369 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSnatEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2817 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeHaVipsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2549 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVRouterAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2393 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSslVpnServerRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2421 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeHighDefinitionMonitorLogAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2661 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateHaVipRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3527 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateCommonBandwidthPackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2441 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/EnablePhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3005 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ListTagResourcesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2425 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSslVpnClientCertRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2897 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouterInterfacesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2539 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveIPv6TranslatorAclListEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2441 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelPhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3043 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/PublishVpnRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2873 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnServersRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2341 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteNatGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3853 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeForwardTableEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3784 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteTableListRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2327 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteGlobalAccelerationInstanceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3891 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnConnectionAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2359 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TerminateVirtualBorderRouterRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3213 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnPbrRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2227 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2175 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVSwitchRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2935 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2749 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCustomerGatewayAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2661 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3327 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBgpGroupAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2831 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpcAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2579 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2417 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteCustomerGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2441 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeletePhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2577 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewaysRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2563 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclListEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3305 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouteTableAttributesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2387 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRegionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2513 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpNetworksRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2657 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2579 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddBandwidthPackageIpsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4075 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2201 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ReleaseEipAddressRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2181 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteExpressCloudConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2867 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/GrantInstanceToCenRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3509 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBandwidthPackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2345 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DisableVpcClassicLinkRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3999 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4052 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVSwitchesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2529 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewaySpecRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3569 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteTablesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3101 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeAccessPointsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2851 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeExpressCloudConnectionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3871 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateExpressCloudConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3563 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnPbrRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3503 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyForwardEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3274 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2229 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewayAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2521 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2243 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2199 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouteTableRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3549 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpcRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3931 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyPhysicalConnectionAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2705 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnTagResourcesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2665 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateNetworkAclRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2699 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNewProjectEipMonitorDataRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4301 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2199 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipGatewayInfoRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     5989 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UpdateNetworkAclEntriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3097 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateGlobalAccelerationInstanceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2251 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4007 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2521 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateGlobalAccelerationInstanceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3113 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateEipAddressRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2549 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyFlowLogAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3379 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnRouteEntryRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2207 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6GatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3527 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNatGatewaysRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2873 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RevokeInstanceFromCenRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3011 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpPeersRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2203 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnGatewayRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4485 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVirtualBorderRouterAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2513 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3291 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2539 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewayAttributeRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2343 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/EnableVpcClassicLinkRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)       21 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     3114 2019-11-27 07:24:09.000000 aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/endpoint.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/
+-rw-rw-r--   0 admin      (531) admin      (531)       59 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/setup.cfg
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/
+-rw-rw-r--   0 admin      (531) admin      (531)       21 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3114 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/endpoint.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/__init__.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/
+-rw-rw-r--   0 admin      (531) admin      (531)     2661 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2479 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpcAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2057 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ConnectRouterInterfaceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2389 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBandwidthPackageRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2591 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2035 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouterInterfaceAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2203 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2699 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNewProjectEipMonitorDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2927 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2529 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeletionProtectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2873 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnServersRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2217 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNetworkAclAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2557 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddIPv6TranslatorAclListEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2739 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVSwitchAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3097 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateGlobalAccelerationInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2675 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNatGatewaySpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2433 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageSpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3755 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3107 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateEipSegmentAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2209 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRegionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2059 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ActivateRouterInterfaceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2391 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateVpcCidrBlockRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3681 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyForwardEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4635 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2715 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBgpPeerRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2561 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceSpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4105 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3569 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteTablesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4007 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2769 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBandwidthPackagesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4301 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2679 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipMonitorDataRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2199 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2867 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/GrantInstanceToCenRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3043 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/PublishVpnRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2547 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSnatEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2671 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2705 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnTagResourcesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3175 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionOccupancyOrderRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3203 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionSetupOrderRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3687 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3391 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnPbrRouteEntryWeightRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2669 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyHaVipAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2787 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIpv6GatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2587 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNetworkAclAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2829 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateHaVipRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2251 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3189 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVSwitchRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2579 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3853 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeForwardTableEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3023 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnGatewaysRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2355 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RecoverVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3917 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifySslVpnServerRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2549 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyFlowLogAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2243 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2347 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVSwitchAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2447 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TerminatePhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4485 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVirtualBorderRouterAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2171 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeAccessPointsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2669 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateNetworkAclRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2369 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorAclListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2899 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBgpPeerAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2551 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnPbrRouteEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2683 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateCustomerGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2589 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteForwardEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2709 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3213 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnPbrRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     5092 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateNatGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2529 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewaySpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3225 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNetworkAclsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3431 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSnatTableEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2885 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifySnatEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2589 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddCommonBandwidthPackageIpRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3011 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpPeersRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2341 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteNatGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2421 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeHighDefinitionMonitorLogAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4073 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6AddressesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3265 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3379 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2525 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateNetworkAclRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2327 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteGlobalAccelerationInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2657 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2515 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateHaVipRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2513 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVRoutersRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3911 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeGlobalAccelerationInstancesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2239 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DownloadVpnConnectionConfigRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2935 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2441 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelPhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2563 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclListEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2531 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNatGatewayAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3509 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBandwidthPackageRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3261 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateFlowLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3207 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnRouteEntryWeightRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2515 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveGlobalAccelerationInstanceIpRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2417 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouterInterfaceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2423 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ReleaseEipSegmentAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2545 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnRouteEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2749 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCustomerGatewayAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3291 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3905 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSslVpnServerRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2539 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6AddressAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3283 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6EgressOnlyRulesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2229 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewayAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2387 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateVpcCidrBlockRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3005 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ListTagResourcesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2959 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     5825 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouterInterfaceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3527 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateCommonBandwidthPackageRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2243 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ConvertBandwidthPackageRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3485 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateForwardEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3913 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeFlowLogsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2401 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2717 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CompletePhysicalConnectionLOARequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3791 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2393 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSslVpnServerRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2521 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     5989 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UpdateNetworkAclEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2423 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelCommonBandwidthPackageIpBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2709 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnGatewayAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3855 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2175 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ActiveFlowLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2539 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewayAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2175 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteFlowLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2421 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageSpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2661 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2409 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3557 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociatePhysicalConnectionToVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4069 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2873 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RevokeInstanceFromCenRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2361 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2831 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpcAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2357 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorAclListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2743 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipSegmentRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3274 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2337 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteHaVipRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2143 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpcRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2365 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2207 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6GatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2661 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateHaVipRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2343 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/EnableVpcClassicLinkRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3637 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackagePayTypeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2063 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeactivateRouterInterfaceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3227 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnSslServerLogsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3871 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateExpressCloudConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2823 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewaysRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2447 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveCommonBandwidthPackageIpRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3327 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBgpGroupAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3683 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVSwitchesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2345 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DisableVpcClassicLinkRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2391 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionLOARequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2639 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociatePhysicalConnectionFromVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2199 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipGatewayInfoRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2561 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifySslVpnClientCertRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2593 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/MoveResourceGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3563 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnPbrRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2851 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeExpressCloudConnectionsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2353 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2537 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSslVpnClientCertRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2539 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveIPv6TranslatorAclListEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3029 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2831 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TagResourcesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2359 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TerminateVirtualBorderRouterRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2521 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateGlobalAccelerationInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3179 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCommonBandwidthPackagesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2227 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3549 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpcRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2513 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpNetworksRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2181 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelExpressCloudConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2193 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteNetworkAclRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2509 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddGlobalAccelerationInstanceIpRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3861 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteEntryListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2417 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteCustomerGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3891 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnConnectionAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3151 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpcsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2009 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeZonesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2766 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveBandwidthPackageIpsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2553 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2741 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2441 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeletePhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2987 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateGlobalAccelerationInstanceRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3069 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIpv6EgressOnlyRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2673 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddBgpNetworkRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2353 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpPeerRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2665 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateNetworkAclRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2535 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3931 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyPhysicalConnectionAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3291 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateEipAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2193 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouteEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2179 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeactiveFlowLogRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2985 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateIpv6InternetBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3947 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateEipAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2181 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteExpressCloudConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2175 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVSwitchRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3081 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSnatEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2557 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteExpressConnectRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2747 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2917 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2411 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeServerRelatedGlobalAccelerationInstancesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2501 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceSpecRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2441 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/EnablePhysicalConnectionRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2577 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewaysRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2377 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnGatewayRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4075 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorEntryRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3093 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateEipAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     4308 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ApplyPhysicalConnectionLOARequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2821 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6InternetBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2423 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CopyNetworkAclEntriesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2897 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouterInterfacesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3415 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteTableListRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3297 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBgpGroupRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2549 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateRouteTableRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2425 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSslVpnClientCertRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2697 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyEipAddressAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2537 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpNetworkRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     5197 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipAddressesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2477 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6InternetBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3527 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNatGatewaysRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2847 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpGroupsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2765 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeGrantRulesToCenRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2593 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouteTableAttributesRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2589 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageIpBandwidthRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2201 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ReleaseEipAddressRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2441 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6EgressOnlyRuleRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2401 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteCommonBandwidthPackageRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2549 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVRouterAttributeRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2579 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddBandwidthPackageIpsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2817 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeHaVipsRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2452 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/setup.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/
+-rw-rw-r--   0 admin      (531) admin      (531)        1 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       30 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/requires.txt
+-rw-rw-r--   0 admin      (531) admin      (531)    15233 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       13 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     1537 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/PKG-INFO
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/MANIFEST.in
+-rw-rw-r--   0 admin      (531) admin      (531)      527 2020-02-28 09:02:13.000000 aliyun-python-sdk-vpc-3.0.9/README.rst
+-rw-rw-r--   0 admin      (531) admin      (531)     1537 2020-02-28 09:02:14.000000 aliyun-python-sdk-vpc-3.0.9/PKG-INFO
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/setup.py` & `aliyun-python-sdk-vpc-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpc-3.0.8/PKG-INFO` & `aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpc
-Version: 3.0.8
+Version: 3.0.9
 Summary: The vpc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpc
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/README.rst` & `aliyun-python-sdk-vpc-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/PKG-INFO` & `aliyun-python-sdk-vpc-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpc
-Version: 3.0.8
+Version: 3.0.9
 Summary: The vpc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpc
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyun_python_sdk_vpc.egg-info/SOURCES.txt` & `aliyun-python-sdk-vpc-3.0.9/aliyun_python_sdk_vpc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 aliyunsdkvpc/request/v20160428/ActiveFlowLogRequest.py
 aliyunsdkvpc/request/v20160428/AddBandwidthPackageIpsRequest.py
 aliyunsdkvpc/request/v20160428/AddBgpNetworkRequest.py
 aliyunsdkvpc/request/v20160428/AddCommonBandwidthPackageIpRequest.py
 aliyunsdkvpc/request/v20160428/AddGlobalAccelerationInstanceIpRequest.py
 aliyunsdkvpc/request/v20160428/AddIPv6TranslatorAclListEntryRequest.py
 aliyunsdkvpc/request/v20160428/AllocateEipAddressRequest.py
+aliyunsdkvpc/request/v20160428/AllocateEipSegmentAddressRequest.py
 aliyunsdkvpc/request/v20160428/AllocateIpv6InternetBandwidthRequest.py
 aliyunsdkvpc/request/v20160428/ApplyPhysicalConnectionLOARequest.py
 aliyunsdkvpc/request/v20160428/AssociateEipAddressRequest.py
 aliyunsdkvpc/request/v20160428/AssociateGlobalAccelerationInstanceRequest.py
 aliyunsdkvpc/request/v20160428/AssociateHaVipRequest.py
 aliyunsdkvpc/request/v20160428/AssociateNetworkAclRequest.py
 aliyunsdkvpc/request/v20160428/AssociatePhysicalConnectionToVirtualBorderRouterRequest.py
 aliyunsdkvpc/request/v20160428/AssociateRouteTableRequest.py
+aliyunsdkvpc/request/v20160428/AssociateVpcCidrBlockRequest.py
 aliyunsdkvpc/request/v20160428/CancelCommonBandwidthPackageIpBandwidthRequest.py
 aliyunsdkvpc/request/v20160428/CancelExpressCloudConnectionRequest.py
 aliyunsdkvpc/request/v20160428/CancelPhysicalConnectionRequest.py
 aliyunsdkvpc/request/v20160428/CompletePhysicalConnectionLOARequest.py
 aliyunsdkvpc/request/v20160428/ConnectRouterInterfaceRequest.py
 aliyunsdkvpc/request/v20160428/ConvertBandwidthPackageRequest.py
 aliyunsdkvpc/request/v20160428/CopyNetworkAclEntriesRequest.py
@@ -109,14 +111,15 @@
 aliyunsdkvpc/request/v20160428/DescribeBgpPeersRequest.py
 aliyunsdkvpc/request/v20160428/DescribeCommonBandwidthPackagesRequest.py
 aliyunsdkvpc/request/v20160428/DescribeCustomerGatewayRequest.py
 aliyunsdkvpc/request/v20160428/DescribeCustomerGatewaysRequest.py
 aliyunsdkvpc/request/v20160428/DescribeEipAddressesRequest.py
 aliyunsdkvpc/request/v20160428/DescribeEipGatewayInfoRequest.py
 aliyunsdkvpc/request/v20160428/DescribeEipMonitorDataRequest.py
+aliyunsdkvpc/request/v20160428/DescribeEipSegmentRequest.py
 aliyunsdkvpc/request/v20160428/DescribeExpressCloudConnectionsRequest.py
 aliyunsdkvpc/request/v20160428/DescribeFlowLogsRequest.py
 aliyunsdkvpc/request/v20160428/DescribeForwardTableEntriesRequest.py
 aliyunsdkvpc/request/v20160428/DescribeGlobalAccelerationInstancesRequest.py
 aliyunsdkvpc/request/v20160428/DescribeGrantRulesToCenRequest.py
 aliyunsdkvpc/request/v20160428/DescribeHaVipsRequest.py
 aliyunsdkvpc/request/v20160428/DescribeHighDefinitionMonitorLogAttributeRequest.py
@@ -211,14 +214,15 @@
 aliyunsdkvpc/request/v20160428/ModifyVpnGatewayAttributeRequest.py
 aliyunsdkvpc/request/v20160428/ModifyVpnPbrRouteEntryWeightRequest.py
 aliyunsdkvpc/request/v20160428/ModifyVpnRouteEntryWeightRequest.py
 aliyunsdkvpc/request/v20160428/MoveResourceGroupRequest.py
 aliyunsdkvpc/request/v20160428/PublishVpnRouteEntryRequest.py
 aliyunsdkvpc/request/v20160428/RecoverVirtualBorderRouterRequest.py
 aliyunsdkvpc/request/v20160428/ReleaseEipAddressRequest.py
+aliyunsdkvpc/request/v20160428/ReleaseEipSegmentAddressRequest.py
 aliyunsdkvpc/request/v20160428/RemoveBandwidthPackageIpsRequest.py
 aliyunsdkvpc/request/v20160428/RemoveCommonBandwidthPackageIpRequest.py
 aliyunsdkvpc/request/v20160428/RemoveGlobalAccelerationInstanceIpRequest.py
 aliyunsdkvpc/request/v20160428/RemoveIPv6TranslatorAclListEntryRequest.py
 aliyunsdkvpc/request/v20160428/RevokeInstanceFromCenRequest.py
 aliyunsdkvpc/request/v20160428/TagResourcesRequest.py
 aliyunsdkvpc/request/v20160428/TerminatePhysicalConnectionRequest.py
@@ -226,9 +230,10 @@
 aliyunsdkvpc/request/v20160428/UnTagResourcesRequest.py
 aliyunsdkvpc/request/v20160428/UnassociateEipAddressRequest.py
 aliyunsdkvpc/request/v20160428/UnassociateGlobalAccelerationInstanceRequest.py
 aliyunsdkvpc/request/v20160428/UnassociateHaVipRequest.py
 aliyunsdkvpc/request/v20160428/UnassociateNetworkAclRequest.py
 aliyunsdkvpc/request/v20160428/UnassociatePhysicalConnectionFromVirtualBorderRouterRequest.py
 aliyunsdkvpc/request/v20160428/UnassociateRouteTableRequest.py
+aliyunsdkvpc/request/v20160428/UnassociateVpcCidrBlockRequest.py
 aliyunsdkvpc/request/v20160428/UpdateNetworkAclEntriesRequest.py
 aliyunsdkvpc/request/v20160428/__init__.py
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipMonitorDataRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipMonitorDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeEipMonitorDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipMonitorData','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipMonitorData','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpGroupRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteHaVipRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DeleteBgpGroupRequest(RpcRequest):
+class DeleteHaVipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpGroup','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteHaVip','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -38,19 +38,19 @@
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_BgpGroupId(self):
-		return self.get_query_params().get('BgpGroupId')
+	def get_HaVipId(self):
+		return self.get_query_params().get('HaVipId')
 
-	def set_BgpGroupId(self,BgpGroupId):
-		self.add_query_param('BgpGroupId',BgpGroupId)
+	def set_HaVipId(self,HaVipId):
+		self.add_query_param('HaVipId',HaVipId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCommonBandwidthPackagesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCommonBandwidthPackagesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeCommonBandwidthPackagesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCommonBandwidthPackages','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCommonBandwidthPackages','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateFlowLogRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateFlowLogRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateFlowLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateFlowLog','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateFlowLog','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorEntriesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIPv6TranslatorEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_BackendIpv4Port(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVirtualBorderRouterRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteNetworkAclRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteNetworkAclRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteNetworkAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteNetworkAcl','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteNetworkAcl','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnGatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVpnGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyCommonBandwidthPackageAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ConnectRouterInterfaceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ConnectRouterInterfaceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ConnectRouterInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ConnectRouterInterface','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ConnectRouterInterface','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListAttributesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIPv6TranslatorAclListAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorAclListAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorAclListAttributes','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorAclListRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorAclListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateIPv6TranslatorAclListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6TranslatorAclList','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6TranslatorAclList','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociatePhysicalConnectionFromVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociatePhysicalConnectionFromVirtualBorderRouterRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociatePhysicalConnectionFromVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociatePhysicalConnectionFromVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociatePhysicalConnectionFromVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionSetupOrderRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionSetupOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreatePhysicalConnectionSetupOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnectionSetupOrder','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnectionSetupOrder','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AccessPointId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSnatEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSnatEntryRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateSnatEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSnatEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSnatEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_SourceCIDR(self):
 		return self.get_query_params().get('SourceCIDR')
 
 	def set_SourceCIDR(self,SourceCIDR):
 		self.add_query_param('SourceCIDR',SourceCIDR)
 
 	def get_SnatIp(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddIPv6TranslatorAclListEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddIPv6TranslatorAclListEntryRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AddIPv6TranslatorAclListEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddIPv6TranslatorAclListEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddIPv6TranslatorAclListEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipAddressesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipAddressesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeEipAddressesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipAddresses','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipAddresses','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -98,24 +98,19 @@
 
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		for i in range(len(Tags)):	
-			if Tags[i].get('Value') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Value' , Tags[i].get('Value'))
-			if Tags[i].get('Key') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Key' , Tags[i].get('Key'))
+	def get_SegmentInstanceId(self):
+		return self.get_query_params().get('SegmentInstanceId')
 
+	def set_SegmentInstanceId(self,SegmentInstanceId):
+		self.add_query_param('SegmentInstanceId',SegmentInstanceId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSslVpnServerRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBgpGroupAttributeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,94 +16,88 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class CreateSslVpnServerRequest(RpcRequest):
+class ModifyBgpGroupAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSslVpnServer','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBgpGroupAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
+	def get_AuthKey(self):
+		return self.get_query_params().get('AuthKey')
+
+	def set_AuthKey(self,AuthKey):
+		self.add_query_param('AuthKey',AuthKey)
+
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_LocalSubnet(self):
-		return self.get_query_params().get('LocalSubnet')
+	def get_BgpGroupId(self):
+		return self.get_query_params().get('BgpGroupId')
+
+	def set_BgpGroupId(self,BgpGroupId):
+		self.add_query_param('BgpGroupId',BgpGroupId)
+
+	def get_Description(self):
+		return self.get_query_params().get('Description')
 
-	def set_LocalSubnet(self,LocalSubnet):
-		self.add_query_param('LocalSubnet',LocalSubnet)
+	def set_Description(self,Description):
+		self.add_query_param('Description',Description)
 
-	def get_Cipher(self):
-		return self.get_query_params().get('Cipher')
+	def get_PeerAsn(self):
+		return self.get_query_params().get('PeerAsn')
 
-	def set_Cipher(self,Cipher):
-		self.add_query_param('Cipher',Cipher)
+	def set_PeerAsn(self,PeerAsn):
+		self.add_query_param('PeerAsn',PeerAsn)
 
-	def get_ClientIpPool(self):
-		return self.get_query_params().get('ClientIpPool')
+	def get_IsFakeAsn(self):
+		return self.get_query_params().get('IsFakeAsn')
 
-	def set_ClientIpPool(self,ClientIpPool):
-		self.add_query_param('ClientIpPool',ClientIpPool)
+	def set_IsFakeAsn(self,IsFakeAsn):
+		self.add_query_param('IsFakeAsn',IsFakeAsn)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_Compress(self):
-		return self.get_query_params().get('Compress')
-
-	def set_Compress(self,Compress):
-		self.add_query_param('Compress',Compress)
-
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
-	def get_VpnGatewayId(self):
-		return self.get_query_params().get('VpnGatewayId')
-
-	def set_VpnGatewayId(self,VpnGatewayId):
-		self.add_query_param('VpnGatewayId',VpnGatewayId)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_Port(self):
-		return self.get_query_params().get('Port')
-
-	def set_Port(self,Port):
-		self.add_query_param('Port',Port)
-
-	def get_Proto(self):
-		return self.get_query_params().get('Proto')
-
-	def set_Proto(self,Proto):
-		self.add_query_param('Proto',Proto)
-
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+		self.add_query_param('Name',Name)
+
+	def get_LocalAsn(self):
+		return self.get_query_params().get('LocalAsn')
+
+	def set_LocalAsn(self,LocalAsn):
+		self.add_query_param('LocalAsn',LocalAsn)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpNetworkRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpNetworkRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteBgpNetworkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpNetwork','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpNetwork','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnConnectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVpnConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnRouteEntryWeightRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnRouteEntryWeightRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVpnRouteEntryWeightRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnRouteEntryWeight','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnRouteEntryWeight','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeFlowLogsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeFlowLogsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeFlowLogsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeFlowLogs','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeFlowLogs','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribePhysicalConnectionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribePhysicalConnections','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribePhysicalConnections','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TerminatePhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TerminatePhysicalConnectionRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class TerminatePhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TerminatePhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TerminatePhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeSslVpnClientCertsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnClientCerts','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnClientCerts','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnSslServerLogsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnSslServerLogsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnSslServerLogsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnSslServerLogs','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnSslServerLogs','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -62,14 +62,20 @@
 
 	def get__From(self):
 		return self.get_query_params().get('From')
 
 	def set__From(self,_From):
 		self.add_query_param('From',_From)
 
+	def get_SslVpnClientCertId(self):
+		return self.get_query_params().get('SslVpnClientCertId')
+
+	def set_SslVpnClientCertId(self,SslVpnClientCertId):
+		self.add_query_param('SslVpnClientCertId',SslVpnClientCertId)
+
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySslVpnClientCertRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifySslVpnClientCertRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifySslVpnClientCertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifySslVpnClientCert','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifySslVpnClientCert','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TagResourcesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TagResourcesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TagResources','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TagResources','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeGlobalAccelerationInstancesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeGlobalAccelerationInstancesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeGlobalAccelerationInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeGlobalAccelerationInstances','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeGlobalAccelerationInstances','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IpAddress(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6InternetBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6InternetBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIpv6InternetBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6InternetBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6InternetBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouterInterfaceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouterInterfaceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteRouterInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouterInterface','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouterInterface','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ActivateRouterInterfaceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ActivateRouterInterfaceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ActivateRouterInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ActivateRouterInterface','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ActivateRouterInterface','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnPbrRouteEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnPbrRouteEntriesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnPbrRouteEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnPbrRouteEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnPbrRouteEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVirtualBorderRouterRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateNetworkAclRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateNetworkAclRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateNetworkAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateNetworkAcl','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateNetworkAcl','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CopyNetworkAclEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CopyNetworkAclEntriesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CopyNetworkAclEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CopyNetworkAclEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CopyNetworkAclEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIpv6EgressOnlyRuleRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIpv6EgressOnlyRuleRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateIpv6EgressOnlyRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIpv6EgressOnlyRule','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIpv6EgressOnlyRule','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionLOARequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribePhysicalConnectionLOARequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribePhysicalConnectionLOARequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribePhysicalConnectionLOA','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribePhysicalConnectionLOA','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnConnectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVpnConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IkeConfig(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackagePayTypeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackagePayTypeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyCommonBandwidthPackagePayTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackagePayType','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackagePayType','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ConvertBandwidthPackageRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ConvertBandwidthPackageRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ConvertBandwidthPackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ConvertBandwidthPackage','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ConvertBandwidthPackage','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNatGatewaySpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNatGatewaySpecRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyNatGatewaySpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNatGatewaySpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNatGatewaySpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveBandwidthPackageIpsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveBandwidthPackageIpsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RemoveBandwidthPackageIpsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveBandwidthPackageIps','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveBandwidthPackageIps','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNatGatewayAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNatGatewayAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyNatGatewayAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNatGatewayAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNatGatewayAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNetworkAclsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNetworkAclsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeNetworkAclsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNetworkAcls','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNetworkAcls','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySnatEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifySnatEntryRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifySnatEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifySnatEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifySnatEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_SnatIp(self):
 		return self.get_query_params().get('SnatIp')
 
 	def set_SnatIp(self,SnatIp):
 		self.add_query_param('SnatIp',SnatIp)
 
 	def get_SnatEntryId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIPv6TranslatorsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6Translators','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6Translators','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNetworkAclAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNetworkAclAttributesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeNetworkAclAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNetworkAclAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNetworkAclAttributes','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddGlobalAccelerationInstanceIpRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddGlobalAccelerationInstanceIpRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AddGlobalAccelerationInstanceIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddGlobalAccelerationInstanceIp','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddGlobalAccelerationInstanceIp','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ActiveFlowLogRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ActiveFlowLogRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ActiveFlowLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ActiveFlowLog','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ActiveFlowLog','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6AddressAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6AddressAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIpv6AddressAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6AddressAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6AddressAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AllocateIpv6InternetBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateIpv6InternetBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AllocateIpv6InternetBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AllocateIpv6InternetBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AllocateIpv6InternetBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteCommonBandwidthPackageRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBandwidthPackageRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DeleteCommonBandwidthPackageRequest(RpcRequest):
+class DeleteBandwidthPackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteCommonBandwidthPackage','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBandwidthPackage','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/MoveResourceGroupRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/MoveResourceGroupRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class MoveResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'MoveResourceGroup','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'MoveResourceGroup','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnRouteEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnRouteEntriesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnRouteEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnRouteEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnRouteEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelCommonBandwidthPackageIpBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelCommonBandwidthPackageIpBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CancelCommonBandwidthPackageIpBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelCommonBandwidthPackageIpBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelCommonBandwidthPackageIpBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateForwardEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateForwardEntryRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateForwardEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateForwardEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateForwardEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_ForwardTableId(self):
 		return self.get_query_params().get('ForwardTableId')
 
 	def set_ForwardTableId(self,ForwardTableId):
 		self.add_query_param('ForwardTableId',ForwardTableId)
 
 	def get_InternalIp(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBgpPeerRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBgpPeerRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateBgpPeerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBgpPeer','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBgpPeer','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6AddressesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6AddressesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIpv6AddressesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6Addresses','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6Addresses','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageSpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageSpecRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyBandwidthPackageSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBandwidthPackageSpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBandwidthPackageSpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSnatTableEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSnatTableEntriesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeSnatTableEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSnatTableEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSnatTableEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorAclListRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorAclListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIPv6TranslatorAclListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6TranslatorAclList','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6TranslatorAclList','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddBgpNetworkRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddBgpNetworkRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AddBgpNetworkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddBgpNetwork','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddBgpNetwork','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6EgressOnlyRulesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6EgressOnlyRulesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIpv6EgressOnlyRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6EgressOnlyRules','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6EgressOnlyRules','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnRouteEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVpnRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceSpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceSpecRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyRouterInterfaceSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouterInterfaceSpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouterInterfaceSpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVSwitchRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVSwitchRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVSwitch','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVSwitch','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIPv6TranslatorAclListsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIPv6TranslatorAclListsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorAclLists','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIPv6TranslatorAclLists','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateSslVpnClientCertRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSslVpnClientCertRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateSslVpnClientCertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSslVpnClientCert','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSslVpnClientCert','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIPv6TranslatorBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIPv6TranslatorEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_BackendIpv4Port(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionBandwidthRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyExpressCloudConnectionBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyExpressCloudConnectionBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyExpressCloudConnectionBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteExpressConnectRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteExpressConnectRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteExpressConnectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteExpressConnect','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteExpressConnect','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeletionProtectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeletionProtectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeletionProtectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeletionProtection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeletionProtection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyNetworkAclAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyNetworkAclAttributesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyNetworkAclAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNetworkAclAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyNetworkAclAttributes','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVSwitchAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVSwitchAttributeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVSwitchAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVSwitchAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVSwitchAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBandwidthPackageRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteCommonBandwidthPackageRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DeleteBandwidthPackageRequest(RpcRequest):
+class DeleteCommonBandwidthPackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBandwidthPackage','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteCommonBandwidthPackage','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVRoutersRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVRoutersRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVRoutersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVRouters','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVRouters','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageIpBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageIpBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyCommonBandwidthPackageIpBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageIpBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageIpBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ApplyPhysicalConnectionLOARequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ApplyPhysicalConnectionLOARequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ApplyPhysicalConnectionLOARequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ApplyPhysicalConnectionLOA','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ApplyPhysicalConnectionLOA','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveGlobalAccelerationInstanceIpRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveGlobalAccelerationInstanceIpRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RemoveGlobalAccelerationInstanceIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveGlobalAccelerationInstanceIp','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveGlobalAccelerationInstanceIp','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteForwardEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteForwardEntryRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteForwardEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteForwardEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteForwardEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_ForwardTableId(self):
 		return self.get_query_params().get('ForwardTableId')
 
 	def set_ForwardTableId(self,ForwardTableId):
 		self.add_query_param('ForwardTableId',ForwardTableId)
 
 	def get_ForwardEntryId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpcsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteTableListRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DescribeVpcsRequest(RpcRequest):
+class DescribeRouteTableListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpcs','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteTableList','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -38,54 +38,37 @@
 
 	def get_PageNumber(self):
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self,PageNumber):
 		self.add_query_param('PageNumber',PageNumber)
 
-	def get_VpcName(self):
-		return self.get_query_params().get('VpcName')
-
-	def set_VpcName(self,VpcName):
-		self.add_query_param('VpcName',VpcName)
-
 	def get_ResourceGroupId(self):
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self,ResourceGroupId):
 		self.add_query_param('ResourceGroupId',ResourceGroupId)
 
+	def get_RouteTableName(self):
+		return self.get_query_params().get('RouteTableName')
+
+	def set_RouteTableName(self,RouteTableName):
+		self.add_query_param('RouteTableName',RouteTableName)
+
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		for i in range(len(Tags)):	
-			if Tags[i].get('Value') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Value' , Tags[i].get('Value'))
-			if Tags[i].get('Key') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Key' , Tags[i].get('Key'))
-
-
-	def get_IsDefault(self):
-		return self.get_query_params().get('IsDefault')
+	def get_RouteTableId(self):
+		return self.get_query_params().get('RouteTableId')
 
-	def set_IsDefault(self,IsDefault):
-		self.add_query_param('IsDefault',IsDefault)
-
-	def get_DryRun(self):
-		return self.get_query_params().get('DryRun')
-
-	def set_DryRun(self,DryRun):
-		self.add_query_param('DryRun',DryRun)
+	def set_RouteTableId(self,RouteTableId):
+		self.add_query_param('RouteTableId',RouteTableId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -97,12 +80,24 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
+	def get_RouterType(self):
+		return self.get_query_params().get('RouterType')
+
+	def set_RouterType(self,RouterType):
+		self.add_query_param('RouterType',RouterType)
+
+	def get_RouterId(self):
+		return self.get_query_params().get('RouterId')
+
+	def set_RouterId(self,RouterId):
+		self.add_query_param('RouterId',RouterId)
+
 	def get_VpcId(self):
 		return self.get_query_params().get('VpcId')
 
 	def set_VpcId(self,VpcId):
 		self.add_query_param('VpcId',VpcId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeZonesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeZonesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeZonesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeZones','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeZones','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBgpGroupRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBgpGroupRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateBgpGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBgpGroup','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBgpGroup','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AuthKey(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelExpressCloudConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelExpressCloudConnectionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CancelExpressCloudConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelExpressCloudConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelExpressCloudConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnConnectionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnConnections','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnConnections','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveCommonBandwidthPackageIpRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveCommonBandwidthPackageIpRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RemoveCommonBandwidthPackageIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveCommonBandwidthPackageIp','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveCommonBandwidthPackageIp','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouterInterfaceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouterInterfaceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateRouterInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouterInterface','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouterInterface','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AccessPointId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteHaVipRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DisableVpcClassicLinkRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DeleteHaVipRequest(RpcRequest):
+class DisableVpcClassicLinkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteHaVip','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DisableVpcClassicLink','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -38,20 +38,14 @@
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_HaVipId(self):
-		return self.get_query_params().get('HaVipId')
-
-	def set_HaVipId(self,HaVipId):
-		self.add_query_param('HaVipId',HaVipId)
-
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
@@ -60,8 +54,14 @@
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_VpcId(self):
+		return self.get_query_params().get('VpcId')
+
+	def set_VpcId(self,VpcId):
+		self.add_query_param('VpcId',VpcId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBgpPeerAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBgpPeerAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyBgpPeerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBgpPeerAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBgpPeerAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageSpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCommonBandwidthPackageSpecRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyCommonBandwidthPackageSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageSpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCommonBandwidthPackageSpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CompletePhysicalConnectionLOARequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CompletePhysicalConnectionLOARequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CompletePhysicalConnectionLOARequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CompletePhysicalConnectionLOA','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CompletePhysicalConnectionLOA','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_LineCode(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpcAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpcAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpcAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpcAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpcAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIpv6GatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIpv6GatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateIpv6GatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIpv6Gateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIpv6Gateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6EgressOnlyRuleRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6EgressOnlyRuleRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIpv6EgressOnlyRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6EgressOnlyRule','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6EgressOnlyRule','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIPv6TranslatorAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateNetworkAclRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateNetworkAclRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociateNetworkAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateNetworkAcl','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateNetworkAcl','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyHaVipAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyHaVipAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyHaVipAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyHaVipAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyHaVipAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouteEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_RouteEntryName(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpcRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpcRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVpcRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpc','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpc','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnPbrRouteEntryWeightRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnPbrRouteEntryWeightRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVpnPbrRouteEntryWeightRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnPbrRouteEntryWeight','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnPbrRouteEntryWeight','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_RouteSource(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateGlobalAccelerationInstanceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateGlobalAccelerationInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AssociateGlobalAccelerationInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateGlobalAccelerationInstance','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateGlobalAccelerationInstance','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBandwidthPackagesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBandwidthPackagesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeBandwidthPackagesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBandwidthPackages','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBandwidthPackages','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifySslVpnServerRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateExpressCloudConnectionRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,94 +16,106 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifySslVpnServerRequest(RpcRequest):
+class CreateExpressCloudConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifySslVpnServer','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateExpressCloudConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_ClientToken(self):
-		return self.get_query_params().get('ClientToken')
+	def get_PortType(self):
+		return self.get_query_params().get('PortType')
 
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
+	def set_PortType(self,PortType):
+		self.add_query_param('PortType',PortType)
 
-	def get_SslVpnServerId(self):
-		return self.get_query_params().get('SslVpnServerId')
+	def get_Description(self):
+		return self.get_query_params().get('Description')
 
-	def set_SslVpnServerId(self,SslVpnServerId):
-		self.add_query_param('SslVpnServerId',SslVpnServerId)
+	def set_Description(self,Description):
+		self.add_query_param('Description',Description)
 
-	def get_LocalSubnet(self):
-		return self.get_query_params().get('LocalSubnet')
+	def get_RedundantEccId(self):
+		return self.get_query_params().get('RedundantEccId')
 
-	def set_LocalSubnet(self,LocalSubnet):
-		self.add_query_param('LocalSubnet',LocalSubnet)
+	def set_RedundantEccId(self,RedundantEccId):
+		self.add_query_param('RedundantEccId',RedundantEccId)
 
-	def get_Cipher(self):
-		return self.get_query_params().get('Cipher')
+	def get_PeerLocation(self):
+		return self.get_query_params().get('PeerLocation')
 
-	def set_Cipher(self,Cipher):
-		self.add_query_param('Cipher',Cipher)
-
-	def get_ClientIpPool(self):
-		return self.get_query_params().get('ClientIpPool')
-
-	def set_ClientIpPool(self,ClientIpPool):
-		self.add_query_param('ClientIpPool',ClientIpPool)
+	def set_PeerLocation(self,PeerLocation):
+		self.add_query_param('PeerLocation',PeerLocation)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_Compress(self):
-		return self.get_query_params().get('Compress')
+	def get_Bandwidth(self):
+		return self.get_query_params().get('Bandwidth')
 
-	def set_Compress(self,Compress):
-		self.add_query_param('Compress',Compress)
+	def set_Bandwidth(self,Bandwidth):
+		self.add_query_param('Bandwidth',Bandwidth)
 
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
+	def get_PeerCity(self):
+		return self.get_query_params().get('PeerCity')
+
+	def set_PeerCity(self,PeerCity):
+		self.add_query_param('PeerCity',PeerCity)
+
+	def get_IDCardNo(self):
+		return self.get_query_params().get('IDCardNo')
+
+	def set_IDCardNo(self,IDCardNo):
+		self.add_query_param('IDCardNo',IDCardNo)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_Port(self):
-		return self.get_query_params().get('Port')
+	def get_ContactMail(self):
+		return self.get_query_params().get('ContactMail')
+
+	def set_ContactMail(self,ContactMail):
+		self.add_query_param('ContactMail',ContactMail)
+
+	def get_ContactTel(self):
+		return self.get_query_params().get('ContactTel')
 
-	def set_Port(self,Port):
-		self.add_query_param('Port',Port)
+	def set_ContactTel(self,ContactTel):
+		self.add_query_param('ContactTel',ContactTel)
 
-	def get_Proto(self):
-		return self.get_query_params().get('Proto')
+	def get_IdcSP(self):
+		return self.get_query_params().get('IdcSP')
 
-	def set_Proto(self,Proto):
-		self.add_query_param('Proto',Proto)
+	def set_IdcSP(self,IdcSP):
+		self.add_query_param('IdcSP',IdcSP)
 
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
 		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVSwitchAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVSwitchAttributesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVSwitchAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVSwitchAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVSwitchAttributes','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnGatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVpnGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateRouteTableRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateRouteTableRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AssociateRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateRouteTable','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateRouteTable','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateNatGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateNatGatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateNatGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateNatGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateNatGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6InternetBandwidthRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6InternetBandwidthRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIpv6InternetBandwidthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6InternetBandwidth','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6InternetBandwidth','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteBgpPeerRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpPeerRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteBgpPeerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpPeer','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpPeer','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeServerRelatedGlobalAccelerationInstancesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeServerRelatedGlobalAccelerationInstancesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeServerRelatedGlobalAccelerationInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeServerRelatedGlobalAccelerationInstances','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeServerRelatedGlobalAccelerationInstances','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddCommonBandwidthPackageIpRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddCommonBandwidthPackageIpRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AddCommonBandwidthPackageIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddCommonBandwidthPackageIp','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddCommonBandwidthPackageIp','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -56,12 +56,18 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
+	def get_IpType(self):
+		return self.get_query_params().get('IpType')
+
+	def set_IpType(self,IpType):
+		self.add_query_param('IpType',IpType)
+
 	def get_IpInstanceId(self):
 		return self.get_query_params().get('IpInstanceId')
 
 	def set_IpInstanceId(self,IpInstanceId):
 		self.add_query_param('IpInstanceId',IpInstanceId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpGroupsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpGroupsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeBgpGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpGroups','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpGroups','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteFlowLogRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteFlowLogRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteFlowLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteFlowLog','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteFlowLog','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeactiveFlowLogRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeactiveFlowLogRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeactiveFlowLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeactiveFlowLog','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeactiveFlowLog','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteEntryListRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteEntryListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeRouteEntryListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteEntryList','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteEntryList','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeactivateRouterInterfaceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeactivateRouterInterfaceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeactivateRouterInterfaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeactivateRouterInterface','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeactivateRouterInterface','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceSpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceSpecRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyGlobalAccelerationInstanceSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyGlobalAccelerationInstanceSpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyGlobalAccelerationInstanceSpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewaysRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewaysRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIpv6GatewaysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6Gateways','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6Gateways','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnGatewayAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnGatewayAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVpnGatewayAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnGatewayAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnGatewayAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AllocateEipAddressRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AllocateEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AllocateEipAddress','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AllocateEipAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateHaVipRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateHaVipRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AssociateHaVipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateHaVip','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateHaVip','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionOccupancyOrderRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionOccupancyOrderRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreatePhysicalConnectionOccupancyOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnectionOccupancyOrder','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnectionOccupancyOrder','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RecoverVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RecoverVirtualBorderRouterRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RecoverVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RecoverVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RecoverVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DownloadVpnConnectionConfigRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DownloadVpnConnectionConfigRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DownloadVpnConnectionConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DownloadVpnConnectionConfig','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DownloadVpnConnectionConfig','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateHaVipRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateHaVipRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateHaVipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateHaVip','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateHaVip','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IpAddress(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIPv6TranslatorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6Translator','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6Translator','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnGatewaysRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnGatewaysRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnGatewaysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnGateways','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnGateways','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociatePhysicalConnectionToVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociatePhysicalConnectionToVirtualBorderRouterRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AssociatePhysicalConnectionToVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociatePhysicalConnectionToVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociatePhysicalConnectionToVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateEipAddressRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateEipAddressRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociateEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateEipAddress','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateEipAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_AllocationId(self):
 		return self.get_query_params().get('AllocationId')
 
 	def set_AllocationId(self,AllocationId):
 		self.add_query_param('AllocationId',AllocationId)
 
 	def get_InstanceType(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyEipAddressAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyEipAddressAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyEipAddressAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyEipAddressAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyEipAddressAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateRouteTableRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateRouteTableRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociateRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateRouteTable','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateRouteTable','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouteTableRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouteTableRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouteTable','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouteTable','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouterInterfaceAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouterInterfaceAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeRouterInterfaceAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouterInterfaceAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouterInterfaceAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateCustomerGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateCustomerGatewayRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateCustomerGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateCustomerGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateCustomerGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IpAddress(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyGlobalAccelerationInstanceAttributesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyGlobalAccelerationInstanceAttributesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyGlobalAccelerationInstanceAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyGlobalAccelerationInstanceAttributes','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeGrantRulesToCenRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeGrantRulesToCenRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeGrantRulesToCenRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeGrantRulesToCen','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeGrantRulesToCen','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSnatEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSnatEntryRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteSnatEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSnatEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSnatEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_SnatEntryId(self):
 		return self.get_query_params().get('SnatEntryId')
 
 	def set_SnatEntryId(self,SnatEntryId):
 		self.add_query_param('SnatEntryId',SnatEntryId)
 
 	def get_ResourceOwnerAccount(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeHaVipsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeHaVipsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeHaVipsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeHaVips','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeHaVips','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVRouterAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVRouterAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVRouterAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVRouterAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVRouterAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSslVpnServerRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSslVpnServerRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteSslVpnServerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSslVpnServer','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSslVpnServer','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeHighDefinitionMonitorLogAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeHighDefinitionMonitorLogAttributeRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeHighDefinitionMonitorLogAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeHighDefinitionMonitorLogAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeHighDefinitionMonitorLogAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateHaVipRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateHaVipRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociateHaVipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateHaVip','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateHaVip','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateCommonBandwidthPackageRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateCommonBandwidthPackageRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateCommonBandwidthPackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateCommonBandwidthPackage','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateCommonBandwidthPackage','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/EnablePhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/EnablePhysicalConnectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class EnablePhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'EnablePhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'EnablePhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ListTagResourcesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ListTagResourcesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ListTagResources','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ListTagResources','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteSslVpnClientCertRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteSslVpnClientCertRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteSslVpnClientCertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSslVpnClientCert','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteSslVpnClientCert','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouterInterfacesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouterInterfacesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeRouterInterfacesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouterInterfaces','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouterInterfaces','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RemoveIPv6TranslatorAclListEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RemoveIPv6TranslatorAclListEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RemoveIPv6TranslatorAclListEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveIPv6TranslatorAclListEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RemoveIPv6TranslatorAclListEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CancelPhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CancelPhysicalConnectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CancelPhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelPhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CancelPhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/PublishVpnRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/PublishVpnRouteEntryRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class PublishVpnRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'PublishVpnRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'PublishVpnRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnServersRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnServersRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeSslVpnServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnServers','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnServers','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteNatGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteNatGatewayRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteNatGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteNatGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteNatGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeForwardTableEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeForwardTableEntriesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeForwardTableEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeForwardTableEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeForwardTableEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteTableListRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVSwitchesRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DescribeRouteTableListRequest(RpcRequest):
+class DescribeVSwitchesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteTableList','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVSwitches','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -44,43 +44,38 @@
 
 	def get_ResourceGroupId(self):
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self,ResourceGroupId):
 		self.add_query_param('ResourceGroupId',ResourceGroupId)
 
-	def get_RouteTableName(self):
-		return self.get_query_params().get('RouteTableName')
-
-	def set_RouteTableName(self,RouteTableName):
-		self.add_query_param('RouteTableName',RouteTableName)
-
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		for i in range(len(Tags)):	
-			if Tags[i].get('Value') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Value' , Tags[i].get('Value'))
-			if Tags[i].get('Key') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Key' , Tags[i].get('Key'))
+	def get_IsDefault(self):
+		return self.get_query_params().get('IsDefault')
 
+	def set_IsDefault(self,IsDefault):
+		self.add_query_param('IsDefault',IsDefault)
 
 	def get_RouteTableId(self):
 		return self.get_query_params().get('RouteTableId')
 
 	def set_RouteTableId(self,RouteTableId):
 		self.add_query_param('RouteTableId',RouteTableId)
 
+	def get_DryRun(self):
+		return self.get_query_params().get('DryRun')
+
+	def set_DryRun(self,DryRun):
+		self.add_query_param('DryRun',DryRun)
+
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
@@ -91,24 +86,30 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_RouterType(self):
-		return self.get_query_params().get('RouterType')
-
-	def set_RouterType(self,RouterType):
-		self.add_query_param('RouterType',RouterType)
+	def get_VSwitchId(self):
+		return self.get_query_params().get('VSwitchId')
 
-	def get_RouterId(self):
-		return self.get_query_params().get('RouterId')
-
-	def set_RouterId(self,RouterId):
-		self.add_query_param('RouterId',RouterId)
+	def set_VSwitchId(self,VSwitchId):
+		self.add_query_param('VSwitchId',VSwitchId)
 
 	def get_VpcId(self):
 		return self.get_query_params().get('VpcId')
 
 	def set_VpcId(self,VpcId):
-		self.add_query_param('VpcId',VpcId)
+		self.add_query_param('VpcId',VpcId)
+
+	def get_VSwitchName(self):
+		return self.get_query_params().get('VSwitchName')
+
+	def set_VSwitchName(self,VSwitchName):
+		self.add_query_param('VSwitchName',VSwitchName)
+
+	def get_ZoneId(self):
+		return self.get_query_params().get('ZoneId')
+
+	def set_ZoneId(self,ZoneId):
+		self.add_query_param('ZoneId',ZoneId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteGlobalAccelerationInstanceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteGlobalAccelerationInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteGlobalAccelerationInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteGlobalAccelerationInstance','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteGlobalAccelerationInstance','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpnConnectionAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpnConnectionAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVpnConnectionAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnConnectionAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpnConnectionAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_IkeConfig(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/TerminateVirtualBorderRouterRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/TerminateVirtualBorderRouterRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class TerminateVirtualBorderRouterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TerminateVirtualBorderRouter','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'TerminateVirtualBorderRouter','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVpnPbrRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVpnPbrRouteEntryRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVpnPbrRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnPbrRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVpnPbrRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_RouteSource(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnConnectionRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteVSwitchRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteVSwitchRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteVSwitchRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVSwitch','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteVSwitch','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVirtualBorderRoutersForPhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVirtualBorderRoutersForPhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVirtualBorderRoutersForPhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyCustomerGatewayAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyCustomerGatewayAttributeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyCustomerGatewayAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCustomerGatewayAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyCustomerGatewayAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVirtualBorderRoutersRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVirtualBorderRoutersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVirtualBorderRouters','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVirtualBorderRouters','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBgpGroupAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,72 +16,66 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifyBgpGroupAttributeRequest(RpcRequest):
+class CreateIPv6TranslatorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBgpGroupAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6Translator','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_AuthKey(self):
-		return self.get_query_params().get('AuthKey')
-
-	def set_AuthKey(self,AuthKey):
-		self.add_query_param('AuthKey',AuthKey)
-
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_BgpGroupId(self):
-		return self.get_query_params().get('BgpGroupId')
-
-	def set_BgpGroupId(self,BgpGroupId):
-		self.add_query_param('BgpGroupId',BgpGroupId)
-
-	def get_Description(self):
-		return self.get_query_params().get('Description')
+	def get_Spec(self):
+		return self.get_query_params().get('Spec')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
+	def set_Spec(self,Spec):
+		self.add_query_param('Spec',Spec)
 
-	def get_PeerAsn(self):
-		return self.get_query_params().get('PeerAsn')
+	def get_Duration(self):
+		return self.get_query_params().get('Duration')
 
-	def set_PeerAsn(self,PeerAsn):
-		self.add_query_param('PeerAsn',PeerAsn)
+	def set_Duration(self,Duration):
+		self.add_query_param('Duration',Duration)
 
-	def get_IsFakeAsn(self):
-		return self.get_query_params().get('IsFakeAsn')
+	def get_AutoPay(self):
+		return self.get_query_params().get('AutoPay')
 
-	def set_IsFakeAsn(self,IsFakeAsn):
-		self.add_query_param('IsFakeAsn',IsFakeAsn)
+	def set_AutoPay(self,AutoPay):
+		self.add_query_param('AutoPay',AutoPay)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
+	def get_Bandwidth(self):
+		return self.get_query_params().get('Bandwidth')
+
+	def set_Bandwidth(self,Bandwidth):
+		self.add_query_param('Bandwidth',Bandwidth)
+
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
@@ -92,12 +86,18 @@
 
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
 		self.add_query_param('Name',Name)
 
-	def get_LocalAsn(self):
-		return self.get_query_params().get('LocalAsn')
+	def get_PayType(self):
+		return self.get_query_params().get('PayType')
+
+	def set_PayType(self,PayType):
+		self.add_query_param('PayType',PayType)
+
+	def get_PricingCycle(self):
+		return self.get_query_params().get('PricingCycle')
 
-	def set_LocalAsn(self,LocalAsn):
-		self.add_query_param('LocalAsn',LocalAsn)
+	def set_PricingCycle(self,PricingCycle):
+		self.add_query_param('PricingCycle',PricingCycle)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVpcAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVpcAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyVpcAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpcAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVpcAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyBandwidthPackageAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyBandwidthPackageAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBandwidthPackageAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyBandwidthPackageAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteCustomerGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteCustomerGatewayRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteCustomerGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteCustomerGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteCustomerGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeletePhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeletePhysicalConnectionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeletePhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeletePhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeletePhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewaysRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewaysRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeCustomerGatewaysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCustomerGateways','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCustomerGateways','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclListEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclListEntryRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIPv6TranslatorAclListEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAclListEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAclListEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouteTableAttributesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AllocateEipSegmentAddressRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,53 +16,47 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifyRouteTableAttributesRequest(RpcRequest):
+class AllocateEipSegmentAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouteTableAttributes','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AllocateEipSegmentAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_Description(self):
-		return self.get_query_params().get('Description')
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
 
-	def get_RouteTableName(self):
-		return self.get_query_params().get('RouteTableName')
+	def get_ResourceGroupId(self):
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_RouteTableName(self,RouteTableName):
-		self.add_query_param('RouteTableName',RouteTableName)
+	def set_ResourceGroupId(self,ResourceGroupId):
+		self.add_query_param('ResourceGroupId',ResourceGroupId)
 
-	def get_ResourceUid(self):
-		return self.get_query_params().get('ResourceUid')
+	def get_Netmode(self):
+		return self.get_query_params().get('Netmode')
 
-	def set_ResourceUid(self,ResourceUid):
-		self.add_query_param('ResourceUid',ResourceUid)
-
-	def get_RouteTableId(self):
-		return self.get_query_params().get('RouteTableId')
-
-	def set_RouteTableId(self,RouteTableId):
-		self.add_query_param('RouteTableId',RouteTableId)
+	def set_Netmode(self,Netmode):
+		self.add_query_param('Netmode',Netmode)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -74,24 +68,24 @@
 
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
+	def get_EipMask(self):
+		return self.get_query_params().get('EipMask')
+
+	def set_EipMask(self,EipMask):
+		self.add_query_param('EipMask',EipMask)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_KbpsBandwidth(self):
-		return self.get_query_params().get('KbpsBandwidth')
-
-	def set_KbpsBandwidth(self,KbpsBandwidth):
-		self.add_query_param('KbpsBandwidth',KbpsBandwidth)
-
-	def get_ResourceBid(self):
-		return self.get_query_params().get('ResourceBid')
+	def get_InternetChargeType(self):
+		return self.get_query_params().get('InternetChargeType')
 
-	def set_ResourceBid(self,ResourceBid):
-		self.add_query_param('ResourceBid',ResourceBid)
+	def set_InternetChargeType(self,InternetChargeType):
+		self.add_query_param('InternetChargeType',InternetChargeType)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRegionsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRegionsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,33 +19,27 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRegions','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRegions','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_ProductType(self):
-		return self.get_query_params().get('ProductType')
-
-	def set_ProductType(self,ProductType):
-		self.add_query_param('ProductType',ProductType)
-
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpNetworksRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpNetworksRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeBgpNetworksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpNetworks','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpNetworks','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIPv6TranslatorEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIPv6TranslatorEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6TranslatorEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIPv6TranslatorEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AddBandwidthPackageIpsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AddBandwidthPackageIpsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AddBandwidthPackageIpsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddBandwidthPackageIps','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AddBandwidthPackageIps','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateIPv6TranslatorEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6TranslatorEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6TranslatorEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_BackendIpv4Port(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ReleaseEipAddressRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ReleaseEipAddressRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ReleaseEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ReleaseEipAddress','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ReleaseEipAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteExpressCloudConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteExpressCloudConnectionRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteExpressCloudConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteExpressCloudConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteExpressCloudConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/GrantInstanceToCenRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/GrantInstanceToCenRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class GrantInstanceToCenRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'GrantInstanceToCen','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'GrantInstanceToCen','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateBandwidthPackageRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateBandwidthPackageRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateBandwidthPackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBandwidthPackage','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateBandwidthPackage','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DisableVpcClassicLinkRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/EnableVpcClassicLinkRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DisableVpcClassicLinkRequest(RpcRequest):
+class EnableVpcClassicLinkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DisableVpcClassicLink','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'EnableVpcClassicLink','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateRouteEntryRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -86,20 +86,14 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_PrivateIpAddress(self):
-		return self.get_query_params().get('PrivateIpAddress')
-
-	def set_PrivateIpAddress(self,PrivateIpAddress):
-		self.add_query_param('PrivateIpAddress',PrivateIpAddress)
-
 	def get_NextHopLists(self):
 		return self.get_query_params().get('NextHopLists')
 
 	def set_NextHopLists(self,NextHopLists):
 		for i in range(len(NextHopLists)):	
 			if NextHopLists[i].get('Weight') is not None:
 				self.add_query_param('NextHopList.' + str(i + 1) + '.Weight' , NextHopLists[i].get('Weight'))
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVSwitchesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpcRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,70 +16,65 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DescribeVSwitchesRequest(RpcRequest):
+class CreateVpcRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVSwitches','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpc','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
 
-	def get_ResourceGroupId(self):
-		return self.get_query_params().get('ResourceGroupId')
+	def get_EnableIpv6(self):
+		return self.get_query_params().get('EnableIpv6')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
+	def set_EnableIpv6(self,EnableIpv6):
+		self.add_query_param('EnableIpv6',EnableIpv6)
 
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
+	def get_Description(self):
+		return self.get_query_params().get('Description')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_Description(self,Description):
+		self.add_query_param('Description',Description)
 
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
+	def get_VpcName(self):
+		return self.get_query_params().get('VpcName')
 
-	def set_Tags(self,Tags):
-		for i in range(len(Tags)):	
-			if Tags[i].get('Value') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Value' , Tags[i].get('Value'))
-			if Tags[i].get('Key') is not None:
-				self.add_query_param('Tag.' + str(i + 1) + '.Key' , Tags[i].get('Key'))
+	def set_VpcName(self,VpcName):
+		self.add_query_param('VpcName',VpcName)
 
+	def get_ResourceGroupId(self):
+		return self.get_query_params().get('ResourceGroupId')
 
-	def get_IsDefault(self):
-		return self.get_query_params().get('IsDefault')
-
-	def set_IsDefault(self,IsDefault):
-		self.add_query_param('IsDefault',IsDefault)
+	def set_ResourceGroupId(self,ResourceGroupId):
+		self.add_query_param('ResourceGroupId',ResourceGroupId)
 
-	def get_RouteTableId(self):
-		return self.get_query_params().get('RouteTableId')
+	def get_UserCidr(self):
+		return self.get_query_params().get('UserCidr')
 
-	def set_RouteTableId(self,RouteTableId):
-		self.add_query_param('RouteTableId',RouteTableId)
+	def set_UserCidr(self,UserCidr):
+		self.add_query_param('UserCidr',UserCidr)
 
 	def get_DryRun(self):
 		return self.get_query_params().get('DryRun')
 
 	def set_DryRun(self,DryRun):
 		self.add_query_param('DryRun',DryRun)
 
@@ -97,30 +92,18 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_VSwitchId(self):
-		return self.get_query_params().get('VSwitchId')
-
-	def set_VSwitchId(self,VSwitchId):
-		self.add_query_param('VSwitchId',VSwitchId)
-
-	def get_VpcId(self):
-		return self.get_query_params().get('VpcId')
-
-	def set_VpcId(self,VpcId):
-		self.add_query_param('VpcId',VpcId)
-
-	def get_VSwitchName(self):
-		return self.get_query_params().get('VSwitchName')
+	def get_Ipv6CidrBlock(self):
+		return self.get_query_params().get('Ipv6CidrBlock')
 
-	def set_VSwitchName(self,VSwitchName):
-		self.add_query_param('VSwitchName',VSwitchName)
+	def set_Ipv6CidrBlock(self,Ipv6CidrBlock):
+		self.add_query_param('Ipv6CidrBlock',Ipv6CidrBlock)
 
-	def get_ZoneId(self):
-		return self.get_query_params().get('ZoneId')
+	def get_CidrBlock(self):
+		return self.get_query_params().get('CidrBlock')
 
-	def set_ZoneId(self,ZoneId):
-		self.add_query_param('ZoneId',ZoneId)
+	def set_CidrBlock(self,CidrBlock):
+		self.add_query_param('CidrBlock',CidrBlock)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewaySpecRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewaySpecRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIpv6GatewaySpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6GatewaySpec','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6GatewaySpec','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeRouteTablesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeRouteTablesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeRouteTablesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteTables','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeRouteTables','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeAccessPointsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpcsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,76 +16,82 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DescribeAccessPointsRequest(RpcRequest):
+class DescribeVpcsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeAccessPoints','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpcs','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_Type(self):
-		return self.get_query_params().get('Type')
-
-	def set_Type(self,Type):
-		self.add_query_param('Type',Type)
-
 	def get_PageNumber(self):
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self,PageNumber):
 		self.add_query_param('PageNumber',PageNumber)
 
+	def get_VpcName(self):
+		return self.get_query_params().get('VpcName')
+
+	def set_VpcName(self,VpcName):
+		self.add_query_param('VpcName',VpcName)
+
+	def get_ResourceGroupId(self):
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self,ResourceGroupId):
+		self.add_query_param('ResourceGroupId',ResourceGroupId)
+
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
+	def get_IsDefault(self):
+		return self.get_query_params().get('IsDefault')
+
+	def set_IsDefault(self,IsDefault):
+		self.add_query_param('IsDefault',IsDefault)
+
+	def get_DryRun(self):
+		return self.get_query_params().get('DryRun')
+
+	def set_DryRun(self,DryRun):
+		self.add_query_param('DryRun',DryRun)
+
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
+	def get_OwnerAccount(self):
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self,OwnerAccount):
+		self.add_query_param('OwnerAccount',OwnerAccount)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_Filters(self):
-		return self.get_query_params().get('Filters')
-
-	def set_Filters(self,Filters):
-		for i in range(len(Filters)):	
-			for j in range(len(Filters[i].get('Values'))):
-				if Filters[i].get('Values')[j] is not None:
-					self.add_query_param('Filter.' + str(i + 1) + '.Value.'+str(j + 1), Filters[i].get('Values')[j])
-			if Filters[i].get('Key') is not None:
-				self.add_query_param('Filter.' + str(i + 1) + '.Key' , Filters[i].get('Key'))
-
-
-	def get_HostOperator(self):
-		return self.get_query_params().get('HostOperator')
-
-	def set_HostOperator(self,HostOperator):
-		self.add_query_param('HostOperator',HostOperator)
-
-	def get_Name(self):
-		return self.get_query_params().get('Name')
+	def get_VpcId(self):
+		return self.get_query_params().get('VpcId')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_VpcId(self,VpcId):
+		self.add_query_param('VpcId',VpcId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeExpressCloudConnectionsRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeExpressCloudConnectionsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeExpressCloudConnectionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeExpressCloudConnections','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeExpressCloudConnections','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateExpressCloudConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyVirtualBorderRouterAttributeRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,106 +16,118 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class CreateExpressCloudConnectionRequest(RpcRequest):
+class ModifyVirtualBorderRouterAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateExpressCloudConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVirtualBorderRouterAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_PortType(self):
-		return self.get_query_params().get('PortType')
+	def get_CircuitCode(self):
+		return self.get_query_params().get('CircuitCode')
 
-	def set_PortType(self,PortType):
-		self.add_query_param('PortType',PortType)
+	def set_CircuitCode(self,CircuitCode):
+		self.add_query_param('CircuitCode',CircuitCode)
+
+	def get_AssociatedPhysicalConnections(self):
+		return self.get_query_params().get('AssociatedPhysicalConnections')
+
+	def set_AssociatedPhysicalConnections(self,AssociatedPhysicalConnections):
+		self.add_query_param('AssociatedPhysicalConnections',AssociatedPhysicalConnections)
+
+	def get_VlanId(self):
+		return self.get_query_params().get('VlanId')
+
+	def set_VlanId(self,VlanId):
+		self.add_query_param('VlanId',VlanId)
+
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
 
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
-	def get_RedundantEccId(self):
-		return self.get_query_params().get('RedundantEccId')
+	def get_VbrId(self):
+		return self.get_query_params().get('VbrId')
+
+	def set_VbrId(self,VbrId):
+		self.add_query_param('VbrId',VbrId)
+
+	def get_PeerGatewayIp(self):
+		return self.get_query_params().get('PeerGatewayIp')
+
+	def set_PeerGatewayIp(self,PeerGatewayIp):
+		self.add_query_param('PeerGatewayIp',PeerGatewayIp)
+
+	def get_DetectMultiplier(self):
+		return self.get_query_params().get('DetectMultiplier')
+
+	def set_DetectMultiplier(self,DetectMultiplier):
+		self.add_query_param('DetectMultiplier',DetectMultiplier)
+
+	def get_PeeringSubnetMask(self):
+		return self.get_query_params().get('PeeringSubnetMask')
 
-	def set_RedundantEccId(self,RedundantEccId):
-		self.add_query_param('RedundantEccId',RedundantEccId)
+	def set_PeeringSubnetMask(self,PeeringSubnetMask):
+		self.add_query_param('PeeringSubnetMask',PeeringSubnetMask)
 
-	def get_PeerLocation(self):
-		return self.get_query_params().get('PeerLocation')
+	def get_LocalGatewayIp(self):
+		return self.get_query_params().get('LocalGatewayIp')
 
-	def set_PeerLocation(self,PeerLocation):
-		self.add_query_param('PeerLocation',PeerLocation)
+	def set_LocalGatewayIp(self,LocalGatewayIp):
+		self.add_query_param('LocalGatewayIp',LocalGatewayIp)
+
+	def get_MinTxInterval(self):
+		return self.get_query_params().get('MinTxInterval')
+
+	def set_MinTxInterval(self,MinTxInterval):
+		self.add_query_param('MinTxInterval',MinTxInterval)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_Bandwidth(self):
-		return self.get_query_params().get('Bandwidth')
-
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
-	def get_PeerCity(self):
-		return self.get_query_params().get('PeerCity')
-
-	def set_PeerCity(self,PeerCity):
-		self.add_query_param('PeerCity',PeerCity)
-
-	def get_IDCardNo(self):
-		return self.get_query_params().get('IDCardNo')
-
-	def set_IDCardNo(self,IDCardNo):
-		self.add_query_param('IDCardNo',IDCardNo)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_ContactMail(self):
-		return self.get_query_params().get('ContactMail')
-
-	def set_ContactMail(self,ContactMail):
-		self.add_query_param('ContactMail',ContactMail)
-
-	def get_ContactTel(self):
-		return self.get_query_params().get('ContactTel')
-
-	def set_ContactTel(self,ContactTel):
-		self.add_query_param('ContactTel',ContactTel)
-
-	def get_IdcSP(self):
-		return self.get_query_params().get('IdcSP')
+	def get_MinRxInterval(self):
+		return self.get_query_params().get('MinRxInterval')
 
-	def set_IdcSP(self,IdcSP):
-		self.add_query_param('IdcSP',IdcSP)
+	def set_MinRxInterval(self,MinRxInterval):
+		self.add_query_param('MinRxInterval',MinRxInterval)
 
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
 		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnPbrRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnPbrRouteEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVpnPbrRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnPbrRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnPbrRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_RouteSource(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyForwardEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyForwardEntryRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyForwardEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyForwardEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyForwardEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
 	def get_ForwardTableId(self):
 		return self.get_query_params().get('ForwardTableId')
 
 	def set_ForwardTableId(self,ForwardTableId):
 		self.add_query_param('ForwardTableId',ForwardTableId)
 
 	def get_InternalIp(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouteEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewayAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeIpv6GatewayAttributeRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeIpv6GatewayAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6GatewayAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeIpv6GatewayAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIPv6TranslatorAclAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyIPv6TranslatorAclAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAclAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIPv6TranslatorAclAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeCustomerGatewayRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeCustomerGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCustomerGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeCustomerGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteRouteTableRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteRouteTableRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteRouteTableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouteTable','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteRouteTable','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpcRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNatGatewaysRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,71 +16,71 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class CreateVpcRequest(RpcRequest):
+class DescribeNatGatewaysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpc','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNatGateways','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_ClientToken(self):
-		return self.get_query_params().get('ClientToken')
+	def get_Spec(self):
+		return self.get_query_params().get('Spec')
 
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
+	def set_Spec(self,Spec):
+		self.add_query_param('Spec',Spec)
 
-	def get_EnableIpv6(self):
-		return self.get_query_params().get('EnableIpv6')
+	def get_PageNumber(self):
+		return self.get_query_params().get('PageNumber')
 
-	def set_EnableIpv6(self,EnableIpv6):
-		self.add_query_param('EnableIpv6',EnableIpv6)
-
-	def get_Description(self):
-		return self.get_query_params().get('Description')
-
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_VpcName(self):
-		return self.get_query_params().get('VpcName')
-
-	def set_VpcName(self,VpcName):
-		self.add_query_param('VpcName',VpcName)
+	def set_PageNumber(self,PageNumber):
+		self.add_query_param('PageNumber',PageNumber)
 
 	def get_ResourceGroupId(self):
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self,ResourceGroupId):
 		self.add_query_param('ResourceGroupId',ResourceGroupId)
 
-	def get_UserCidr(self):
-		return self.get_query_params().get('UserCidr')
+	def get_NatType(self):
+		return self.get_query_params().get('NatType')
+
+	def set_NatType(self,NatType):
+		self.add_query_param('NatType',NatType)
+
+	def get_PageSize(self):
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
+
+	def get_NatGatewayId(self):
+		return self.get_query_params().get('NatGatewayId')
 
-	def set_UserCidr(self,UserCidr):
-		self.add_query_param('UserCidr',UserCidr)
+	def set_NatGatewayId(self,NatGatewayId):
+		self.add_query_param('NatGatewayId',NatGatewayId)
 
-	def get_DryRun(self):
-		return self.get_query_params().get('DryRun')
+	def get_InstanceChargeType(self):
+		return self.get_query_params().get('InstanceChargeType')
 
-	def set_DryRun(self,DryRun):
-		self.add_query_param('DryRun',DryRun)
+	def set_InstanceChargeType(self,InstanceChargeType):
+		self.add_query_param('InstanceChargeType',InstanceChargeType)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -92,18 +92,18 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_Ipv6CidrBlock(self):
-		return self.get_query_params().get('Ipv6CidrBlock')
+	def get_VpcId(self):
+		return self.get_query_params().get('VpcId')
 
-	def set_Ipv6CidrBlock(self,Ipv6CidrBlock):
-		self.add_query_param('Ipv6CidrBlock',Ipv6CidrBlock)
+	def set_VpcId(self,VpcId):
+		self.add_query_param('VpcId',VpcId)
 
-	def get_CidrBlock(self):
-		return self.get_query_params().get('CidrBlock')
+	def get_Name(self):
+		return self.get_query_params().get('Name')
 
-	def set_CidrBlock(self,CidrBlock):
-		self.add_query_param('CidrBlock',CidrBlock)
+	def set_Name(self,Name):
+		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyPhysicalConnectionAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyPhysicalConnectionAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyPhysicalConnectionAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyPhysicalConnectionAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyPhysicalConnectionAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnTagResourcesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnTagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnTagResources','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnTagResources','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateNetworkAclRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateNetworkAclRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class AssociateNetworkAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateNetworkAcl','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateNetworkAcl','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNewProjectEipMonitorDataRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeNewProjectEipMonitorDataRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeNewProjectEipMonitorDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNewProjectEipMonitorData','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNewProjectEipMonitorData','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyRouterInterfaceAttributeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyRouterInterfaceAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouterInterfaceAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyRouterInterfaceAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OppositeRouterId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeEipGatewayInfoRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipGatewayInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeEipGatewayInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipGatewayInfo','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipGatewayInfo','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UpdateNetworkAclEntriesRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UpdateNetworkAclEntriesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UpdateNetworkAclEntriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UpdateNetworkAclEntries','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UpdateNetworkAclEntries','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateGlobalAccelerationInstanceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateGlobalAccelerationInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateGlobalAccelerationInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateGlobalAccelerationInstance','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateGlobalAccelerationInstance','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeSslVpnClientCertRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeSslVpnClientCertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnClientCert','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeSslVpnClientCert','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreatePhysicalConnectionRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreatePhysicalConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnection','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreatePhysicalConnection','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AccessPointId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/UnassociateGlobalAccelerationInstanceRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/UnassociateGlobalAccelerationInstanceRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class UnassociateGlobalAccelerationInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateGlobalAccelerationInstance','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'UnassociateGlobalAccelerationInstance','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/AssociateEipAddressRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeEipSegmentRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,53 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class AssociateEipAddressRequest(RpcRequest):
+class DescribeEipSegmentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateEipAddress','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeEipSegment','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_AllocationId(self):
-		return self.get_query_params().get('AllocationId')
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
 
-	def set_AllocationId(self,AllocationId):
-		self.add_query_param('AllocationId',AllocationId)
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
 
-	def get_Mode(self):
-		return self.get_query_params().get('Mode')
+	def get_PageNumber(self):
+		return self.get_query_params().get('PageNumber')
 
-	def set_Mode(self,Mode):
-		self.add_query_param('Mode',Mode)
+	def set_PageNumber(self,PageNumber):
+		self.add_query_param('PageNumber',PageNumber)
 
-	def get_InstanceRegionId(self):
-		return self.get_query_params().get('InstanceRegionId')
+	def get_PageSize(self):
+		return self.get_query_params().get('PageSize')
 
-	def set_InstanceRegionId(self,InstanceRegionId):
-		self.add_query_param('InstanceRegionId',InstanceRegionId)
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
 
-	def get_InstanceType(self):
-		return self.get_query_params().get('InstanceType')
+	def get_SegmentInstanceId(self):
+		return self.get_query_params().get('SegmentInstanceId')
 
-	def set_InstanceType(self,InstanceType):
-		self.add_query_param('InstanceType',InstanceType)
+	def set_SegmentInstanceId(self,SegmentInstanceId):
+		self.add_query_param('SegmentInstanceId',SegmentInstanceId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -72,20 +72,8 @@
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_PrivateIpAddress(self):
-		return self.get_query_params().get('PrivateIpAddress')
-
-	def set_PrivateIpAddress(self,PrivateIpAddress):
-		self.add_query_param('PrivateIpAddress',PrivateIpAddress)
-
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
-
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+		self.add_query_param('OwnerId',OwnerId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyFlowLogAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyFlowLogAttributeRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class ModifyFlowLogAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyFlowLogAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyFlowLogAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateVpnRouteEntryRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateVpnRouteEntryRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class CreateVpnRouteEntryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnRouteEntry','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateVpnRouteEntry','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DeleteIpv6GatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteIpv6GatewayRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DeleteIpv6GatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6Gateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteIpv6Gateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeNatGatewaysRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/AssociateEipAddressRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,71 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class DescribeNatGatewaysRequest(RpcRequest):
+class AssociateEipAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeNatGateways','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'AssociateEipAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_Spec(self):
-		return self.get_query_params().get('Spec')
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
 
-	def set_Spec(self,Spec):
-		self.add_query_param('Spec',Spec)
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
 
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
+	def get_AllocationId(self):
+		return self.get_query_params().get('AllocationId')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
+	def set_AllocationId(self,AllocationId):
+		self.add_query_param('AllocationId',AllocationId)
 
-	def get_ResourceGroupId(self):
-		return self.get_query_params().get('ResourceGroupId')
+	def get_Mode(self):
+		return self.get_query_params().get('Mode')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
+	def set_Mode(self,Mode):
+		self.add_query_param('Mode',Mode)
 
-	def get_NatType(self):
-		return self.get_query_params().get('NatType')
+	def get_InstanceRegionId(self):
+		return self.get_query_params().get('InstanceRegionId')
 
-	def set_NatType(self,NatType):
-		self.add_query_param('NatType',NatType)
+	def set_InstanceRegionId(self,InstanceRegionId):
+		self.add_query_param('InstanceRegionId',InstanceRegionId)
 
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
+	def get_InstanceType(self):
+		return self.get_query_params().get('InstanceType')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_NatGatewayId(self):
-		return self.get_query_params().get('NatGatewayId')
-
-	def set_NatGatewayId(self,NatGatewayId):
-		self.add_query_param('NatGatewayId',NatGatewayId)
-
-	def get_InstanceChargeType(self):
-		return self.get_query_params().get('InstanceChargeType')
-
-	def set_InstanceChargeType(self,InstanceChargeType):
-		self.add_query_param('InstanceChargeType',InstanceChargeType)
+	def set_InstanceType(self,InstanceType):
+		self.add_query_param('InstanceType',InstanceType)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -92,18 +80,18 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_VpcId(self):
-		return self.get_query_params().get('VpcId')
+	def get_PrivateIpAddress(self):
+		return self.get_query_params().get('PrivateIpAddress')
 
-	def set_VpcId(self,VpcId):
-		self.add_query_param('VpcId',VpcId)
+	def set_PrivateIpAddress(self,PrivateIpAddress):
+		self.add_query_param('PrivateIpAddress',PrivateIpAddress)
 
-	def get_Name(self):
-		return self.get_query_params().get('Name')
+	def get_InstanceId(self):
+		return self.get_query_params().get('InstanceId')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_InstanceId(self,InstanceId):
+		self.add_query_param('InstanceId',InstanceId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/RevokeInstanceFromCenRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/RevokeInstanceFromCenRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class RevokeInstanceFromCenRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RevokeInstanceFromCen','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'RevokeInstanceFromCen','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeBgpPeersRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeBgpPeersRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeBgpPeersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpPeers','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeBgpPeers','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/DescribeVpnGatewayRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DescribeVpnGatewayRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
 class DescribeVpnGatewayRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnGateway','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DescribeVpnGateway','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyVirtualBorderRouterAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/CreateSslVpnServerRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,118 +16,106 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifyVirtualBorderRouterAttributeRequest(RpcRequest):
+class CreateSslVpnServerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyVirtualBorderRouterAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateSslVpnServer','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_CircuitCode(self):
-		return self.get_query_params().get('CircuitCode')
-
-	def set_CircuitCode(self,CircuitCode):
-		self.add_query_param('CircuitCode',CircuitCode)
-
-	def get_AssociatedPhysicalConnections(self):
-		return self.get_query_params().get('AssociatedPhysicalConnections')
-
-	def set_AssociatedPhysicalConnections(self,AssociatedPhysicalConnections):
-		self.add_query_param('AssociatedPhysicalConnections',AssociatedPhysicalConnections)
-
-	def get_VlanId(self):
-		return self.get_query_params().get('VlanId')
-
-	def set_VlanId(self,VlanId):
-		self.add_query_param('VlanId',VlanId)
-
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_Description(self):
-		return self.get_query_params().get('Description')
-
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_VbrId(self):
-		return self.get_query_params().get('VbrId')
+	def get_LocalSubnet(self):
+		return self.get_query_params().get('LocalSubnet')
 
-	def set_VbrId(self,VbrId):
-		self.add_query_param('VbrId',VbrId)
+	def set_LocalSubnet(self,LocalSubnet):
+		self.add_query_param('LocalSubnet',LocalSubnet)
 
-	def get_PeerGatewayIp(self):
-		return self.get_query_params().get('PeerGatewayIp')
+	def get_EnableMultiFactorAuth(self):
+		return self.get_query_params().get('EnableMultiFactorAuth')
 
-	def set_PeerGatewayIp(self,PeerGatewayIp):
-		self.add_query_param('PeerGatewayIp',PeerGatewayIp)
+	def set_EnableMultiFactorAuth(self,EnableMultiFactorAuth):
+		self.add_query_param('EnableMultiFactorAuth',EnableMultiFactorAuth)
 
-	def get_DetectMultiplier(self):
-		return self.get_query_params().get('DetectMultiplier')
+	def get_IDaaSInstanceId(self):
+		return self.get_query_params().get('IDaaSInstanceId')
 
-	def set_DetectMultiplier(self,DetectMultiplier):
-		self.add_query_param('DetectMultiplier',DetectMultiplier)
+	def set_IDaaSInstanceId(self,IDaaSInstanceId):
+		self.add_query_param('IDaaSInstanceId',IDaaSInstanceId)
 
-	def get_PeeringSubnetMask(self):
-		return self.get_query_params().get('PeeringSubnetMask')
+	def get_Cipher(self):
+		return self.get_query_params().get('Cipher')
 
-	def set_PeeringSubnetMask(self,PeeringSubnetMask):
-		self.add_query_param('PeeringSubnetMask',PeeringSubnetMask)
+	def set_Cipher(self,Cipher):
+		self.add_query_param('Cipher',Cipher)
 
-	def get_LocalGatewayIp(self):
-		return self.get_query_params().get('LocalGatewayIp')
+	def get_ClientIpPool(self):
+		return self.get_query_params().get('ClientIpPool')
 
-	def set_LocalGatewayIp(self,LocalGatewayIp):
-		self.add_query_param('LocalGatewayIp',LocalGatewayIp)
-
-	def get_MinTxInterval(self):
-		return self.get_query_params().get('MinTxInterval')
-
-	def set_MinTxInterval(self,MinTxInterval):
-		self.add_query_param('MinTxInterval',MinTxInterval)
+	def set_ClientIpPool(self,ClientIpPool):
+		self.add_query_param('ClientIpPool',ClientIpPool)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
+	def get_Compress(self):
+		return self.get_query_params().get('Compress')
+
+	def set_Compress(self,Compress):
+		self.add_query_param('Compress',Compress)
+
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
+	def get_VpnGatewayId(self):
+		return self.get_query_params().get('VpnGatewayId')
+
+	def set_VpnGatewayId(self,VpnGatewayId):
+		self.add_query_param('VpnGatewayId',VpnGatewayId)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_MinRxInterval(self):
-		return self.get_query_params().get('MinRxInterval')
+	def get_Port(self):
+		return self.get_query_params().get('Port')
+
+	def set_Port(self,Port):
+		self.add_query_param('Port',Port)
+
+	def get_Proto(self):
+		return self.get_query_params().get('Proto')
 
-	def set_MinRxInterval(self,MinRxInterval):
-		self.add_query_param('MinRxInterval',MinRxInterval)
+	def set_Proto(self,Proto):
+		self.add_query_param('Proto',Proto)
 
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
 		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewayAttributeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifyExpressCloudConnectionAttributeRequest(RpcRequest):
+class ModifyIpv6GatewayAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyExpressCloudConnectionAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6GatewayAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -38,20 +38,14 @@
 
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
-	def get_EccId(self):
-		return self.get_query_params().get('EccId')
-
-	def set_EccId(self,EccId):
-		self.add_query_param('EccId',EccId)
-
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
@@ -62,12 +56,18 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
+	def get_Ipv6GatewayId(self):
+		return self.get_query_params().get('Ipv6GatewayId')
+
+	def set_Ipv6GatewayId(self,Ipv6GatewayId):
+		self.add_query_param('Ipv6GatewayId',Ipv6GatewayId)
+
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
 		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/CreateIPv6TranslatorRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ModifyExpressCloudConnectionAttributeRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,88 +16,76 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class CreateIPv6TranslatorRequest(RpcRequest):
+class ModifyExpressCloudConnectionAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'CreateIPv6Translator','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyExpressCloudConnectionAttribute','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_ClientToken(self):
-		return self.get_query_params().get('ClientToken')
+	def get_Description(self):
+		return self.get_query_params().get('Description')
 
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
+	def set_Description(self,Description):
+		self.add_query_param('Description',Description)
 
-	def get_Spec(self):
-		return self.get_query_params().get('Spec')
+	def get_EccId(self):
+		return self.get_query_params().get('EccId')
 
-	def set_Spec(self,Spec):
-		self.add_query_param('Spec',Spec)
-
-	def get_Duration(self):
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self,Duration):
-		self.add_query_param('Duration',Duration)
-
-	def get_AutoPay(self):
-		return self.get_query_params().get('AutoPay')
-
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
+	def set_EccId(self,EccId):
+		self.add_query_param('EccId',EccId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_Bandwidth(self):
-		return self.get_query_params().get('Bandwidth')
-
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
+	def get_CeIp(self):
+		return self.get_query_params().get('CeIp')
+
+	def set_CeIp(self,CeIp):
+		self.add_query_param('CeIp',CeIp)
+
+	def get_BgpAs(self):
+		return self.get_query_params().get('BgpAs')
+
+	def set_BgpAs(self,BgpAs):
+		self.add_query_param('BgpAs',BgpAs)
+
+	def get_PeIp(self):
+		return self.get_query_params().get('PeIp')
+
+	def set_PeIp(self,PeIp):
+		self.add_query_param('PeIp',PeIp)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
 	def get_Name(self):
 		return self.get_query_params().get('Name')
 
 	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
-
-	def get_PayType(self):
-		return self.get_query_params().get('PayType')
-
-	def set_PayType(self,PayType):
-		self.add_query_param('PayType',PayType)
-
-	def get_PricingCycle(self):
-		return self.get_query_params().get('PricingCycle')
-
-	def set_PricingCycle(self,PricingCycle):
-		self.add_query_param('PricingCycle',PricingCycle)
+		self.add_query_param('Name',Name)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/ModifyIpv6GatewayAttributeRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/ReleaseEipSegmentAddressRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,41 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class ModifyIpv6GatewayAttributeRequest(RpcRequest):
+class ReleaseEipSegmentAddressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ModifyIpv6GatewayAttribute','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'ReleaseEipSegmentAddress','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_Description(self):
-		return self.get_query_params().get('Description')
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
+	def get_SegmentInstanceId(self):
+		return self.get_query_params().get('SegmentInstanceId')
+
+	def set_SegmentInstanceId(self,SegmentInstanceId):
+		self.add_query_param('SegmentInstanceId',SegmentInstanceId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
@@ -54,20 +60,8 @@
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Ipv6GatewayId(self):
-		return self.get_query_params().get('Ipv6GatewayId')
-
-	def set_Ipv6GatewayId(self,Ipv6GatewayId):
-		self.add_query_param('Ipv6GatewayId',Ipv6GatewayId)
-
-	def get_Name(self):
-		return self.get_query_params().get('Name')
-
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+		self.add_query_param('OwnerId',OwnerId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/request/v20160428/EnableVpcClassicLinkRequest.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/request/v20160428/DeleteBgpGroupRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpc.endpoint import endpoint_data
 
-class EnableVpcClassicLinkRequest(RpcRequest):
+class DeleteBgpGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'EnableVpcClassicLink','vpc')
+		RpcRequest.__init__(self, 'Vpc', '2016-04-28', 'DeleteBgpGroup','Vpc')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
@@ -38,14 +38,20 @@
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
+	def get_BgpGroupId(self):
+		return self.get_query_params().get('BgpGroupId')
+
+	def set_BgpGroupId(self,BgpGroupId):
+		self.add_query_param('BgpGroupId',BgpGroupId)
+
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
@@ -54,14 +60,8 @@
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_VpcId(self):
-		return self.get_query_params().get('VpcId')
-
-	def set_VpcId(self,VpcId):
-		self.add_query_param('VpcId',VpcId)
+		self.add_query_param('OwnerId',OwnerId)
```

### Comparing `aliyun-python-sdk-vpc-3.0.8/aliyunsdkvpc/endpoint.py` & `aliyun-python-sdk-vpc-3.0.9/aliyunsdkvpc/endpoint.py`

 * *Files identical despite different names*

