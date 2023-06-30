# Comparing `tmp/qcloud_setup-1.0.0.tar.gz` & `tmp/qcloud_setup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.0.tar", last modified: Thu Jun 29 02:26:01 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.1.tar", last modified: Fri Jun 30 01:18:13 2023, max compression
```

## Comparing `qcloud_setup-1.0.0.tar` & `qcloud_setup-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 02:26:01.849576 qcloud_setup-1.0.0/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.0/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    15741 2023-06-29 02:26:01.849405 qcloud_setup-1.0.0/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    14714 2023-06-29 00:56:35.000000 qcloud_setup-1.0.0/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-06-28 22:20:03.000000 qcloud_setup-1.0.0/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 02:26:01.848642 qcloud_setup-1.0.0/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    15741 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-06-29 02:26:01.000000 qcloud_setup-1.0.0/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-29 02:26:01.849614 qcloud_setup-1.0.0/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      913 2023-06-29 01:02:00.000000 qcloud_setup-1.0.0/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 02:26:01.847485 qcloud_setup-1.0.0/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 02:26:01.849213 qcloud_setup-1.0.0/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.0/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.0/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.0/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6125 2023-06-25 23:43:46.000000 qcloud_setup-1.0.0/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    53484 2023-06-29 02:23:13.000000 qcloud_setup-1.0.0/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.629621 qcloud_setup-1.0.1/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.1/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)    15417 2023-06-30 01:18:13.629401 qcloud_setup-1.0.1/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    14390 2023-06-30 01:18:08.000000 qcloud_setup-1.0.1/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-06-30 01:17:39.000000 qcloud_setup-1.0.1/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.628588 qcloud_setup-1.0.1/qcloud_setup.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)    15417 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-06-30 01:18:13.000000 qcloud_setup-1.0.1/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-30 01:18:13.629661 qcloud_setup-1.0.1/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      913 2023-06-30 01:17:50.000000 qcloud_setup-1.0.1/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.627412 qcloud_setup-1.0.1/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:18:13.629195 qcloud_setup-1.0.1/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.1/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6125 2023-06-25 23:43:46.000000 qcloud_setup-1.0.1/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    53484 2023-06-29 02:23:13.000000 qcloud_setup-1.0.1/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.0/LICENSE.txt` & `qcloud_setup-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.0/PKG-INFO` & `qcloud_setup-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_setup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -115,15 +115,15 @@
 
 ## Prequisites
 
 The Q-Cloud infrastructure requires you to have python (v3.7 or later)
 installed.  You can install the package, along with its dependencies, using the
 following:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_setup
+python3 -m pip install qcloud_setup
 ```
 Ensure plcuster is on your path by typing the following:
 ```
 which pcluster
 ```
 If it is not, you will need to find the pcluster script within your python
 environment and add its location to your path.
@@ -370,28 +370,14 @@
 You can also open an ssh connection to the head node using the following:
 
 ```
 qcloud_setup  --shell
 ```
 
 
-## Costs
-
-If you will not be submitting jobs for an extended period of time, be sure to suspend
-or terminate the cluster.
-
-AWS charges $0.005/hr for reserving an EIP that is not associated with an instance.
-
-Approximate EBS storage costs: 10Gb $1/month
-
-S3 storage
-
-EIP costs
-
-
 ## Troubleshooting
 
 - When launching the cluster, if you receive permission problems associated
   with lambda functions, check to ensure that the IAM policy (QCloudIamPolicy) has been
   created in the same region as the cluster.
 
 - When submitting jobs, a job ID should be returned. This is a random
```

### Comparing `qcloud_setup-1.0.0/README.md` & `qcloud_setup-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 ## Prequisites
 
 The Q-Cloud infrastructure requires you to have python (v3.7 or later)
 installed.  You can install the package, along with its dependencies, using the
 following:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_setup
+python3 -m pip install qcloud_setup
 ```
 Ensure plcuster is on your path by typing the following:
 ```
 which pcluster
 ```
 If it is not, you will need to find the pcluster script within your python
 environment and add its location to your path.
@@ -345,28 +345,14 @@
 You can also open an ssh connection to the head node using the following:
 
 ```
 qcloud_setup  --shell
 ```
 
 
-## Costs
-
-If you will not be submitting jobs for an extended period of time, be sure to suspend
-or terminate the cluster.
-
-AWS charges $0.005/hr for reserving an EIP that is not associated with an instance.
-
-Approximate EBS storage costs: 10Gb $1/month
-
-S3 storage
-
-EIP costs
-
-
 ## Troubleshooting
 
 - When launching the cluster, if you receive permission problems associated
   with lambda functions, check to ensure that the IAM policy (QCloudIamPolicy) has been
   created in the same region as the cluster.
 
 - When submitting jobs, a job ID should be returned. This is a random
```

### Comparing `qcloud_setup-1.0.0/pyproject.toml` & `qcloud_setup-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.0"
+version = "1.0.1"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_setup-1.0.0/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.1/qcloud_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-setup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -115,15 +115,15 @@
 
 ## Prequisites
 
 The Q-Cloud infrastructure requires you to have python (v3.7 or later)
 installed.  You can install the package, along with its dependencies, using the
 following:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_setup
+python3 -m pip install qcloud_setup
 ```
 Ensure plcuster is on your path by typing the following:
 ```
 which pcluster
 ```
 If it is not, you will need to find the pcluster script within your python
 environment and add its location to your path.
@@ -370,28 +370,14 @@
 You can also open an ssh connection to the head node using the following:
 
 ```
 qcloud_setup  --shell
 ```
 
 
-## Costs
-
-If you will not be submitting jobs for an extended period of time, be sure to suspend
-or terminate the cluster.
-
-AWS charges $0.005/hr for reserving an EIP that is not associated with an instance.
-
-Approximate EBS storage costs: 10Gb $1/month
-
-S3 storage
-
-EIP costs
-
-
 ## Troubleshooting
 
 - When launching the cluster, if you receive permission problems associated
   with lambda functions, check to ensure that the IAM policy (QCloudIamPolicy) has been
   created in the same region as the cluster.
 
 - When submitting jobs, a job ID should be returned. This is a random
```

### Comparing `qcloud_setup-1.0.0/setup.py` & `qcloud_setup-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.0",
+    version="1.0.1",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"),
```

### Comparing `qcloud_setup-1.0.0/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.1/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.0/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.1/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.0/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.1/src/qcloud_setup/iam-policy.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.0/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.1/src/qcloud_setup/qcloud_admin.py`

 * *Files identical despite different names*

