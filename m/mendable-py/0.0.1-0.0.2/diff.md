# Comparing `tmp/mendable-py-0.0.1.tar.gz` & `tmp/mendable-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mendable-py-0.0.1.tar", last modified: Thu Jun 29 15:10:31 2023, max compression
+gzip compressed data, was "mendable-py-0.0.2.tar", last modified: Fri Jun 30 12:59:23 2023, max compression
```

## Comparing `mendable-py-0.0.1.tar` & `mendable-py-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-29 15:10:31.000000 mendable-py-0.0.1/
--rw-r--r--   0 ericciarla   (501) staff       (20)      251 2023-06-29 15:10:31.000000 mendable-py-0.0.1/PKG-INFO
--rw-r--r--   0 ericciarla   (501) staff       (20)      993 2023-06-29 15:10:08.000000 mendable-py-0.0.1/README.md
-drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable/
--rw-r--r--   0 ericciarla   (501) staff       (20)       29 2023-06-29 13:59:24.000000 mendable-py-0.0.1/mendable/__init__.py
--rw-r--r--   0 ericciarla   (501) staff       (20)     2554 2023-06-29 13:59:13.000000 mendable-py-0.0.1/mendable/chatapp.py
-drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/
--rw-r--r--   0 ericciarla   (501) staff       (20)      251 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/PKG-INFO
--rw-r--r--   0 ericciarla   (501) staff       (20)      233 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/SOURCES.txt
--rw-r--r--   0 ericciarla   (501) staff       (20)        1 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/dependency_links.txt
--rw-r--r--   0 ericciarla   (501) staff       (20)        9 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/requires.txt
--rw-r--r--   0 ericciarla   (501) staff       (20)        9 2023-06-29 15:10:31.000000 mendable-py-0.0.1/mendable_py.egg-info/top_level.txt
--rw-r--r--   0 ericciarla   (501) staff       (20)       38 2023-06-29 15:10:31.000000 mendable-py-0.0.1/setup.cfg
--rw-r--r--   0 ericciarla   (501) staff       (20)      345 2023-06-29 14:00:21.000000 mendable-py-0.0.1/setup.py
+drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-30 12:59:23.982113 mendable-py-0.0.2/
+-rw-r--r--   0 ericciarla   (501) staff       (20)      251 2023-06-30 12:59:23.981972 mendable-py-0.0.2/PKG-INFO
+-rw-r--r--   0 ericciarla   (501) staff       (20)     1350 2023-06-30 12:57:21.000000 mendable-py-0.0.2/README.md
+drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-30 12:59:23.980558 mendable-py-0.0.2/mendable/
+-rw-r--r--   0 ericciarla   (501) staff       (20)       29 2023-06-29 13:59:24.000000 mendable-py-0.0.2/mendable/__init__.py
+-rw-r--r--   0 ericciarla   (501) staff       (20)     2575 2023-06-30 12:54:46.000000 mendable-py-0.0.2/mendable/chatapp.py
+drwxr-xr-x   0 ericciarla   (501) staff       (20)        0 2023-06-30 12:59:23.981749 mendable-py-0.0.2/mendable_py.egg-info/
+-rw-r--r--   0 ericciarla   (501) staff       (20)      251 2023-06-30 12:59:23.000000 mendable-py-0.0.2/mendable_py.egg-info/PKG-INFO
+-rw-r--r--   0 ericciarla   (501) staff       (20)      233 2023-06-30 12:59:23.000000 mendable-py-0.0.2/mendable_py.egg-info/SOURCES.txt
+-rw-r--r--   0 ericciarla   (501) staff       (20)        1 2023-06-30 12:59:23.000000 mendable-py-0.0.2/mendable_py.egg-info/dependency_links.txt
+-rw-r--r--   0 ericciarla   (501) staff       (20)        9 2023-06-30 12:59:23.000000 mendable-py-0.0.2/mendable_py.egg-info/requires.txt
+-rw-r--r--   0 ericciarla   (501) staff       (20)        9 2023-06-30 12:59:23.000000 mendable-py-0.0.2/mendable_py.egg-info/top_level.txt
+-rw-r--r--   0 ericciarla   (501) staff       (20)       38 2023-06-30 12:59:23.982174 mendable-py-0.0.2/setup.cfg
+-rw-r--r--   0 ericciarla   (501) staff       (20)      345 2023-06-30 12:59:07.000000 mendable-py-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mendable-py-0.0.1/mendable/chatapp.py` & `mendable-py-0.0.2/mendable/chatapp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import requests
 import time
 
 class ChatApp:
-    def __init__(self):
-        self.api_key = os.getenv('MENDABLE_API_KEY')
-        self.conversation_id = self._get_new_conversation_id()
-        self.history = []
+    def __init__(self, api_key=None):
+        self.api_key = api_key or os.getenv('MENDABLE_API_KEY')
+        if self.api_key is None:
+            raise ValueError('No API key provided')
 
     def _get_new_conversation_id(self):
         new_conversation_response = requests.post("https://api.mendable.ai/v0/newConversation", json={"api_key": self.api_key}).json()
         if new_conversation_response.get('conversation_id'):
             return new_conversation_response['conversation_id']
         else:
             raise Exception('Failed to create a new conversation')
```

