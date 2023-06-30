# Comparing `tmp/herdmod-0.1.0.tar.gz` & `tmp/herdmod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.1.0.tar", last modified: Fri Jun 30 14:46:29 2023, max compression
+gzip compressed data, was "herdmod-0.1.1.tar", last modified: Fri Jun 30 15:52:49 2023, max compression
```

## Comparing `herdmod-0.1.0.tar` & `herdmod-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.782374 herdmod-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 14:46:19.000000 herdmod-0.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 14:46:19.000000 herdmod-0.1.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 14:46:19.000000 herdmod-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 14:46:29.782374 herdmod-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-30 14:46:19.000000 herdmod-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.778375 herdmod-0.1.0/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.782374 herdmod-0.1.0/herdmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.782374 herdmod-0.1.0/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.782374 herdmod-0.1.0/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.782374 herdmod-0.1.0/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-30 14:46:19.000000 herdmod-0.1.0/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:46:29.778375 herdmod-0.1.0/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 14:46:29.000000 herdmod-0.1.0/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 14:46:29.000000 herdmod-0.1.0/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:46:29.000000 herdmod-0.1.0/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 14:46:29.000000 herdmod-0.1.0/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:46:29.000000 herdmod-0.1.0/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:46:29.782374 herdmod-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 14:46:19.000000 herdmod-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.415645 herdmod-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 15:52:33.000000 herdmod-0.1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 15:52:33.000000 herdmod-0.1.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 15:52:33.000000 herdmod-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 15:52:49.411645 herdmod-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-30 15:52:33.000000 herdmod-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:52:49.415645 herdmod-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 15:52:33.000000 herdmod-0.1.1/setup.py
```

### Comparing `herdmod-0.1.0/COPYING` & `herdmod-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.0/COPYING.lesser` & `herdmod-0.1.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.0/NOTICE` & `herdmod-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.0/PKG-INFO` & `herdmod-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.1.0
+Version: 0.1.1
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.1.0/README.md` & `herdmod-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.0/herdmod/helpers/helpers.py` & `herdmod-0.1.1/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.0/herdmod/listen/listen.py` & `herdmod-0.1.1/herdmod/listen/listen.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class ListenerCanceled(Exception):
     pass
 
 pyroherd.errors.ListenerCanceled = ListenerCanceled
 
 
 @patch(pyroherd.client.Client)
-class Client():
+class Client:
     @patchable
     def __init__(self, *args, **kwargs):
         self.listening = {}
         self.using_mod = True
         
         self.old__init__(*args, **kwargs)
     
@@ -54,16 +54,47 @@
         if not listener or listener['future'].done():
             return
         
         listener['future'].set_exception(ListenerCanceled())
         self.clear_listener(chat_id, listener['future'])
 
 
+@patch(pyroherd.handlers.callback_query_handler.CallbackQueryHandler)
+class CallbackQueryHandler:
+    @patchable
+    def __init__(self, callback: callable, filters=None):
+        self.user_callback = callback
+        self.old__init__(self.resolve_listener, filters)
+    
+    @patchable
+    async def resolve_listener(self, client, query, *args):
+        listener = client.listening.get(query.message.chat.id)
+        if listener and not listener['future'].done():
+            listener['future'].set_result(message)
+        else:
+            if listener and listener['future'].done():
+                client.clear_listener(query.message.chat.id, listener['future'])
+            await self.user_callback(client, query, *args)
+    
+    @patchable
+    async def check(self, client, query):
+        listener = client.listening.get(query.message.chat.id)
+        
+        if listener and not listener['future'].done():
+            return await listener['filters'](client, query) if callable(listener['filters']) else True
+            
+        return (
+            await self.filters(client, query)
+            if callable(self.filters)
+            else True
+        )
+
+
 @patch(pyroherd.handlers.message_handler.MessageHandler)
-class MessageHandler():
+class MessageHandler:
     @patchable
     def __init__(self, callback: callable, filters=None):
         self.user_callback = callback
         self.old__init__(self.resolve_listener, filters)
     
     @patchable
     async def resolve_listener(self, client, message, *args):
@@ -72,27 +103,42 @@
             listener['future'].set_result(message)
         else:
             if listener and listener['future'].done():
                 client.clear_listener(message.chat.id, listener['future'])
             await self.user_callback(client, message, *args)
     
     @patchable
-    async def check(self, client, update):
-        listener = client.listening.get(update.chat.id)
+    async def check(self, client, message):
+        listener = client.listening.get(message.chat.id)
         
         if listener and not listener['future'].done():
-            return await listener['filters'](client, update) if callable(listener['filters']) else True
+            return await listener['filters'](client, message) if callable(listener['filters']) else True
             
         return (
-            await self.filters(client, update)
+            await self.filters(client, message)
             if callable(self.filters)
             else True
         )
 
 
+@patch(pyroherd.types.bots_and_keyboards.callback_query.CallbackQuery)
+class CallbackQuery(pyroherd.types.CallbackQuery):
+    @patchable
+    def listen(self, *args, **kwargs):
+        return self._client.listen(self.message.chat.id, *args, **kwargs)
+
+    @patchable
+    def ask(self, *args, **kwargs):
+        return self._client.ask(self.message.chat.id, *args, **kwargs)
+
+    @patchable
+    def cancel_listener(self):
+        return self._client.cancel_listener(self.message.chat.id)
+
+
 @patch(pyroherd.types.messages_and_media.message.Message)
 class Message(pyroherd.types.Message):
     @patchable
     def listen(self, *args, **kwargs):
         return self._client.listen(self.chat.id, *args, **kwargs)
 
     @patchable
```

### Comparing `herdmod-0.1.0/herdmod.egg-info/PKG-INFO` & `herdmod-0.1.1/herdmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.1.0
+Version: 0.1.1
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.1.0/setup.py` & `herdmod-0.1.1/setup.py`

 * *Files identical despite different names*

