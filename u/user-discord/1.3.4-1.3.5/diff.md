# Comparing `tmp/user_discord-1.3.4.tar.gz` & `tmp/user_discord-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.4.tar", last modified: Thu Jun 29 23:20:38 2023, max compression
+gzip compressed data, was "user_discord-1.3.5.tar", last modified: Thu Jun 29 23:25:37 2023, max compression
```

## Comparing `user_discord-1.3.4.tar` & `user_discord-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 23:20:38.587233 user_discord-1.3.4/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:20:38.587233 user_discord-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 23:20:38.587233 user_discord-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-06-29 23:20:26.000000 user_discord-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:20:38.555985 user_discord-1.3.4/user_discord/
--rw-rw-rw-   0        0        0      598 2023-06-29 23:20:22.000000 user_discord-1.3.4/user_discord/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-06-29 23:20:15.000000 user_discord-1.3.4/user_discord/socket.py
--rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.4/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:20:38.587233 user_discord-1.3.4/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.4/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.4/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.4/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:20:38.571609 user_discord-1.3.4/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:20:37.000000 user_discord-1.3.4/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-29 23:20:38.000000 user_discord-1.3.4/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 23:20:37.000000 user_discord-1.3.4/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-29 23:20:37.000000 user_discord-1.3.4/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 23:20:37.000000 user_discord-1.3.4/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.885252 user_discord-1.3.5/
+-rw-rw-rw-   0        0        0      335 2023-06-29 23:25:37.886251 user_discord-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 23:25:37.888252 user_discord-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-06-29 23:25:32.000000 user_discord-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.856026 user_discord-1.3.5/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-06-29 23:25:29.000000 user_discord-1.3.5/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     1891 2023-06-29 23:20:15.000000 user_discord-1.3.5/user_discord/socket.py
+-rw-rw-rw-   0        0        0     4102 2023-06-29 23:25:15.000000 user_discord-1.3.5/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.883254 user_discord-1.3.5/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.5/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.5/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.5/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.876258 user_discord-1.3.5/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.4/README.md` & `user_discord-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.4/setup.py` & `user_discord-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.4",
+    version="1.3.5",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.4/user_discord/__init__.py` & `user_discord-1.3.5/user_discord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.3.4' != __newest__:
+if '1.3.5' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.3.4/user_discord/socket.py` & `user_discord-1.3.5/user_discord/socket.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.4/user_discord/utils/objects.py` & `user_discord-1.3.5/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.4/user_discord/utils/payloads.py` & `user_discord-1.3.5/user_discord/utils/payloads.py`

 * *Files identical despite different names*

