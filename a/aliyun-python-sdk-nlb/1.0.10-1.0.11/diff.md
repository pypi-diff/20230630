# Comparing `tmp/aliyun-python-sdk-nlb-1.0.10.tar.gz` & `tmp/aliyun-python-sdk-nlb-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-nlb-1.0.10.tar", last modified: Wed Jan 11 10:21:53 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-nlb-1.0.11.tar", last modified: Fri Jun 30 06:00:04 2023, max compression
```

## Comparing `aliyun-python-sdk-nlb-1.0.10.tar` & `aliyun-python-sdk-nlb-1.0.11.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/
--rw-r--r--   0 root         (0) root         (0)      575 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1538 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3090 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/
--rw-r--r--   0 root         (0) root         (0)     2850 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/AddServersToServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/AttachCommonBandwidthPackageToLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5476 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2628 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     6198 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DetachCommonBandwidthPackageFromLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DisableLoadBalancerIpv6InternetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/EnableLoadBalancerIpv6InternetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetJobStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetListenerHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetLoadBalancerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListListenerCertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListListenersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListLoadBalancersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListServerGroupServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3252 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListSystemSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2833 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/LoadBalancerJoinSecurityGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/LoadBalancerLeaveSecurityGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2660 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/RemoveServersFromServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/StartListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/StopListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAddressTypeConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2652 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateSecurityPolicyAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     5204 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateServerGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2983 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateServerGroupServersAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-11 10:21:53.000000 aliyun-python-sdk-nlb-1.0.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-01-11 10:21:52.000000 aliyun-python-sdk-nlb-1.0.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AddServersToServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AssociateAdditionalCertificatesWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AttachCommonBandwidthPackageToLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6616 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DetachCommonBandwidthPackageFromLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DisableLoadBalancerIpv6InternetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DisassociateAdditionalCertificatesWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/EnableLoadBalancerIpv6InternetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetJobStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetListenerHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetLoadBalancerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListListenerCertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListListenersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListLoadBalancersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListServerGroupServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListSystemSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/LoadBalancerJoinSecurityGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/LoadBalancerLeaveSecurityGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/MoveResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/RemoveServersFromServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/StartListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/StopListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAddressTypeConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateSecurityPolicyAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateServerGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateServerGroupServersAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-30 06:00:04.000000 aliyun-python-sdk-nlb-1.0.11/setup.py
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/LICENSE` & `aliyun-python-sdk-nlb-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/PKG-INFO` & `aliyun-python-sdk-nlb-1.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nlb
-Version: 1.0.10
+Version: 1.0.11
 Summary: The nlb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nlb
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/README.rst` & `aliyun-python-sdk-nlb-1.0.11/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/PKG-INFO` & `aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-nlb
-Version: 1.0.10
+Version: 1.0.11
 Summary: The nlb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-nlb
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyun_python_sdk_nlb.egg-info/SOURCES.txt` & `aliyun-python-sdk-nlb-1.0.11/aliyun_python_sdk_nlb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 aliyun_python_sdk_nlb.egg-info/dependency_links.txt
 aliyun_python_sdk_nlb.egg-info/requires.txt
 aliyun_python_sdk_nlb.egg-info/top_level.txt
 aliyunsdknlb/__init__.py
 aliyunsdknlb/endpoint.py
 aliyunsdknlb/request/__init__.py
 aliyunsdknlb/request/v20220430/AddServersToServerGroupRequest.py
+aliyunsdknlb/request/v20220430/AssociateAdditionalCertificatesWithListenerRequest.py
 aliyunsdknlb/request/v20220430/AttachCommonBandwidthPackageToLoadBalancerRequest.py
 aliyunsdknlb/request/v20220430/CreateListenerRequest.py
 aliyunsdknlb/request/v20220430/CreateLoadBalancerRequest.py
 aliyunsdknlb/request/v20220430/CreateSecurityPolicyRequest.py
 aliyunsdknlb/request/v20220430/CreateServerGroupRequest.py
 aliyunsdknlb/request/v20220430/DeleteListenerRequest.py
 aliyunsdknlb/request/v20220430/DeleteLoadBalancerRequest.py
 aliyunsdknlb/request/v20220430/DeleteSecurityPolicyRequest.py
 aliyunsdknlb/request/v20220430/DeleteServerGroupRequest.py
 aliyunsdknlb/request/v20220430/DescribeRegionsRequest.py
 aliyunsdknlb/request/v20220430/DescribeZonesRequest.py
 aliyunsdknlb/request/v20220430/DetachCommonBandwidthPackageFromLoadBalancerRequest.py
 aliyunsdknlb/request/v20220430/DisableLoadBalancerIpv6InternetRequest.py
+aliyunsdknlb/request/v20220430/DisassociateAdditionalCertificatesWithListenerRequest.py
 aliyunsdknlb/request/v20220430/EnableLoadBalancerIpv6InternetRequest.py
 aliyunsdknlb/request/v20220430/GetJobStatusRequest.py
 aliyunsdknlb/request/v20220430/GetListenerAttributeRequest.py
 aliyunsdknlb/request/v20220430/GetListenerHealthStatusRequest.py
 aliyunsdknlb/request/v20220430/GetLoadBalancerAttributeRequest.py
 aliyunsdknlb/request/v20220430/ListListenerCertificatesRequest.py
 aliyunsdknlb/request/v20220430/ListListenersRequest.py
@@ -36,14 +38,15 @@
 aliyunsdknlb/request/v20220430/ListSecurityPolicyRequest.py
 aliyunsdknlb/request/v20220430/ListServerGroupServersRequest.py
 aliyunsdknlb/request/v20220430/ListServerGroupsRequest.py
 aliyunsdknlb/request/v20220430/ListSystemSecurityPolicyRequest.py
 aliyunsdknlb/request/v20220430/ListTagResourcesRequest.py
 aliyunsdknlb/request/v20220430/LoadBalancerJoinSecurityGroupRequest.py
 aliyunsdknlb/request/v20220430/LoadBalancerLeaveSecurityGroupRequest.py
+aliyunsdknlb/request/v20220430/MoveResourceGroupRequest.py
 aliyunsdknlb/request/v20220430/RemoveServersFromServerGroupRequest.py
 aliyunsdknlb/request/v20220430/StartListenerRequest.py
 aliyunsdknlb/request/v20220430/StopListenerRequest.py
 aliyunsdknlb/request/v20220430/TagResourcesRequest.py
 aliyunsdknlb/request/v20220430/UntagResourcesRequest.py
 aliyunsdknlb/request/v20220430/UpdateListenerAttributeRequest.py
 aliyunsdknlb/request/v20220430/UpdateLoadBalancerAddressTypeConfigRequest.py
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/endpoint.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/AddServersToServerGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AddServersToServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/AttachCommonBandwidthPackageToLoadBalancerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AttachCommonBandwidthPackageToLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateListenerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateListenerRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,23 @@
 		self.add_body_params('ServerGroupId', ServerGroupId)
 	def get_CertificateIdss(self): # RepeatList
 		return self.get_body_params().get('CertificateIds')
 
 	def set_CertificateIdss(self, CertificateIds):  # RepeatList
 		for depth1 in range(len(CertificateIds)):
 			self.add_body_params('CertificateIds.' + str(depth1 + 1), CertificateIds[depth1])
+	def get_Tags(self): # RepeatList
+		return self.get_body_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_AlpnEnabled(self): # Boolean
 		return self.get_body_params().get('AlpnEnabled')
 
 	def set_AlpnEnabled(self, AlpnEnabled):  # Boolean
 		self.add_body_params('AlpnEnabled', AlpnEnabled)
 	def get_EndPort(self): # Integer
 		return self.get_body_params().get('EndPort')
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateLoadBalancerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateLoadBalancerRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,23 @@
 	def set_LoadBalancerName(self, LoadBalancerName):  # String
 		self.add_body_params('LoadBalancerName', LoadBalancerName)
 	def get_AddressType(self): # String
 		return self.get_body_params().get('AddressType')
 
 	def set_AddressType(self, AddressType):  # String
 		self.add_body_params('AddressType', AddressType)
+	def get_Tags(self): # RepeatList
+		return self.get_body_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_BandwidthPackageId(self): # String
 		return self.get_body_params().get('BandwidthPackageId')
 
 	def set_BandwidthPackageId(self, BandwidthPackageId):  # String
 		self.add_body_params('BandwidthPackageId', BandwidthPackageId)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateSecurityPolicyRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateSecurityPolicyAttributeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class CreateSecurityPolicyRequest(RpcRequest):
+class UpdateSecurityPolicyAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'CreateSecurityPolicy','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'UpdateSecurityPolicyAttribute','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_body_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_body_params('ClientToken', ClientToken)
-	def get_ResourceGroupId(self): # String
-		return self.get_body_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_Cipherss(self): # RepeatList
 		return self.get_body_params().get('Ciphers')
 
 	def set_Cipherss(self, Ciphers):  # RepeatList
 		for depth1 in range(len(Ciphers)):
 			self.add_body_params('Ciphers.' + str(depth1 + 1), Ciphers[depth1])
 	def get_TlsVersionss(self): # RepeatList
@@ -59,7 +54,12 @@
 	def set_SecurityPolicyName(self, SecurityPolicyName):  # String
 		self.add_body_params('SecurityPolicyName', SecurityPolicyName)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
+	def get_SecurityPolicyId(self): # String
+		return self.get_body_params().get('SecurityPolicyId')
+
+	def set_SecurityPolicyId(self, SecurityPolicyId):  # String
+		self.add_body_params('SecurityPolicyId', SecurityPolicyId)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/CreateServerGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateServerGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,23 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_Protocol(self): # String
 		return self.get_body_params().get('Protocol')
 
 	def set_Protocol(self, Protocol):  # String
 		self.add_body_params('Protocol', Protocol)
+	def get_Tags(self): # RepeatList
+		return self.get_body_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
 	def get_ConnectionDrainEnabled(self): # Boolean
 		return self.get_body_params().get('ConnectionDrainEnabled')
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteListenerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteLoadBalancerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteSecurityPolicyRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteSecurityPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DeleteServerGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DeleteServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DescribeRegionsRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DescribeZonesRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DetachCommonBandwidthPackageFromLoadBalancerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DetachCommonBandwidthPackageFromLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/DisableLoadBalancerIpv6InternetRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/DisableLoadBalancerIpv6InternetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/EnableLoadBalancerIpv6InternetRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/EnableLoadBalancerIpv6InternetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetJobStatusRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetJobStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetListenerAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetListenerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetListenerHealthStatusRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetListenerHealthStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/GetLoadBalancerAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/GetLoadBalancerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListListenerCertificatesRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListTagResourcesRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,40 +16,55 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class ListListenerCertificatesRequest(RpcRequest):
+class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'ListListenerCertificates','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'ListTagResources','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ListenerId(self): # String
-		return self.get_body_params().get('ListenerId')
-
-	def set_ListenerId(self, ListenerId):  # String
-		self.add_body_params('ListenerId', ListenerId)
 	def get_NextToken(self): # String
 		return self.get_body_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_body_params('NextToken', NextToken)
 	def get_PageSize(self): # Integer
 		return self.get_body_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_body_params('PageSize', PageSize)
+	def get_Tag(self): # Array
+		return self.get_body_params().get('Tag')
+
+	def set_Tag(self, Tag):  # Array
+		for index1, value1 in enumerate(Tag):
+			if value1.get('Key') is not None:
+				self.add_body_params('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
+			if value1.get('Value') is not None:
+				self.add_body_params('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
+	def get_ResourceId(self): # Array
+		return self.get_body_params().get('ResourceId')
+
+	def set_ResourceId(self, ResourceId):  # Array
+		for index1, value1 in enumerate(ResourceId):
+			self.add_body_params('ResourceId.' + str(index1 + 1), value1)
+	def get_ResourceType(self): # String
+		return self.get_body_params().get('ResourceType')
+
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_body_params('ResourceType', ResourceType)
 	def get_MaxResults(self): # Integer
 		return self.get_body_params().get('MaxResults')
 
 	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_body_params('MaxResults', MaxResults)
 	def get_Page(self): # Integer
 		return self.get_body_params().get('Page')
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListListenersRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListListenersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 		for depth1 in range(len(LoadBalancerIds)):
 			self.add_query_param('LoadBalancerIds.' + str(depth1 + 1), LoadBalancerIds[depth1])
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
+	def get_Tag(self): # Array
+		return self.get_query_params().get('Tag')
+
+	def set_Tag(self, Tag):  # Array
+		for index1, value1 in enumerate(Tag):
+			if value1.get('Key') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
+			if value1.get('Value') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
 	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
 	def set_ListenerProtocol(self, ListenerProtocol):  # String
 		self.add_query_param('ListenerProtocol', ListenerProtocol)
 	def get_ListenerIdss(self): # RepeatList
 		return self.get_query_params().get('ListenerIds')
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListLoadBalancersRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListLoadBalancersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListSecurityPolicyRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListSecurityPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListServerGroupServersRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListServerGroupServersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListServerGroupsRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/ListServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListSystemSecurityPolicyRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/LoadBalancerJoinSecurityGroupRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,53 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class ListSystemSecurityPolicyRequest(RpcRequest):
+class LoadBalancerJoinSecurityGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'ListSystemSecurityPolicy','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'LoadBalancerJoinSecurityGroup','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Channel(self): # String
-		return self.get_body_params().get('Channel')
+	def get_ClientToken(self): # String
+		return self.get_body_params().get('ClientToken')
 
-	def set_Channel(self, Channel):  # String
-		self.add_body_params('Channel', Channel)
-	def get_OwnerIdLoginEmail(self): # String
-		return self.get_body_params().get('OwnerIdLoginEmail')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_body_params('ClientToken', ClientToken)
+	def get_DryRun(self): # Boolean
+		return self.get_body_params().get('DryRun')
+
+	def set_DryRun(self, DryRun):  # Boolean
+		self.add_body_params('DryRun', DryRun)
+	def get_SecurityGroupIdss(self): # RepeatList
+		return self.get_body_params().get('SecurityGroupIds')
+
+	def set_SecurityGroupIdss(self, SecurityGroupIds):  # RepeatList
+		for depth1 in range(len(SecurityGroupIds)):
+			self.add_body_params('SecurityGroupIds.' + str(depth1 + 1), SecurityGroupIds[depth1])
+	def get_LoadBalancerId(self): # String
+		return self.get_body_params().get('LoadBalancerId')
 
-	def set_OwnerIdLoginEmail(self, OwnerIdLoginEmail):  # String
-		self.add_body_params('OwnerIdLoginEmail', OwnerIdLoginEmail)
-	def get_CallerBidLoginEmail(self): # String
-		return self.get_body_params().get('CallerBidLoginEmail')
-
-	def set_CallerBidLoginEmail(self, CallerBidLoginEmail):  # String
-		self.add_body_params('CallerBidLoginEmail', CallerBidLoginEmail)
-	def get_CallerUidLoginEmail(self): # String
-		return self.get_body_params().get('CallerUidLoginEmail')
-
-	def set_CallerUidLoginEmail(self, CallerUidLoginEmail):  # String
-		self.add_body_params('CallerUidLoginEmail', CallerUidLoginEmail)
-	def get_RequestContent(self): # String
-		return self.get_body_params().get('RequestContent')
-
-	def set_RequestContent(self, RequestContent):  # String
-		self.add_body_params('RequestContent', RequestContent)
-	def get_ResourceOwnerAccount(self): # String
-		return self.get_body_params().get('ResourceOwnerAccount')
-
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_body_params('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
-		return self.get_body_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_body_params('OwnerAccount', OwnerAccount)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_body_params('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/ListTagResourcesRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/TagResourcesRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class ListTagResourcesRequest(RpcRequest):
+class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'ListTagResources','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'TagResources','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_NextToken(self): # String
-		return self.get_body_params().get('NextToken')
+	def get_ClientToken(self): # String
+		return self.get_body_params().get('ClientToken')
 
-	def set_NextToken(self, NextToken):  # String
-		self.add_body_params('NextToken', NextToken)
-	def get_PageSize(self): # Integer
-		return self.get_body_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_body_params('PageSize', PageSize)
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_body_params('ClientToken', ClientToken)
 	def get_Tag(self): # Array
 		return self.get_body_params().get('Tag')
 
 	def set_Tag(self, Tag):  # Array
 		for index1, value1 in enumerate(Tag):
 			if value1.get('Key') is not None:
 				self.add_body_params('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
@@ -52,22 +47,17 @@
 				self.add_body_params('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
 	def get_ResourceId(self): # Array
 		return self.get_body_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # Array
 		for index1, value1 in enumerate(ResourceId):
 			self.add_body_params('ResourceId.' + str(index1 + 1), value1)
+	def get_DryRun(self): # Boolean
+		return self.get_body_params().get('DryRun')
+
+	def set_DryRun(self, DryRun):  # Boolean
+		self.add_body_params('DryRun', DryRun)
 	def get_ResourceType(self): # String
 		return self.get_body_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_body_params('ResourceType', ResourceType)
-	def get_MaxResults(self): # Integer
-		return self.get_body_params().get('MaxResults')
-
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_body_params('MaxResults', MaxResults)
-	def get_Page(self): # Integer
-		return self.get_body_params().get('Page')
-
-	def set_Page(self, Page):  # Integer
-		self.add_body_params('Page', Page)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/LoadBalancerJoinSecurityGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/LoadBalancerLeaveSecurityGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class LoadBalancerJoinSecurityGroupRequest(RpcRequest):
+class LoadBalancerLeaveSecurityGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'LoadBalancerJoinSecurityGroup','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'LoadBalancerLeaveSecurityGroup','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/LoadBalancerLeaveSecurityGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/StartListenerRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,39 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class LoadBalancerLeaveSecurityGroupRequest(RpcRequest):
+class StartListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'LoadBalancerLeaveSecurityGroup','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'StartListener','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_body_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_body_params('ClientToken', ClientToken)
+	def get_ListenerId(self): # String
+		return self.get_body_params().get('ListenerId')
+
+	def set_ListenerId(self, ListenerId):  # String
+		self.add_body_params('ListenerId', ListenerId)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
-	def get_SecurityGroupIdss(self): # RepeatList
-		return self.get_body_params().get('SecurityGroupIds')
-
-	def set_SecurityGroupIdss(self, SecurityGroupIds):  # RepeatList
-		for depth1 in range(len(SecurityGroupIds)):
-			self.add_body_params('SecurityGroupIds.' + str(depth1 + 1), SecurityGroupIds[depth1])
-	def get_LoadBalancerId(self): # String
-		return self.get_body_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self, LoadBalancerId):  # String
-		self.add_body_params('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/RemoveServersFromServerGroupRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/RemoveServersFromServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/StartListenerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/StopListenerRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class StartListenerRequest(RpcRequest):
+class StopListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'StartListener','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'StopListener','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/StopListenerRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/AssociateAdditionalCertificatesWithListenerRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class StopListenerRequest(RpcRequest):
+class AssociateAdditionalCertificatesWithListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'StopListener','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'AssociateAdditionalCertificatesWithListener','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -42,7 +42,13 @@
 	def set_ListenerId(self, ListenerId):  # String
 		self.add_body_params('ListenerId', ListenerId)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
+	def get_AdditionalCertificateIdss(self): # RepeatList
+		return self.get_body_params().get('AdditionalCertificateIds')
+
+	def set_AdditionalCertificateIdss(self, AdditionalCertificateIds):  # RepeatList
+		for depth1 in range(len(AdditionalCertificateIds)):
+			self.add_body_params('AdditionalCertificateIds.' + str(depth1 + 1), AdditionalCertificateIds[depth1])
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/TagResourcesRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UntagResourcesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,39 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class TagResourcesRequest(RpcRequest):
+class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'TagResources','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'UntagResources','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_body_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_body_params('ClientToken', ClientToken)
-	def get_Tag(self): # Array
-		return self.get_body_params().get('Tag')
+	def get_All(self): # Boolean
+		return self.get_body_params().get('All')
 
-	def set_Tag(self, Tag):  # Array
-		for index1, value1 in enumerate(Tag):
-			if value1.get('Key') is not None:
-				self.add_body_params('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
-			if value1.get('Value') is not None:
-				self.add_body_params('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
+	def set_All(self, All):  # Boolean
+		self.add_body_params('All', All)
 	def get_ResourceId(self): # Array
 		return self.get_body_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # Array
 		for index1, value1 in enumerate(ResourceId):
 			self.add_body_params('ResourceId.' + str(index1 + 1), value1)
 	def get_DryRun(self): # Boolean
@@ -57,7 +53,13 @@
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
 	def get_ResourceType(self): # String
 		return self.get_body_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_body_params('ResourceType', ResourceType)
+	def get_TagKey(self): # Array
+		return self.get_body_params().get('TagKey')
+
+	def set_TagKey(self, TagKey):  # Array
+		for index1, value1 in enumerate(TagKey):
+			self.add_body_params('TagKey.' + str(index1 + 1), value1)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateListenerAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateListenerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAddressTypeConfigRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAddressTypeConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerProtectionRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateLoadBalancerZonesRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateLoadBalancerZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateSecurityPolicyAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/CreateSecurityPolicyRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,36 +16,50 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdknlb.endpoint import endpoint_data
 
-class UpdateSecurityPolicyAttributeRequest(RpcRequest):
+class CreateSecurityPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'UpdateSecurityPolicyAttribute','nlb')
+		RpcRequest.__init__(self, 'Nlb', '2022-04-30', 'CreateSecurityPolicy','nlb')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_body_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_body_params('ClientToken', ClientToken)
+	def get_ResourceGroupId(self): # String
+		return self.get_body_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_Cipherss(self): # RepeatList
 		return self.get_body_params().get('Ciphers')
 
 	def set_Cipherss(self, Ciphers):  # RepeatList
 		for depth1 in range(len(Ciphers)):
 			self.add_body_params('Ciphers.' + str(depth1 + 1), Ciphers[depth1])
+	def get_Tags(self): # RepeatList
+		return self.get_body_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_body_params('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_TlsVersionss(self): # RepeatList
 		return self.get_body_params().get('TlsVersions')
 
 	def set_TlsVersionss(self, TlsVersions):  # RepeatList
 		for depth1 in range(len(TlsVersions)):
 			self.add_body_params('TlsVersions.' + str(depth1 + 1), TlsVersions[depth1])
 	def get_SecurityPolicyName(self): # String
@@ -54,12 +68,7 @@
 	def set_SecurityPolicyName(self, SecurityPolicyName):  # String
 		self.add_body_params('SecurityPolicyName', SecurityPolicyName)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
-	def get_SecurityPolicyId(self): # String
-		return self.get_body_params().get('SecurityPolicyId')
-
-	def set_SecurityPolicyId(self, SecurityPolicyId):  # String
-		self.add_body_params('SecurityPolicyId', SecurityPolicyId)
```

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateServerGroupAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateServerGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/aliyunsdknlb/request/v20220430/UpdateServerGroupServersAttributeRequest.py` & `aliyun-python-sdk-nlb-1.0.11/aliyunsdknlb/request/v20220430/UpdateServerGroupServersAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-nlb-1.0.10/setup.py` & `aliyun-python-sdk-nlb-1.0.11/setup.py`

 * *Files identical despite different names*

