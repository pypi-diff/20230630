# Comparing `tmp/nonebot_plugin_poke-0.0.4.tar.gz` & `tmp/nonebot_plugin_poke-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.0.5.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.4.tar` & `nonebot_plugin_poke-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/LICENSE
--rw-r--r--   0        0        0     2923 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/README.md
--rw-r--r--   0        0        0     3441 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     3895 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      922 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2923 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/README.md
+-rw-r--r--   0        0        0     3441 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     3988 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      922 2023-06-30 08:51:01.737677 nonebot_plugin_poke-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.4/LICENSE` & `nonebot_plugin_poke-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.4/README.md` & `nonebot_plugin_poke-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/__init__.py` & `nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ...... .^...**.O@...\O^ .     \.....`   .^ /.,^.=O@OO`=O@^..OO`.=OO\
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
-__version__ = "0.0.2"
+__version__ = "0.0.5"
 __plugin_meta__ = PluginMetadata(
     name="戳一戳事件",
     description='自定义戳一戳事件',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_poke",
     supported_adapters={"~onebot.v11"},
```

### Comparing `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.0.5/nonebot_plugin_poke/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,19 @@
             if acc_file.is_file() and acc_file.suffix.lower() in [".wav",".mp3",".acc"]:
                 acc_file_list.append(str(acc_file))
         send_acc = random.choice(acc_file_list)
         await matcher.send(MessageSegment.record(send_acc))
     
 async def poke_send(event:PokeNotifyEvent,matcher:Matcher):
     if config.poke_send_poke:
-        await matcher.send(Message(f"[CQ:poke,qq={event.user_id}]"))
+        await matcher.send(Message([
+        MessageSegment("poke",  {
+           "qq": f"{event.user_id}"
+       })
+    ]))
     else:
         return
     
 async def pic_text_send(event:PokeNotifyEvent,matcher:Matcher):
     """发送图片和text"""
     pic_file_path = config.poke_path
     pic_file_path.joinpath('pic').mkdir(parents=True, exist_ok=True)
@@ -76,15 +80,15 @@
         send_text.replace('我',config.bot_nickname)
     else:
         send_text:str = ''
     await matcher.send(MessageSegment.image(send_pic)+send_text)
 
 async def poke_rule(event:PokeNotifyEvent):
     """黑白名单判断"""
-    if isinstance(event,PokeNotifyEvent):
+    if isinstance(event,PokeNotifyEvent) and event.target_id == event.self_id:
         group = event.group_id
         if config.poke_black:
             if group in config.poke_ban_group:
                 return False
             else:
                 return True
         else:
```

### Comparing `nonebot_plugin_poke-0.0.4/pyproject.toml` & `nonebot_plugin_poke-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.0.4"
+version = "0.0.5"
 description = "群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
```

### Comparing `nonebot_plugin_poke-0.0.4/PKG-INFO` & `nonebot_plugin_poke-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.5 Summary:
 ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

