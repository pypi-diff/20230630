# Comparing `tmp/gpt4-api-0.2.1.tar.gz` & `tmp/gpt4-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.2.1.tar", last modified: Fri Jun 30 06:37:44 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.2.2.tar", last modified: Fri Jun 30 06:52:10 2023, max compression
```

## Comparing `gpt4-api-0.2.1.tar` & `gpt4-api-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.1/api/Logger.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.1/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    10232 2023-06-30 06:37:12.000000 gpt4-api-0.2.1/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-30 06:37:44.000000 gpt4-api-0.2.1/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.1/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.2/api/Logger.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.2/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10236 2023-06-30 06:51:34.000000 gpt4-api-0.2.2/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.2/setup.py
```

### Comparing `gpt4-api-0.2.1/api/Logger.py` & `gpt4-api-0.2.2/api/Logger.py`

 * *Files identical despite different names*

### Comparing `gpt4-api-0.2.1/api/gpt.py` & `gpt4-api-0.2.2/api/gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 import time
 import openai
 import asyncio
 from pathlib import Path
 from multiprocessing import JoinableQueue
 from queue import Empty
-from Logger import Logger
+from api.Logger import Logger
 logging = Logger(__name__)
 
 
 class call_black_parameter(object):
     def __init__(self, response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name):
         self.response_str = response_str
         self.messages = messages
```

### Comparing `gpt4-api-0.2.1/setup.py` & `gpt4-api-0.2.2/setup.py`

 * *Files identical despite different names*

