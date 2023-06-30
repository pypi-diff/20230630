# Comparing `tmp/herdmod-0.0.0.tar.gz` & `tmp/herdmod-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.0.0.tar", last modified: Thu Jun 29 16:03:08 2023, max compression
+gzip compressed data, was "herdmod-0.0.1.tar", last modified: Fri Jun 30 03:57:37 2023, max compression
```

## Comparing `herdmod-0.0.0.tar` & `herdmod-0.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-29 16:02:56.000000 herdmod-0.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-29 16:02:56.000000 herdmod-0.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-29 16:02:56.000000 herdmod-0.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-29 16:03:08.046916 herdmod-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-29 16:02:56.000000 herdmod-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod/nav/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/nav/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-29 16:02:56.000000 herdmod-0.0.0/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:03:08.046916 herdmod-0.0.0/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-06-29 16:03:08.000000 herdmod-0.0.0/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 16:03:08.000000 herdmod-0.0.0/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:03:08.000000 herdmod-0.0.0/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 16:03:08.000000 herdmod-0.0.0/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 16:03:08.000000 herdmod-0.0.0/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:03:08.046916 herdmod-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 16:02:56.000000 herdmod-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 03:57:24.000000 herdmod-0.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 03:57:24.000000 herdmod-0.0.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 03:57:24.000000 herdmod-0.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-30 03:57:37.247982 herdmod-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-30 03:57:24.000000 herdmod-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/nav/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.247982 herdmod-0.0.1/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 03:57:24.000000 herdmod-0.0.1/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:57:37.243982 herdmod-0.0.1/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 03:57:37.000000 herdmod-0.0.1/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:57:37.247982 herdmod-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 03:57:24.000000 herdmod-0.0.1/setup.py
```

### Comparing `herdmod-0.0.0/COPYING` & `herdmod-0.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/COPYING.lesser` & `herdmod-0.0.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/NOTICE` & `herdmod-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/PKG-INFO` & `herdmod-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.0
+Version: 0.0.1
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -12,47 +12,47 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # herdmod
-A monkeypatcher add-on for Pyroherd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
 
-In other words, it is a compilation of utilities i developed for improving my personal experience with Pyroherd.
-It works **together** with Pyroherd, it is **not** a fork/modded version. It does monkeypatching to add features to Pyroherd classes on the go (so i don't need to update on every Pyroherd's release).
+In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
+It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
 # config.py
 import herdmod
 from pyroherd import Client
 
 app = Client('my_session')
 ```
 
-Then you can, from another file, do `from config import app` to import the modded Pyroherd Client we created above. It will be modded globally.
+Then you can, from another file, do `from config import app` to import the modded herd Client we created above. It will be modded globally.
 
 All the patches are applied automatically as soon as herdmod is imported.
 
 ## Methods
 All herdmod methods are callable by any of these ways:
 - `await Client.<method>(identifier, ...)`
 - `await Chat.<method>()`
 - `await User.<method>()`
 
-In the last two, Pyroherd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
+In the last two, herd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
 
 These are the methods herdmod adds:
 - `listen(identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Awaits for a new message in the specified chat and returns its Message object. If listener_type is set to `ListenerTypes.CALLBACK_QUERY`, it awaits and returns a CallbackQuery object.
 You can pass Update Filters to the `filters` parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 `identifier` is a tuple containing, in this exact order, (chat_id, user_id, message_id). It lets you specify exactly which update you want. You don't need to worry about that if you mostly use the bound methods.
-`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `PyromodConfig.unnalowed_click_alert_text`. If False, no text is shown.
+`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `HerdmodConfig.unnalowed_click_alert_text`. If False, no text is shown.
 
 - `ask(text, identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Same as `listen`, but sends a message to identifier[0] before and only then waits for a response.
 You can additionally pass any of the `Client.send_message()` parameters. Check the example below.
 The object of the sent message is returned inside of the attribute `request`
 
 Example:
@@ -118,15 +118,15 @@
 def page_data(page):
     return f'view_page {page}'
 def item_data(item, page):
     return f'view_item {item} {page}'
 def item_title(item, page):
     return f'Item {item} of page {page}'
 
-@Client.on_message(filters.regex('/nav'))
+@Client.on_msg(filters.regex('/nav'))
 async def on_nav(c,m):
     objects = [*range(1,100)]
     page = Pagination(
         objects,
         page_data=page_data, # callback to define the callback_data for page buttons in the bottom
         item_data=item_data, # callback to define the callback_data for each item button
         item_title=item_title # callback to define the text for each item button
@@ -134,28 +134,28 @@
     index = 0 # in which page is it now? (used to calculate the offset)
     lines = 5 # how many lines of the keyboard to include for the items
     columns = how many columns include in each items' line
     kb = page.create(index, lines, columns)
     await m.reply('Test', reply_markup=ikb(kb))
 ```
 
-## herdmod.PyroherdConfig
+## herdmod.HerdmodConfig
 It lets you do some tweaks on herdmod behavior.
 ```python
-class PyromodConfig:
+class HerdmodConfig:
     timeout_handler = None
     stopped_handler = None
     throw_exceptions = True
     unallowed_click_alert = True
     unallowed_click_alert_text = (
         "[herdmod] You're not expected to click this button."
     )
 ```
 `timeout_handler` and `stopped_handler` are callbacks that receive (identifier, listener_data) as arguments. timeout_handler receives an extra arg `timeout`. When they are in use, herdmod won't throw the exceptions ListenerStopped and ListenedTimeout.
 
 ### Copyright & License
-This project may include snippets of Pyroherd code
-- Pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2017-2022 Dan <<https://github.com/delivrance>>
+This project may include snippets of herd code
+- pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2022-2025 OnTheHerd <<https://github.com/OnTheHerd>>
 
 Licensed under the terms of the [GNU Lesser General Public License v3 or later (LGPLv3+)](COPYING.lesser)
```

### Comparing `herdmod-0.0.0/README.md` & `herdmod-0.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # herdmod
-A monkeypatcher add-on for Pyroherd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
 
-In other words, it is a compilation of utilities i developed for improving my personal experience with Pyroherd.
-It works **together** with Pyroherd, it is **not** a fork/modded version. It does monkeypatching to add features to Pyroherd classes on the go (so i don't need to update on every Pyroherd's release).
+In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
+It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
 # config.py
 import herdmod
 from pyroherd import Client
 
 app = Client('my_session')
 ```
 
-Then you can, from another file, do `from config import app` to import the modded Pyroherd Client we created above. It will be modded globally.
+Then you can, from another file, do `from config import app` to import the modded herd Client we created above. It will be modded globally.
 
 All the patches are applied automatically as soon as herdmod is imported.
 
 ## Methods
 All herdmod methods are callable by any of these ways:
 - `await Client.<method>(identifier, ...)`
 - `await Chat.<method>()`
 - `await User.<method>()`
 
-In the last two, Pyroherd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
+In the last two, herd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
 
 These are the methods herdmod adds:
 - `listen(identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Awaits for a new message in the specified chat and returns its Message object. If listener_type is set to `ListenerTypes.CALLBACK_QUERY`, it awaits and returns a CallbackQuery object.
 You can pass Update Filters to the `filters` parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 `identifier` is a tuple containing, in this exact order, (chat_id, user_id, message_id). It lets you specify exactly which update you want. You don't need to worry about that if you mostly use the bound methods.
-`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `PyromodConfig.unnalowed_click_alert_text`. If False, no text is shown.
+`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `HerdmodConfig.unnalowed_click_alert_text`. If False, no text is shown.
 
 - `ask(text, identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Same as `listen`, but sends a message to identifier[0] before and only then waits for a response.
 You can additionally pass any of the `Client.send_message()` parameters. Check the example below.
 The object of the sent message is returned inside of the attribute `request`
 
 Example:
@@ -101,15 +101,15 @@
 def page_data(page):
     return f'view_page {page}'
 def item_data(item, page):
     return f'view_item {item} {page}'
 def item_title(item, page):
     return f'Item {item} of page {page}'
 
-@Client.on_message(filters.regex('/nav'))
+@Client.on_msg(filters.regex('/nav'))
 async def on_nav(c,m):
     objects = [*range(1,100)]
     page = Pagination(
         objects,
         page_data=page_data, # callback to define the callback_data for page buttons in the bottom
         item_data=item_data, # callback to define the callback_data for each item button
         item_title=item_title # callback to define the text for each item button
@@ -117,28 +117,28 @@
     index = 0 # in which page is it now? (used to calculate the offset)
     lines = 5 # how many lines of the keyboard to include for the items
     columns = how many columns include in each items' line
     kb = page.create(index, lines, columns)
     await m.reply('Test', reply_markup=ikb(kb))
 ```
 
-## herdmod.PyroherdConfig
+## herdmod.HerdmodConfig
 It lets you do some tweaks on herdmod behavior.
 ```python
-class PyromodConfig:
+class HerdmodConfig:
     timeout_handler = None
     stopped_handler = None
     throw_exceptions = True
     unallowed_click_alert = True
     unallowed_click_alert_text = (
         "[herdmod] You're not expected to click this button."
     )
 ```
 `timeout_handler` and `stopped_handler` are callbacks that receive (identifier, listener_data) as arguments. timeout_handler receives an extra arg `timeout`. When they are in use, herdmod won't throw the exceptions ListenerStopped and ListenedTimeout.
 
 ### Copyright & License
-This project may include snippets of Pyroherd code
-- Pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2017-2022 Dan <<https://github.com/delivrance>>
+This project may include snippets of herd code
+- pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2022-2025 OnTheHerd <<https://github.com/OnTheHerd>>
 
 Licensed under the terms of the [GNU Lesser General Public License v3 or later (LGPLv3+)](COPYING.lesser)
```

### Comparing `herdmod-0.0.0/herdmod/helpers/helpers.py` & `herdmod-0.0.1/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/herdmod/listen/listen.py` & `herdmod-0.0.1/herdmod/listen/listen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import pyroherd
 from enum import Enum
 from typing import Optional, Callable, Union
-from ..utils import patch, patchable, PyrosexmodConfig
+from ..utils import patch, patchable, HerdmodConfig
 
 loop = asyncio.get_event_loop()
 
 
 class ListenerStopped(Exception):
     pass
 
@@ -54,19 +54,19 @@
         }
 
         self.listeners[listener_type].update({identifier: listener_data})
 
         try:
             return await asyncio.wait_for(future, timeout)
         except asyncio.exceptions.TimeoutError:
-            if callable(PyrosexmodConfig.timeout_handler):
-                PyrosexmodConfig.timeout_handler(
+            if callable(HerdmodConfig.timeout_handler):
+                HerdmodConfig.timeout_handler(
                     identifier, listener_data, timeout
                 )
-            elif PyrosexmodConfig.throw_exceptions:
+            elif HerdmodConfig.throw_exceptions:
                 raise ListenerTimeout(timeout)
 
     @patchable
     async def ask(
         self,
         text,
         identifier: tuple,
@@ -151,17 +151,17 @@
 
         if not listener:
             return
         elif listener["future"].done():
             del self.listeners[listener_type][identifier]
             return
 
-        if callable(PyrosexmodConfig.stopped_handler):
-            PyrosexmodConfig.stopped_handler(identifier, listener)
-        elif PyrosexmodConfig.throw_exceptions:
+        if callable(HerdmodConfig.stopped_handler):
+            HerdmodConfig.stopped_handler(identifier, listener)
+        elif HerdmodConfig.throw_exceptions:
             listener["future"].set_exception(ListenerStopped())
 
         del self.listeners[listener_type][identifier]
 
 
 @patch(pyroherd.handlers.message_handler.MessageHandler)
 class MessageHandler:
@@ -228,15 +228,15 @@
     async def check(self, client, query):
         listener = client.match_listener(
             (query.message.chat.id, query.from_user.id, query.message.id),
             ListenerTypes.CALLBACK_QUERY,
         )[0]
 
         # managing unallowed user clicks
-        if PyrosexmodConfig.unallowed_click_alert:
+        if HerdmodConfig.unallowed_click_alert:
             permissive_listener = client.match_listener(
                 identifier_pattern=(
                     query.message.chat.id,
                     None,
                     query.message.id,
                 ),
                 listener_type=ListenerTypes.CALLBACK_QUERY,
@@ -245,15 +245,15 @@
             if (permissive_listener and not listener) and permissive_listener[
                 "unallowed_click_alert"
             ]:
                 alert = (
                     permissive_listener["unallowed_click_alert"]
                     if type(permissive_listener["unallowed_click_alert"])
                     == str
-                    else PyrosexmodConfig.unallowed_click_alert_text
+                    else HerdmodConfig.unallowed_click_alert_text
                 )
                 await query.answer(alert)
                 return False
 
         filters = listener["filters"] if listener else self.filters
 
         return await filters(client, query) if callable(filters) else True
```

### Comparing `herdmod-0.0.0/herdmod/nav/pagination.py` & `herdmod-0.0.1/herdmod/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/herdmod/utils/utils.py` & `herdmod-0.0.1/herdmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.0/herdmod.egg-info/PKG-INFO` & `herdmod-0.0.1/herdmod.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.0
+Version: 0.0.1
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -12,47 +12,47 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 # herdmod
-A monkeypatcher add-on for Pyroherd which does conversation handling and other cool stuff.
+A monkeypatcher add-on for herd which does conversation handling and other cool stuff.
 
-In other words, it is a compilation of utilities i developed for improving my personal experience with Pyroherd.
-It works **together** with Pyroherd, it is **not** a fork/modded version. It does monkeypatching to add features to Pyroherd classes on the go (so i don't need to update on every Pyroherd's release).
+In other words, it is a compilation of utilities i developed for improving my personal experience with herd.
+It works **together** with herd, it is **not** a fork/modded version. It does monkeypatching to add features to herd classes on the go (so i don't need to update on every herd's release).
 
 ## Usage
 Import `herdmod` one time in your script and you'll already be able to use the modified pyroherdgram in all your handlers. Example:
 ```python
 # config.py
 import herdmod
 from pyroherd import Client
 
 app = Client('my_session')
 ```
 
-Then you can, from another file, do `from config import app` to import the modded Pyroherd Client we created above. It will be modded globally.
+Then you can, from another file, do `from config import app` to import the modded herd Client we created above. It will be modded globally.
 
 All the patches are applied automatically as soon as herdmod is imported.
 
 ## Methods
 All herdmod methods are callable by any of these ways:
 - `await Client.<method>(identifier, ...)`
 - `await Chat.<method>()`
 - `await User.<method>()`
 
-In the last two, Pyroherd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
+In the last two, herd automatically gets the ids from the object, to compound the `identifier` tuple that `Client.listen` uses.
 
 These are the methods herdmod adds:
 - `listen(identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Awaits for a new message in the specified chat and returns its Message object. If listener_type is set to `ListenerTypes.CALLBACK_QUERY`, it awaits and returns a CallbackQuery object.
 You can pass Update Filters to the `filters` parameter just like you do for the update handlers. e.g. `filters=filters.photo & filters.bot`
 `identifier` is a tuple containing, in this exact order, (chat_id, user_id, message_id). It lets you specify exactly which update you want. You don't need to worry about that if you mostly use the bound methods.
-`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `PyromodConfig.unnalowed_click_alert_text`. If False, no text is shown.
+`unnalowed_click_alert` is the text that users will see in an alert when the button is not waiting for them to click. If True, it uses the default text at `HerdmodConfig.unnalowed_click_alert_text`. If False, no text is shown.
 
 - `ask(text, identifier, filters=None, listener_type=ListenerTypes.MESSAGE, timeout=None, unallowed_click_alert=True)`
 Same as `listen`, but sends a message to identifier[0] before and only then waits for a response.
 You can additionally pass any of the `Client.send_message()` parameters. Check the example below.
 The object of the sent message is returned inside of the attribute `request`
 
 Example:
@@ -118,15 +118,15 @@
 def page_data(page):
     return f'view_page {page}'
 def item_data(item, page):
     return f'view_item {item} {page}'
 def item_title(item, page):
     return f'Item {item} of page {page}'
 
-@Client.on_message(filters.regex('/nav'))
+@Client.on_msg(filters.regex('/nav'))
 async def on_nav(c,m):
     objects = [*range(1,100)]
     page = Pagination(
         objects,
         page_data=page_data, # callback to define the callback_data for page buttons in the bottom
         item_data=item_data, # callback to define the callback_data for each item button
         item_title=item_title # callback to define the text for each item button
@@ -134,28 +134,28 @@
     index = 0 # in which page is it now? (used to calculate the offset)
     lines = 5 # how many lines of the keyboard to include for the items
     columns = how many columns include in each items' line
     kb = page.create(index, lines, columns)
     await m.reply('Test', reply_markup=ikb(kb))
 ```
 
-## herdmod.PyroherdConfig
+## herdmod.HerdmodConfig
 It lets you do some tweaks on herdmod behavior.
 ```python
-class PyromodConfig:
+class HerdmodConfig:
     timeout_handler = None
     stopped_handler = None
     throw_exceptions = True
     unallowed_click_alert = True
     unallowed_click_alert_text = (
         "[herdmod] You're not expected to click this button."
     )
 ```
 `timeout_handler` and `stopped_handler` are callbacks that receive (identifier, listener_data) as arguments. timeout_handler receives an extra arg `timeout`. When they are in use, herdmod won't throw the exceptions ListenerStopped and ListenedTimeout.
 
 ### Copyright & License
-This project may include snippets of Pyroherd code
-- Pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2017-2022 Dan <<https://github.com/delivrance>>
+This project may include snippets of herd code
+- pyroherd - Telegram MTProto API Client Library for Python. Copyright (C) 2022-2025 OnTheHerd <<https://github.com/OnTheHerd>>
 
 Licensed under the terms of the [GNU Lesser General Public License v3 or later (LGPLv3+)](COPYING.lesser)
```

### Comparing `herdmod-0.0.0/setup.py` & `herdmod-0.0.1/setup.py`

 * *Files identical despite different names*

