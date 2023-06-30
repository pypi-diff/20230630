# Comparing `tmp/mentord-1.1.8.tar.gz` & `tmp/mentord-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.8.tar", last modified: Fri Jun 30 07:50:02 2023, max compression
+gzip compressed data, was "mentord-1.1.9.tar", last modified: Fri Jun 30 07:58:32 2023, max compression
```

## Comparing `mentord-1.1.8.tar` & `mentord-1.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.159554 mentord-1.1.8/
--rw-rw-rw-   0        0        0      652 2023-06-30 07:50:02.159554 mentord-1.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.146575 mentord-1.1.8/mentord/
--rw-rw-rw-   0        0        0      112 2023-06-30 07:49:49.000000 mentord-1.1.8/mentord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.155561 mentord-1.1.8/mentord/classes/
--rw-rw-rw-   0        0        0     2039 2023-06-30 07:48:41.000000 mentord-1.1.8/mentord/classes/channel.py
--rw-rw-rw-   0        0        0     1423 2023-06-30 07:46:28.000000 mentord-1.1.8/mentord/classes/guild.py
--rw-rw-rw-   0        0        0      732 2023-06-30 07:46:30.000000 mentord-1.1.8/mentord/classes/member.py
--rw-rw-rw-   0        0        0     1496 2023-06-30 07:48:31.000000 mentord-1.1.8/mentord/classes/message.py
--rw-rw-rw-   0        0        0     2836 2023-06-30 07:48:23.000000 mentord-1.1.8/mentord/classes/user.py
--rw-rw-rw-   0        0        0      934 2023-06-30 07:49:33.000000 mentord-1.1.8/mentord/client.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.157571 mentord-1.1.8/mentord/events/
--rw-rw-rw-   0        0        0     2001 2023-06-30 07:49:12.000000 mentord-1.1.8/mentord/events/eon_message.py
--rw-rw-rw-   0        0        0     1404 2023-06-30 07:49:06.000000 mentord-1.1.8/mentord/events/eon_ready.py
--rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.8/mentord/httpc.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.158556 mentord-1.1.8/mentord/utils/
--rw-rw-rw-   0        0        0      806 2023-06-30 07:49:22.000000 mentord-1.1.8/mentord/utils/channel_opers.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:50:02.150569 mentord-1.1.8/mentord.egg-info/
--rw-rw-rw-   0        0        0      652 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-30 07:50:02.000000 mentord-1.1.8/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:50:02.160552 mentord-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-06-30 07:49:36.000000 mentord-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.358698 mentord-1.1.9/
+-rw-rw-rw-   0        0        0      652 2023-06-30 07:58:32.359197 mentord-1.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.347216 mentord-1.1.9/mentord/
+-rw-rw-rw-   0        0        0      112 2023-06-30 07:49:49.000000 mentord-1.1.9/mentord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.355203 mentord-1.1.9/mentord/classes/
+-rw-rw-rw-   0        0        0     2047 2023-06-30 07:55:46.000000 mentord-1.1.9/mentord/classes/channel.py
+-rw-rw-rw-   0        0        0     1339 2023-06-30 07:55:54.000000 mentord-1.1.9/mentord/classes/guild.py
+-rw-rw-rw-   0        0        0      648 2023-06-30 07:56:02.000000 mentord-1.1.9/mentord/classes/member.py
+-rw-rw-rw-   0        0        0     1504 2023-06-30 07:56:08.000000 mentord-1.1.9/mentord/classes/message.py
+-rw-rw-rw-   0        0        0     2844 2023-06-30 07:56:15.000000 mentord-1.1.9/mentord/classes/user.py
+-rw-rw-rw-   0        0        0      939 2023-06-30 07:57:38.000000 mentord-1.1.9/mentord/client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.357200 mentord-1.1.9/mentord/events/
+-rw-rw-rw-   0        0        0     2028 2023-06-30 07:56:43.000000 mentord-1.1.9/mentord/events/eon_message.py
+-rw-rw-rw-   0        0        0     1433 2023-06-30 07:56:58.000000 mentord-1.1.9/mentord/events/eon_ready.py
+-rw-rw-rw-   0        0        0      972 2023-06-30 07:57:07.000000 mentord-1.1.9/mentord/httpc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.358199 mentord-1.1.9/mentord/utils/
+-rw-rw-rw-   0        0        0      806 2023-06-30 07:49:22.000000 mentord-1.1.9/mentord/utils/channel_opers.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:32.350711 mentord-1.1.9/mentord.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-30 07:58:32.000000 mentord-1.1.9/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:58:32.359696 mentord-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-06-30 07:58:23.000000 mentord-1.1.9/setup.py
```

### Comparing `mentord-1.1.8/PKG-INFO` & `mentord-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.8
+Version: 1.1.9
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.8/mentord/classes/channel.py` & `mentord-1.1.9/mentord/classes/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class ChannelIsNoneObject(Exception):
     ...
 
 
 from .message import *
 from .guild import *
-from httpc import *
+from mentord.httpc import *
 
 
 class Channel:
 
     """
     #### Channel object contains data
     #### about the channel in guild.
```

### Comparing `mentord-1.1.8/mentord/classes/guild.py` & `mentord-1.1.9/mentord/classes/guild.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 class GuildIsNoneObject(Exception):
     ...
 
-from classes import *
-from client import Client
-from events import *
-from httpc import *
-from utils import *
+from mentord.client import *
 
 class Guild:
 
     """
     #### Guild object contains data
     #### about the guild.
     """
```

### Comparing `mentord-1.1.8/mentord/classes/message.py` & `mentord-1.1.9/mentord/classes/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class MessageIsNoneObject(Exception):
     ...
 
 from .channel import *
 from .guild import *
-from httpc import *
+from mentord.httpc import *
 from .member import *
 
 
 class Message:
 
     """
     #### Message object contains data
```

### Comparing `mentord-1.1.8/mentord/classes/user.py` & `mentord-1.1.9/mentord/classes/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class UserIsNoneObject(Exception):
     ...
 
 
 from .channel import *
 from .guild import *
-from httpc import *
+from mentord.httpc import *
 
 
 class User:
 
     """
     #### The User object contains data
     #### about the connected object by token.
```

### Comparing `mentord-1.1.8/mentord/client.py` & `mentord-1.1.9/mentord/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class IncorrectToken(Exception):
     ...
 
 
-from .classes import User
+from .classes.user import User
 from .httpc import *
 from .events import *
 
 
 class Client:
 
     """
```

### Comparing `mentord-1.1.8/mentord/events/eon_message.py` & `mentord-1.1.9/mentord/events/eon_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from threading import Thread
 from time import sleep
 
-from classes import Message
-from client import Client
-from httpc import *
+from mentord.classes.message import Message
+from mentord.client import *
+from mentord.httpc import *
 from requests import Response
 
 
 class on_message:
 
     """
     #### The function will be called when a new message is received.
```

### Comparing `mentord-1.1.8/mentord/events/eon_ready.py` & `mentord-1.1.9/mentord/events/eon_ready.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from threading import Thread
 from time import sleep
 
-from classes import User
-from client import Client, IncorrectToken
-from httpc import *
+from mentord.classes.user import User
+from mentord.client import Client, IncorrectToken
+from mentord.httpc import *
 
 class on_ready:
 
     """
     #### The function will be called when the bot is fully ready.
     """
```

### Comparing `mentord-1.1.8/mentord/httpc.py` & `mentord-1.1.9/mentord/httpc.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.8/mentord/utils/channel_opers.py` & `mentord-1.1.9/mentord/utils/channel_opers.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.8/mentord.egg-info/PKG-INFO` & `mentord-1.1.9/mentord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.8
+Version: 1.1.9
 Summary: A sync library for creating self bots in python!
 Description-Content-Type: text/markdown
 
 
 ### Example use:
 
 ```python
```

### Comparing `mentord-1.1.8/setup.py` & `mentord-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="mentord",
-    version="1.1.8",
+    version="1.1.9",
     description="A sync library for creating self bots in python!",
     packages=["mentord", "mentord/classes", "mentord/events", "mentord/utils"],
     long_description_content_type="text/markdown",
     long_description="""
 ### Example use:
 
 ```python
```

