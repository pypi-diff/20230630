# Comparing `tmp/user_discord-1.3.0.tar.gz` & `tmp/user_discord-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.0.tar", last modified: Thu Jun 29 22:28:14 2023, max compression
+gzip compressed data, was "user_discord-1.3.1.tar", last modified: Thu Jun 29 22:54:50 2023, max compression
```

## Comparing `user_discord-1.3.0.tar` & `user_discord-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.035215 user_discord-1.3.0/
--rw-rw-rw-   0        0        0      335 2023-06-29 22:28:14.035215 user_discord-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 22:28:14.038211 user_discord-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-06-29 22:25:57.000000 user_discord-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:28:13.989290 user_discord-1.3.0/user_discord/
--rw-rw-rw-   0        0        0      598 2023-06-29 22:24:19.000000 user_discord-1.3.0/user_discord/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-06-29 22:27:38.000000 user_discord-1.3.0/user_discord/socket.py
--rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.0/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.033210 user_discord-1.3.0/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.0/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.0/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.0/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:28:14.026635 user_discord-1.3.0/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 22:28:13.000000 user_discord-1.3.0/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 22:54:50.695622 user_discord-1.3.1/
+-rw-rw-rw-   0        0        0      335 2023-06-29 22:54:50.695622 user_discord-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:54:50.695622 user_discord-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-06-29 22:54:36.000000 user_discord-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:54:50.617471 user_discord-1.3.1/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-06-29 22:54:44.000000 user_discord-1.3.1/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-06-29 22:41:40.000000 user_discord-1.3.1/user_discord/socket.py
+-rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.1/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:54:50.679972 user_discord-1.3.1/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.1/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.1/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.1/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:54:50.664349 user_discord-1.3.1/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-06-29 22:54:50.000000 user_discord-1.3.1/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-29 22:54:50.000000 user_discord-1.3.1/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:54:50.000000 user_discord-1.3.1/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 22:54:50.000000 user_discord-1.3.1/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 22:54:50.000000 user_discord-1.3.1/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.0/README.md` & `user_discord-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.0/setup.py` & `user_discord-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.0",
+    version="1.3.1",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.0/user_discord/__init__.py` & `user_discord-1.3.1/user_discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.3.0' != __newest__:
+if '1.3.1' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.3.0/user_discord/socket.py` & `user_discord-1.3.1/user_discord/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         time.sleep(timer)
         self.send_json(payload)
 
     def start_ws(self):
       self.ws = websocket.WebSocket()
       self.ws.connect('wss://gateway.discord.gg/?encoding=json')
       identify = self.send_json(StartSocket(self.token))
-      self.session_id = identify[1]['d']['session_id']
+      self.session_id = identify['d']['session_id']
       Thread(target=self.event_manager).start()
+      while True:
+        self.heartbeat()
 
     def get_object(self, data):
       if data['t'] == 'MESSAGE_CREATE':
         return MessageContent(data).MessageContent
       
       return data
```

### Comparing `user_discord-1.3.0/user_discord/user_discord.py` & `user_discord-1.3.1/user_discord/user_discord.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.0/user_discord/utils/objects.py` & `user_discord-1.3.1/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.0/user_discord/utils/payloads.py` & `user_discord-1.3.1/user_discord/utils/payloads.py`

 * *Files identical despite different names*

