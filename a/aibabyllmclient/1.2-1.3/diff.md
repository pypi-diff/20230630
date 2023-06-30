# Comparing `tmp/aibabyllmclient-1.2.tar.gz` & `tmp/aibabyllmclient-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibabyllmclient-1.2.tar", last modified: Fri Jun 30 02:36:58 2023, max compression
+gzip compressed data, was "aibabyllmclient-1.3.tar", last modified: Fri Jun 30 02:48:22 2023, max compression
```

## Comparing `aibabyllmclient-1.2.tar` & `aibabyllmclient-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/PKG-INFO
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/aibabyllmclient/
--rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.2/aibabyllmclient/__init__.py
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/aibabyllmclient/core/
--rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.2/aibabyllmclient/core/__init__.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     5412 2023-06-09 07:57:58.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_code_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)    40871 2023-06-09 07:57:58.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_core_meta_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_media_llm_req_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_media_llm_res_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)    41066 2023-06-09 07:57:58.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_service_pb2.py
--rwxrwxr-x   0 zh        (1000) zh        (1000)     7822 2023-06-09 07:57:59.000000 aibabyllmclient-1.2/aibabyllmclient/core/tongos_service_pb2_grpc.py
--rw-rw-r--   0 zh        (1000) zh        (1000)     3300 2023-06-30 01:35:46.000000 aibabyllmclient-1.2/aibabyllmclient/llmserver_call.py
--rw-rw-r--   0 zh        (1000) zh        (1000)      603 2023-06-30 01:36:24.000000 aibabyllmclient-1.2/aibabyllmclient/main.py
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/aibabyllmclient.egg-info/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:36:58.000000 aibabyllmclient-1.2/aibabyllmclient.egg-info/PKG-INFO
--rw-rw-r--   0 zh        (1000) zh        (1000)      557 2023-06-30 02:36:58.000000 aibabyllmclient-1.2/aibabyllmclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 02:36:58.000000 aibabyllmclient-1.2/aibabyllmclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)       16 2023-06-30 02:36:58.000000 aibabyllmclient-1.2/aibabyllmclient.egg-info/top_level.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 02:36:58.797560 aibabyllmclient-1.2/setup.cfg
--rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 02:36:47.000000 aibabyllmclient-1.2/setup.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/PKG-INFO
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/aibabyllmclient/
+-rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.3/aibabyllmclient/__init__.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/aibabyllmclient/core/
+-rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.3/aibabyllmclient/core/__init__.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     5412 2023-06-09 07:57:58.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_code_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)    40871 2023-06-09 07:57:58.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_core_meta_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_media_llm_req_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     3378 2023-06-09 07:57:59.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_media_llm_res_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)    41066 2023-06-09 07:57:58.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_service_pb2.py
+-rwxrwxr-x   0 zh        (1000) zh        (1000)     7822 2023-06-09 07:57:59.000000 aibabyllmclient-1.3/aibabyllmclient/core/tongos_service_pb2_grpc.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)     3316 2023-06-30 02:46:32.000000 aibabyllmclient-1.3/aibabyllmclient/llmserver_call.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)      619 2023-06-30 02:47:53.000000 aibabyllmclient-1.3/aibabyllmclient/main.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/aibabyllmclient.egg-info/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:48:22.000000 aibabyllmclient-1.3/aibabyllmclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zh        (1000) zh        (1000)      557 2023-06-30 02:48:22.000000 aibabyllmclient-1.3/aibabyllmclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 02:48:22.000000 aibabyllmclient-1.3/aibabyllmclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       16 2023-06-30 02:48:22.000000 aibabyllmclient-1.3/aibabyllmclient.egg-info/top_level.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 02:48:22.254967 aibabyllmclient-1.3/setup.cfg
+-rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 02:48:18.000000 aibabyllmclient-1.3/setup.py
```

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_code_pb2.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_code_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_core_meta_pb2.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_core_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_media_llm_req_pb2.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_media_llm_req_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_media_llm_res_pb2.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_media_llm_res_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_service_pb2.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_service_pb2.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/core/tongos_service_pb2_grpc.py` & `aibabyllmclient-1.3/aibabyllmclient/core/tongos_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aibabyllmclient-1.2/aibabyllmclient/llmserver_call.py` & `aibabyllmclient-1.3/aibabyllmclient/llmserver_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import base64
 import json
 import logging
 import time
 import grpc
 import numpy as np
 from google.protobuf import any_pb2
-from core import (
+from aibabyllmclient.core import (
     tongos_core_meta_pb2,
     tongos_service_pb2,
     tongos_service_pb2_grpc,
 )
 
 from core import tongos_media_llm_req_pb2
 from core import tongos_media_llm_res_pb2
```

### Comparing `aibabyllmclient-1.2/aibabyllmclient/main.py` & `aibabyllmclient-1.3/aibabyllmclient/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This is a sample Python script.
 
 # Press Shift+F10 to execute it or replace it with your code.
 # Press Double Shift to search everywhere for classes, files, tool windows, actions, and settings.
-from llmserver_call import call_llmserver
+from aibabyllmclient.llmserver_call import call_llmserver
 
 
 def print_hi(name):
     # Use a breakpoint in the code line below to debug your script.
     print(f'Hi, {name}')  # Press Ctrl+F8 to toggle the breakpoint.
```

### Comparing `aibabyllmclient-1.2/aibabyllmclient.egg-info/SOURCES.txt` & `aibabyllmclient-1.3/aibabyllmclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

