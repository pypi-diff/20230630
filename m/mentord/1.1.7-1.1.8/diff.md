# Comparing `tmp/mentord-1.1.7.tar.gz` & `tmp/mentord-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.7.tar", last modified: Thu Jun 29 18:37:28 2023, max compression
+gzip compressed data, was "mentord-1.1.8.tar", last modified: Fri Jun 30 07:50:02 2023, max compression
```

## Comparing `mentord-1.1.7.tar` & `mentord-1.1.8.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.597506 mentord-1.1.7/
--rw-rw-rw-   0        0        0      652 2023-06-29 18:37:28.597506 mentord-1.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.582530 mentord-1.1.7/mentord/
--rw-rw-rw-   0        0        0      112 2023-06-29 18:20:54.000000 mentord-1.1.7/mentord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.591516 mentord-1.1.7/mentord/classes/
--rw-rw-rw-   0        0        0      114 2023-06-29 18:09:36.000000 mentord-1.1.7/mentord/classes/__init__.py
--rw-rw-rw-   0        0        0     2019 2023-06-29 18:09:33.000000 mentord-1.1.7/mentord/classes/channel.py
--rw-rw-rw-   0        0        0     1309 2023-06-29 18:06:30.000000 mentord-1.1.7/mentord/classes/guild.py
--rw-rw-rw-   0        0        0      618 2023-06-29 18:07:07.000000 mentord-1.1.7/mentord/classes/member.py
--rw-rw-rw-   0        0        0     1431 2023-06-29 18:06:36.000000 mentord-1.1.7/mentord/classes/message.py
--rw-rw-rw-   0        0        0     2836 2023-06-29 18:09:19.000000 mentord-1.1.7/mentord/classes/user.py
--rw-rw-rw-   0        0        0      959 2023-06-29 18:23:13.000000 mentord-1.1.7/mentord/client.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.594511 mentord-1.1.7/mentord/events/
--rw-rw-rw-   0        0        0       54 2023-06-29 17:25:45.000000 mentord-1.1.7/mentord/events/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-06-29 18:08:05.000000 mentord-1.1.7/mentord/events/eon_message.py
--rw-rw-rw-   0        0        0     1375 2023-06-29 18:08:49.000000 mentord-1.1.7/mentord/events/eon_ready.py
--rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.7/mentord/httpc.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.596508 mentord-1.1.7/mentord/utils/
--rw-rw-rw-   0        0        0       28 2023-06-29 18:20:49.000000 mentord-1.1.7/mentord/utils/__init__.py
--rw-rw-rw-   0        0        0      772 2023-06-29 18:20:33.000000 mentord-1.1.7/mentord/utils/channel_opers.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.586025 mentord-1.1.7/mentord.egg-info/
--rw-rw-rw-   0        0        0      652 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 18:37:28.598505 mentord-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-06-29 18:37:05.000000 mentord-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.159554 mentord-1.1.8/
+-rw-rw-rw-   0        0        0      652 2023-06-30 07:50:02.159554 mentord-1.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.146575 mentord-1.1.8/mentord/
+-rw-rw-rw-   0        0        0      112 2023-06-30 07:49:49.000000 mentord-1.1.8/mentord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.155561 mentord-1.1.8/mentord/classes/
+-rw-rw-rw-   0        0        0     2039 2023-06-30 07:48:41.000000 mentord-1.1.8/mentord/classes/channel.py
+-rw-rw-rw-   0        0        0     1423 2023-06-30 07:46:28.000000 mentord-1.1.8/mentord/classes/guild.py
+-rw-rw-rw-   0        0        0      732 2023-06-30 07:46:30.000000 mentord-1.1.8/mentord/classes/member.py
+-rw-rw-rw-   0        0        0     1496 2023-06-30 07:48:31.000000 mentord-1.1.8/mentord/classes/message.py
+-rw-rw-rw-   0        0        0     2836 2023-06-30 07:48:23.000000 mentord-1.1.8/mentord/classes/user.py
+-rw-rw-rw-   0        0        0      934 2023-06-30 07:49:33.000000 mentord-1.1.8/mentord/client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.157571 mentord-1.1.8/mentord/events/
+-rw-rw-rw-   0        0        0     2001 2023-06-30 07:49:12.000000 mentord-1.1.8/mentord/events/eon_message.py
+-rw-rw-rw-   0        0        0     1404 2023-06-30 07:49:06.000000 mentord-1.1.8/mentord/events/eon_ready.py
+-rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.8/mentord/httpc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.158556 mentord-1.1.8/mentord/utils/
+-rw-rw-rw-   0        0        0      806 2023-06-30 07:49:22.000000 mentord-1.1.8/mentord/utils/channel_opers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.150569 mentord-1.1.8/mentord.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:50:02.160552 mentord-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-06-30 07:49:36.000000 mentord-1.1.8/setup.py
```

### Comparing `mentord-1.1.7/PKG-INFO` & `mentord-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.7
+Version: 1.1.8
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.7/mentord/classes/channel.py` & `mentord-1.1.8/mentord/classes/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class ChannelIsNoneObject(Exception):
     ...
 
 
-from httpc import *
-
 from .message import *
+from .guild import *
+from httpc import *
 
 
 class Channel:
 
     """
     #### Channel object contains data
     #### about the channel in guild.
```

### Comparing `mentord-1.1.7/mentord/classes/guild.py` & `mentord-1.1.8/mentord/classes/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,78 @@
-class GuildIsNoneObject(Exception):
+class MessageIsNoneObject(Exception):
     ...
 
+from .channel import *
+from .guild import *
+from httpc import *
+from .member import *
 
-class Guild:
+
+class Message:
 
     """
-    #### Guild object contains data
-    #### about the guild.
+    #### Message object contains data
+    #### about a message in a certain guild and in a certain channel.
     """
 
-    def __init__(self, guild: dict) -> None:
-        self.guild: dict = guild
+    def __init__(self, message: dict) -> None:
+        self.message: dict = message
 
     def __check__(self) -> None:
-        if self.guild is None:
-            raise GuildIsNoneObject("The guild parameter was not passed...")
+        if self.message is None:
+            raise MessageIsNoneObject("The message parameter was not passed...")
 
     @property
     def id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
-            `int: id guild`
+            `int: id message`
         """
 
         self.__check__()
 
-        return int(self.guild["id"])
+        return int(self.message["id"])
 
     @property
-    def name(self) -> str:
+    def channel_id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
-            `str: name guild`
+            `int: channel id message`
         """
 
         self.__check__()
 
-        return str(self.guild["name"])
+        return int(self.message["channel_id"])
 
     @property
-    def icon(self) -> str:
+    def content(self) -> str:
         """
         Params:
             `None`
 
         Returns:
-            `str: icon guild in hash`
+            `str: content message`
         """
 
         self.__check__()
 
-        return str(self.guild["icon"])
+        return str(self.message["channel_id"])
 
     @property
-    def owner_id(self) -> int:
+    def author(self) -> str:
         """
         Params:
             `None`
 
         Returns:
-            `int: owner guild id`
+            `User: author message`
         """
 
         self.__check__()
 
-        return int(self.guild["owner_guild"])
+        return Member(self.message["author"])
```

### Comparing `mentord-1.1.7/mentord/classes/user.py` & `mentord-1.1.8/mentord/classes/user.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.7/mentord/client.py` & `mentord-1.1.8/mentord/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 class IncorrectToken(Exception):
     ...
 
 
-from .classes import *
+from .classes import User
 from .httpc import *
 from .events import *
-import utils.channel_opers
 
 
 class Client:
 
     """
     #### Main client class.
     """
```

### Comparing `mentord-1.1.7/mentord/events/eon_message.py` & `mentord-1.1.8/mentord/events/eon_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from threading import Thread
 from time import sleep
 
-from classes import *
+from classes import Message
 from client import Client
+from httpc import *
 from requests import Response
 
 
 class on_message:
 
     """
     #### The function will be called when a new message is received.
@@ -52,14 +53,12 @@
                     messages: dict = self.get_messages_id()
 
                 if response.json().count != 0:
                     for message in response.json():
                         func(Message(message))
                         messages[channel.id] = Message(message).id
 
-                print(response.json())
-
             sleep(self.delay)
 
     def create_thread(self, func, args) -> None:
         new_t = Thread(target=func, args=args)
         new_t.start()
```

### Comparing `mentord-1.1.7/mentord/events/eon_ready.py` & `mentord-1.1.8/mentord/events/eon_ready.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from threading import Thread
 from time import sleep
 
-import client
-from classes import *
-
+from classes import User
+from client import Client, IncorrectToken
+from httpc import *
 
 class on_ready:
 
     """
     #### The function will be called when the bot is fully ready.
     """
 
-    def __init__(self, client: client.Client, rdelay: float = 5.0):
+    def __init__(self, client: Client, rdelay: float = 5.0):
         self.client: client.Client = client
         self.rdelay: float = rdelay
 
     def __call__(self, func) -> None:
         while self.client.user is None:
             sleep(0.5)
 
         self.create_thread(self.reconnect_loop)
 
         func()
 
     def reconnect_loop(self) -> None:
         while True:
-            connect_request = client.MentordRequest(
+            connect_request = MentordRequest(
                 url="https://discordapp.com/api/v9/users/@me",
                 headers={
                     "Authorization": self.client.user.token,
                     "Content-Type": "application/json",
                 },
             ).GET()
 
             if connect_request.status_code != 200:
-                raise client.IncorrectToken(
+                raise IncorrectToken(
                     "ConnectionError: check a token, it is invalid."
                 )
                 exit()
 
             self.client.user: User = User(
                 connect_request.json(), self.client.user.token
             )
```

### Comparing `mentord-1.1.7/mentord/httpc.py` & `mentord-1.1.8/mentord/httpc.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.7/mentord/utils/channel_opers.py` & `mentord-1.1.8/mentord/utils/channel_opers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from client import *
+from classes import Channel
+from client import Client
 from httpc import *
 
 
 class ChannelOperations:
 
     """
     #### Channel operations...
```

### Comparing `mentord-1.1.7/mentord.egg-info/PKG-INFO` & `mentord-1.1.8/mentord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.7
+Version: 1.1.8
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.7/setup.py` & `mentord-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="mentord",
-    version="1.1.7",
+    version="1.1.8",
     description="A sync library for creating self bots in python!",
     packages=["mentord", "mentord/classes", "mentord/events", "mentord/utils"],
     long_description_content_type="text/markdown",
     long_description="""
 ### Example use:
 
 ```python
```

