# Comparing `tmp/th2_grpc_act_template-4.0.1.tar.gz` & `tmp/th2_grpc_act_template-4.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_template-4.0.1.tar", last modified: Fri Jun 30 13:57:57 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_template-4.0.1.dev0.tar", last modified: Wed Mar  1 09:09:56 2023, max compression
```

## Comparing `th2_grpc_act_template-4.0.1.tar` & `th2_grpc_act_template-4.0.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-06-30 13:57:07.000000 th2_grpc_act_template-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-30 13:57:07.000000 th2_grpc_act_template-4.0.1/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-30 13:57:07.000000 th2_grpc_act_template-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-30 13:57:39.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-06-30 13:57:07.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-30 13:57:57.000000 th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-03-01 09:09:37.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-01 09:09:07.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-01 09:09:55.000000 th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_template-4.0.1/PKG-INFO` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_act_template
-Version: 4.0.1
+Name: th2-grpc-act-template
+Version: 4.0.1.dev0
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
         
@@ -55,26 +55,22 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.0.1
+        + Dependency check pipeline step added
+        
         ### 4.0.0
         
-        + Update to `th2-grpc-common` version `4.0.0`
+        + Update to `th2-grpc-common` version `4.2.0`
         + Marked deprecated fields as `reserved`
         
-        ### 3.12.0
-        + grpc version bump to `1.48.2`
-        + protobuf version bump to `3.21.7`
-        + serviceGenerator version bump to `3.3.1`
-        + Add dependency check pipeline step.
-        + Add dev-release workflow.
-        
         ### 3.11.0
         
         + Add `multiSendMessage` method for sending several messages at once
         
         ### 3.10.0
         
         + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
```

### Comparing `th2_grpc_act_template-4.0.1/README.md` & `th2_grpc_act_template-4.0.1.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,26 +47,22 @@
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 4.0.1
++ Dependency check pipeline step added
+
 ### 4.0.0
 
-+ Update to `th2-grpc-common` version `4.0.0`
++ Update to `th2-grpc-common` version `4.2.0`
 + Marked deprecated fields as `reserved`
 
-### 3.12.0
-+ grpc version bump to `1.48.2`
-+ protobuf version bump to `3.21.7`
-+ serviceGenerator version bump to `3.3.1`
-+ Add dependency check pipeline step.
-+ Add dev-release workflow.
-
 ### 3.11.0
 
 + Add `multiSendMessage` method for sending several messages at once
 
 ### 3.10.0
 
 + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
```

### Comparing `th2_grpc_act_template-4.0.1/setup.py` & `th2_grpc_act_template-4.0.1.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     long_description_content_type='text/markdown',
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-grpc-act-template',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
-        'th2-grpc-common>=4.2.0,<5',
+        'th2-grpc-common==4.1.0.dev4105266708',
         'mypy-protobuf==3.2'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
```

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_service.py` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template.proto` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2.py` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2.pyi` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template/act_template_pb2_grpc.py` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template/act_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/PKG-INFO` & `th2_grpc_act_template-4.0.1.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-act-template
-Version: 4.0.1
+Name: th2_grpc_act_template
+Version: 4.0.1.dev0
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
         
@@ -55,26 +55,22 @@
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.0.1
+        + Dependency check pipeline step added
+        
         ### 4.0.0
         
-        + Update to `th2-grpc-common` version `4.0.0`
+        + Update to `th2-grpc-common` version `4.2.0`
         + Marked deprecated fields as `reserved`
         
-        ### 3.12.0
-        + grpc version bump to `1.48.2`
-        + protobuf version bump to `3.21.7`
-        + serviceGenerator version bump to `3.3.1`
-        + Add dependency check pipeline step.
-        + Add dev-release workflow.
-        
         ### 3.11.0
         
         + Add `multiSendMessage` method for sending several messages at once
         
         ### 3.10.0
         
         + Add `placeOrderCancelReplaceRequest` method for sending `OrderCancelReplaceRequest`
```

### Comparing `th2_grpc_act_template-4.0.1/th2_grpc_act_template.egg-info/SOURCES.txt` & `th2_grpc_act_template-4.0.1.dev0/th2_grpc_act_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

