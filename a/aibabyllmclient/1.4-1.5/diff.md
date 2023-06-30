# Comparing `tmp/aibabyllmclient-1.4.tar.gz` & `tmp/aibabyllmclient-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibabyllmclient-1.4.tar", last modified: Fri Jun 30 02:51:37 2023, max compression
+gzip compressed data, was "aibabyllmclient-1.5.tar", last modified: Fri Jun 30 02:53:30 2023, max compression
```

## Comparing `aibabyllmclient-1.4.tar` & `aibabyllmclient-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/PKG-INFO
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/aibabyllmclient/
--rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.4/aibabyllmclient/__init__.py
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/aibabyllmclient/core/
--rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.4/aibabyllmclient/core/__init__.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     5412 2023-06-09 07:57:58.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_code_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)    40871 2023-06-09 07:57:58.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_core_meta_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_media_llm_req_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_media_llm_res_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)    41098 2023-06-30 02:51:09.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_service_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     7838 2023-06-30 02:51:09.000000 aibabyllmclient-1.4/aibabyllmclient/core/tongos_service_pb2_grpc.py
--rw-rw-r--   0 zh        (1000) zh        (1000)     3316 2023-06-30 02:46:32.000000 aibabyllmclient-1.4/aibabyllmclient/llmserver_call.py
--rw-rw-r--   0 zh        (1000) zh        (1000)      619 2023-06-30 02:47:53.000000 aibabyllmclient-1.4/aibabyllmclient/main.py
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/aibabyllmclient.egg-info/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:51:37.000000 aibabyllmclient-1.4/aibabyllmclient.egg-info/PKG-INFO
--rw-rw-r--   0 zh        (1000) zh        (1000)      557 2023-06-30 02:51:37.000000 aibabyllmclient-1.4/aibabyllmclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 02:51:37.000000 aibabyllmclient-1.4/aibabyllmclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)       16 2023-06-30 02:51:37.000000 aibabyllmclient-1.4/aibabyllmclient.egg-info/top_level.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 02:51:37.733889 aibabyllmclient-1.4/setup.cfg
--rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 02:51:22.000000 aibabyllmclient-1.4/setup.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:53:30.199517 aibabyllmclient-1.5/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:53:30.199517 aibabyllmclient-1.5/PKG-INFO
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:53:30.195516 aibabyllmclient-1.5/aibabyllmclient/
+-rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.5/aibabyllmclient/__init__.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:53:30.199517 aibabyllmclient-1.5/aibabyllmclient/core/
+-rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.5/aibabyllmclient/core/__init__.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     5412 2023-06-09 07:57:58.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_code_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)    40871 2023-06-09 07:57:58.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_core_meta_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_media_llm_req_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_media_llm_res_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)    41098 2023-06-30 02:51:09.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_service_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     7838 2023-06-30 02:51:09.000000 aibabyllmclient-1.5/aibabyllmclient/core/tongos_service_pb2_grpc.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)     3348 2023-06-30 02:53:14.000000 aibabyllmclient-1.5/aibabyllmclient/llmserver_call.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)      619 2023-06-30 02:47:53.000000 aibabyllmclient-1.5/aibabyllmclient/main.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:53:30.195516 aibabyllmclient-1.5/aibabyllmclient.egg-info/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:53:30.000000 aibabyllmclient-1.5/aibabyllmclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zh        (1000) zh        (1000)      557 2023-06-30 02:53:30.000000 aibabyllmclient-1.5/aibabyllmclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 02:53:30.000000 aibabyllmclient-1.5/aibabyllmclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       16 2023-06-30 02:53:30.000000 aibabyllmclient-1.5/aibabyllmclient.egg-info/top_level.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 02:53:30.199517 aibabyllmclient-1.5/setup.cfg
+-rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 02:53:29.000000 aibabyllmclient-1.5/setup.py
```

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_code_pb2.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_code_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_core_meta_pb2.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_core_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_media_llm_req_pb2.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_media_llm_req_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_media_llm_res_pb2.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_media_llm_res_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_service_pb2.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_service_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/core/tongos_service_pb2_grpc.py` & `aibabyllmclient-1.5/aibabyllmclient/core/tongos_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient/llmserver_call.py` & `aibabyllmclient-1.5/aibabyllmclient/llmserver_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from google.protobuf import any_pb2
 from aibabyllmclient.core import (
     tongos_core_meta_pb2,
     tongos_service_pb2,
     tongos_service_pb2_grpc,
 )
 
-from core import tongos_media_llm_req_pb2
-from core import tongos_media_llm_res_pb2
+from aibabyllmclient.core import tongos_media_llm_req_pb2
+from aibabyllmclient.core import tongos_media_llm_res_pb2
 
 
 # from private_protocol.tongos_protocol.media.vision import tongos_media_cv_pb2
 
 
 def got_packet(ts: int, prompt):
     # pg
```

### Comparing `aibabyllmclient-1.4/aibabyllmclient/main.py` & `aibabyllmclient-1.5/aibabyllmclient/main.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.4/aibabyllmclient.egg-info/SOURCES.txt` & `aibabyllmclient-1.5/aibabyllmclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

