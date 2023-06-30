# Comparing `tmp/amplify_aws_utils-0.4.2.tar.gz` & `tmp/amplify_aws_utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amplify_aws_utils-0.4.2.tar", last modified: Wed Mar 15 14:27:36 2023, max compression
+gzip compressed data, was "dist/amplify_aws_utils-0.4.3.tar", last modified: Fri Jun 30 16:08:13 2023, max compression
```

## Comparing `amplify_aws_utils-0.4.2.tar` & `amplify_aws_utils-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (116)       80 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3933 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2759 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/
--rw-r--r--   0 runner    (1001) docker     (116)       92 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1335 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2707 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/ec2.py
--rw-r--r--   0 runner    (1001) docker     (116)     8902 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (116)     9498 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/spotinst.py
--rw-r--r--   0 runner    (1001) docker     (116)     2295 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/clients/sts.py
--rw-r--r--   0 runner    (1001) docker     (116)      575 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/jitter.py
--rw-r--r--   0 runner    (1001) docker     (116)    15789 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/resource_helper.py
--rw-r--r--   0 runner    (1001) docker     (116)     1122 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/s3_uri.py
--rw-r--r--   0 runner    (1001) docker     (116)      127 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/amplify_aws_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3933 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      707 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      261 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      432 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/requirements.pip
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-15 14:27:36.000000 amplify_aws_utils-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2199 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      268 2023-03-15 14:27:35.000000 amplify_aws_utils-0.4.2/test-requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/spotinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/clients/sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/resource_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/s3_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 16:08:12.000000 amplify_aws_utils-0.4.3/amplify_aws_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/requirements.pip
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:08:13.000000 amplify_aws_utils-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 16:08:11.000000 amplify_aws_utils-0.4.3/test-requirements.pip
```

### Comparing `amplify_aws_utils-0.4.2/PKG-INFO` & `amplify_aws_utils-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: amplify_aws_utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Utility functions for working with AWS resources
 Home-page: https://github.com/amplify-education/amplify_aws_utils/
 Author: Amplify Education
 Author-email: astronauts.core@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Grade)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Coverage)
```

### Comparing `amplify_aws_utils-0.4.2/README.md` & `amplify_aws_utils-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/clients/config.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/config.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/clients/ec2.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/ec2.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/clients/s3.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,7 +250,31 @@
         throttled_call(
             self.s3.copy_object,
             Bucket=destination_bucket,
             Key=destination_key,
             CopySource={"Bucket": source_bucket, "Key": source_key},
             **kwargs
         )
+
+    def copy(
+            self,
+            source_bucket: str,
+            destination_bucket: str,
+            source_key: str,
+            destination_key: str,
+            **kwargs
+    ):
+        """
+        Convenience function for copying an S3 object from one bucket to another with multipart uplaod.
+        :param source_bucket: Name of the source bucket.
+        :param destination_bucket: Name of the destination bucket.
+        :param source_key: Name of the source object.
+        :param destination_key: Name of the destination object.
+        :param kwargs: Any additional arguments to pass to the underlying boto call.
+        """
+        throttled_call(
+            self.s3.copy,
+            Bucket=destination_bucket,
+            Key=destination_key,
+            CopySource={"Bucket": source_bucket, "Key": source_key},
+            **kwargs
+        )
```

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/clients/spotinst.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/spotinst.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/clients/sts.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/clients/sts.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/exceptions.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/jitter.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/jitter.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/resource_helper.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/resource_helper.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils/s3_uri.py` & `amplify_aws_utils-0.4.3/amplify_aws_utils/s3_uri.py`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/PKG-INFO` & `amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: amplify-aws-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Utility functions for working with AWS resources
 Home-page: https://github.com/amplify-education/amplify_aws_utils/
 Author: Amplify Education
 Author-email: astronauts.core@amplify.com
 License: MIT
 Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Grade)
         [![Codacy Badge](https://api.codacy.com/project/badge/Coverage/9f6400386de74fe0b86acd6a081f3302)](https://www.codacy.com/app/amplify-education/amplify_aws_utils?utm_source=github.com&utm_medium=referral&utm_content=amplify-education/amplify_aws_utils&utm_campaign=Badge_Coverage)
```

### Comparing `amplify_aws_utils-0.4.2/amplify_aws_utils.egg-info/SOURCES.txt` & `amplify_aws_utils-0.4.3/amplify_aws_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amplify_aws_utils-0.4.2/setup.py` & `amplify_aws_utils-0.4.3/setup.py`

 * *Files identical despite different names*

