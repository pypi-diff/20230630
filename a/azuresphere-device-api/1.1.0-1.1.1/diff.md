# Comparing `tmp/azuresphere-device-api-1.1.0.tar.gz` & `tmp/azuresphere-device-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azuresphere-device-api-1.1.0.tar", last modified: Fri Apr 28 03:06:42 2023, max compression
+gzip compressed data, was "azuresphere-device-api-1.1.1.tar", last modified: Fri Jun 30 09:45:15 2023, max compression
```

## Comparing `azuresphere-device-api-1.1.0.tar` & `azuresphere-device-api-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/
--rw-rw-rw-   0        0        0     1093 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2411 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1907 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.561559 azuresphere-device-api-1.1.0/azuresphere_device_api/
--rw-rw-rw-   0        0        0      201 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/__init__.py
--rw-rw-rw-   0        0        0     3475 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/app.py
--rw-rw-rw-   0        0        0      714 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/capabilities.py
--rw-rw-rw-   0        0        0     5398 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/certificate.py
-drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/azuresphere_device_api/certs/
--rw-rw-rw-   0        0        0      826 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/certs/device_rest_api_certificate.pem
--rw-rw-rw-   0        0        0     3557 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/device.py
--rw-rw-rw-   0        0        0     3558 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/devices.py
--rw-rw-rw-   0        0        0    14392 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/error_handler.py
--rw-rw-rw-   0        0        0      980 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/exceptions.py
--rw-rw-rw-   0        0        0      545 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/image.py
--rw-rw-rw-   0        0        0     1856 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/manufacturing.py
--rw-rw-rw-   0        0        0     8220 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/network.py
--rw-rw-rw-   0        0        0     3017 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/sideload.py
--rw-rw-rw-   0        0        0    11952 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/utils.py
--rw-rw-rw-   0        0        0     2180 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/validation.py
--rw-rw-rw-   0        0        0    15076 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/azuresphere_device_api/wifi.py
-drwxrwxrwx   0        0        0        0 2023-04-28 03:06:42.561559 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/
--rw-rw-rw-   0        0        0     2411 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-28 03:06:28.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-04-28 03:06:42.000000 azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1129 2023-04-28 03:05:18.000000 azuresphere-device-api-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 03:06:42.577187 azuresphere-device-api-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2337 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1835 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/azuresphere_device_api/
+-rw-rw-rw-   0        0        0      201 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/__init__.py
+-rw-rw-rw-   0        0        0     3475 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/app.py
+-rw-rw-rw-   0        0        0      714 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/capabilities.py
+-rw-rw-rw-   0        0        0     5398 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/certificate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/azuresphere_device_api/certs/
+-rw-rw-rw-   0        0        0      826 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/certs/device_rest_api_certificate.pem
+-rw-rw-rw-   0        0        0     3557 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/device.py
+-rw-rw-rw-   0        0        0     3558 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/devices.py
+-rw-rw-rw-   0        0        0    14392 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/error_handler.py
+-rw-rw-rw-   0        0        0      980 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/exceptions.py
+-rw-rw-rw-   0        0        0      545 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/image.py
+-rw-rw-rw-   0        0        0     1856 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/manufacturing.py
+-rw-rw-rw-   0        0        0     8220 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/network.py
+-rw-rw-rw-   0        0        0     3017 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/sideload.py
+-rw-rw-rw-   0        0        0    12212 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/utils.py
+-rw-rw-rw-   0        0        0     2180 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/validation.py
+-rw-rw-rw-   0        0        0    15076 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/azuresphere_device_api/wifi.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/
+-rw-rw-rw-   0        0        0     2337 2023-06-30 09:45:15.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-06-30 09:45:15.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:45:15.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 09:44:59.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:45:15.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-06-30 09:45:15.000000 azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1129 2023-06-30 09:44:11.000000 azuresphere-device-api-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:45:15.050624 azuresphere-device-api-1.1.1/setup.cfg
```

### Comparing `azuresphere-device-api-1.1.0/LICENSE.txt` & `azuresphere-device-api-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/PKG-INFO` & `azuresphere-device-api-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azuresphere-device-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for interacting with Azure Sphere devices using the inbuilt REST server.
 Author-email: Microsoft <azspheremfrsamplesup@microsoft.com>
 Keywords: azure,sphere,device,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -14,40 +14,40 @@
 # Microsoft Azure Sphere Device REST APIs for Python
 
 Microsoft Azure Sphere Device REST APIs for Python enables users to interact with an Azure Sphere device using REST APIs.
 
 ## Installation
 
 You can find Microsoft Azure Sphere Device REST APIs for Python on [PyPi](https://pypi.org/project/azuresphere_device_api/).
+
 1. If you haven't already, [install and/or upgrade the pip](https://pip.pypa.io/en/stable/installing/)
    of your Python environment to a recent version.
 2. Run `pip install azuresphere_device_api`.
 
-## Versions
-
-This library follows [Semantic Versioning](http://semver.org/).
-
 ## Usage
 
 Before using Microsoft Azure Sphere Device REST APIs for Python, you must install the Azure Sphere SDK.
+
 - To install the Azure Sphere SDK on Windows, follow the [Windows Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk?pivots=cli).
 - To install the Azure Sphere SDK on Linux, follow the [Linux Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk-linux?pivots=cli-linux).
 
 ### Sample
-The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
+
+The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
 
 ### Active device IP address
 
 By default, this package will target Azure Sphere devices with IP address `192.168.35.2`. To change the active Azure Sphere device, call `set_active_device_ip_address` API as below:
+
 ```
 from azuresphere_device_api import devices
 devices.set_active_device_ip_address("<Device_Ip_Address")
 ```
 
 ## Documentation
 
-Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src).
+Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src).
 
 ## Supported host operating systems
 
-* Windows 10 and 11
-* Ubuntu 18.04 and 20.04
+- Windows 10 and 11
+- Ubuntu 18.04, 20.04, 22.04
```

### Comparing `azuresphere-device-api-1.1.0/README.md` & `azuresphere-device-api-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Microsoft Azure Sphere Device REST APIs for Python
 
 Microsoft Azure Sphere Device REST APIs for Python enables users to interact with an Azure Sphere device using REST APIs.
 
 ## Installation
 
 You can find Microsoft Azure Sphere Device REST APIs for Python on [PyPi](https://pypi.org/project/azuresphere_device_api/).
+
 1. If you haven't already, [install and/or upgrade the pip](https://pip.pypa.io/en/stable/installing/)
    of your Python environment to a recent version.
 2. Run `pip install azuresphere_device_api`.
 
-## Versions
-
-This library follows [Semantic Versioning](http://semver.org/).
-
 ## Usage
 
 Before using Microsoft Azure Sphere Device REST APIs for Python, you must install the Azure Sphere SDK.
+
 - To install the Azure Sphere SDK on Windows, follow the [Windows Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk?pivots=cli).
 - To install the Azure Sphere SDK on Linux, follow the [Linux Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk-linux?pivots=cli-linux).
 
 ### Sample
-The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
+
+The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
 
 ### Active device IP address
 
 By default, this package will target Azure Sphere devices with IP address `192.168.35.2`. To change the active Azure Sphere device, call `set_active_device_ip_address` API as below:
+
 ```
 from azuresphere_device_api import devices
 devices.set_active_device_ip_address("<Device_Ip_Address")
 ```
 
 ## Documentation
 
-Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src).
+Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src).
 
 ## Supported host operating systems
 
-* Windows 10 and 11
-* Ubuntu 18.04 and 20.04
+- Windows 10 and 11
+- Ubuntu 18.04, 20.04, 22.04
```

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/app.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/app.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/capabilities.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/capabilities.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/certificate.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/certificate.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/certs/device_rest_api_certificate.pem` & `azuresphere-device-api-1.1.1/azuresphere_device_api/certs/device_rest_api_certificate.pem`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/device.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/device.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/devices.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/devices.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/error_handler.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/error_handler.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/exceptions.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/image.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/image.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/manufacturing.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/manufacturing.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/network.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/network.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/sideload.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/sideload.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/utils.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -167,20 +167,22 @@
     # Create URL
     if api_type == AzureSphereDeviceApiRequestType.LOCAL_DEVICE_URL:
         url_to_use = f"http://localhost:48938/{api}"
         header = {'Accept': 'application/json'}
         return get_response_code_content(requests.get(
             url_to_use,
             verify=str(_CERT_PATH),
+            allow_redirects=False,
             headers=header), api_type)
 
     return get_response_code_content(__make_request(
         method="GET",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
     ), api_type)
 
 
 def delete_request(api: str) -> dict:
     """Makes a "DELETE" request with the given API endpoint.
 
@@ -192,14 +194,15 @@
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     return get_response_code_content(__make_request(
         method="DELETE",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
     ))
 
 
 def post_request_no_body(api: str) -> dict:
     """Makes a "POST" request with the given API endpoint and no JSON body.
 
@@ -211,14 +214,15 @@
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     return get_response_code_content(__make_request(
         method="POST",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
     ))
 
 
 def post_request(api: str, body: Any) -> dict:
     """Makes a "POST" request with the given API endpoint and json body.
 
@@ -232,14 +236,15 @@
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     return get_response_code_content(__make_request(
         method="POST",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
         json=body
     ))
 
 
 def patch_request(api: str, body: Any) -> dict:
     """Makes a "PATCH" request with the given API endpoint and json body, returning the response as
@@ -255,14 +260,15 @@
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     return get_response_code_content(__make_request(
         method="PATCH",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
         json=body
     ))
 
 
 def put_request(api: str, body: Any) -> dict:
     """Makes a "PUT" request with the given API endpoint and json body, returning the response as
@@ -279,14 +285,15 @@
     :raises: requests.exceptions
     :raises: AzureSphereDeviceApiException
     """
     return get_response_code_content(__make_request(
         method="PUT",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=__device_rest_api_headers(),
         json=body
     ))
 
 
 def put_request_octet_stream(api: str, body: Any) -> dict:
     """Makes a "PUT" request with the given API endpoint and json body, returning the response as
@@ -306,14 +313,15 @@
     devicerestapi_headers = __device_rest_api_headers()
     devicerestapi_headers["Content-Type"] = "application/octet-stream"
 
     return get_response_code_content(__make_request(
         method="PUT",
         url=_create_url(api),
         verify=str(_CERT_PATH),
+        allow_redirects=False,
         headers=devicerestapi_headers,
         data=body
     ))
 
 
 def is_uuid(uuid: str) -> bool:
     """Validates if a given string represents a valid UUID.
```

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/validation.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/validation.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api/wifi.py` & `azuresphere-device-api-1.1.1/azuresphere_device_api/wifi.py`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/PKG-INFO` & `azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azuresphere-device-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A library for interacting with Azure Sphere devices using the inbuilt REST server.
 Author-email: Microsoft <azspheremfrsamplesup@microsoft.com>
 Keywords: azure,sphere,device,api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -14,40 +14,40 @@
 # Microsoft Azure Sphere Device REST APIs for Python
 
 Microsoft Azure Sphere Device REST APIs for Python enables users to interact with an Azure Sphere device using REST APIs.
 
 ## Installation
 
 You can find Microsoft Azure Sphere Device REST APIs for Python on [PyPi](https://pypi.org/project/azuresphere_device_api/).
+
 1. If you haven't already, [install and/or upgrade the pip](https://pip.pypa.io/en/stable/installing/)
    of your Python environment to a recent version.
 2. Run `pip install azuresphere_device_api`.
 
-## Versions
-
-This library follows [Semantic Versioning](http://semver.org/).
-
 ## Usage
 
 Before using Microsoft Azure Sphere Device REST APIs for Python, you must install the Azure Sphere SDK.
+
 - To install the Azure Sphere SDK on Windows, follow the [Windows Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk?pivots=cli).
 - To install the Azure Sphere SDK on Linux, follow the [Linux Quickstart](https://learn.microsoft.com/azure-sphere/install/install-sdk-linux?pivots=cli-linux).
 
 ### Sample
-The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
+
+The [display_ip_deviceid sample](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src/Python/device_api_sample) gets the list of attached devices, displays the device IP address, and device ID.
 
 ### Active device IP address
 
 By default, this package will target Azure Sphere devices with IP address `192.168.35.2`. To change the active Azure Sphere device, call `set_active_device_ip_address` API as below:
+
 ```
 from azuresphere_device_api import devices
 devices.set_active_device_ip_address("<Device_Ip_Address")
 ```
 
 ## Documentation
 
-Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-samples/blob/main/Manufacturing/src).
+Microsoft Azure Sphere Device REST APIs for Python documentation is available at [Azure Sphere Device REST APIs Docs](https://github.com/Azure/azure-sphere-tools/blob/main/Manufacturing/src).
 
 ## Supported host operating systems
 
-* Windows 10 and 11
-* Ubuntu 18.04 and 20.04
+- Windows 10 and 11
+- Ubuntu 18.04, 20.04, 22.04
```

### Comparing `azuresphere-device-api-1.1.0/azuresphere_device_api.egg-info/SOURCES.txt` & `azuresphere-device-api-1.1.1/azuresphere_device_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azuresphere-device-api-1.1.0/pyproject.toml` & `azuresphere-device-api-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 addopts = "-ra -vv"
 testpaths = [
     "package_tests",
 ]
 
 [project]
 name = "azuresphere-device-api"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name="Microsoft", email="azspheremfrsamplesup@microsoft.com" }
 ]
 keywords = ["azure", "sphere", "device", "api"]
 readme = "README.md"
 description = "A library for interacting with Azure Sphere devices using the inbuilt REST server."
 classifiers = [
```

