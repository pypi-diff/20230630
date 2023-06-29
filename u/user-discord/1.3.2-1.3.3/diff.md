# Comparing `tmp/user_discord-1.3.2.tar.gz` & `tmp/user_discord-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.2.tar", last modified: Thu Jun 29 23:07:57 2023, max compression
+gzip compressed data, was "user_discord-1.3.3.tar", last modified: Thu Jun 29 23:12:38 2023, max compression
```

## Comparing `user_discord-1.3.2.tar` & `user_discord-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 23:07:56.931664 user_discord-1.3.2/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:07:56.931664 user_discord-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 23:07:56.934664 user_discord-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-06-29 23:07:32.000000 user_discord-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:07:56.744995 user_discord-1.3.2/user_discord/
--rw-rw-rw-   0        0        0      598 2023-06-29 23:07:36.000000 user_discord-1.3.2/user_discord/__init__.py
--rw-rw-rw-   0        0        0     1843 2023-06-29 23:07:14.000000 user_discord-1.3.2/user_discord/socket.py
--rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.2/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:07:56.928667 user_discord-1.3.2/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.2/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.2/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.2/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:07:56.877906 user_discord-1.3.2/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:07:55.000000 user_discord-1.3.2/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-29 23:07:55.000000 user_discord-1.3.2/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 23:07:55.000000 user_discord-1.3.2/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-29 23:07:55.000000 user_discord-1.3.2/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 23:07:55.000000 user_discord-1.3.2/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 23:12:38.610268 user_discord-1.3.3/
+-rw-rw-rw-   0        0        0      335 2023-06-29 23:12:38.610268 user_discord-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 23:12:38.610268 user_discord-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-06-29 23:12:25.000000 user_discord-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:12:38.563393 user_discord-1.3.3/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-06-29 23:07:36.000000 user_discord-1.3.3/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-06-29 23:11:30.000000 user_discord-1.3.3/user_discord/socket.py
+-rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.3.3/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:12:38.610268 user_discord-1.3.3/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.3/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.3/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.3/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:12:38.610268 user_discord-1.3.3/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-06-29 23:12:38.000000 user_discord-1.3.3/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-29 23:12:38.000000 user_discord-1.3.3/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 23:12:38.000000 user_discord-1.3.3/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 23:12:38.000000 user_discord-1.3.3/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 23:12:38.000000 user_discord-1.3.3/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.2/README.md` & `user_discord-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.2/setup.py` & `user_discord-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.2",
+    version="1.3.3",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.2/user_discord/__init__.py` & `user_discord-1.3.3/user_discord/__init__.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.2/user_discord/socket.py` & `user_discord-1.3.3/user_discord/socket.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,16 +46,16 @@
       while True:
         time.sleep(timer)
         self.send_json(payload)
 
     def start_ws(self):
       self.ws = websocket.WebSocket()
       self.ws.connect('wss://gateway.discord.gg/?encoding=json')
-      identify = self.send_json(StartSocket(self.token))
-      self.session_id = identify['d']['session_id']
+      self.send_json(StartSocket(self.token))
+      self.session_id = self.receive_json()['d']['session_id']
       Thread(target=self.event_manager).start()
 
     def get_object(self, data):
       if data['t'] == 'MESSAGE_CREATE':
         return MessageContent(data).MessageContent
       
       return data
```

### Comparing `user_discord-1.3.2/user_discord/user_discord.py` & `user_discord-1.3.3/user_discord/user_discord.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.2/user_discord/utils/objects.py` & `user_discord-1.3.3/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.2/user_discord/utils/payloads.py` & `user_discord-1.3.3/user_discord/utils/payloads.py`

 * *Files identical despite different names*

