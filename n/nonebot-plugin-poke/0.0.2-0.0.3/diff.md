# Comparing `tmp/nonebot_plugin_poke-0.0.2.tar.gz` & `tmp/nonebot_plugin_poke-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.2.tar` & `nonebot_plugin_poke-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/LICENSE
--rw-r--r--   0        0        0     2923 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/README.md
--rw-r--r--   0        0        0     3455 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     3786 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      922 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2923 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/README.md
+-rw-r--r--   0        0        0     3441 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     3895 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      922 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.2/LICENSE` & `nonebot_plugin_poke-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.2/README.md` & `nonebot_plugin_poke-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/__init__.py` & `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
-poke_ = on_notice(rule=to_me(), block=config.poke_block, 
+poke_ = on_notice(block=config.poke_block, 
                   priority=config.poke_priority, rlue=poke_rule)
 
 
 
 @poke_.handle()
 async def _(event: PokeNotifyEvent,matcher:Matcher):
     await poke_send(event,matcher)
```

### Comparing `nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,18 +76,21 @@
         send_text.replace('我',config.bot_nickname)
     else:
         send_text:str = ''
     await matcher.send(MessageSegment.image(send_pic)+send_text)
 
 async def poke_rule(event:PokeNotifyEvent):
     """黑白名单判断"""
-    group = event.group_id
-    if config.poke_black:
-        if group in config.poke_ban_group:
-            return False
+    if isinstance(event,PokeNotifyEvent):
+        group = event.group_id
+        if config.poke_black:
+            if group in config.poke_ban_group:
+                return False
+            else:
+                return True
         else:
-            return True
+            if group in config.poke_allow_group:
+                return True
+            else:
+                return False
     else:
-        if group in config.poke_allow_group:
-            return True
-        else:
-            return False        
+        return False
```

### Comparing `nonebot_plugin_poke-0.0.2/pyproject.toml` & `nonebot_plugin_poke-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.0.2"
+version = "0.0.3"
 description = "群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
```

### Comparing `nonebot_plugin_poke-0.0.2/PKG-INFO` & `nonebot_plugin_poke-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.0.2
+Version: 0.0.3
 Summary: 群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.3 Summary:
 ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

