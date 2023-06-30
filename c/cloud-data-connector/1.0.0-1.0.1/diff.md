# Comparing `tmp/cloud_data_connector-1.0.0.tar.gz` & `tmp/cloud_data_connector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_data_connector-1.0.0.tar", last modified: Tue May  9 06:17:17 2023, max compression
+gzip compressed data, was "cloud_data_connector-1.0.1.tar", last modified: Fri Jun 30 19:47:14 2023, max compression
```

## Comparing `cloud_data_connector-1.0.0.tar` & `cloud_data_connector-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    17815 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/PKG-INFO
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)    17291 2023-05-08 16:20:39.000000 cloud_data_connector-1.0.0/README.md
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1049 2023-05-08 16:00:45.000000 cloud_data_connector-1.0.0/pyproject.toml
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      405 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/security.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    17815 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1160 2023-05-09 06:17:17.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      312 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       15 2023-05-09 06:17:16.000000 cloud_data_connector-1.0.0/src/cloud_data_connector.egg-info/top_level.txt
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/data_connector/
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.563636 cloud_data_connector-1.0.0/src/data_connector/aws/
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     5811 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/README.md
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      777 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/aws/__init__.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1604 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/connector.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2966 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/downloader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2196 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/aws/uploader.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/azure/
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      670 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/AzureML.md
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2439 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/azure/README.md
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      942 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/azure/__init__.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     3640 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/connector.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1756 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/connector_object.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     3325 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/downloader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2173 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/ml_uploader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     4520 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/azure/uploader.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/gcp/
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     6426 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/README.md
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      813 2023-05-03 05:11:51.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/__init__.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     7435 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/connector.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     2905 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/downloader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     7468 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/query.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)     1716 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/gcp/uploader.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-05-09 06:17:17.567636 cloud_data_connector-1.0.0/src/data_connector/int/
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)        0 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/__init__.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      971 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_connector.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      912 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_downloader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      990 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/src/data_connector/int/int_uploader.py
--rwxrwxrwx   0 mapineda (12146662) mlp_labs (21495)      580 2023-04-25 19:15:48.000000 cloud_data_connector-1.0.0/tox.ini
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    11357 2023-06-30 19:44:30.000000 cloud_data_connector-1.0.1/LICENSE
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    31670 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    18199 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/README.md
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    31670 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1044 2023-06-30 19:47:14.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)        1 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      304 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)       15 2023-06-30 19:47:13.000000 cloud_data_connector-1.0.1/cloud_data_connector.egg-info/top_level.txt
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/data_connector/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/__init__.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.590604 cloud_data_connector-1.0.1/data_connector/aws/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     6181 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      777 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1604 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2966 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2196 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/aws/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/azure/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      670 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/AzureML.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2483 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      942 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     3640 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1756 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/connector_object.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     3326 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2173 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/ml_uploader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     4520 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/azure/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/gcp/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)    10397 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/README.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      813 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     7435 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     2921 2023-06-30 19:43:49.000000 cloud_data_connector-1.0.1/data_connector/gcp/downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     7468 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/gcp/query.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1736 2023-06-30 19:43:49.000000 cloud_data_connector-1.0.1/data_connector/gcp/uploader.py
+drwxr-sr-x   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/data_connector/int/
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)        0 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/__init__.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      971 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_connector.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      912 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_downloader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      990 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/data_connector/int/int_uploader.py
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)     1223 2023-06-30 19:44:50.000000 cloud_data_connector-1.0.1/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)      405 2023-06-30 19:43:23.000000 cloud_data_connector-1.0.1/security.md
+-rw-r--r--   0 mapineda (12146662) ansible   (1005)       38 2023-06-30 19:47:14.594604 cloud_data_connector-1.0.1/setup.cfg
```

### Comparing `cloud_data_connector-1.0.0/PKG-INFO` & `cloud_data_connector-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-Metadata-Version: 2.1
-Name: cloud_data_connector
-Version: 1.0.0
-Summary: Intel's cloud data connector
-Author-email: IntelAI <IntelAI@intel.com>
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown
+# Cloud Data Connector
 
-<!---
--->
+[![Intel: AI](https://img.shields.io/badge/intel-AI-0071C5)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
+[![Python](https://img.shields.io/badge/Python-3.8/3.9/3.10-green)](https://www.intel.com/content/www/us/en/developer/topic-technology/artificial-intelligence/overview.html)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![security: SNYK](https://img.shields.io/badge/Security-SNYK-yellow)](https://github.com/PyCQA/bandit)
+[![security: BDBA](https://img.shields.io/badge/Security-BDBA-yellow)](https://github.com/PyCQA/bandit)
+[![security: Checkmarks](https://img.shields.io/badge/Security-Checkmarks-yellow)](https://github.com/PyCQA/bandit)
+
+
+_____
 ## Overview
 ---
 data_connector is a tool to connect to AzureML, Azure blob, GCP storage, GCP Big Query  and AWS storage S3. 
 The goal is provide all cloud managers in one place and provide documentation for an easy integration.
 
 For more details, visit the [Data Connector](https://github.com/IntelAI/models/tree/master/datasets/data_connector) GitHub repository.
 <br/><br/>
@@ -47,15 +43,15 @@
 ```bash
 conda create -n venv python=3.10 -c conda-forge
 conda activate venv
 ```
 
 You can install the package with:
 ```bash
-python -m pip install intel-cloud-data-connector
+python -m pip install cloud-data-connector
 ```
 
 Please follow module specific documentation for use case, hands-examples.
 1. data_connector/azure/README.md
 2. data_connector/azure/AzureML.md
 3. data_connector/aws/README.md
 4. data_connector/gcp/README.md
@@ -425,8 +421,8 @@
 <br/><br/>
 
 
 ## Support
 ---
 If you have questions or issues about this package, contact the [Support Team](mailto:IntelAI@intel.com).
 data_connector has an Apache license, as found in the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
-Dependencies versions higher than currently implemented ones are in beta and should be used with caution.
+Dependencies versions higher than currently implemented ones are in beta and should be used with caution.
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/aws/README.md` & `cloud_data_connector-1.0.1/data_connector/aws/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Data Connector AWS S3 
+# Cloud Data Connector: AWS S3 
 
 Data Connector for AWS S3 allows you to connect to S3 buckets and list contents, download and upload files.
 
 ## Access S3 buckets
 
 To access S3 buckets, you will need to sign up for an AWS account and create access keys. 
 
 Access keys consist of an access key ID and secret access key, which are used to sign programmatic requests that you make to AWS.
 
-## Hot to get your access key ID and secret access key
+How to get your access key ID and secret access key
+---
 
 1. Open the IAM console at https://console.aws.amazon.com/iam/.
 2. On the navigation menu, choose Users.
 3. Choose your IAM username.
 4. Open the Security credentials tab, and then choose Create access key.
 5. To see the new access key, choose Show. Your credentials look like the following:
     - Access key ID: my_access_key
@@ -30,151 +31,161 @@
 You can add more configuration settings listed [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables). For example, you can set the `AWS_SESSION_TOKEN`, it is only needed when you are using temporary credentials.
 
 ## Usage
 
 You need to import the DataConnector class.
 
 ```python
-from data_connector.aws.connector import Connector
+from data_connector.aws import Connector as aws_connector
 ```
 
 Connector class has the method connect(), it creates an AWS S3 object, by default the function will create a S3 connector using the credentials saved in your environment variables.
 
 ```python
-connector = Connector()
+aws_bucket_connector = aws_connector()
 ```
 
 Call the connect() method, this will return a connection object for S3. 
 
 ```python
-conection_object = connector.connect()
+aws_conection_object = aws_bucket_connector.connect()
 ```
 
+Downloader
+---
 Import the Downloader class and use the connection object returned by connect() function.
 
+
 ```python
-from data_connector.aws.downloader import Downloader
+from data_connector.aws import Downloader as aws_downloader
 
-downloader = Downloader(conection_object)
+aws_file_downloader = aws_downloader(aws_conection_object)
 ```
 
-The Downloader class has two methods:
 
+
+To download a file use the `download(container_obj, data_file, destiny)` method and specify the next parameters.
+
+- container_obj: The name of the bucket to download from.
+- data_file: The name of the file to download from.
+- destiny: The path to the file to download to.
+
+```python
+from data_connector.aws import Downloader as aws_downloader
+
+downloader = aws_downloader(aws_conection_object)
+file_name = "path/to_file.csv"
+downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
+```
+List Blobs
+---
+[Downloader](#downloader) class has two methods:
 - list_blobs(container_obj): The function to get a list of the objects in a bucket.
 - download(container_obj, data_file, destiny): The function to download a file from a S3 bucket.
 
 A first step with buckets is to list their content using the `list_blobs(container_obj)` method. Specify the next parameter.
 
 - container_obj: The bucket name to list.
 
 ```python
-from data_connector.aws.downloader import Downloader
+from data_connector.aws import Downloader as aws_downloader
 
-downloader = Downloader(conection_object)
+aws_bucket_downloader = aws_downloader(aws_conection_object)
 
-list_blobs = downloader.list_blobs('MY_BUCKET_NAME')
+list_blobs = aws_bucket_downloader.list_blob(
+    'MY_BUCKET_NAME'
+)
 print(list_blobs)
 ```
 
-To download a file use the `download(container_obj, data_file, destiny)` method and specify the next parameters.
-
-- container_obj: The name of the bucket to download from.
-- data_file: The name of the file to download from.
-- destiny: The path to the file to download to.
-
-```python
-from data_connector.aws.downloader import Downloader
-
-downloader = Downloader(conection_object)
-file_name = "path/to_file.csv"
-downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
-```
+Upload
+---
 
 You can import an Uploader class and use the upload method to send a file from you local machine to a bucket. You need to add the connector object to Uploader constructor.
 
 ```python
-from data_connector.aws.uploader import Uploader
-from data_connector.aws.connector import Connector
+from data_connector.aws import Uploader as aws_uploader
+from data_connector.aws  import Connector as aws_connector
 
-connector = Connector()
-conection_object = connector.connect()
-uploader = Uploader(conection_object)
+aws_bucket_connector = aws_connector()
+aws_conection_object = aws_bucket_connector.connect()
+aws_bucker_uploader = aws_uploader(aws_conection_object)
 
 ```
 Specify the next parameters in upload function.
 
 - container_obj: The name of the bucket to upload to.
 - data_file: The path to the file to upload.
-- object_name: The name of the file to upload to.
+- object_name: The name of file in cloud bucket
 
 ```python
-from data_connector.aws.uploader import Uploader
-
-uploader = Uploader(conection_object)
-uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
+aws_bucker_uploader.upload('<bucket_name>', '<path/to_local_file>', '<path/to_object_name>')
 ```
 
+
+Samples
+---
 ### List objects in a bucket
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from data_connector.aws import Connector as aws_connector
+from data_connector.aws import Downloader as aws_downloader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
-connector = Connector()
+aws_bucket_connector = aws_connector()
 # connect to aws using default AWS access keys
 # connect() method uses the configurations settings for AWS account
-conection_object = connector.connect()
+aws_conection_object = aws_bucket_connector.connect()
 # list files from bucket
 # create a downloader to list files
-downloader = Downloader(conection_object)
+aws_downloader = aws_downloader(aws_conection_object)
 # use the list_blobs function
-list_blobs = downloader.list_blobs(bucket_name)
+list_blobs = aws_downloader.list_blobs(bucket_name)
 # list_blobs functions returns all objects in bucket
 print(list_blobs)
 
 ```
 
 ### Download a file
 
 ```python
 # import the dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.downloader import Downloader
+from data_connector.aws import Connector as aws_connector
+from data_connector.aws import Downloader as aws_connector
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
-connector = Connector()
+aws_bucket_connector = aws_connector()
 # connect to aws using default aws access keys
-conection_object = connector.connect()
+aws_conection_object = aws_bucket_connector.connect()
 # download a file from bucket
 # create a Downloader object using a connector object
-downloader = Downloader(conection_object)
+aws_downloader = aws_connector(aws_conection_object)
 # specify the object name to download
 file_name = "path/to_file.csv"
 # download the object
-downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
+aws_downloader.download(bucket_name, file_name, 'path/to_destiny.csv')
 ```
 
 ### Upload a file
 
 ```python
 # import dataconnector package
-from data_connector.aws.connector import Connector
-from data_connector.aws.uploader import Uploader
+from data_connector.aws import Connector as aws_connector
+from data_connector.aws import Uploader as aws_uploader
 
 # specify a S3 bucket name
 bucket_name = 'MY_BUCKET_NAME'
 # create a connector
-connector = Connector()
+aws_bucket_connector = aws_connector()
 # connect to aws using default aws access keys
-conection_object = connector.connect()
+aws_conection_object = aws_bucket_connector.connect()
 # Upload a file
 # create a uploader object using a connection object
-uploader = Uploader(conection_object)
+aws_bucket_uploader = aws_uploader(aws_conection_object)
 # upload a file
-uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
+aws_bucket_uploader.upload(bucket_name, 'path/to_local_file.csv', 'path/to_object_name.csv')
 ```
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/aws/__init__.py` & `cloud_data_connector-1.0.1/data_connector/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/aws/connector.py` & `cloud_data_connector-1.0.1/data_connector/aws/connector.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/aws/downloader.py` & `cloud_data_connector-1.0.1/data_connector/aws/downloader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/aws/uploader.py` & `cloud_data_connector-1.0.1/data_connector/aws/uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/AzureML.md` & `cloud_data_connector-1.0.1/data_connector/azure/AzureML.md`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/README.md` & `cloud_data_connector-1.0.1/data_connector/azure/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Data Connector Azure
-Documentation
--------------
+# Cloud Data Connector: Azure
 
+[Azure ML](./AzureML.md)
+
+---
 ### Abstract
-___
 Data connector for Azure is a tool to connect to Azure Blob and Azure Machine Learning tools.
 
 This tool requires an account on Azure Cloud and an Azure ML worskspace active.
 
 Authentication
 --------------
 Authentication with Azure requires to install [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/authenticate-azure-cli)
@@ -16,38 +16,42 @@
 ```
 This command load certificates to login using simple authentication method. 
 
 
 Storage
 -----------
 All Azure ML Workspaces has an storage blob, with this tool is possible connect to Azure Blob or Azure ML Storage. 
-
+___
 Azure ML
 ----------
 Azure ML is a service to train models connecting data sources and deploy it in production using Azure infrastructure.
 
 Data connector provides a tool to connect to Azure ML workspaces and upload configurations for this proposes.
 
 Sample
----------
-**Blob Connector**
+
+Blob Connector
+---
 ```python
-    from data_connector.azure import connect
+    from data_connector.azure import connect as connect_az
+
     connection_string_sample = """
         DefaultEndpointsProtocol=http;
         AccountName=<YOUR_ACCOUNT_NAME>;
         AccountKey=<YOUR_ACCOUNT_KEY>
         BlobEndpoint=http://127.0.0.1:10000/
         devstoreaccount1;
         QueueEndpoint=http://127.0.0.1:10001/
         devstoreaccount1;
         TableEndpoint=http://127.0.0.1:10002/
         devstoreaccount1;
        """
-    connector = connect(connection_string=connection_string_sample)
+    az_connector = connect_az(
+        connection_string=connection_string_sample
+    )
 
 ```
 How to get a [Connection String](https://learn.microsoft.com/en-us/answers/questions/1071173/where-can-i-find-storage-account-connection-string)? 
 
 ![Azure Connection String Sample](data_connector/../../../docs/img/connection_string.png)
 
 Also you can get connection strings using Azure CLI
@@ -57,27 +61,27 @@
 Or just 
 ```bash
 >az storage account show-connection-string --name <storageAccount> 
 ```
 * This process not works for WSL 
 
 
-**Blob upload**
+Uploader
 ---------
 ```python
-    from data_connector.azure import Uploader
+    from data_connector.azure import Uploader as az_uploader
 
-    uploader = Uploader(connector= connector)
-    uploader.upload(
-        'sample.txt',
-        blob_container_name='sample_container'
+    uploader = az_uploader(connector= az_connector)
+    az_uploader.upload(
+        '<file path>',
+        blob_container_name='<countainer name>'
     )
 ```
 
-**Blob downloader**
+Downloader
 -----
 ```python
     from data_connector.azure import Downloader
 
     downloader = Downloader(connector=connector)
     downloader.download()
 ```
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/__init__.py` & `cloud_data_connector-1.0.1/data_connector/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/connector.py` & `cloud_data_connector-1.0.1/data_connector/azure/connector.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/connector_object.py` & `cloud_data_connector-1.0.1/data_connector/azure/connector_object.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/downloader.py` & `cloud_data_connector-1.0.1/data_connector/azure/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             blob_container = donwload_obj
             blob_container_client = blob_service_client.get_container_client(
                 blob_container
             )
             storage_stream_downloader = blob_container_client.download_blob(
                 data_file
             ).readall()
-            with open(destiny, mode="w") as downloaded_blob:
+            with open(destiny, mode="wb") as downloaded_blob:
                 downloaded_blob.write(storage_stream_downloader)
             self.container_client = blob_container_client
             return blob_container_client
         if isinstance(donwload_obj, Model):
             if not destiny:
                 destiny = "."
             donwload_obj.download(target_dir=destiny, exist_ok=True)
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/ml_uploader.py` & `cloud_data_connector-1.0.1/data_connector/azure/ml_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/azure/uploader.py` & `cloud_data_connector-1.0.1/data_connector/azure/uploader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/gcp/__init__.py` & `cloud_data_connector-1.0.1/data_connector/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/gcp/connector.py` & `cloud_data_connector-1.0.1/data_connector/gcp/connector.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/gcp/downloader.py` & `cloud_data_connector-1.0.1/data_connector/gcp/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     def __init__(self, connector: object):
         if not isinstance(connector, Client):
             raise TypeError("connector must be {}.".format(Client))
         
         super().__init__(connector)
 
 
-    def download(self, container_obj:object, data_file:object, destiny:object) -> object:
+    def download(self, container_obj:object, data_file:object, destination:object) -> object:
         if not isinstance(container_obj, str):
             raise TypeError("container_obj must be str.")
         elif not isinstance(data_file, str):
             raise TypeError("data_file must be str.")
-        elif not isinstance(destiny, str):
-            raise TypeError("destiny must be str.")
+        elif not isinstance(destination, str):
+            raise TypeError("destination must be str.")
         
         try:
             storage_client = self.connector
             bucket = storage_client.get_bucket(container_obj)
             blob = bucket.blob(data_file)
-            with open(destiny, 'wb') as f:
+            with open(destination, 'wb') as f:
                 self.connector.download_blob_to_file(blob, f)
             return True
         except NotFound as e:
             print("blob not found: {}".format(e))
             return False
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/gcp/query.py` & `cloud_data_connector-1.0.1/data_connector/gcp/query.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/gcp/uploader.py` & `cloud_data_connector-1.0.1/data_connector/gcp/uploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 import os
 from google.cloud.exceptions import GoogleCloudError
 class Uploader():
 
     def __init__(self, connector: object):
         self.connector = connector
 
-    def upload_to_bucket(self, container_obj:object, data_file:object, destiny:object) -> object:
+    def upload_to_bucket(self, container_obj:object, data_file:object, destination:object) -> object:
         if not isinstance(container_obj, str):
             raise TypeError("container_obj must be str.")
         elif not isinstance(data_file, str):
             raise TypeError("data_file must be str.")
-        elif not isinstance(destiny, str):
-            raise TypeError("destiny must be str.")
+        elif not isinstance(destination, str):
+            raise TypeError("destination must be str.")
         
         if not os.path.isfile(data_file):
             raise FileNotFoundError("{} not found.".format(data_file))
         
         try:
             storage_client = self.connector
             bucket = storage_client.get_bucket(container_obj)
-            blob = bucket.blob(destiny)
+            blob = bucket.blob(destination)
             blob.upload_from_filename(data_file)
             return True
         except GoogleCloudError as e:
             print(e)
-            raise GoogleCloudError('Failed to copy local file {0} to cloud storage file {1}.'.format(data_file, destiny))
+            raise GoogleCloudError('Failed to copy local file {0} to cloud storage file {1}.'.format(data_file, destination))
```

### Comparing `cloud_data_connector-1.0.0/src/data_connector/int/int_connector.py` & `cloud_data_connector-1.0.1/data_connector/int/int_connector.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/int/int_downloader.py` & `cloud_data_connector-1.0.1/data_connector/int/int_downloader.py`

 * *Files identical despite different names*

### Comparing `cloud_data_connector-1.0.0/src/data_connector/int/int_uploader.py` & `cloud_data_connector-1.0.1/data_connector/int/int_uploader.py`

 * *Files identical despite different names*

