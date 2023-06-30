# Comparing `tmp/cernrequests-0.3.2.tar.gz` & `tmp/cernrequests-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cernrequests-0.3.2.tar", last modified: Tue May 23 17:01:46 2023, max compression
+gzip compressed data, was "cernrequests-0.4.0.tar", last modified: Fri Jun 30 15:32:16 2023, max compression
```

## Comparing `cernrequests-0.3.2.tar` & `cernrequests-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.3.2/LICENSE
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4495 2023-05-23 17:01:46.006574 cernrequests-0.3.2/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4188 2023-05-23 16:53:33.000000 cernrequests-0.3.2/README.md
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.002574 cernrequests-0.3.2/cernrequests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      487 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/__init__.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    14605 2023-05-23 16:47:13.000000 cernrequests-0.3.2/cernrequests/cern-cacert.pem
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/certs.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/cookies.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      760 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/core.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/cernrequests.egg-info/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4495 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      377 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/SOURCES.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/dependency_links.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       16 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/requires.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/top_level.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-05-23 17:01:46.006574 cernrequests-0.3.2/setup.cfg
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1222 2023-05-23 16:47:13.000000 cernrequests-0.3.2/setup.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/tests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-05-23 15:59:26.000000 cernrequests-0.3.2/tests/test_cernrequests.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1515 2023-05-23 16:18:02.000000 cernrequests-0.3.2/tests/test_real_data.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.4.0/LICENSE
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6466 2023-06-30 15:32:16.097247 cernrequests-0.4.0/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6158 2023-06-30 15:28:53.000000 cernrequests-0.4.0/README.md
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.093248 cernrequests-0.4.0/cernrequests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      499 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-06-30 14:11:19.000000 cernrequests-0.4.0/cernrequests/certs.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-06-30 14:19:31.000000 cernrequests-0.4.0/cernrequests/cookies.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1811 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/core.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1475 2023-06-30 15:28:53.000000 cernrequests-0.4.0/cernrequests/token.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/cernrequests.egg-info/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     6466 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      370 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/requires.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-06-30 15:32:16.000000 cernrequests-0.4.0/cernrequests.egg-info/top_level.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-06-30 15:32:16.097247 cernrequests-0.4.0/setup.cfg
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1250 2023-06-30 15:28:53.000000 cernrequests-0.4.0/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-06-30 15:32:16.097247 cernrequests-0.4.0/tests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-06-30 14:14:27.000000 cernrequests-0.4.0/tests/test_cernrequests.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1531 2023-06-30 15:28:53.000000 cernrequests-0.4.0/tests/test_real_data.py
```

### Comparing `cernrequests-0.3.2/LICENSE` & `cernrequests-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.2/cernrequests/certs.py` & `cernrequests-0.4.0/cernrequests/certs.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.2/cernrequests/cookies.py` & `cernrequests-0.4.0/cernrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.2/setup.py` & `cernrequests-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="cernrequests",
-    version="0.3.2",
+    version="0.4.0",
     desription="CERN wrapper around the requests package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CMSTrackerDPG/cernrequests",
     author="Peter Stein",
     author_email="peter.stein@cern.ch",
     packages=["cernrequests"],
     package_dir={"cernrequests": "cernrequests"},
-    package_data={"cernrequests": ["*.pem"]},
-    install_requires=["requests", "future"],
+    # package_data={"cernrequests": ["*.pem"]},
+    install_requires=["requests", "future", "python-dotenv", "pyjwt"],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

### Comparing `cernrequests-0.3.2/tests/test_cernrequests.py` & `cernrequests-0.4.0/tests/test_cernrequests.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.2/tests/test_real_data.py` & `cernrequests-0.4.0/tests/test_real_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 # This software is distributed under the terms of the GNU Lesser General Public
 # Licence version 3 (LGPL Version 3), copied verbatim in the file “LICENSE”
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
+import os
 import json
-import pytest
-
 import requests
-from requests.exceptions import SSLError
 
 import cernrequests
 from cernrequests import certs
 from cernrequests.cookies import get_sso_cookies
+from cernrequests.core import get, get_with_token
 
 
 def test_dqmgui():
     """
     The DQM GUI does not require cookies, but does require Grid User Certificates
     :return:
     """
@@ -32,20 +31,23 @@
     assert expected == cernrequests.get(url).json()
 
 
 def test_rr():
     """
     RunRegistry requires cookies
     """
-    url = "https://cmsrunregistry.web.cern.ch/api/get_all_dataset_names_of_run/357756"
-    cert = certs.default_user_certificate_paths()
-    ca_bundle = certs.where()
-    cookies = get_sso_cookies(url, cert, verify=ca_bundle)
-    response = requests.get(url, cookies=cookies).json()
+
+    url = (
+        "https://dev-cmsrunregistry.web.cern.ch/api/get_all_dataset_names_of_run/357756"
+    )
+    response = get_with_token(
+        url, target_application="dev-cmsrunregistry-sso-proxy"
+    ).json()
     expected = [
-        "/Express/Collisions2022/DQM",
-        "/Express/Commissioning2022/DQM",
+        # TODO: Uncomment this when new SSO is deployed for production RR
+        # "/Express/Collisions2022/DQM",
+        # "/Express/Commissioning2022/DQM",
         "online",
-        "/PromptReco/Collisions2022/DQM",
+        # "/PromptReco/Collisions2022/DQM",
     ]
 
     assert expected == response
```

