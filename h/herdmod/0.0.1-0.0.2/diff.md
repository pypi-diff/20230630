# Comparing `tmp/herdmod-0.0.1.tar.gz` & `tmp/herdmod-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.0.1.tar", last modified: Fri Jun 30 03:57:37 2023, max compression
+gzip compressed data, was "herdmod-0.0.2.tar", last modified: Fri Jun 30 12:03:52 2023, max compression
```

## Comparing `herdmod-0.0.1.tar` & `herdmod-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 03:57:24.000000 herdmod-0.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 03:57:24.000000 herdmod-0.0.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 03:57:24.000000 herdmod-0.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-30 03:57:37.247982 herdmod-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-30 03:57:24.000000 herdmod-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/nav/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/nav/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:57:37.247982 herdmod-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 03:57:24.000000 herdmod-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 12:03:39.000000 herdmod-0.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 12:03:39.000000 herdmod-0.0.2/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 12:03:39.000000 herdmod-0.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:03:52.878147 herdmod-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 12:03:39.000000 herdmod-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/nav/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 12:03:39.000000 herdmod-0.0.2/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:03:52.878147 herdmod-0.0.2/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 12:03:52.000000 herdmod-0.0.2/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:03:52.878147 herdmod-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 12:03:39.000000 herdmod-0.0.2/setup.py
```

### Comparing `herdmod-0.0.1/COPYING` & `herdmod-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/COPYING.lesser` & `herdmod-0.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/NOTICE` & `herdmod-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/PKG-INFO` & `herdmod-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -12,15 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # herdmod
-A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for pyroherd which does conversation handling and other cool stuff.
 
 In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
 It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
```

### Comparing `herdmod-0.0.1/README.md` & `herdmod-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # herdmod
-A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for pyroherd which does conversation handling and other cool stuff.
 
 In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
 It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
```

### Comparing `herdmod-0.0.1/herdmod/helpers/helpers.py` & `herdmod-0.0.2/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/herdmod/listen/listen.py` & `herdmod-0.0.2/herdmod/listen/listen.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,14 +287,30 @@
             (self.chat.id, from_user_id, self.id),
             listener_type=ListenerTypes.CALLBACK_QUERY,
             timeout=timeout,
             filters=filters,
             unallowed_click_alert=alert,
         )
 
+    @patchable
+    def listen(self, *args, **kwargs):
+        return self._client.listen((self.chat.id, self.from_user.id, self.id), *args, **kwargs)
+
+    @patchable
+    def ask(self, text, *args, **kwargs):
+        return self._client.ask(
+            text, (self.chat.id, self.from_user.id, self.id), *args, **kwargs
+        )
+
+    @patchable
+    def stop_listening(self, *args, **kwargs):
+        return self._client.stop_listening(
+            *args, identifier_pattern=(self.chat.id, self.from_user.id, self.id), **kwargs
+        )
+
 
 @patch(pyroherd.types.user_and_chats.chat.Chat)
 class Chat(pyroherd.types.Chat):
     @patchable
     def listen(self, *args, **kwargs):
         return self._client.listen((self.id, None, None), *args, **kwargs)
 
@@ -321,8 +337,8 @@
             text, (self.id, self.id, None), *args, **kwargs
         )
 
     @patchable
     def stop_listening(self, *args, **kwargs):
         return self._client.stop_listening(
             *args, identifier_pattern=(None, self.id, None), **kwargs
-        )
+        )
```

### Comparing `herdmod-0.0.1/herdmod/nav/pagination.py` & `herdmod-0.0.2/herdmod/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/herdmod/utils/utils.py` & `herdmod-0.0.2/herdmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.1/herdmod.egg-info/PKG-INFO` & `herdmod-0.0.2/herdmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -12,15 +12,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # herdmod
-A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for pyroherd which does conversation handling and other cool stuff.
 
 In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
 It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
```

### Comparing `herdmod-0.0.1/setup.py` & `herdmod-0.0.2/setup.py`

 * *Files identical despite different names*

