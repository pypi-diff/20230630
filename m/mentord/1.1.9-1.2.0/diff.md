# Comparing `tmp/mentord-1.1.9.tar.gz` & `tmp/mentord-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.9.tar", last modified: Fri Jun 30 07:58:32 2023, max compression
+gzip compressed data, was "mentord-1.2.0.tar", last modified: Fri Jun 30 10:02:12 2023, max compression
```

## Comparing `mentord-1.1.9.tar` & `mentord-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.358698 mentord-1.1.9/
--rw-rw-rw-   0        0        0      652 2023-06-30 07:58:32.359197 mentord-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.347216 mentord-1.1.9/mentord/
--rw-rw-rw-   0        0        0      112 2023-06-30 07:49:49.000000 mentord-1.1.9/mentord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.355203 mentord-1.1.9/mentord/classes/
--rw-rw-rw-   0        0        0     2047 2023-06-30 07:55:46.000000 mentord-1.1.9/mentord/classes/channel.py
--rw-rw-rw-   0        0        0     1339 2023-06-30 07:55:54.000000 mentord-1.1.9/mentord/classes/guild.py
--rw-rw-rw-   0        0        0      648 2023-06-30 07:56:02.000000 mentord-1.1.9/mentord/classes/member.py
--rw-rw-rw-   0        0        0     1504 2023-06-30 07:56:08.000000 mentord-1.1.9/mentord/classes/message.py
--rw-rw-rw-   0        0        0     2844 2023-06-30 07:56:15.000000 mentord-1.1.9/mentord/classes/user.py
--rw-rw-rw-   0        0        0      939 2023-06-30 07:57:38.000000 mentord-1.1.9/mentord/client.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.357200 mentord-1.1.9/mentord/events/
--rw-rw-rw-   0        0        0     2028 2023-06-30 07:56:43.000000 mentord-1.1.9/mentord/events/eon_message.py
--rw-rw-rw-   0        0        0     1433 2023-06-30 07:56:58.000000 mentord-1.1.9/mentord/events/eon_ready.py
--rw-rw-rw-   0        0        0      972 2023-06-30 07:57:07.000000 mentord-1.1.9/mentord/httpc.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.358199 mentord-1.1.9/mentord/utils/
--rw-rw-rw-   0        0        0      806 2023-06-30 07:49:22.000000 mentord-1.1.9/mentord/utils/channel_opers.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.350711 mentord-1.1.9/mentord.egg-info/
--rw-rw-rw-   0        0        0      652 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:58:32.359696 mentord-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-06-30 07:58:23.000000 mentord-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.676555 mentord-1.2.0/
+-rw-rw-rw-   0        0        0      652 2023-06-30 10:02:12.676555 mentord-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.664074 mentord-1.2.0/mentord/
+-rw-rw-rw-   0        0        0      112 2023-06-30 07:49:49.000000 mentord-1.2.0/mentord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.672561 mentord-1.2.0/mentord/classes/
+-rw-rw-rw-   0        0        0     1963 2023-06-30 09:58:43.000000 mentord-1.2.0/mentord/classes/channel.py
+-rw-rw-rw-   0        0        0     1255 2023-06-30 09:58:29.000000 mentord-1.2.0/mentord/classes/guild.py
+-rw-rw-rw-   0        0        0      722 2023-06-30 10:01:51.000000 mentord-1.2.0/mentord/classes/member.py
+-rw-rw-rw-   0        0        0     1422 2023-06-30 09:58:13.000000 mentord-1.2.0/mentord/classes/message.py
+-rw-rw-rw-   0        0        0     2704 2023-06-30 09:57:59.000000 mentord-1.2.0/mentord/classes/user.py
+-rw-rw-rw-   0        0        0      922 2023-06-30 09:59:06.000000 mentord-1.2.0/mentord/client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.674558 mentord-1.2.0/mentord/events/
+-rw-rw-rw-   0        0        0     2028 2023-06-30 07:56:43.000000 mentord-1.2.0/mentord/events/eon_message.py
+-rw-rw-rw-   0        0        0     1416 2023-06-30 09:58:58.000000 mentord-1.2.0/mentord/events/eon_ready.py
+-rw-rw-rw-   0        0        0      972 2023-06-30 09:59:09.000000 mentord-1.2.0/mentord/httpc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.675557 mentord-1.2.0/mentord/utils/
+-rw-rw-rw-   0        0        0      806 2023-06-30 07:49:22.000000 mentord-1.2.0/mentord/utils/channel_opers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:02:12.667569 mentord-1.2.0/mentord.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-06-30 10:02:12.000000 mentord-1.2.0/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-06-30 10:02:12.000000 mentord-1.2.0/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 10:02:12.000000 mentord-1.2.0/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-30 10:02:12.000000 mentord-1.2.0/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 10:02:12.677554 mentord-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-06-30 10:02:10.000000 mentord-1.2.0/setup.py
```

### Comparing `mentord-1.1.9/PKG-INFO` & `mentord-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.9
+Version: 1.2.0
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.9/mentord/classes/channel.py` & `mentord-1.2.0/mentord/classes/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,44 +13,42 @@
     #### Channel object contains data
     #### about the channel in guild.
     """
 
     def __init__(self, channel: dict) -> None:
         self.channel: dict = channel
 
+        self.__check__()
+
     def __check__(self) -> None:
         if self.channel is None:
             raise ChannelIsNoneObject("The Channel parameter was not passed...")
 
     @property
     def id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: id channel`
         """
 
-        self.__check__()
-
         return int(self.channel["id"])
 
     @property
     def last_message_id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: last message id`
         """
 
-        self.__check__()
-
         return int(self.channel["last_message_id"])
 
     @property
     def recipients(self) -> int:
         """
         Params:
             `None`
@@ -61,29 +59,25 @@
         Keys:
             `id: int (id member)`
             `username: str (username member)`
             `global_name: str (global_name member)`
             `avatar: str (avatar user hash)`
         """
 
-        self.__check__()
-
         return dict(self.channel["recipients"])
 
     def messages(self, token: str) -> list[Message]:
         """
         Params:
             `None`
 
         Returns:
             `list[Message]: list messages object in current channel`
         """
 
-        self.__check__()
-
         response = MentordRequest(
             url="https://discordapp.com/api/v9/channels/{0}/messages?limit=25".format(
                 self.id
             ),
             headers={
                 "Authorization": token,
                 "Content-Type": "application/json",
```

### Comparing `mentord-1.1.9/mentord/classes/guild.py` & `mentord-1.2.0/mentord/classes/guild.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,66 +9,60 @@
     #### Guild object contains data
     #### about the guild.
     """
 
     def __init__(self, guild: dict) -> None:
         self.guild: dict = guild
 
+        self.__check__()
+
     def __check__(self) -> None:
         if self.guild is None:
             raise GuildIsNoneObject("The guild parameter was not passed...")
 
     @property
     def id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: id guild`
         """
 
-        self.__check__()
-
         return int(self.guild["id"])
 
     @property
     def name(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: name guild`
         """
 
-        self.__check__()
-
         return str(self.guild["name"])
 
     @property
     def icon(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: icon guild in hash`
         """
 
-        self.__check__()
-
         return str(self.guild["icon"])
 
     @property
     def owner_id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: owner guild id`
         """
 
-        self.__check__()
-
         return int(self.guild["owner_guild"])
```

### Comparing `mentord-1.1.9/mentord/classes/member.py` & `mentord-1.2.0/mentord/classes/member.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,24 @@
 from mentord.client import *
 
 class Member:
 
     """
     #### Member object contains data
     #### about the participant.
+
+    `Use member dictionary
+    to get variables. (temporarily)`
     """
 
     def __init__(self, member: dict) -> None:
         self.member: dict = member
 
+        self.__check__()
+
     def __check__(self) -> None:
         if self.member is None:
             raise MemberIsNoneObject("The member parameter was not passed...")
 
     @property
     def id(self) -> int:
 
@@ -24,10 +29,10 @@
         Params:
             `None`
 
         Returns:
             `int: id member`
         """
 
-        self.__check__()
-
         return int(self.member["id"])
+
+
```

### Comparing `mentord-1.1.9/mentord/classes/message.py` & `mentord-1.2.0/mentord/classes/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 class MessageIsNoneObject(Exception):
     ...
 
+
 from .channel import *
 from .guild import *
 from mentord.httpc import *
 from .member import *
 
 
 class Message:
@@ -13,66 +14,60 @@
     #### Message object contains data
     #### about a message in a certain guild and in a certain channel.
     """
 
     def __init__(self, message: dict) -> None:
         self.message: dict = message
 
+        self.__check__()
+
     def __check__(self) -> None:
         if self.message is None:
             raise MessageIsNoneObject("The message parameter was not passed...")
 
     @property
     def id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: id message`
         """
 
-        self.__check__()
-
         return int(self.message["id"])
 
     @property
     def channel_id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: channel id message`
         """
 
-        self.__check__()
-
         return int(self.message["channel_id"])
 
     @property
     def content(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: content message`
         """
 
-        self.__check__()
-
         return str(self.message["channel_id"])
 
     @property
     def author(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `User: author message`
         """
 
-        self.__check__()
-
         return Member(self.message["author"])
```

### Comparing `mentord-1.1.9/mentord/classes/user.py` & `mentord-1.2.0/mentord/classes/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,85 +14,77 @@
     #### about the connected object by token.
     """
 
     def __init__(self, user: dict, token: str) -> None:
         self.user: dict = user
         self.token: str = token
 
+        self.__check__()
+
     def __check__(self) -> None:
         if self.user is None:
             raise UserIsNoneObject("The user parameter was not passed...")
 
     @property
     def id(self) -> int:
         """
         Params:
             `None`
 
         Returns:
             `int: id user`
         """
 
-        self.__check__()
-
         return int(self.user["id"])
 
     @property
     def username(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: username`
         """
 
-        self.__check__()
-
         return str(self.user["username"])
 
     @property
     def global_name(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: global name`
         """
 
-        self.__check__()
-
         return str(self.user["global_name"])
 
     @property
     def avatar(self) -> str:
         """
         Params:
             `None`
 
         Returns:
             `str: string hash`
         """
 
-        self.__check__()
-
         return str(self.user["avatar"])
 
     def get_guilds(self) -> list[Guild]:
         """
         Params:
             `None`
 
         Returns:
             `list[Guild]: list guilds current user`
         """
 
-        self.__check__()
-
         connect_request = MentordRequest(
             url="https://discordapp.com/api/v9/users/@me/guilds",
             headers={"Authorization": self.token, "Content-Type": "application/json"},
         ).GET()
 
         if connect_request.status_code != 200:
             raise RequestError(
@@ -106,16 +98,14 @@
         Params:
             `None`
 
         Returns:
             `list[Channel]: list channels current user`
         """
 
-        self.__check__()
-
         connect_request = MentordRequest(
             url="https://discordapp.com/api/v9/users/@me/channels",
             headers={"Authorization": self.token, "Content-Type": "application/json"},
         ).GET()
 
         if connect_request.status_code != 200:
             raise RequestError(
```

### Comparing `mentord-1.1.9/mentord/client.py` & `mentord-1.2.0/mentord/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,18 @@
             `str`: token
 
         Returns:
             `None`
         """
 
         if token is None and token.__len__() <= 0:
-            raise IncorrectToken("Check a token, it is invalid.")
+            raise IncorrectToken("check a token, it is invalid.")
 
         connect_request = MentordRequest(
             url="https://discordapp.com/api/v9/users/@me",
             headers={"Authorization": token, "Content-Type": "application/json"},
         ).GET()
 
         if connect_request.status_code != 200:
-            raise IncorrectToken("ConnectionError: check a token, it is invalid.")
+            raise IncorrectToken("check a token, it is invalid.")
 
         self.user: User = User(connect_request.json(), token)
```

### Comparing `mentord-1.1.9/mentord/events/eon_message.py` & `mentord-1.2.0/mentord/events/eon_message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.9/mentord/events/eon_ready.py` & `mentord-1.2.0/mentord/events/eon_ready.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     "Authorization": self.client.user.token,
                     "Content-Type": "application/json",
                 },
             ).GET()
 
             if connect_request.status_code != 200:
                 raise IncorrectToken(
-                    "ConnectionError: check a token, it is invalid."
+                    "check a token, it is invalid."
                 )
                 exit()
 
             self.client.user: User = User(
                 connect_request.json(), self.client.user.token
             )
```

### Comparing `mentord-1.1.9/mentord/httpc.py` & `mentord-1.2.0/mentord/httpc.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.9/mentord/utils/channel_opers.py` & `mentord-1.2.0/mentord/utils/channel_opers.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.9/mentord.egg-info/PKG-INFO` & `mentord-1.2.0/mentord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.9
+Version: 1.2.0
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.9/setup.py` & `mentord-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="mentord",
-    version="1.1.9",
+    version="1.2.0",
     description="A sync library for creating self bots in python!",
     packages=["mentord", "mentord/classes", "mentord/events", "mentord/utils"],
     long_description_content_type="text/markdown",
     long_description="""
 ### Example use:
 
 ```python
```

