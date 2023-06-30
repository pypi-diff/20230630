# Comparing `tmp/docuware-client-0.1.0.tar.gz` & `tmp/docuware-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docuware-client-0.1.0.tar", last modified: Tue Feb 22 14:02:54 2022, max compression
+gzip compressed data, was "docuware-client-0.2.0.tar", last modified: Fri Jun 30 15:51:56 2023, max compression
```

## Comparing `docuware-client-0.1.0.tar` & `docuware-client-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-02-22 14:02:54.962056 docuware-client-0.1.0/
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1545 2022-02-22 09:42:25.000000 docuware-client-0.1.0/LICENSE
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5952 2022-02-22 14:02:54.962056 docuware-client-0.1.0/PKG-INFO
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5483 2022-02-22 13:53:21.000000 docuware-client-0.1.0/README.md
-drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-02-22 14:02:54.962056 docuware-client-0.1.0/docuware/
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      174 2022-02-22 09:28:07.000000 docuware-client-0.1.0/docuware/__init__.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     2669 2022-02-21 10:01:15.000000 docuware-client-0.1.0/docuware/cidict.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      824 2022-02-16 15:50:29.000000 docuware-client-0.1.0/docuware/cijson.py
-drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-02-22 14:02:54.962056 docuware-client-0.1.0/docuware/cli/
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-01-20 13:36:16.000000 docuware-client-0.1.0/docuware/cli/__init__.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1761 2022-02-22 08:04:50.000000 docuware-client-0.1.0/docuware/cli/api.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     8732 2022-02-22 10:39:48.000000 docuware-client-0.1.0/docuware/cli/dw.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)    22620 2022-02-22 12:24:16.000000 docuware-client-0.1.0/docuware/client.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     4808 2022-02-21 10:58:18.000000 docuware-client-0.1.0/docuware/conn.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      790 2022-02-17 08:33:50.000000 docuware-client-0.1.0/docuware/errors.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     6207 2022-02-21 13:58:30.000000 docuware-client-0.1.0/docuware/parser.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1802 2022-02-22 09:28:53.000000 docuware-client-0.1.0/docuware/structs.py
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     2522 2022-02-21 10:56:33.000000 docuware-client-0.1.0/docuware/utils.py
-drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-02-22 14:02:54.962056 docuware-client-0.1.0/docuware_client.egg-info/
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5952 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/PKG-INFO
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      497 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/SOURCES.txt
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        1 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/dependency_links.txt
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       52 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/entry_points.txt
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       15 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/requires.txt
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        9 2022-02-22 14:02:54.000000 docuware-client-0.1.0/docuware_client.egg-info/top_level.txt
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       38 2022-02-22 14:02:54.962056 docuware-client-0.1.0/setup.cfg
--rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      809 2022-02-22 09:38:17.000000 docuware-client-0.1.0/setup.py
+drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2023-06-30 15:51:56.329857 docuware-client-0.2.0/
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1545 2022-02-22 09:42:25.000000 docuware-client-0.2.0/LICENSE
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5924 2023-06-30 15:51:56.329857 docuware-client-0.2.0/PKG-INFO
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5474 2022-02-22 17:22:12.000000 docuware-client-0.2.0/README.md
+drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2023-06-30 15:51:56.326524 docuware-client-0.2.0/docuware/
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      174 2022-02-22 09:28:07.000000 docuware-client-0.2.0/docuware/__init__.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     2669 2022-02-21 10:01:15.000000 docuware-client-0.2.0/docuware/cidict.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      824 2022-02-16 15:50:29.000000 docuware-client-0.2.0/docuware/cijson.py
+drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2023-06-30 15:51:56.329857 docuware-client-0.2.0/docuware/cli/
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        0 2022-01-20 13:36:16.000000 docuware-client-0.2.0/docuware/cli/__init__.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1761 2022-02-22 08:04:50.000000 docuware-client-0.2.0/docuware/cli/api.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     8732 2022-02-22 10:39:48.000000 docuware-client-0.2.0/docuware/cli/dw.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)    34957 2023-06-20 18:14:12.000000 docuware-client-0.2.0/docuware/client.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     6191 2023-06-20 18:14:12.000000 docuware-client-0.2.0/docuware/conn.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      790 2022-02-17 08:33:50.000000 docuware-client-0.2.0/docuware/errors.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     6207 2022-02-21 13:58:30.000000 docuware-client-0.2.0/docuware/parser.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     1802 2022-02-22 09:28:53.000000 docuware-client-0.2.0/docuware/structs.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     2522 2022-02-21 10:56:33.000000 docuware-client-0.2.0/docuware/utils.py
+drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2023-06-30 15:51:56.329857 docuware-client-0.2.0/docuware_client.egg-info/
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     5924 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/PKG-INFO
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      563 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/SOURCES.txt
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        1 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/dependency_links.txt
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       51 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/entry_points.txt
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       15 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/requires.txt
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)        9 2023-06-30 15:51:56.000000 docuware-client-0.2.0/docuware_client.egg-info/top_level.txt
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)       38 2023-06-30 15:51:56.329857 docuware-client-0.2.0/setup.cfg
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      809 2023-06-30 15:46:37.000000 docuware-client-0.2.0/setup.py
+drwxr-xr-x   0 sschoenberger  (1000) sschoenberger  (1000)        0 2023-06-30 15:51:56.329857 docuware-client-0.2.0/tests/
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)      691 2022-02-17 13:06:59.000000 docuware-client-0.2.0/tests/test_datetime.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     4178 2022-02-21 13:51:27.000000 docuware-client-0.2.0/tests/test_parser.py
+-rw-r--r--   0 sschoenberger  (1000) sschoenberger  (1000)     2066 2022-02-17 12:48:57.000000 docuware-client-0.2.0/tests/test_structs.py
```

### Comparing `docuware-client-0.1.0/LICENSE` & `docuware-client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/PKG-INFO` & `docuware-client-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: docuware-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: DocuWare REST-API client
 Home-page: https://github.com/sniner/docuware-client
 Author: Stefan Schönberger
 Author-email: mail@sniner.dev
-License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -188,28 +187,26 @@
 ```console
 $ dw-client list --file-cabinet Archive
 ```
 
 You can also display a (partial) selection of the contents of individual fields:
 
 ```console
-$ dw-client list --file-cabinet Archive --dialog custom --field DocNo(partial) 
+$ dw-client list --file-cabinet Archive --dialog custom --field DocNo
 ```
 
 
 ## Further reading
 
 * Entry point to [DocuWare's official documentation][2] of the REST API.
-* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf
+* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf`
 
 
 ## License
 
 This work is released under the BSD 3 license. You may use and redistribute this software as long as the copyright
 notice is preserved.
 
 
 [1]: https://docuware.com/
 [2]: https://developer.docuware.com/rest/index.html
 
-
-
```

### Comparing `docuware-client-0.1.0/README.md` & `docuware-client-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -172,22 +172,22 @@
 ```console
 $ dw-client list --file-cabinet Archive
 ```
 
 You can also display a (partial) selection of the contents of individual fields:
 
 ```console
-$ dw-client list --file-cabinet Archive --dialog custom --field DocNo(partial) 
+$ dw-client list --file-cabinet Archive --dialog custom --field DocNo
 ```
 
 
 ## Further reading
 
 * Entry point to [DocuWare's official documentation][2] of the REST API.
-* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf
+* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf`
 
 
 ## License
 
 This work is released under the BSD 3 license. You may use and redistribute this software as long as the copyright
 notice is preserved.
```

### Comparing `docuware-client-0.1.0/docuware/cidict.py` & `docuware-client-0.2.0/docuware/cidict.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/cijson.py` & `docuware-client-0.2.0/docuware/cijson.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/cli/api.py` & `docuware-client-0.2.0/docuware/cli/api.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/cli/dw.py` & `docuware-client-0.2.0/docuware/cli/dw.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/errors.py` & `docuware-client-0.2.0/docuware/errors.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/parser.py` & `docuware-client-0.2.0/docuware/parser.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/structs.py` & `docuware-client-0.2.0/docuware/structs.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware/utils.py` & `docuware-client-0.2.0/docuware/utils.py`

 * *Files identical despite different names*

### Comparing `docuware-client-0.1.0/docuware_client.egg-info/PKG-INFO` & `docuware-client-0.2.0/docuware_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: docuware-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: DocuWare REST-API client
 Home-page: https://github.com/sniner/docuware-client
 Author: Stefan Schönberger
 Author-email: mail@sniner.dev
-License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -188,28 +187,26 @@
 ```console
 $ dw-client list --file-cabinet Archive
 ```
 
 You can also display a (partial) selection of the contents of individual fields:
 
 ```console
-$ dw-client list --file-cabinet Archive --dialog custom --field DocNo(partial) 
+$ dw-client list --file-cabinet Archive --dialog custom --field DocNo
 ```
 
 
 ## Further reading
 
 * Entry point to [DocuWare's official documentation][2] of the REST API.
-* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf
+* Notable endpoint: `/DocuWare/Platform/Content/PlatformLinkModel.pdf`
 
 
 ## License
 
 This work is released under the BSD 3 license. You may use and redistribute this software as long as the copyright
 notice is preserved.
 
 
 [1]: https://docuware.com/
 [2]: https://developer.docuware.com/rest/index.html
 
-
-
```

### Comparing `docuware-client-0.1.0/setup.py` & `docuware-client-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "docuware-client",
-    version = "0.1.0",
+    version = "0.2.0",
     description = "DocuWare REST-API client",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/sniner/docuware-client",
     author = "Stefan Schönberger",
     author_email = "mail@sniner.dev",
     install_requires=[
```

