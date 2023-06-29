# Comparing `tmp/user_discord-1.2.9.tar.gz` & `tmp/user_discord-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.2.9.tar", last modified: Sat Jun 24 18:39:48 2023, max compression
+gzip compressed data, was "user_discord-1.3.0.tar", last modified: Thu Jun 29 22:28:14 2023, max compression
```

## Comparing `user_discord-1.2.9.tar` & `user_discord-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.346453 user_discord-1.2.9/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:39:48.346453 user_discord-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 18:39:48.348450 user_discord-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 18:39:09.000000 user_discord-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.307203 user_discord-1.2.9/user_discord/
--rw-rw-rw-   0        0        0      604 2023-06-24 18:39:18.000000 user_discord-1.2.9/user_discord/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.2.9/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.344448 user_discord-1.2.9/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.2.9/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.9/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.9/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.337519 user_discord-1.2.9/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-06-24 18:39:48.000000 user_discord-1.2.9/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.035215 user_discord-1.3.0/
+-rw-rw-rw-   0        0        0      335 2023-06-29 22:28:14.035215 user_discord-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:28:14.038211 user_discord-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-06-29 22:25:57.000000 user_discord-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:13.989290 user_discord-1.3.0/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-06-29 22:24:19.000000 user_discord-1.3.0/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-06-29 22:27:38.000000 user_discord-1.3.0/user_discord/socket.py
+-rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.0/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.033210 user_discord-1.3.0/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.0/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.0/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.0/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.026635 user_discord-1.3.0/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.2.9/README.md` & `user_discord-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.9/user_discord/__init__.py` & `user_discord-1.3.0/user_discord/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #Using template from https://github.com/Minori101/Amino.fix/blob/main/aminofix/__init__.py :D THANKS
 
 __title__ = 'user_discord'
 __author__ = 'nxSlayer'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 nxSlayer'
 
-from .user_discord import SocketDiscord
+from .socket import SocketDiscord
 from .user_discord import ClientDiscord
 from .utils import objects
 from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.2.9' != __newest__:
+if '1.3.0' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.2.9/user_discord/user_discord.py` & `user_discord-1.3.0/user_discord/user_discord.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.9/user_discord/utils/objects.py` & `user_discord-1.3.0/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.9/user_discord/utils/payloads.py` & `user_discord-1.3.0/user_discord/utils/payloads.py`

 * *Files identical despite different names*

