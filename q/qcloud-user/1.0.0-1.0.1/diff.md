# Comparing `tmp/qcloud_user-1.0.0.tar.gz` & `tmp/qcloud_user-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_user-1.0.0.tar", last modified: Thu Jun 29 05:57:17 2023, max compression
+gzip compressed data, was "qcloud_user-1.0.1.tar", last modified: Fri Jun 30 01:16:38 2023, max compression
```

## Comparing `qcloud_user-1.0.0.tar` & `qcloud_user-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 05:57:17.228724 qcloud_user-1.0.0/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.0/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)     4443 2023-06-29 05:57:17.228570 qcloud_user-1.0.0/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)     3444 2023-06-29 00:57:30.000000 qcloud_user-1.0.0/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      721 2023-06-28 22:19:48.000000 qcloud_user-1.0.0/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 05:57:17.228041 qcloud_user-1.0.0/qcloud_user.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)     4443 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      316 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       44 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      153 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       12 2023-06-29 05:57:17.000000 qcloud_user-1.0.0/qcloud_user.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-29 05:57:17.228767 qcloud_user-1.0.0/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      793 2023-06-29 01:19:45.000000 qcloud_user-1.0.0/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 05:57:17.226669 qcloud_user-1.0.0/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-29 05:57:17.228345 qcloud_user-1.0.0/src/qcloud_user/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.0/src/qcloud_user/__init__.py
--rwxr-x---   0 agilbert   (501) staff       (20)    21719 2023-06-29 05:57:07.000000 qcloud_user-1.0.0/src/qcloud_user/qcloud_user.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.796097 qcloud_user-1.0.1/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.1/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)     4398 2023-06-30 01:16:38.795974 qcloud_user-1.0.1/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)     3399 2023-06-30 01:14:34.000000 qcloud_user-1.0.1/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      721 2023-06-30 01:16:24.000000 qcloud_user-1.0.1/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.795577 qcloud_user-1.0.1/qcloud_user.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)     4398 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      316 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       44 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      153 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       12 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-30 01:16:38.796135 qcloud_user-1.0.1/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      793 2023-06-30 01:16:33.000000 qcloud_user-1.0.1/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.794350 qcloud_user-1.0.1/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.795794 qcloud_user-1.0.1/src/qcloud_user/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.1/src/qcloud_user/__init__.py
+-rwxr-x---   0 agilbert   (501) staff       (20)    21719 2023-06-29 05:57:07.000000 qcloud_user-1.0.1/src/qcloud_user/qcloud_user.py
```

### Comparing `qcloud_user-1.0.0/LICENSE.txt` & `qcloud_user-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.0/PKG-INFO` & `qcloud_user-1.0.1/qcloud_user.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud_user
-Version: 1.0.0
+Name: qcloud-user
+Version: 1.0.1
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -31,15 +31,15 @@
 
 
 ## Setup
 
 Before submitting any calculations, you will need to install and configure
 the Q-Cloud command line interface:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_user
+python3 -m pip install  qcloud_user
 qcloud --configure
 ```
 You will be prompted for several configuration values that can be obtained from
 your Q-Cloud administrator.  You should have received an email with an initial
 password for your account, and you will be prompted to change this the first
 time you attempt to submit a job.
```

### Comparing `qcloud_user-1.0.0/README.md` & `qcloud_user-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 ## Setup
 
 Before submitting any calculations, you will need to install and configure
 the Q-Cloud command line interface:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_user
+python3 -m pip install  qcloud_user
 qcloud --configure
 ```
 You will be prompted for several configuration values that can be obtained from
 your Q-Cloud administrator.  You should have received an email with an initial
 password for your account, and you will be prompted to change this the first
 time you attempt to submit a job.
```

### Comparing `qcloud_user-1.0.0/pyproject.toml` & `qcloud_user-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_user"
-version = "1.0.0"
+version = "1.0.1"
 description = "Q-Cloud CLI for users" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_user-1.0.0/qcloud_user.egg-info/PKG-INFO` & `qcloud_user-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud-user
-Version: 1.0.0
+Name: qcloud_user
+Version: 1.0.1
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -31,15 +31,15 @@
 
 
 ## Setup
 
 Before submitting any calculations, you will need to install and configure
 the Q-Cloud command line interface:
 ```
-python3 -m pip install --index-url https://jubilee.q-chem.com/qcpip  qcloud_user
+python3 -m pip install  qcloud_user
 qcloud --configure
 ```
 You will be prompted for several configuration values that can be obtained from
 your Q-Cloud administrator.  You should have received an email with an initial
 password for your account, and you will be prompted to change this the first
 time you attempt to submit a job.
```

### Comparing `qcloud_user-1.0.0/setup.py` & `qcloud_user-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="qcloud_user",
     python_requires='>=3.7',
-    version="1.0.0",
+    version="1.0.1",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="CLI for interacting with Q-Cloud clusters",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['qcloud_user'],
```

### Comparing `qcloud_user-1.0.0/src/qcloud_user/qcloud_user.py` & `qcloud_user-1.0.1/src/qcloud_user/qcloud_user.py`

 * *Files identical despite different names*

