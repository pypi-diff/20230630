# Comparing `tmp/herdmod-0.0.2.tar.gz` & `tmp/herdmod-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.0.2.tar", last modified: Fri Jun 30 12:03:52 2023, max compression
+gzip compressed data, was "herdmod-0.0.3.tar", last modified: Fri Jun 30 12:21:53 2023, max compression
```

## Comparing `herdmod-0.0.2.tar` & `herdmod-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 12:03:39.000000 herdmod-0.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 12:03:39.000000 herdmod-0.0.2/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 12:03:39.000000 herdmod-0.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:03:52.878147 herdmod-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 12:03:39.000000 herdmod-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/nav/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/nav/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:03:52.878147 herdmod-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 12:03:39.000000 herdmod-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 12:21:40.000000 herdmod-0.0.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 12:21:40.000000 herdmod-0.0.3/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 12:21:40.000000 herdmod-0.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:21:53.360037 herdmod-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 12:21:40.000000 herdmod-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/nav/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 12:21:40.000000 herdmod-0.0.3/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:21:53.360037 herdmod-0.0.3/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:21:53.000000 herdmod-0.0.3/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 12:21:53.000000 herdmod-0.0.3/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:21:53.000000 herdmod-0.0.3/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 12:21:53.000000 herdmod-0.0.3/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 12:21:53.000000 herdmod-0.0.3/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:21:53.360037 herdmod-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 12:21:40.000000 herdmod-0.0.3/setup.py
```

### Comparing `herdmod-0.0.2/COPYING` & `herdmod-0.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/COPYING.lesser` & `herdmod-0.0.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/NOTICE` & `herdmod-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/PKG-INFO` & `herdmod-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.0.2/README.md` & `herdmod-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/herdmod/helpers/helpers.py` & `herdmod-0.0.3/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/herdmod/listen/listen.py` & `herdmod-0.0.3/herdmod/listen/listen.py`

 * *Files 10% similar despite different names*

```diff
@@ -288,57 +288,26 @@
             listener_type=ListenerTypes.CALLBACK_QUERY,
             timeout=timeout,
             filters=filters,
             unallowed_click_alert=alert,
         )
 
     @patchable
-    def listen(self, *args, **kwargs):
-        return self._client.listen((self.chat.id, self.from_user.id, self.id), *args, **kwargs)
-
-    @patchable
-    def ask(self, text, *args, **kwargs):
-        return self._client.ask(
-            text, (self.chat.id, self.from_user.id, self.id), *args, **kwargs
-        )
-
-    @patchable
-    def stop_listening(self, *args, **kwargs):
-        return self._client.stop_listening(
-            *args, identifier_pattern=(self.chat.id, self.from_user.id, self.id), **kwargs
-        )
-
-
-@patch(pyroherd.types.user_and_chats.chat.Chat)
-class Chat(pyroherd.types.Chat):
-    @patchable
-    def listen(self, *args, **kwargs):
-        return self._client.listen((self.id, None, None), *args, **kwargs)
-
-    @patchable
-    def ask(self, text, *args, **kwargs):
-        return self._client.ask(text, (self.id, None, None), *args, **kwargs)
-
-    @patchable
-    def stop_listening(self, *args, **kwargs):
-        return self._client.stop_listening(
-            *args, identifier_pattern=(self.id, None, None), **kwargs
+    async def listen(self, *args, **kwargs):
+        return await self._client.listen(
+            (self.chat.id, self.from_user.id, self.id),
+            *args, **kwargs
         )
 
-
-@patch(pyroherd.types.user_and_chats.user.User)
-class User(pyroherd.types.User):
-    @patchable
-    def listen(self, *args, **kwargs):
-        return self._client.listen((None, self.id, None), *args, **kwargs)
-
     @patchable
-    def ask(self, text, *args, **kwargs):
-        return self._client.ask(
-            text, (self.id, self.id, None), *args, **kwargs
+    async def ask(self, text, *args, **kwargs):
+        return await self._client.ask(
+            text, (self.chat.id, self.from_user.id, self.id), *args, **kwargs
         )
 
     @patchable
-    def stop_listening(self, *args, **kwargs):
-        return self._client.stop_listening(
-            *args, identifier_pattern=(None, self.id, None), **kwargs
+    async def stop_listening(self, *args, **kwargs):
+        return await self._client.stop_listening(
+            *args, 
+            identifier_pattern=(self.chat.id, self.from_user.id, self.id),
+            **kwargs
         )
```

### Comparing `herdmod-0.0.2/herdmod/nav/pagination.py` & `herdmod-0.0.3/herdmod/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/herdmod/utils/utils.py` & `herdmod-0.0.3/herdmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.2/herdmod.egg-info/PKG-INFO` & `herdmod-0.0.3/herdmod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.0.2/setup.py` & `herdmod-0.0.3/setup.py`

 * *Files identical despite different names*

