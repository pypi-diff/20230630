# Comparing `tmp/simple_sqs_client-0.9.3.tar.gz` & `tmp/simple_sqs_client-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_sqs_client-0.9.3.tar", last modified: Fri Jun 30 07:01:47 2023, max compression
+gzip compressed data, was "simple_sqs_client-0.9.4.tar", last modified: Fri Jun 30 07:32:42 2023, max compression
```

## Comparing `simple_sqs_client-0.9.3.tar` & `simple_sqs_client-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:01:47.085448 simple_sqs_client-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/src/simple_sqs_client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/src/simple_sqs_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/src/simple_sqs_client/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/src/simple_sqs_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/src/simple_sqs_client/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/src/simple_sqs_client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-30 07:01:47.000000 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 07:01:47.000000 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:01:47.000000 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 07:01:47.000000 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 07:01:47.000000 simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:01:47.089448 simple_sqs_client-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-30 07:01:35.000000 simple_sqs_client-0.9.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:32:42.405601 simple_sqs_client-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/src/simple_sqs_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/src/simple_sqs_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/src/simple_sqs_client/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/src/simple_sqs_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/src/simple_sqs_client/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/src/simple_sqs_client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-30 07:32:42.000000 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 07:32:42.000000 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:32:42.000000 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 07:32:42.000000 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 07:32:42.000000 simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:32:42.409602 simple_sqs_client-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-30 07:32:30.000000 simple_sqs_client-0.9.4/tests/test_client.py
```

### Comparing `simple_sqs_client-0.9.3/LICENSE` & `simple_sqs_client-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_sqs_client-0.9.3/PKG-INFO` & `simple_sqs_client-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_sqs_client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Very simple SQS Client
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Aleksander Laurowski
 Author-email: aleksander.laurowski191@gmail.com
 Project-URL: Documentation, https://github.com/tomchen/example_pypi_package
 Project-URL: Bug Reports, https://github.com/tomchen/example_pypi_package/issues
 Project-URL: Source Code, https://github.com/tomchen/example_pypi_package
```

### Comparing `simple_sqs_client-0.9.3/setup.py` & `simple_sqs_client-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `simple_sqs_client-0.9.3/src/simple_sqs_client/builder.py` & `simple_sqs_client-0.9.4/src/simple_sqs_client/builder.py`

 * *Files identical despite different names*

### Comparing `simple_sqs_client-0.9.3/src/simple_sqs_client/client.py` & `simple_sqs_client-0.9.4/src/simple_sqs_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         if self.sqs is not None:
             self.sqs.close()
 
     def _init_client(self):
         """
         Initializes the SQS client using the specified AWS credentials and region.
         """
-        self.sqs = boto3.client('simple_sqs_client', region_name=self.region_name,
+        self.sqs = boto3.client('sqs', region_name=self.region_name,
                                 aws_access_key_id=self.aws_access_key_id,
                                 aws_secret_access_key=self.aws_secret_access_key)
 
     def send_message(self, body: str) -> dict:
         """
         Sends a message to the SQS queue.
```

### Comparing `simple_sqs_client-0.9.3/src/simple_sqs_client/test_client.py` & `simple_sqs_client-0.9.4/src/simple_sqs_client/test_client.py`

 * *Files identical despite different names*

### Comparing `simple_sqs_client-0.9.3/src/simple_sqs_client.egg-info/PKG-INFO` & `simple_sqs_client-0.9.4/src/simple_sqs_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-sqs-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Very simple SQS Client
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Aleksander Laurowski
 Author-email: aleksander.laurowski191@gmail.com
 Project-URL: Documentation, https://github.com/tomchen/example_pypi_package
 Project-URL: Bug Reports, https://github.com/tomchen/example_pypi_package/issues
 Project-URL: Source Code, https://github.com/tomchen/example_pypi_package
```

### Comparing `simple_sqs_client-0.9.3/tests/test_client.py` & `simple_sqs_client-0.9.4/tests/test_client.py`

 * *Files identical despite different names*

