# Comparing `tmp/botocore-a-la-carte-codeguru-security-1.29.163.tar.gz` & `tmp/botocore-a-la-carte-codeguru-security-1.29.164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codeguru-security-1.29.163.tar", last modified: Thu Jun 29 01:39:52 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-codeguru-security-1.29.164.tar", last modified: Fri Jun 30 01:38:40 2023, max compression
```

## Comparing `botocore-a-la-carte-codeguru-security-1.29.163.tar` & `botocore-a-la-carte-codeguru-security-1.29.164.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.984202 botocore-a-la-carte-codeguru-security-1.29.163/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 01:39:52.984202 botocore-a-la-carte-codeguru-security-1.29.163/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.980202 botocore-a-la-carte-codeguru-security-1.29.163/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.980202 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.980202 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.984202 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-06-29 01:39:42.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-29 01:39:42.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    54052 2023-06-29 01:39:42.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:39:52.984202 botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:39:52.984202 botocore-a-la-carte-codeguru-security-1.29.163/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-29 01:39:52.000000 botocore-a-la-carte-codeguru-security-1.29.163/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-06-30 01:38:31.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-30 01:38:31.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54052 2023-06-30 01:38:31.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 01:38:40.563593 botocore-a-la-carte-codeguru-security-1.29.164/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 01:38:40.000000 botocore-a-la-carte-codeguru-security-1.29.164/setup.py
```

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/LICENSE.txt` & `botocore-a-la-carte-codeguru-security-1.29.164/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/PKG-INFO` & `botocore-a-la-carte-codeguru-security-1.29.164/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codeguru-security
-Version: 1.29.163
+Version: 1.29.164
 Summary: codeguru-security data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/paginators-1.json` & `botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/botocore/data/codeguru-security/2018-05-10/service-2.json` & `botocore-a-la-carte-codeguru-security-1.29.164/botocore/data/codeguru-security/2018-05-10/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/botocore_a_la_carte_codeguru_security.egg-info/PKG-INFO` & `botocore-a-la-carte-codeguru-security-1.29.164/botocore_a_la_carte_codeguru_security.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-codeguru-security
-Version: 1.29.163
+Version: 1.29.164
 Summary: codeguru-security data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-codeguru-security-1.29.163/setup.py` & `botocore-a-la-carte-codeguru-security-1.29.164/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-codeguru-security',
-    version="1.29.163",
+    version="1.29.164",
     description='codeguru-security data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/codeguru-security/*/*.json'],
```

