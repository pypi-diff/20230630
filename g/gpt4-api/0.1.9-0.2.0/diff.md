# Comparing `tmp/gpt4-api-0.1.9.tar.gz` & `tmp/gpt4-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.1.9.tar", last modified: Mon Jun 12 07:30:24 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.2.0.tar", last modified: Thu Jun 29 09:16:26 2023, max compression
```

## Comparing `gpt4-api-0.1.9.tar` & `gpt4-api-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.1.9/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    10470 2023-06-12 07:29:22.000000 gpt4-api-0.1.9/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-12 07:30:24.000000 gpt4-api-0.1.9/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.1.9/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-29 09:16:26.000000 gpt4-api-0.2.0/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-29 09:16:26.000000 gpt4-api-0.2.0/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-29 09:16:26.000000 gpt4-api-0.2.0/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.0/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10553 2023-06-29 09:15:31.000000 gpt4-api-0.2.0/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-29 09:16:26.000000 gpt4-api-0.2.0/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-29 09:16:25.000000 gpt4-api-0.2.0/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-06-29 09:16:25.000000 gpt4-api-0.2.0/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-29 09:16:25.000000 gpt4-api-0.2.0/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-29 09:16:25.000000 gpt4-api-0.2.0/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-29 09:16:25.000000 gpt4-api-0.2.0/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-29 09:16:26.000000 gpt4-api-0.2.0/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.0/setup.py
```

### Comparing `gpt4-api-0.1.9/api/gpt.py` & `gpt4-api-0.2.0/api/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import time
 import openai
 import asyncio
 from pathlib import Path
 from multiprocessing import JoinableQueue
 from queue import Empty
 
-logging.basicConfig(filename='gpt.log', level=logging.INFO, format='%(asctime)s %(levelname)s: %(message)s')
-console_handler = logging.StreamHandler()
-console_handler.setLevel(logging.INFO)
-console_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s: %(message)s'))
-logging = logging.getLogger()
-logging.addHandler(console_handler)
+# logging.basicConfig(filename='gpt.log', level=logging.INFO, format='%(asctime)s %(levelname)s: %(message)s')
+# console_handler = logging.StreamHandler()
+# console_handler.setLevel(logging.INFO)
+# console_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s: %(message)s'))
+# logging = logging.getLogger()
+# logging.addHandler(console_handler)
 
 
 class call_black_parameter(object):
     def __init__(self, response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name):
         self.response_str = response_str
         self.messages = messages
         self.elapsed_time = elapsed_time
@@ -33,14 +33,15 @@
         self.max_retries = max_retries
         self.task_queue = JoinableQueue()
         self.key_lock = threading.Lock()
         self.usable_openai_keys = self.process_token(keys=keys)
         self.key_limit = key_limit
         # 模型
         self.model = model
+        logging.info(f"use model: {model} temperature: {temperature}")
         # 用于控制生成文本的随机性和创造性的参数。值越高，生成文本越随机和创造性；值越低，生成文本越可预测和保守
         self.temperature = temperature
         # 用于对生成文本进行选择的参数，它表示只选择所有可能的令牌中累计概率高于给定阈值的那些令牌。默认值为1，表示选择所有可能的令牌
         self.top_p = top_p
         # 用于惩罚生成文本中未出现过的片段的参数。默认值为0，表示不进行惩罚
         self.presence_penalty = presence_penalty
         # 用于惩罚生成文本中频繁出现的重复片段的参数。默认值为0，表示不进行惩罚
```

### Comparing `gpt4-api-0.1.9/setup.py` & `gpt4-api-0.2.0/setup.py`

 * *Files identical despite different names*

